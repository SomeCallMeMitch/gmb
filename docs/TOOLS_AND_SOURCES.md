# Tool Research, Pricing and Data Sources

**Historical tool architecture/pricing baseline: 2026-10-14 PT.** See **[Geo-Grid Tool Comparison, 2026-10-15](GEO_GRID_TOOL_COMPARISON_2026-10-15.md)** for newer, broader vendor/Reddit research and verified trial restrictions. This existing file is deliberately kept as an earlier data architecture and pricing snapshot. **Prices change. Recheck official vendor pricing and account-level features before purchasing.** Last checked official pricing pages on 2026-10-14 where marked verified; the remainder are historical leads to investigate.

## Architectural principle: two different jobs

1. **Business discovery/enrichment**: Get all (or a broad sample of) businesses matching a category/area, reviews, rating, category, website, phone, address, lat/lng, status, Place ID and GBP/Maps URL. Do this cheaply and broadly using **Outscraper** or a comparable source.
2. **Localized rank measurement**: Measure visibility at many points around one business for a specific keyword and date. Do this selectively on promising leads with **Whitespark Local Ranking Grids**, **Local Falcon**, or comparable specialist. The first task cannot substitute for the second.

**Caution:** Outscraper search result sequence is a raw *returned order for a particular query*, not an independently confirmed Google Maps rank at a known geospatial point. Business discovery can be broader than page-one results; do not cap at ten unless sampling is intentional. A previous recommendation was to cap a first category/city experiment at 30 to conserve credits, then raise based on completeness. Actual pilot was 150 records across three queries.

## Price/features comparison

