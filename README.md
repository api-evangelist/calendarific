# Calendarific (calendarific)

Worldwide public holidays REST API covering 230+ countries. Calendarific provides
national, local, religious, and observance holiday data with localization across
many ISO-639 languages. Used for ecommerce scheduling, HR systems, travel planning,
payroll, and global operations.

**APIs.yml:** [apis.yml](apis.yml)

## Type
- **x-type:** company
- **x-tier:** 3 (bulk-registered from public-apis)
- **source:** [public-apis/public-apis](https://github.com/public-apis/public-apis) — category: Calendar

## APIs

### Calendarific Holiday API
- **Base URL:** `https://calendarific.com/api/v2`
- **Documentation:** https://calendarific.com/api-documentation
- **Authentication:** API key via `api_key` query parameter
- **Operations:**
  - `GET /holidays` — List holidays by country and year (with optional month/day/type/location/language filters)
  - `GET /countries` — List supported countries with ISO-3166 codes
  - `GET /languages` — List supported languages with ISO-639 codes

## Artifacts

| Artifact | Path |
|---|---|
| OpenAPI | [`openapi/calendarific-openapi.yml`](openapi/calendarific-openapi.yml) |
| JSON Schema | [`json-schema/`](json-schema/) (holiday, country, language) |
| JSON Structure | [`json-structure/`](json-structure/) (holiday, country, language) |
| JSON-LD | [`json-ld/calendarific-context.jsonld`](json-ld/calendarific-context.jsonld) |
| Examples | [`examples/`](examples/) (holidays, countries, languages) |
| Spectral Rules | [`rules/calendarific-rules.yml`](rules/calendarific-rules.yml) |
| Vocabulary | [`vocabulary/calendarific-vocabulary.yml`](vocabulary/calendarific-vocabulary.yml) |
| Capabilities (shared) | [`capabilities/shared/calendarific-holidays.yaml`](capabilities/shared/calendarific-holidays.yaml) |
| Capabilities (workflows) | [`capabilities/holiday-calendar-sync.yaml`](capabilities/holiday-calendar-sync.yaml), [`capabilities/global-coverage-catalog.yaml`](capabilities/global-coverage-catalog.yaml) |
| Plans / Pricing | [`plans/calendarific-plans-pricing.yml`](plans/calendarific-plans-pricing.yml) |
| Rate Limits | [`rate-limits/calendarific-rate-limits.yml`](rate-limits/calendarific-rate-limits.yml) |
| FinOps | [`finops/calendarific-finops.yml`](finops/calendarific-finops.yml) |

## SDKs

| Language | Repo |
|---|---|
| Python | https://github.com/calendarific/python-calendarific |
| Node.js | https://github.com/calendarific/node-calendarific |
| PHP | https://github.com/calendarific/php-calendarific |
| Ruby | https://github.com/calendarific/ruby-calendarific |
| Go | https://github.com/calendarific/go-calendarific |
| .NET (community) | https://github.com/guibranco/calendarific-sdk-dotnet |
| PowerShell (community) | https://github.com/rchaganti/PSCalendarific |
| Elixir (community) | https://github.com/Bounceapp/elixir-calendarific |

## MCP Servers
- **Calendarific MCP Server** (community) — https://github.com/noalimoy/calendarific-mcp-server

## Plans (Pricing)

| Plan | Price | Monthly Quota | Support |
|---|---|---|---|
| Free | $0 | 500 requests/month | Community |
| Starter | $12/mo or $100/yr | 10,000 requests/month | Email |
| Business | $500/yr | 50,000 requests/month | Priority |
| Enterprise | $4,000/yr | 50,000,000 requests/month | Dedicated |

Free tier additionally enforces a 1,000 requests/day soft cap (HTTP 429 on overage).

## Tags
Calendar, Public APIs, Holidays, Worldwide, Localization

## Timestamps
- **Created:** 2026-05-28
- **Modified:** 2026-05-29

## Maintainers
- **Kin Lane** — kin@apievangelist.com
