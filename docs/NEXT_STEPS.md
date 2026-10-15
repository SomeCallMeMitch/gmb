# Decisions, Open Questions and Next 30 Days

Updated 2026-10-14 PT. Prioritize fast, cheap, measurable market validation over building a large product before demand is proven.

## What has been decided

- The project is an agency selling **Google Maps visibility** and related local SEO services, not a software-only startup.
- The strategy is broad low-cost business discovery, selective geo-grid tracking, transparent before/after evidence and monthly recurring relationships.
- **Outscraper** is already in use; first category is **auto repair shop**; first actual data: 150 records in Concord/Vallejo.
- **Do not** use only the first ten Outscraper search results or assume returned order is a ranking. Favor good businesses with commercially meaningful opportunity, review parity and suitable addresses.
- An initial low-cost grid tool choice is **Whitespark Local Ranking Grids**; evaluate **Local Falcon** as an alternative if its reporting, prospect enrichment, Claude connector and API justify price differences.
- The proposed vendor service is narrow and outsourced. Other ongoing SEO and GBP services may be supplied separately.

## Unknowns to resolve

| Priority | Question | Proposed validation |
|---|---|---|
| P0 | Who is the actual white-label drive-ranking vendor? | Get company name, site, written terms and method description |
| P0 | Are the >=20 free trials real, fully free, and under our control? | Written offer: restrictions, start/end, automatic billing, trial capacity |
| P0 | What physical-address criteria must the client satisfy? | Ask vendor for exact eligibility examples; don't conflate with Google's service-area rules |
| P0 | Do ranking improvements recur consistently under a matched measurement framework? | Independent pre/post grid; fixed scan design, comparable untreated businesses where possible |
| P0 | Can the user/client see a material lift in qualified customer inquiries? | Access GBP/call/appointment data where authorized; distinguish rank from calls |
| P1 | Is Whitespark sufficient for automated exports, bulk imports and white-label reports? | Use 200 free credits to test UX, CSV/report output and competitor details |
| P1 | Is Local Falcon worth $24.99+ vs Whitespark $10/20? | Compare same term, center, radius, date and competitor analysis; review API feature gating |
| P1 | Are the 12 auto-repair leads independent owners with qualifying locations? | Quick manual verification and fresh review comparison |
| P1 | Does a personalized audit get prospect responses? | Send first 20 high-relevance emails/calls, measure response and meeting rates |
| P1 | What is the real cost of GBP / on-site SEO add-on fulfillment? | Time study, clear scope and contractor rates |
| P2 | Which vertical/city combos have strongest economics? | Compare auto repair, roofing, HVAC, auto body etc after first pilot |
| P2 | How much automation warrants a Base44 app? | Decide after 100–200 contacts or first recurring customers |

## Week-by-week action plan

### Week 1 — Vendor & tool validation

- [ ] Collect vendor identity and trial terms, cancellation, fulfillment reporting and risk allocation.
- [ ] Check Outscraper remaining free record allowance and reconcile actual source rows.
- [ ] Sign up to Whitespark's grid trial (200 credits advertised when last checked), optionally Local Falcon's 100-credit trial.
- [ ] Open existing 12-lead shortlist and select 3–5 that appear truly owner-operated and location-eligible.
- [ ] Select two commercially meaningful auto repair keywords and appropriate grid center/radius.

### Week 2 — Measured ranking diagnostics

- [ ] Run matching 5x5 geo-grids for 3 candidates x 2 keywords (150 credits baseline).
- [ ] Evaluate actual top 3/share and leading competitors' review counts.
- [ ] Select the two most compelling audit reports and export a client-friendly version.
- [ ] Screen independently owned shops by phone/site, avoiding misidentification of chains.
- [ ] Identify any additional local SEO/GBP weaknesses the agency can legitimately address.

### Week 3 — Sales and limited pilots

- [ ] Test 2–3 outreach scripts across email, calls and short personalized videos.
- [ ] Start a simple prospect log, opt-outs and follow-up dates.
- [ ] Aim for 3–5 permissioned pilot agreements if vendor conditions are appropriate.
- [ ] Lock before/after grid settings and event notes; track whether other GBP/site/review changes occur.

### Week 4 — Evaluate business viability

- [ ] Compare grids at comparable settings, plus other real indicators (calls, route requests, appointments) where accessible.
- [ ] Calculate reached owners, positive responses, actual meetings, trial-to-paid conversion, effort/cost per sale.
- [ ] Learn willingness to pay at $500 vs premium alternatives and whether clients would buy a $100–$200 SEO add-on.
- [ ] Decide: scale pilot, revise vertical/market, renegotiate vendor, or emphasize more durable GBP/website SEO fulfillment.

## MVP application idea (only after market validation)

A Base44 prospecting CRM with:

1. Market/city + business category selector.
2. Imports from Outscraper CSV/API with Place ID dedupe and source attribution.
3. Lead list with rating/reviews, address eligibility, chain flag, website, stage and opportunity score **with interpretable reasons**.
4. Geo-grid scans per keyword with dated baseline/follow-up visuals and exported reports.
5. Competitor review parity and top 3/grid coverage comparison.
6. Pipeline stages: discovered -> qualified -> audited -> contacted -> responded -> pilot -> paying -> retained/cancelled.
7. Communications templates (human-reviewed), reminders and follow-up schedule.
8. Basic business economics dashboard and CAC/retention/cohort metrics.

Do not bypass Base44 platform guardrails: use supported React/Tailwind/shadcn/lucide stack, `@/entities` and `@/integrations/Core`, defensive loading/null states and server-side API secrets; no new standalone auth system.

## Continuity checklist for the next ChatGPT session

1. Tell the assistant: “Read this repo's README and AGENTS.md, then docs/OUTSCRAPER_PILOT.md and NEXT_STEPS.md.”
2. If raw data are needed, reattach `Outscraper-20261015034444s0636.xlsx` and/or `Google_Maps_Prospect_Analysis.xlsx`, as they are **not** stored in this public repo.
3. Ask to confirm live grid vendor pricing before purchasing (pricing is date-sensitive).
4. Supply name/site of white-label fulfillment company if available; it is still a major open dependency.
5. After first grid report is generated, save actual keyword, timestamp, radius and pin positions before claiming gains.

## Definition of an informative first pilot

This project reaches its first meaningful milestone when it has (a) a clean list of 30+ screened, relevant prospects in one target market, (b) 3 independent actual geo-grid baselines with competitor comparisons, (c) 10+ documented owner outreach attempts with outcomes, and (d) at least one fully measured permissioned trial with both rank and business-action evidence when obtainable. This is a learning milestone, not a guarantee of ROI.
