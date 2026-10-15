---
name: engrate-create-and-validate-clearing-period
description: Create a new clearing period for MABIS, validate the data, and calculate its imbalance.
api: openapi/engrate-openapi.json
operations:
- create_clearing_period_schedule_management_v1_mabis_clearing_periods_post
- validate_clearing_data_schedule_management_v1_mabis_clearing_periods__uid__validate_get
- calculate_imbalance_schedule_management_v1_mabis_clearing_periods__uid__imbalance_get
generated: '2026-10-15'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/engrate-openapi.json ; every operationId checked against the contract
---

# engrate-create-and-validate-clearing-period

Create a new clearing period for MABIS, validate the data, and calculate its imbalance.

## Steps

1. 1. Call `create_clearing_period_schedule_management_v1_mabis_clearing_periods_post` with the required request body and include the `Authorization` header (apiKey).
2. 2. Call `validate_clearing_data_schedule_management_v1_mabis_clearing_periods__uid__validate_get` using the `uid` returned from step 1 and include the `Authorization` header.
3. 3. Call `calculate_imbalance_schedule_management_v1_mabis_clearing_periods__uid__imbalance_get` with the same `uid` and include the `Authorization` header.

## Rules

- Authentication: All requests must include an `Authorization` header containing the API key (apiKeyAuth).
- Idempotency: POST requests (`create_clearing_period_schedule_management_v1_mabis_clearing_periods_post`) should be made idempotent by the client if the API supports an Idempotency-Key header (not documented, so client should avoid duplicate calls).
