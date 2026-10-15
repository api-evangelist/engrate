---
name: engrate-engr-ate-create-schedule-workflow
description: Create a new schedule and retrieve its details.
api: openapi/engrate-openapi.json
operations:
- create_schedule_schedule_management_v1_schedules_post
- get_schedule_schedule_management_v1_schedules__uid__get
generated: '2026-10-15'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/engrate-openapi.json ; every operationId checked against the contract
---

# engrate-engr-ate-create-schedule-workflow

Create a new schedule and retrieve its details.

## Steps

1. 1. `create_schedule_schedule_management_v1_schedules_post` – send a POST to /schedule-management/v1/schedules with the required request body fields (e.g., name, start_time, recurrence).
2. 2. `get_schedule_schedule_management_v1_schedules__uid__get` – send a GET to /schedule-management/v1/schedules/{uid} using the `uid` returned from the create call.

## Rules

- Include the API key in the `Authorization` header as defined by the `apiKeyAuth` scheme.
- The POST operation is idempotent when a unique `Idempotency-Key` header is provided.