| Tool | Role | Confirmed listed price/limits on 2026-10-14 | Notes |
|---|---|---|---|
| [Outscraper Google Maps Scraper](https://outscraper.com/pricing/) | Discovery/enrichment | First **500 businesses $0** in free tier; usage after 500 up to 100k listed **$3/1,000 records**; pay-as-you-go | Excel/CSV/JSON; API on paid tier; user account active and first export complete. Verify whether free usage refreshes by period in the actual account. |
| [Whitespark Local Ranking Grids](https://whitespark.ca/local-ranking-grids/) | Geo-grid scans | **$10/2,000**, **$20/5,000**, **$50/15,000** credits monthly; 200 free trial credits shown | Cheapest low-dollar grid test; no assumption that all advanced integration/reporting features equal Falcon. |
| [Local Falcon](https://www.localfalcon.com/pricing) | Geo-grid, reporting, competitor research, sales enablement, automation | **$24.99/7,500** credits/month Starter; **$49.99/15,150** Basic; **$99.99/31,250** Pro | 1 credit per grid point; 100 free trial credits noted; monthly unused credits expire. Sales Enablement costs **1 credit per lead lookup**; Claude connector included with plan and consumes grid credits for new scans. Verify exact plan gating of API/white-label features. |
| [Local Viking](https://localviking.com/) | GBP management + grids | Previously suggested ~$39/month / 7,500 grid credits, **not confirmed current**; [help article](https://help.localviking.com/en/articles/8257402-purchasing-credits) mentions 10k geo-grid credits for $49/mo (2023 article) | Must verify current plan tiers and whether it requires connected listings. |
| [BrightLocal](https://www.brightlocal.com/) | Broad local SEO toolkit incl. audit/grid/reporting | Previously discussed ~$41/mo for 1 location, **not verified current** | More useful as a fuller SEO platform than as lowest-cost grid source; compare add-on limits carefully. |
| [Whitespark Local Rank Tracker](https://whitespark.ca/local-rank-tracker/) | Traditional position tracker, separate product | Previously discussed ~$17/mo for 100 location-keywords, **not reverified** | Do not confuse with Whitespark Local Ranking Grids. |
| [Apify](https://apify.com/store) | Alternative Maps extraction actors | Varies by actor and plan; no uniform price | Evaluate reliability/coverage only if Outscraper proves insufficient. |
| [Google Places API](https://developers.google.com/maps/documentation/places/web-service/overview) | Official business discovery and lookups | Billing by API field/request type (check official SKU pricing) | Does **not** natively return specialist keyword rankings over arbitrary rank-grid points. Official data use restrictions must be reviewed. |

### Geo-grid credit examples

- 3x3 = **9** points per keyword scan.
- 5x5 = **25** points per keyword scan.
- 7x7 = **49** points per keyword scan.
- 9x9 = **81** points per keyword scan.
- At 5x5, 3 keywords for one location/one round = **75** credits. At 5x5, 2 keywords for 3 businesses/one round = **150** credits. A matching after-scan doubles usage. All of these assume one credit per point and no extra AI/report credits.
- 7,500 Local Falcon credits theoretically cover 300 scans of 5x5 one-keyword grids (before other use); 2,000 Whitespark credits cover 80 analogous scans.
- At similar scale, Falcon Starter 7,500 credits/$24.99 and Whitespark $20/5,000 each cost roughly $0.0033–$0.004 per point; price gap not decisive relative to exports/automation capabilities.

### Local Falcon sales enablement nuance

The [pricing page](https://www.localfalcon.com/pricing) advertises a **1-credit/lookup Sales Enablement** tool and Claude connector. Earlier conversation discussed a workflow that begins with a CSV of business names/addresses and retrieves GBP data. It is valuable for **enrichment**, but should **not be treated as a guaranteed citywide category discovery engine**. Outscraper is better suited to initial all-business discovery. The tool can perform grids after list qualification.

### Research URLs

- Outscraper pricing: https://outscraper.com/pricing/
- Outscraper scraper product: https://outscraper.com/google-maps-scraper-data/
- Whitespark Local Ranking Grids: https://whitespark.ca/local-ranking-grids/
- Local Falcon pricing: https://www.localfalcon.com/pricing
- Local Falcon Sales Enablement guide: https://app.localfalcon.com/knowledge-base/kb54-how-to-use-the-local-falcon-sales-enablement-tool
- Local Viking credit help (older): https://help.localviking.com/en/articles/8257402-purchasing-credits
- BrightLocal: https://www.brightlocal.com/
- Apify: https://apify.com/store
- Google Places API overview: https://developers.google.com/maps/documentation/places/web-service/overview
- Google Search local ranking explanation: https://support.google.com/business/answer/7091
- Google Business Profile guidelines: https://support.google.com/business/answer/3038177

## Data schema for future automation

### Discovery (Outscraper or another API)

Required: `source_query`, `business_name`, `place_id`, `category`, `rating`, `reviews_count`, `address`, `city`, `latitude`, `longitude`, `website`, `phone`, `google_maps_url`, `business_status`, `source_result_order`, `collected_at`.

Optional: `claimed_status`, `service_area_business`, `hours`, `other_categories`, `review_recency`, `independent_chain_flag`, `contact_decision_maker` (private), `observed_conversion_quality`.

### Grid scan

`place_id`, `keyword`, `scan_vendor`, `scan_time`, `grid_center`, `grid_size`, `grid_spacing_or_radius`, `search_language`, `device_or_method` (if selectable), `point_lat_lon`, `rank_position` (including not found), `top_3_share`, `average_rank`, `competitor_ids`, `report_url`, `raw_export_reference`.

### Sales

`prospect_id`, `qualification_score`, `score_version`, `reason_codes`, `offer_tier`, `channel`, `contacted_date`, `response_date`, `meeting`, `trial_start_end`, `consent`, `paid_start`, `monthly_price`, `cancellation`, `observed_business_outcome`.

**Data governance:** use Place ID as a dedupe key where available; record origin and time of extraction; do not publish nonpublic personal contacts/lead intelligence in a public repository.

## Build-vs-buy recommendation

**Now:** Outscraper export -> spreadsheet or lightweight CSV analysis -> choose five leads -> Whitespark and/or Falcon grid comparison -> personalized outreach. Don't build the app yet.

**Later, once sales validated:** Base44 front end and Entities database for market selector, leads, filters, score rationale, grid artifacts and outreach stages; external scheduled API/worker for Outscraper/geo-grid data providers; AI to summarize grounded evidence and draft personalized scripts. Use supported Base44 integrations and guardrails (see `AGENTS.md`). Browser control through ChatGPT Work or Claude can assist supervised research, but is not a dependable replacement for licensed extraction/API feeds at scale.
