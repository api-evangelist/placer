---
name: Pull visit metrics for a place
description: Search Placer for a point of interest, then retrieve foot-traffic visit metrics for it.
api: openapi/placer-papi-openapi.json
operations:
  - "GET /v1/poi"
  - "POST /v1/reports/visit-metrics"
  - "POST /v1/reports/visit-trends"
---

# Pull visit metrics for a place

Use the Placer Public API (PAPI, base `https://papi.placer.ai`) to find a
venue and measure its foot traffic.

## Auth
Send `x-api-key: <YOUR_KEY>` on every request. A missing/invalid key returns
HTTP 403.

## Steps
1. **Find the entity** — `GET /v1/poi` with filters (name, category, or a
   `radius` around a lat/long). Paginate with `skip` (first 1000 results
   available). Read the `isPermitted` flag on each result — if `false` you may
   not run reports for that entity.
2. **Request visit metrics** — `POST /v1/reports/visit-metrics` with the
   entity id(s) and a date range. If the report is not yet cached the API
   returns HTTP 202 (code 3005, IN_PROGRESS) — re-send the identical request
   until it returns 200. See `conventions/placer-conventions.yml`.
3. **Optional trend** — `POST /v1/reports/visit-trends` for a time series over
   the same entity.

## Rules
- Respect the rate limits in `rate-limits/placer-rate-limits.yml` (reports
  preparation = 5000/hour; 10 calls/sec; 5 concurrent). Calls ending 202/429/5XX
  do not count against the weekly quota.
- Handle error codes per `errors/placer-error-codes.yml` (e.g. 1025
  UNDELIVERABLE_ENTITY = blocked by privacy policy; 1016 RESTRICTED_AREA).
