# AI Handoff / Project Memory

Last updated: 2026-10-14 (Pacific). Repository: `SomeCallMeMitch/gmb`.

## Latest direction — governs all earlier notes

Mitch has **not joined Jumper Local/Jumper Media** and **does not have access to its grid tool**. Do not describe that tool as currently available or make provider-tool access a prerequisite for research.

**Immediate task:** prepare/continue a comprehensive Deep Research study of the opportunity to start a Google Maps ranking agency with a **free one-week ranking demonstration before the prospect buys**. Study the business, market and sales model broadly using the Internet. The previous sales report is preliminary and does not complete this assignment.

- Accept the provider's ability to produce its described ranking improvements as a working assumption, per Mitch. Do not center the study on re-proving fulfillment.
- The provider has offered to rank **three businesses free**, and free prospect trials are part of the proposed model.
- The provider says it supplies a ranking/grid tool to members; any future role must be distinguished from tools usable before joining.
- Primary questions: demand, competitors and comparable offers, best customers, prospecting, reaching owners, trial-to-paid selling, pricing, costs/CAC, ongoing value, retention, workload and launch feasibility.
- A one-week ranking demonstration is not an assumed one-week revenue/customer guarantee.
- Read `docs/DEEP_RESEARCH_BRIEF.md` for the full assignment and `docs/PROVIDER_TOOLKIT_BRIEF.md` for the detailed PDF summary with page references.
- `docs/DEEP_RESEARCH_PROMPT.md` contains the copyable new-chat prompt.
- The raw PDF is not in GitHub; the page-referenced summary is available here. If the original is attached to the research chat, read it directly.
- Preserve useful earlier research, but do not treat `docs/SALES_RESEARCH.md` as a comprehensive opportunity study or repeat only its tactical recommendations.

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
7. Preliminary web research covers grid-based prospecting, review evidence, owner contact research, outreach, trial-to-paid process, measurement and economics. See `docs/SALES_RESEARCH.md` with its source register.

## Provider kit: useful operating guidance and ambiguities

The kit suggests verified physical address on GBP, 10+ positive reviews, 3.5+ rating, linked keyword-relevant site, 3–5 keywords, generally >70% coverage and ARP <12 with room to improve Top 3 share. Two relevant qualifying keywords strengthen a prospect.

Coverage is defined as top-20 presence; Top 3% is a separate measure. Do not reject 100% top-20 coverage alone if Top 3 share is weak. Ask provider to clarify inconsistent wording, ARP missing-result handling and actual grid geometry. Do not confuse 5x5 pins with miles across or radius.

Use the free trial commercially: qualify, agree terms and baseline, book the results appointment, activate, show matched before/after, offer continuation. A rank lift is not automatically a particular number of new customers.

## Next actions

1. Conduct the broad agency-opportunity study specified in `docs/DEEP_RESEARCH_BRIEF.md`.
2. Compare real current agency offers, practitioner/owner experiences, channels, verticals, pricing, acquisition/retention economics and operational demands.
3. Recommend whether/how to proceed, with scenarios and a 30/60/90-day plan.
4. Research affordable ranking/prospect qualification options usable before joining; evaluate a provider tool only as a future possibility.
5. After the opportunity study, choose implementation and trial steps based on its conclusions. Actual scans/outreach/trials are not prerequisites for completing the research.
6. Save sourced findings and decisions to the repo when authorized tools are available.

## Read next

- `docs/DEEP_RESEARCH_BRIEF.md` — full current opportunity-research assignment.
- `docs/PROVIDER_TOOLKIT_BRIEF.md` — detailed source PDF summary.
- `docs/DEEP_RESEARCH_PROMPT.md` — new-chat prompt.
- `docs/SALES_RESEARCH.md` — preliminary sources and tactical recommendations, not the final opportunity study.
- `docs/DEEP_RESEARCH_PLAN.md` — revised sales-focused research scope.
- `docs/NEXT_STEPS.md` — current execution priorities.
- `docs/OUTSCRAPER_PILOT.md` — historical export and shortlist evidence.
- `docs/PROJECT_CONTEXT.md`, `BUSINESS_MODEL.md`, `TOOLS_AND_SOURCES.md`, `PROSPECTING_PLAYBOOK.md` — earlier detailed background. Where priorities conflict, this handoff and Mitch's latest instructions control.

## Data and communication discipline

Keep facts, user-reported terms, provider claims, planning assumptions, and recommendations identifiable. Show actual matched measurements; do not invent rank positions, search volumes, customer-loss estimates, outreach results or case studies. Do not send outreach without explicit authorization. Keep private contact lists, raw purchased data, credentials and confidential documents out of this public repository.

## Technical preferences if an app is later justified

Base44 with React, Tailwind, shadcn/ui, lucide-react, react-router-dom, react-hook-form, recharts, react-quill, moment/date-fns, lodash, three.js, react-leaflet and @hello-pangea/dnd only. Use Base44 Entities SDK (`@/entities`), User methods, Core integrations, and `createPageUrl('PageName')`. Defensive null checks and loading indicators; no new auth pages; keys server-side. Use an external provider/worker for unsupported scraping/API work.
