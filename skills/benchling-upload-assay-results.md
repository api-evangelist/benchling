---
name: benchling-upload-assay-results
description: >-
  Push instrument or analysis results into Benchling as Results attached to an
  assay Run, the canonical lab-integration flow. Includes discovering the result
  schema, batching, and the per-hour throughput ceiling that governs this
  endpoint specifically.
api: benchling:benchling-v3-api
generated: '2026-08-15'
method: generated
source: >-
  Grounded in openapi/benchling-v3-openapi.yaml. Every operationId below was
  verified present in that spec on 2026-08-15.
operations:
  - ResultSchema.List
  - ResultSchema.Get
  - RunSchema.List
  - Run.List
  - Run.Get
  - Result.Create
  - Result.BatchCreate
  - Result.List
---

# Upload assay results to Benchling

Base URL: `https://{tenant}.benchling.com/api/v3`.

This is the flow behind most instrument integrations: an analysis produces
numbers, and those numbers become Results rows in a schema-defined table,
optionally attached to a Run.

## Discover the schema

1. `ResultSchema.List` — `GET /result-schema/items`. Result payloads are
   entirely schema-driven; the columns are tenant configuration, not OpenAPI
   properties.
2. `ResultSchema.Get` — `GET /result-schema/{result_schema_id}`. Read the field
   names, types and any dropdown-constrained values before building rows.
3. `RunSchema.List` / `Run.List` — `GET /run-schema/items`,
   `GET /run/items`. Find the run this batch of results belongs to, if any.

## Write the results

4. `Result.BatchCreate` — `POST /result:batch-create` for a set of rows in one
   synchronous request.
5. `Result.Create` — `POST /result` for a single row.

## Verify

6. `Result.List` — `GET /result/items`, filtered to the run or schema, to
   confirm the rows landed. Use `returning` to fetch only the fields you check.

## Limits that bite on this flow specifically

- **100 results per request, 10,000 requests per hour.** This endpoint has its
  own documented ceiling, separate from the general rate limits.
- **Throughput limit.** Independently of request rate, Benchling caps objects
  created or updated per hour — "tens of thousands" — and the ceiling moves with
  system load. A large backfill will hit this before it hits the request limit.
- **No idempotency key.** A retried batch creates duplicate result rows. Track
  which batches succeeded on your side.
- **413** if the payload exceeds 100MB.
- **429** is not queued for resubmission; back off with jitter.

## Getting results back out

For analysis, the Data Warehouse (direct Postgres) is the intended read path
rather than paging the API: see
`https://docs.benchling.com/docs/getting-started`. Keep polling to 4-5 times per
minute and no more than 100 concurrent connections per user.

References: `conventions/benchling-conventions.yml`,
`rate-limits/benchling-rate-limits.yml`, `errors/benchling-problem-types.yml`.
