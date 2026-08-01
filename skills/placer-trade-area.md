---
name: Analyze the trade area of a place
description: Compute the true trade area, drive-time, and demographics for a Placer point of interest.
api: openapi/placer-papi-openapi.json
operations:
  - "GET /v1/poi"
  - "POST /v1/reports/true-trade-area"
  - "POST /v1/reports/trade-area/drive-time"
  - "POST /v1/reports/trade-area-demographics"
---

# Analyze the trade area of a place

## Auth
Send `x-api-key: <YOUR_KEY>` on every request (base `https://papi.placer.ai`).

## Steps
1. **Resolve the entity** — `GET /v1/poi` to obtain the POI id (check
   `isPermitted`).
2. **True trade area** — `POST /v1/reports/true-trade-area` for the visitor-origin
   polygon of the POI.
3. **Drive-time** — `POST /v1/reports/trade-area/drive-time` for an
   isochrone-based catchment.
4. **Demographics** — `POST /v1/reports/trade-area-demographics` to enrich the
   trade area with population/demographic attributes (requires the demographics
   data-source permission, else 401 code 1001 UNAUTHORIZED_DATA_SOURCE).

## Rules
- Report endpoints are async/cached: an HTTP 202 (code 3005) means re-send the
  same request until 200 (`conventions/placer-conventions.yml`).
- Reports-preparation quota is 5000/hour; see `rate-limits/placer-rate-limits.yml`.
- Full error semantics in `errors/placer-error-codes.yml`.
