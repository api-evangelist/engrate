---
name: engrate-calculate-tariff-cost
description: Calculate the cost of a specific tariff using the cost‑of‑energy API.
api: openapi/engrate-openapi.json
operations:
- list_tariffs_cost_of_energy_v1_tariffs_get
- get_tariff_cost_of_energy_v1_tariffs__tariff_id__get
- calculate_tariff_cost_of_energy_v1_calculate_post
generated: '2026-10-15'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/engrate-openapi.json ; every operationId checked against the contract
---

# engrate-calculate-tariff-cost

Calculate the cost of a specific tariff using the cost‑of‑energy API.

## Steps

1. 1. `list_tariffs_cost_of_energy_v1_tariffs_get` – no required query parameters.
2. 2. `get_tariff_cost_of_energy_v1_tariffs__tariff_id__get` – path parameter `tariff_id` from the list response.
3. 3. `calculate_tariff_cost_of_energy_v1_calculate_post` – body fields as defined in the contract for the calculation request.

## Rules

- Include the `Authorization` header with the API key (apiKeyAuth).
- POST `/cost-of-energy/v1/calculate` is not idempotent; avoid retrying without a new request body.
