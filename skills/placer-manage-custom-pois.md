---
name: Create and manage custom POIs and tags
description: Create, read, update, delete custom Placer points of interest and organize them with tags.
api: openapi/placer-papi-openapi.json
operations:
  - "POST /v1/poi/custom-poi"
  - "GET /v1/poi/custom-poi/{id}"
  - "PUT /v1/poi/custom-poi/{id}"
  - "DELETE /v1/poi/custom-poi/{id}"
  - "POST /v1/poi/tags/"
  - "PUT /v1/poi/tags/"
  - "DELETE /v1/poi/tags/"
---

# Create and manage custom POIs and tags

Define your own venues (custom POIs) and organize your portfolio with tags.

## Auth
Send `x-api-key: <YOUR_KEY>` on every request (base `https://papi.placer.ai`).

## Steps
1. **Create a custom POI** — `POST /v1/poi/custom-poi` with the geometry and
   metadata. Returns the new custom POI id.
2. **Read / update / delete** — `GET`, `PUT`, `DELETE`
   `/v1/poi/custom-poi/{id}`.
3. **Tag entities** — `POST /v1/poi/tags/` to create a tag and attach entities,
   `PUT /v1/poi/tags/` to modify tag membership, `DELETE /v1/poi/tags/` to
   remove.

## Rules
- Manage-POIs quota is 360/min or 10000/hour
  (`rate-limits/placer-rate-limits.yml`).
- A wrong/missing key returns 403; permission problems return 403 code 1008.
  See `errors/placer-error-codes.yml`.
