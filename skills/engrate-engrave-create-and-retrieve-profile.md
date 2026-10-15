---
name: engrate-engrave-create-and-retrieve-profile
description: Create a new profile and then retrieve its details.
api: openapi/engrate-openapi.json
operations:
- create_profile_cost_of_energy_v1_profiles_post
- get_profile_cost_of_energy_v1_profiles__profile_id__get
generated: '2026-10-15'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/engrate-openapi.json ; every operationId checked against the contract
---

# engrate-engrave-create-and-retrieve-profile

Create a new profile and then retrieve its details.

## Steps

1. 1. Call `create_profile_cost_of_energy_v1_profiles_post` with the required request body fields for a profile.
2. 2. Call `get_profile_cost_of_energy_v1_profiles__profile_id__get` using the `profile_id` returned from the create step.

## Rules

- Auth: Include an `Authorization` header with the API key (apiKeyAuth).
