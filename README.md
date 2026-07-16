# SnapAPI

REST API for turning any URL into visual captures or structured data with a single
call — screenshots (PNG, JPEG, WebP, AVIF), full-page PDFs, scroll videos (MP4,
WebM, GIF), markdown/text/metadata extraction tuned for AI pipelines, and multi-page
scraping with anti-bot stealth and proxy support. Also offers bring-your-own-key AI
page analysis (OpenAI/Anthropic), batch and async processing with webhooks, device
emulation, and optional cloud storage — all powered by headless Chromium.

- **Website:** https://snapapi.pics
- **Documentation:** https://snapapi.pics/docs.html
- **API reference:** https://api.snapapi.pics/v1/docs
- **OpenAPI:** [openapi/snapapi-pics-openapi.json](openapi/snapapi-pics-openapi.json) (3.1.0, v2.0.0)
- **Base URL:** https://api.snapapi.pics
- **Auth:** `X-Api-Key` header (or `Authorization: Bearer`)
- **Free tier:** 200 requests/month, no credit card
- **SDKs:** 8 official SDKs
- **Author:** Aleksei Serebriakov (support@snapapi.pics)

## APIs

| API | Endpoint(s) |
| --- | --- |
| Screenshot | `POST`/`GET /v1/screenshot`, `/v1/screenshot/batch`, `/v1/screenshot/async/{jobId}` |
| PDF | `POST /v1/pdf` |
| Video | `POST /v1/video` |
| Content Extraction | `POST`/`GET /v1/extract` |
| Scrape | `POST`/`GET /v1/scrape` |
| AI Analyze (BYOK) | `POST /v1/analyze` |
| Usage & Capabilities | `GET /v1/usage`, `/v1/devices`, `/v1/capabilities` |

## Note on naming

This is **SnapAPI at `snapapi.pics`** (by Aleksei Serebriakov). It is distinct from
the separately-cataloged [`snapapi`](../snapapi/) provider at `snap.michaelcli.com`,
which shares the product name but is a different domain and a smaller v1 surface.

---

Cataloged on [APIs.io](https://apis.io/) by [API Evangelist](https://apievangelist.com/).
Source: inbound submission from the author (2026-07-16).
