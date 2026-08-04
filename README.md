# ColorfulClouds (colorfulclouds)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

ColorfulClouds Tech (彩云科技, Beijing-based) operates the Caiyun Weather API (api.caiyunapp.com), a hyperlocal weather + air quality forecasting service with minute-level precipitation, hourly forecasts up to 360 hours, daily forecasts up to 15 days, real-time AQI/pollutant readings, severe-weather alerts, and a precipitation map raster. The v2.6 platform powers consumer apps (Amap, Sina Weather) and enterprise weather integrations across China and globally, billed via tiered token plans on the Open Platform.

**APIs.json:** [https://docs.caiyunapp.com/weather-api/](https://docs.caiyunapp.com/weather-api/)

## Tags

- Weather
- Forecasting
- Air Quality
- Precipitation
- Hyperlocal
- Geospatial
- China

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-30

## APIs

### Caiyun Weather API

Caiyun Weather API v2.6 — hyperlocal weather, minute-level precipitation, hourly/daily forecasts, air quality, life indices, severe-weather alerts, and a precipitation map raster. Single base URL with token in path and lng,lat in path, returning a unified JSON envelope with status, location, timezone, and a result block that contains realtime/minutely/hourly/daily/ alert sub-objects depending on the endpoint or granu parameter.

- **Human URL:** [https://docs.caiyunapp.com/weather-api/](https://docs.caiyunapp.com/weather-api/)
- **Base URL:** `https://api.caiyunapp.com/v2.6`

#### Tags

- Weather
- Forecasting
- Air Quality
- Precipitation
- Alerts

#### Properties

- [Documentation](https://docs.caiyunapp.com/weather-api/)
- [Sign Up](https://platform.caiyunapp.com/)
- [OpenAPI](openapi/colorfulclouds-caiyun-weather-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/colorfulclouds-caiyun-weather.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/colorfulclouds-caiyun-weather.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [SDK](https://pypi.org/project/cy-weather-api/)
- [Code Examples](https://github.com/caiyunapp/caiyun-weather-api-python-sdk)

## Common Properties

- [Website](https://caiyunapp.com/)
- [Documentation](https://docs.caiyunapp.com/weather-api/)
- [Developer Portal](https://platform.caiyunapp.com/)
- [GitHub Organization](https://github.com/caiyunapp)
- [Tools](https://github.com/caiyunapp/mcp-caiyun-weather)
- [Tools](https://github.com/caiyunapp/skills)
- [Tools](https://github.com/caiyunapp/aqi-hub)
- [Tools](https://github.com/caiyunapp/cyeva)
- [Plans](plans/colorfulclouds-plans-pricing.yml)
- [Rate Limits](rate-limits/colorfulclouds-rate-limits.yml)
- [Fin Ops](finops/colorfulclouds-finops.yml)
- [Rules](rules/colorfulclouds-rules.yml)
- [Vocabulary](vocabulary/colorfulclouds-vocabulary.yml)
- [J S O N L D Context](json-ld/colorfulclouds-context.jsonld)
- [Public APIs Listing](https://github.com/public-apis/public-apis)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
