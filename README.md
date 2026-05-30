# ColorfulClouds (colorfulclouds)

ColorfulClouds Tech (彩云科技, Beijing-based) operates the Caiyun Weather API (api.caiyunapp.com), a hyperlocal weather + air quality forecasting service with minute-level precipitation, hourly forecasts up to 360 hours, daily forecasts up to 15 days, real-time AQI/pollutant readings, severe-weather alerts, and a precipitation map raster. The v2.6 platform powers consumer apps (Amap, Sina Weather) and enterprise weather integrations across China and globally, billed via tiered token plans on the Open Platform.

**URL:** [docs.caiyunapp.com/weather-api/](https://docs.caiyunapp.com/weather-api/)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

- Weather, Forecasting, Air Quality, Precipitation, Hyperlocal, Geospatial, China

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-30

## APIs

### Caiyun Weather API

Caiyun Weather API v2.6 — hyperlocal weather, minute-level precipitation, hourly/daily forecasts, air quality, life indices, severe-weather alerts, and a precipitation map raster. Single base URL with token in path and lng,lat in path, returning a unified JSON envelope with status, location, timezone, and a result block that contains realtime/minutely/hourly/daily/alert sub-objects depending on the endpoint or granu parameter.

**Human URL:** [docs.caiyunapp.com/weather-api/](https://docs.caiyunapp.com/weather-api/)

**Base URL:** `https://api.caiyunapp.com/v2.6`

#### Tags

- Weather, Forecasting, Air Quality, Precipitation, Alerts

#### Properties

- [Documentation](https://docs.caiyunapp.com/weather-api/)
- [Sign Up](https://platform.caiyunapp.com/)
- [OpenAPI](openapi/colorfulclouds-caiyun-weather-openapi.yml)
- [Python SDK](https://pypi.org/project/cy-weather-api/)
- [Python SDK Source](https://github.com/caiyunapp/caiyun-weather-api-python-sdk)
- [Naftiko Capability — Weather Combined](capabilities/caiyun-weather-weather.yaml)
- [Naftiko Capability — Realtime](capabilities/caiyun-weather-realtime.yaml)
- [Naftiko Capability — Forecast](capabilities/caiyun-weather-forecast.yaml)
- [Naftiko Capability — Air Quality](capabilities/caiyun-weather-air-quality.yaml)
- [Naftiko Capability — Alerts](capabilities/caiyun-weather-alerts.yaml)
- [Naftiko Capability — Precipitation Map](capabilities/caiyun-weather-precipitation-map.yaml)

## Common Properties

- [Website](https://caiyunapp.com/)
- [Documentation](https://docs.caiyunapp.com/weather-api/)
- [Developer Portal](https://platform.caiyunapp.com/)
- [GitHub Organization](https://github.com/caiyunapp)
- [MCP Server (Caiyun Weather)](https://github.com/caiyunapp/mcp-caiyun-weather)
- [Claude Code Skills (Caiyun Weather)](https://github.com/caiyunapp/skills)
- [AQI Hub (Air Quality Index Calculator)](https://github.com/caiyunapp/aqi-hub)
- [cyeva (Forecast Accuracy Evaluation Toolkit)](https://github.com/caiyunapp/cyeva)
- [Plans](plans/colorfulclouds-plans-pricing.yml)
- [Rate Limits](rate-limits/colorfulclouds-rate-limits.yml)
- [FinOps](finops/colorfulclouds-finops.yml)
- [Spectral Rules](rules/colorfulclouds-rules.yml)
- [Vocabulary](vocabulary/colorfulclouds-vocabulary.yml)
- [JSON-LD Context](json-ld/colorfulclouds-context.jsonld)
- [Public APIs Listing](https://github.com/public-apis/public-apis)

## Features

| Name | Description |
|------|-------------|
| Minute-Level Precipitation | 120-minute precipitation nowcasting with 1-minute resolution and 1-kilometer geographic precision based on radar + AI nowcasting models. |
| Hourly Forecast | Hourly weather forecast for up to 360 hours covering temperature, humidity, cloud cover, weather phenomenon (skycon), precipitation, wind, pressure, visibility, downward shortwave radiation, and AQI. |
| Daily Forecast | Daily forecast for up to 15 days with min/max/avg temperature, humidity, cloud cover, pressure, visibility, wind, plus daytime (08h-20h) and nighttime (20h-32h) splits for skycon, precipitation, and wind. |
| Real-Time Air Quality | PM2.5, PM10, O3, SO2, NO2, CO concentrations and AQI calculated under both Chinese (HJ 633-2012) and US EPA standards with category descriptors. |
| Severe Weather Alerts | Official Chinese Meteorological Administration alerts (typhoon, rainstorm, blizzard, etc.) with title, code, status, description, region, adcode, and publication timestamp. |
| Life Indices | Daily and real-time life indices including ultraviolet, comfort, cold risk, dressing, and car-washing recommendations. |
| Precipitation Map Raster | Radar + nowcast precipitation map tiles for embedding live precipitation animations into consumer and operational dashboards. |
| Sky Condition (Skycon) Enum | Normalized weather phenomenon enum (CLEAR_DAY, PARTLY_CLOUDY_DAY, CLOUDY, LIGHT_HAZE, HEAVY_RAIN, STORM_SNOW, DUST, SAND, WIND, etc.) suitable for icon-driven UIs. |
| Multi-Language Output | Localized descriptions in zh_CN, zh_TW, ja, en_GB, and en_US selectable via the lang query parameter. |
| Unit System Selection | Switch between metric, metric:v1, metric:v2, imperial, and SI unit systems via the unit query parameter. |

## Use Cases

| Name | Description |
|------|-------------|
| Mobile Weather Apps | Power consumer weather apps with realtime conditions, minute-level rain forecasts, and severe-weather alerts in a single combined call. |
| Smart Home / IoT Integration | Drive smart-home automations (close windows on rain, dim lights at sunset, adjust HVAC) using realtime + minutely + daily astronomical data. |
| Logistics and Delivery Routing | Use hourly forecasts and precipitation nowcasts to reroute couriers, delay flights, and pre-position field crews before rain or snow events. |
| Outdoor Event Planning | Combine daily forecasts, life indices, and alerts to plan outdoor events, sports, construction, and agricultural operations 5-15 days ahead. |
| Air-Quality-Aware Mobility | Cycling, running, and route-planning apps surface PM2.5/AQI to recommend healthier routes and times. |

## Integrations

| Name | Description |
|------|-------------|
| Claude / Anthropic Agents | First-party MCP server (caiyunapp/mcp-caiyun-weather) and Claude Code skills (caiyunapp/skills) expose realtime, hourly, daily, historical, and alert lookups as agent tools. |
| Home Assistant | Community Home Assistant component (Yonsm/ZhiCaiYun) wraps the Caiyun API for smart-home automations. |
| Amap (Gaode Maps) | Caiyun forecasts are surfaced inside Amap navigation and weather widgets as a partner data source. |
| Sina Weather | Sina Weather embeds Caiyun nowcasts and 5-day forecasts in its consumer products. |
| Wego CLI | Community fork of the wego terminal weather app (caiyunapp/wego) supports Caiyun as a backend. |

## Solutions

| Name | Description |
|------|-------------|
| Hyperlocal Weather Platform | Pair the combined /weather endpoint with the precipitation map raster to ship a complete hyperlocal weather product covering realtime, minutely, hourly, daily, alerts, and map overlays. |
| Agent-Ready Weather Intelligence | Run the official MCP server alongside the installable Claude Code skills to give LLM agents tool-grounded access to Caiyun forecasts and alerts. |
| Air Quality Surveillance | Combine /realtime air quality, /hourly AQI series, and the open-source aqi-hub library to publish dashboards, alerts, and exposure analytics. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Caiyun Weather API](openapi/colorfulclouds-caiyun-weather-openapi.yml) — 8 operations across 6 tags (Realtime, Forecast, Weather, Air Quality, Alerts, Precipitation Map); 45 component schemas.

### JSON Schema

44 JSON Schema files generated from the OpenAPI components — one per domain object (Realtime, Minutely, Hourly, Daily, AirQualityRealtime, Alert, SkyCon, Wind, etc.). Browse `json-schema/`.

### JSON Structure

44 JSON Structure (json-structure.org) files mirroring the JSON Schemas with stricter typing. Browse `json-structure/`.

### JSON-LD

- [ColorfulClouds JSON-LD Context](json-ld/colorfulclouds-context.jsonld) — 36 type declarations + 87 property terms aligning Caiyun schemas with schema.org and XSD datatypes.

### Examples

44 realistic example payloads, one per JSON Schema. Browse `examples/`.

## Capabilities

Naftiko capabilities, one self-contained file per business surface. Each file declares both a REST exposer and an MCP exposer over its inline `consumes` block.

### Per-Tag Capabilities

| Capability | Operations | Lead Operation |
|------------|------------|----------------|
| [Realtime](capabilities/caiyun-weather-realtime.yaml) | 1 | Get Realtime Weather |
| [Forecast](capabilities/caiyun-weather-forecast.yaml) | 3 | Get Hourly Weather Forecast |
| [Weather Combined](capabilities/caiyun-weather-weather.yaml) | 1 | Get Combined Weather Envelope |
| [Air Quality](capabilities/caiyun-weather-air-quality.yaml) | 1 | Get Realtime Air Quality |
| [Alerts](capabilities/caiyun-weather-alerts.yaml) | 1 | Get Severe Weather Alerts |
| [Precipitation Map](capabilities/caiyun-weather-precipitation-map.yaml) | 1 | Get Precipitation Map Tile |

## Vocabulary

- [ColorfulClouds Vocabulary](vocabulary/colorfulclouds-vocabulary.yml) — Unified taxonomy mapping 8 resources, 1 action verb, 6 workflows, and 11 personas across operational (OpenAPI) and capability (Naftiko) dimensions.

## Rules

- [Caiyun Weather Spectral Rules](rules/colorfulclouds-rules.yml) — 39 rules across 12 categories enforcing path-token convention, snake_case JSON, camelCase operationIds, "Caiyun Weather" summary prefix, GET-only methods, and SkyCon enum integrity.

## Plans, Rate Limits, and FinOps

- [Plans / Pricing](plans/colorfulclouds-plans-pricing.yml) — Free Developer (400 req/day, 3-day forecast), Standard / Paid (extended horizons, map tiles), Enterprise (custom SLA + OEM).
- [Rate Limits](rate-limits/colorfulclouds-rate-limits.yml) — Per-token daily quota with gateway burst throttling; exponential backoff + token rotation + coordinate quantization recommended.
- [FinOps (FOCUS 1.3)](finops/colorfulclouds-finops.yml) — Tiered Subscription + Usage-Based, meters on api_requests / map_tiles / forecast_horizon_overage / subscription / enterprise_commit.

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
