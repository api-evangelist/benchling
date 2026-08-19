---
name: benchling-inventory-transfer
description: >-
  Create sample containers in Benchling inventory and transfer contents between
  them, including the asynchronous task poll the transfer endpoint returns.
api: benchling:benchling-v3-api
generated: '2026-08-15'
method: generated
source: >-
  Grounded in openapi/benchling-v3-openapi.yaml. Every operationId below was
  verified present in that spec on 2026-08-15.
operations:
  - ContainerSchema.List
  - Location.List
  - Box.List
  - Plate.List
  - Plate.wells.List
  - Container.Create
  - Container.BatchCreate
  - Container.Get
  - Container.List
  - Container.Transfer
  - Container.Transfer.Get
  - Container.UpdateContentConcentration
  - Container.RemoveContent
---

# Move samples in Benchling inventory

Base URL: `https://{tenant}.benchling.com/api/v3`.

Benchling's inventory model is physical: a Container (tube, vial, cryotube) sits
inside a parent storage object — a Box, a Plate or a Location — and holds
contents at a concentration.

## Locate the storage graph

1. `ContainerSchema.List` — `GET /container-schema/items` for the container type
   and its configured fields.
2. `Location.List` / `Box.List` / `Plate.List` — find the parent storage.
   `Plate.wells.List` — `GET /plate/{plate_id}/wells/items` — enumerates wells.

## Create containers

3. `Container.Create` — `POST /container`, or `Container.BatchCreate` —
   `POST /container:batch-create` for up to 25 in one synchronous call.

## Transfer

4. `Container.Transfer` — `POST /container:transfer`. This is an **asynchronous**
   operation: it returns a task.
5. `Container.Transfer.Get` — `GET /tasks/container/transfer/{task_id}`. Poll
   until the task completes; do not assume success from the 2xx on step 4.
6. `Container.UpdateContentConcentration` and `Container.RemoveContent` adjust
   contents in place.

## Verify

7. `Container.Get` — `GET /container/{container_id}` to confirm parent storage
   and contents.

## Limits

- Transfer into containers is capped at **5000** entities per request — the
  highest documented bulk ceiling in the API.
- Batch endpoints take 25 objects; bulk create takes 1000 for most types.
- **No idempotency key.** A retried transfer can move material twice. Poll the
  task rather than retrying blind.
- 429s are not queued; back off with jitter and watch `x-rate-limit-reset`.

References: `data-model/benchling-data-model.yml`,
`rate-limits/benchling-rate-limits.yml`, `conventions/benchling-conventions.yml`.
