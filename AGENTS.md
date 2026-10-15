# AI Handoff / Project Memory

Last updated: 2026-10-14 (Pacific). Repository: `SomeCallMeMitch/gmb`.

## Current direction — read before older project documents

Mitch has explicitly clarified the strategy:

- **Assume the provider can deliver its stated ranking improvement.** This is the planning assumption; no independently measured client outcome is yet recorded here. Do not make another vendor-effectiveness investigation a prerequisite for sales research or initial prospect work unless Mitch asks.
- Provider materials are branded **Jumper Local / Jumper Media**. The attached Agency Reseller Tool Kit was reviewed in the current project conversation. The raw PDF is not stored in this public repository.
- The provider supplies its own **ranking/geo-grid tool**. Prefer using it before recommending another paid grid platform.
- The immediate concrete offer is **three companies ranked for free**. Free trials can be offered to prospects. Earlier references to 20+ trials are background; use the latest three-company offer for immediate planning.
- Main business tasks: find businesses with commercially relevant keyword ranking opportunities, reach the owner or authorized buyer, demonstrate a measured improvement, then sell recurring service.
- Outscraper's returned order cannot select the best prospects. Actual grids for specific terms and locations are the priority. The existing export remains a useful inventory.
- The completed sales desk-research report is `docs/SALES_RESEARCH.md`. Read it before repeating general tool, sales, or prospecting research.

## What this project is

Build a small, scalable agency selling Google Maps visibility and related GBP/website/local SEO services to real local businesses. Outsourced fulfillment supplies the narrow ranking service; our agency controls prospect qualification, sales, customer relationships, reporting and complementary services.

Mitch favors practical, cost-efficient tests and has marketing/sales experience and local SEO familiarity. The business depends on provider delivery; under the current instruction, assume that part works and research the commercial process.

## Working business facts and assumptions

- Reported vendor cost: **$300 per business/month**.
- Working retail price: **$500/month**, giving **$200/client/month before operating/acquisition expenses**, a 40% margin before those costs.
- $597–$697 alternatives are ideas to test after learning from actual sales; not validated prices.
- GBP/site SEO add-ons of $100–$200/month have been discussed, but delivery scope/cost are not established.
- Proposed continuation: month-to-month with uncomplicated cancellation. State actual trial and continuation terms in advance; do not silently activate paid billing.
- Working geography: Benicia, Vallejo, Fairfield, Concord, Napa and nearby Northern California. First actual export is Concord/Vallejo, not Benicia.
- Prefer credible, owner-operated businesses with strong recent reviews relative to visible competitors, relevant search demand, address/provider fit, enough job contribution, capacity and a reachable buyer.
- A low-review shop outranking a much better-reviewed competitor may still struggle to win customers. Review parity matters alongside ranking.

## Existing work — do not repeat it blindly

1. Outscraper account created and initial category research performed.
2. Original export `Outscraper-20261015034444s0636.xlsx`: **150 distinct Place IDs**, 96 Concord, 54 Vallejo, 148 operational at export. Three source queries (87, 54 and 9 rows); source query geography does not perfectly match returned business geography.
3. Derived `Google_Maps_Prospect_Analysis.xlsx`: Overview, Priority Leads (12), All 150, Scoring Guide. Initial scores are screening heuristics, not validated predictions.
4. Candidates include Sonoma Auto Tech, The Repair Shop, Clayton Valley Auto Service, Gene's Auto Repair and others. Their current relevant grid rankings are **not yet established**.
5. The Repair Shop in Concord was previously suggested as a first study, not proven the best candidate.
6. Raw spreadsheets are not in GitHub or automatically available to future chats. Request attachments only if row-level work needs them; use documented summaries otherwise.
7. Completed current web research covers grid-based prospecting, review evidence, owner contact research, outreach, trial-to-paid process, measurement and economics. See `docs/SALES_RESEARCH.md` with its source register.

## Provider kit: useful operating guidance and ambiguities

The kit suggests verified physical address on GBP, 10+ positive reviews, 3.5+ rating, linked keyword-relevant site, 3–5 keywords, generally >70% coverage and ARP <12 with room to improve Top 3 share. Two relevant qualifying keywords strengthen a prospect.

Coverage is defined as top-20 presence; Top 3% is a separate measure. Do not reject 100% top-20 coverage alone if Top 3 share is weak. Ask provider to clarify inconsistent wording, ARP missing-result handling and actual grid geometry. Do not confuse 5x5 pins with miles across or radius.

Use the free trial commercially: qualify, agree terms and baseline, book the results appointment, activate, show matched before/after, offer continuation. A rank lift is not automatically a particular number of new customers.

## Next actions

1. Get provider-tool URL/access or actual grid exports/screenshots. Inspect pre-activation scanning, competitor views, reports and repeat settings.
2. Scan relevant terms for 5–10 shortlisted businesses.
3. Identify at least two relevant qualifying terms, compare reviews, verify address/site fit, and establish decision-maker access.
4. Select **three** businesses based on grids and buyer readiness, not Outscraper sequence.
5. Agree the free trial, continuation price/scope, and results review before activation.
6. Track actual buyer reach, show rate, trials, paid conversion, support effort, retention and reasons lost.
7. Deepen research based on the observed bottleneck. Build software only after the manual workflow repeats.

## Read next

- `docs/SALES_RESEARCH.md` — completed research and practical recommendations.
- `docs/DEEP_RESEARCH_PLAN.md` — revised sales-focused research scope.
- `docs/NEXT_STEPS.md` — current execution priorities.
- `docs/OUTSCRAPER_PILOT.md` — historical export and shortlist evidence.
- `docs/PROJECT_CONTEXT.md`, `BUSINESS_MODEL.md`, `TOOLS_AND_SOURCES.md`, `PROSPECTING_PLAYBOOK.md` — earlier detailed background. Where priorities conflict, this handoff and Mitch's latest instructions control.

## Data and communication discipline

Keep facts, user-reported terms, provider claims, planning assumptions, and recommendations identifiable. Show actual matched measurements; do not invent rank positions, search volumes, customer-loss estimates, outreach results or case studies. Do not send outreach without explicit authorization. Keep private contact lists, raw purchased data, credentials and confidential documents out of this public repository.

## Technical preferences if an app is later justified

Base44 with React, Tailwind, shadcn/ui, lucide-react, react-router-dom, react-hook-form, recharts, react-quill, moment/date-fns, lodash, three.js, react-leaflet and @hello-pangea/dnd only. Use Base44 Entities SDK (`@/entities`), User methods, Core integrations, and `createPageUrl('PageName')`. Defensive null checks and loading indicators; no new auth pages; keys server-side. Use an external provider/worker for unsupported scraping/API work.
