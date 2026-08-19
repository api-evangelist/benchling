---
name: benchling-register-dna-sequence
description: >-
  Create a DNA sequence in Benchling and register it into the tenant's Registry
  so it receives a controlled entityRegistryId. Covers discovering the tenant's
  registry and entity schema first, because Benchling entity payloads are
  schema-driven and cannot be written blind.
api: benchling:benchling-v3-api
generated: '2026-08-15'
method: generated
source: >-
  Grounded in openapi/benchling-v3-openapi.yaml. Every operationId below was
  verified present in that spec on 2026-08-15.
operations:
  - Registry.List
  - EntitySchema.List
  - Folder.List
  - DnaSequence.Create
  - DnaSequence.BatchCreate
  - DnaSequence.Get
---

# Register a DNA sequence in Benchling

Base URL: `https://{tenant}.benchling.com/api/v3` — tenant-scoped. There is no
shared host; use the customer's own subdomain.

## Before you write anything

Benchling entities are **schema-driven**. The fields on a DNA sequence are not
in the OpenAPI — they are configured per tenant and arrive as `schemaFields`.
Writing without reading the schema first is the most common failure.

1. `Registry.List` — `GET /registry/items`. A tenant may have more than one
   registry. Registration is what assigns the controlled `entityRegistryId`.
2. `EntitySchema.List` — `GET /entity-schema/items`. Find the DNA sequence
   schema you are registering against and read its field definitions.
3. `Folder.List` — `GET /folder/items`. Every entity lives in a folder; you
   need a folder id (or a project) for the create call.

All three are paginated: `pageSize` (default 50, max 100) plus the opaque
`nextToken` cursor. Use `returning` to trim the response to the ids you need.

## Create the sequence

4. `DnaSequence.Create` — `POST /dna-sequence`. Supply `bases`, `name`,
   `isCircular`, the folder, the schema, and the registry plus naming strategy
   if this entity should be registered on creation.
5. For more than one sequence, use `DnaSequence.BatchCreate` —
   `POST /dna-sequence:batch-create` — up to 25 objects in a single synchronous
   request. Above that, use the bulk family.

## Verify

6. `DnaSequence.Get` — `GET /dna-sequence/{dna_sequence_id}`. Confirm
   `entityRegistryId` is populated. If it is null the entity was created but not
   registered.

## Rules that apply to this flow

- **No idempotency key.** Benchling publishes no `Idempotency-Key` header. A
  retried `POST /dna-sequence` creates a SECOND sequence. Before retrying a call
  whose response you did not see, list by name and check.
- **Errors are RFC 9457.** v3 returns `application/problem+json` with `type`,
  `title`, `detail`, `status`, `instance`. A 500 additionally carries `errorId`
  — quote it to support@benchling.com.
- **429 is not queued.** Back off exponentially with jitter, capped around 15s.
  Read `x-rate-limit-remaining` and `x-rate-limit-reset`; there is no
  `Retry-After`.
- **5xx means stop.** Benchling explicitly warns that 5xx can occur before the
  rate-limit bucket is exhausted, and that you should significantly back off or
  abort.
- Bulk create limits: 1000 entities per request for most types (2500 for custom
  entities), 100MB total payload.

References: `conventions/benchling-conventions.yml`,
`errors/benchling-problem-types.yml`, `rate-limits/benchling-rate-limits.yml`.
