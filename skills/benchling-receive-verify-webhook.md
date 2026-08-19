---
name: benchling-receive-verify-webhook
description: >-
  Receive a Benchling App webhook and verify its signature before acting on it,
  then fetch the referenced object. Covers the JWKS rotation rule and the
  SUFFIXED vs STABLE URL routing choice that decides what path Benchling POSTs
  to.
api: benchling:benchling-v3-api
generated: '2026-08-15'
method: generated
source: >-
  Grounded in the webhooks block of openapi/benchling-v3-openapi.yaml and
  https://docs.benchling.com/docs/webhook-verification. Event names and payload
  schemas taken verbatim from the spec.
operations:
  - Entry.Get
  - DnaSequence.Get
  - CustomEntity.Get
  - Project.Get
  - Run.Get
---

# Receive and verify a Benchling webhook

Benchling delivers 14 v3 events as HTTP POSTs to a Benchling App's configured
webhook URL: `v3.customEntity.created`, `v3.customEntity.updated`,
`v3.dnaOligo.created/updated`, `v3.dnaSequence.created/updated`,
`v3.entry.created`, `v3.project.created/updated`,
`v3.rnaOligo.created/updated`, `v3.rnaSequence.created/updated`,
`v3.run.created`. Each carries a typed envelope
(`<Object><Event>WebhookEnvelopeV3`).

## 1. Know which URL you are listening on

The App's `webhookUrlRouting` setting decides the effective path:

| Routing | Events | App lifecycle | Canvas |
| --- | --- | --- | --- |
| `SUFFIXED` (default) | `$WEBHOOK_URL/event` | `$WEBHOOK_URL/lifecycle` | `$WEBHOOK_URL/canvas` |
| `STABLE` | `$WEBHOOK_URL` | `$WEBHOOK_URL` | `$WEBHOOK_URL` |

Pick `STABLE` when your endpoint is a fixed URL you do not control the path of
(Zapier, Slack, Workato). Keep `SUFFIXED` for path-routed architectures.

## 2. Verify before you trust

Three headers arrive with every delivery:

- `Webhook-Id` — unique per message, **stable across resends**
- `Webhook-Timestamp` — seconds since epoch
- `Webhook-Signature` — base64, space-delimited list of signatures

Steps:

1. Compare `Webhook-Timestamp` against your own UTC clock. Benchling recommends
   a **5-minute** tolerance. Reject anything outside it.
2. Build `signed_content` as `{Webhook-Id}.{Webhook-Timestamp}.{raw_body}` —
   the RAW body, not a re-serialised one.
3. Fetch the app's JWKS from
   `https://apps.benchling.com/api/v1/apps/{app_definition_id}/jwks` (legacy
   apps: `https://benchling.com/apps/jwks/{app_installation_id}`).
4. Verify the ECDSA signature against those keys.

**Never hardcode the keys.** Benchling rotates the keypair frequently; re-fetch
the JWKS at intervals of **no more than 6 hours** and cache between fetches.

Optionally allowlist Benchling's source IPs — the range is per-tenant and
supplied by your account team, not published.

## 3. Acknowledge, then act

Return **HTTP 200** to acknowledge receipt. Do the work asynchronously; a slow
handler risks a redelivery, and because `Webhook-Id` is stable across resends it
is the natural de-duplication key — which matters, since the REST API offers no
idempotency key of its own.

## 4. Fetch the object

The envelope identifies the changed object; read the current state with
`Entry.Get`, `DnaSequence.Get`, `CustomEntity.Get`, `Project.Get` or `Run.Get`.
Do not treat the webhook payload as the authoritative record.

## Related: EventBridge

A second, older event stream (23 `v2.*` events, including assay runs, workflow
tasks, entity registration and requests) is delivered through Amazon
EventBridge into the customer's own AWS account rather than over HTTP. Different
transport, different catalog — see `asyncapi/benchling-webhooks.yml`.
