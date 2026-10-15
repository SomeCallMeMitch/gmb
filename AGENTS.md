# AI Handoff / Project Memory

Last updated: 2026-10-14 (Pacific). Repository: `SomeCallMeMitch/gmb`.

## What this project is

Build a small, scalable, white-label local search/Google Maps visibility agency for real local businesses. Acquire customers using a compelling, measurable before-and-after Google Maps rank grid. The business owner has marketing/sales experience and local SEO familiarity. The strategy is to sell the results and account relationship while outsourced fulfillment handles a narrow ranking service; upsell legitimate GBP/website/local SEO enhancements.

## Most important known facts

- Hypothesized outsourced service **cost: $300 per business per month**, target sell price **$500/month**, yielding **$200/client/month gross contribution** before any operating and acquisition expenses (40% gross margin). Test higher prices ($597–$697) after proof of value.
- Potential add-on services: Google Business Profile optimization, posting, website local SEO, citations/content; tentative **$100–$200/month** additional price (models often use $150), but fulfillment cost/time not yet estimated.
- The unnamed fulfillment vendor claims rankings can improve quickly (about a week) via gamified **physical visits/drives** by local Google Guides/participants, offered white-label. They reportedly offered **at least 20 free pilot trials** initially, possibly more based on success. No verified independent documentation or contract yet. User is confident the method works based on prior experience. Potential Google policy risk remains; do not guarantee rankings or claim zero detection risk.
- Vendor reportedly cannot service some businesses lacking a usable public physical address, even though Google permits compliant service-area businesses to hide addresses. The vendor's eligibility rule is narrower than Google's GBP eligibility.
- Desired prospects: high-value, owner-operated local services with physical locations, solid reviews/ratings, room to improve map visibility, and enough conversion potential to justify recurring fees. User emphasizes a shop with 15 reviews ranking above shops with 300/500 may still get poor clicks; review parity matters as much as ranking.
- Go-to-market: remove perceived risk by providing a no-charge diagnostic / qualifying pilot, objectively measure gains, sell month-to-month with easy cancellation. Avoid promising a specific rank or revenue result.
- Working geography: Benicia, Vallejo, Fairfield, Concord, Napa and nearby Northern California cities. **First actual export covers Concord and Vallejo, not Benicia**.
- Discovery and rank assessment are distinct: use Outscraper to get listings and business details; score/filter candidates; only then buy 5x5 or 7x7 geo-grid scans for best candidates using a tool such as Whitespark or Local Falcon. Outscraper returned order is not a measured geo-grid ranking.

## Real progress

1. User signed up for **Outscraper**, uploaded its category list (`categories.xlsx`, reported 4,274 categories), and ran an initial auto-repair search.
2. First export (`Outscraper-20261015034444s0636.xlsx`) contains **150 rows, 150 distinct Google Place IDs; 96 Concord, 54 Vallejo; 148 operational** at export. Three queries: 87 for `auto repair shop, 94522, Concord, CA, US`; 54 for `auto repair shop, 94592, Vallejo, CA, US`; 9 for `auto repair shop, 94518, Concord, CA, US`. ZIP-query geography and results do not perfectly correspond.
3. A separate analysis workbook (`Google_Maps_Prospect_Analysis.xlsx`) contains Overview, Priority Leads (12), All 150, Scoring Guide. It is not yet in GitHub. Its scores are **heuristics, not validated predictions**.
4. Lead examples: Sonoma Auto Tech (Vallejo, 4.7 / 67 reviews, returned 11); The Repair Shop (Concord, 4.9 / 68, returned 22); Clayton Valley Auto Service (Concord, 4.8 / 64, returned 28); Gene's Auto Repair (Vallejo, 4.6 / 128, returned 15); TrueTest Auto Repair (Concord, 5.0 / 71, returned 12). These orders are per source query and not verified Maps positions.
5. Recommended first full test case was **The Repair Shop in Concord**. Still needs current eligibility and grid verification.

## Required research/decisions before scaling

- Get white-label vendor identity, methodology, contract, data and eligibility rules. Validate trials and outcome measurements.
- Verify **current** pricing, per-credit mechanics, API access, bulk upload and report export for Outscraper, Whitespark, Local Falcon, Local Viking, BrightLocal, Apify. Earlier chat prices are date-sensitive, not verified purchase quotes.
- Run baseline geographic grids at fixed center/radius/grid resolution/keyword/time settings, and repeat with same settings; track business outcomes as available.
- Select target verticals using review parity, address suitability, high job economics, category relevance, competition and geography. Avoid trying to sell competing clients mutually incompatible ranking guarantees in the same exact market.
- Run outreach tests, measure real response/meeting/trial-to-paid conversion and customer retention; model CAC and direct fulfillment cost.

## Read these files next

- `docs/PROJECT_CONTEXT.md` and `docs/BUSINESS_MODEL.md` for strategy and finances.
- `docs/TOOLS_AND_SOURCES.md` and `docs/PROSPECTING_PLAYBOOK.md` for data/API and ops.
- `docs/OUTSCRAPER_PILOT.md` for exported results and shortlist.
- `docs/NEXT_STEPS.md` for an executable test plan.

## Notes for future chats / assistants

- The owner favors concrete, cost-efficient tests rather than complex software before validation. Give practical proposals and work from actual uploaded/exported data when available.
- Distinguish **facts from user-reported vendor claims, analytical hypotheses, and unverified tool pricing**. Do not confuse result order with actual ranking.
- Tech preference if eventually building an app: **Base44 + React, Tailwind, shadcn/ui, lucide-react, react-router-dom, react-hook-form, recharts, react-quill, moment/date-fns, lodash, three.js, react-leaflet and @hello-pangea/dnd only**. Use Base44 Entities SDK (`@/entities`), User methods, and Core integrations; `createPageUrl('PageName')` for internal routes; defensive null checks and loading indicators; no new auth pages, avoid unsupported libraries. Keep API keys server-side and treat Google scraping/APIs as an external worker/service, not unsupported direct browser logic.
- Repository is currently public; do not commit unapproved private customer contact data, account secrets, or proprietary contracts.
