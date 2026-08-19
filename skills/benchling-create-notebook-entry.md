---
name: benchling-create-notebook-entry
description: >-
  Create an electronic lab notebook Entry in Benchling from a template, read its
  parts, and follow it through review. The ELN is the surface most integrations
  write narrative and structured experiment records into.
api: benchling:benchling-v3-api
generated: '2026-08-15'
method: generated
source: >-
  Grounded in openapi/benchling-v3-openapi.yaml. Every operationId below was
  verified present in that spec on 2026-08-15.
operations:
  - EntrySchema.List
  - EntryTemplate.List
  - EntryTemplate.Get
  - Project.List
  - Folder.List
  - Entry.Create
  - Entry.Get
  - Entry.Update
  - Entry.parts.List
  - Entry.authors.List
  - Entry.applicableReviewProcesses.List
---

# Create a Benchling notebook entry

Base URL: `https://{tenant}.benchling.com/api/v3`.

## Find the template and its home

1. `EntrySchema.List` — `GET /entry-schema/items`. Entries may conform to a
   schema defining custom fields.
2. `EntryTemplate.List` — `GET /entry-template/items`, then
   `EntryTemplate.Get` — `GET /entry-template/{entry_template_id}`. Creating
   from a template is how teams keep entry structure consistent.
3. `Project.List` / `Folder.List`. An entry belongs to a folder, and its
   project determines which review processes apply.

## Create and populate

4. `Entry.Create` — `POST /entry`, referencing the template, folder, schema and
   any `schemaFields`.
5. `Entry.Update` — `PATCH /entry/{entry_id}` to set fields or change authors.
6. `Entry.parts.List` — `GET /entry/{entry_id}/parts/items` to walk the entry's
   content: sections, text, tables and structured result tables.

## Review

7. `Entry.applicableReviewProcesses.List` —
   `GET /entry/{entry_id}/applicable-review-processes/items` shows which review
   processes the entry's project configures.
8. `Entry.authors.List` — `GET /entry/{entry_id}/authors/items`. Authors default
   to the creator but can be changed.

## Notes

- Entry mutation endpoints in v3 were still in limited availability at the time
  this spec was captured; the schema description says so explicitly. Confirm
  availability on the target tenant before relying on `Entry.Create` in
  production, and check `openapi/benchling-entries-api-openapi.yml` for the v2
  equivalents.
- Entries are the records that make 21 CFR Part 11 / GxP posture matter; changes
  are audited. `AuditLog.List` — `GET /audit-log/items` — exposes the trail.
- **No idempotency key**: a retried `POST /entry` creates a second entry.
- Errors are RFC 9457 problem details; 429s are not queued.

References: `conventions/benchling-conventions.yml`,
`lifecycle/benchling-lifecycle.yml`, `security/benchling-trust-center.yml`.
