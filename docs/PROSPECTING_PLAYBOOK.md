# Prospecting, Qualification and Sales Playbook

Updated 2026-10-14 PT. The objective is **a low-cost repeatable process for finding clients likely to benefit financially**, not merely anyone whose ranking might be moved.

## 1. Choose a market and category

Initial launch markets: Benicia, Vallejo, Fairfield, Concord; later Napa / adjacent areas. Start with a limited combination such as **auto repair shop in Concord and Vallejo** (already researched), then expand to auto body/collision, roofing, HVAC, plumbers etc after learning the category's business economics.

Use category, geographic boundary, and target phrase separately. An Outscraper query based on `94522, Concord` can return businesses in other ZIP codes; verify actual `city`, lat/lng and service catchment. **Query string is not the business address.**

## 2. Discover broadly, not just the visible top ten

Outscraper should return a broad slice of businesses by Maps category / query. Start 30 results/query when testing category completeness; expand to 50–100 or a bounding area if warranted. The existing pilot returned 150 total rows across three auto repair queries; this was well within the published first-500-record free tier.

Capture and retain **source query and returned sequence**, but do not label sequence as confirmed local rank. Review an actual local grid for that. The attractive client may appear beyond the first 10 results.

## 3. Clean and qualify

1. Deduplicate by `place_id` (then normalized name+address if absent).
2. Remove closed, irrelevant, outside-area, or misleading listings.
3. Flag chains/franchises and non-owner-operated businesses that may not have local decision-making power.
4. Check vendor-specific address suitability. Google-hidden service-area businesses may still be fine for GBP/website SEO, even if disqualified from the drive-based vendor.
5. Look for review credibility **relative to actual local top competitors**, not an arbitrary static count. Rating under 4.5 or much lower reviews than market incumbents may reduce sales/ROI potential.
6. Check website existence/quality, profile completeness, business category and service match, and likely job economics.
7. Check local competition to avoid conflicts among paying clients.
8. Flag promising businesses for grids, without asserting a particular rank.

### Example preliminary screening score (not yet validated)

Use 100 points as a convenient prototype, with actual rules recalibrated after early client results:

| Component | Max points | What to evaluate |
|---|---:|---|
| Reputation / review parity | 25 | Good average rating plus reviews comparable to existing winners |
| Commercial value | 20 | Margin per job, customer lifetime value, ability to pay |
| Preliminary Maps gap | 20 | Has evidence of rank opportunity, but not a fake precise Outscraper rank |
| Local business / address fit | 15 | Real local company, accessible decision maker and vendor eligibility |
| Website/GBP improvement potential | 10 | Obvious missing but fixable basics; don't reward spam |
| Outreach readiness | 10 | Usable contact route and compelling specific observation |

The already-produced `Google_Maps_Prospect_Analysis.xlsx` used a **different initial heuristic** and assigned several candidates scores of 100. Do not compare these with the new proposed score without explicitly versioning the model. The workbook's score is screening, **not a prediction of ranking or business results**.

## 4. Run geo-grid scans only on a shortlist

- Select 5 candidates per market/category at most initially. Run 5x5 grids for 2–3 commercial keywords each; 5 candidates x25 points x2 keywords = **250 credits** for one scan round.
- Choose meaningful terms such as `auto repair`, `auto repair shop`, `brake repair`, not only exact business categories. Keyword relevance varies by prospect.
- Use consistent center, radius/spacing, grid size, keyword, location, date/time and same rank measurement provider for baseline vs follow-up.
- Assess percentage of grid points in **top 3**, average visible rank, visibility by neighborhood, competitor review parity, and distance from search points.
- Don't present one rank from one query as a universal claim. A #4 may be #1 near the store and unranked 2 miles away.
- Keep both raw export and a shareable screenshot/report. Use neutral language like “measured at these grid points on this date”.

## 5. Build persuasive individual prospect audits

Each report should include: location, keyword(s), scan date/time, annotated grid, real top competitors (with their review evidence), geographic visibility gap, local buyer search intent, 2–3 credible opportunities, likely next actions, constraints and an invitation for a pilot. A colored red/yellow/green grid is easier to understand than a keyword ranking spreadsheet, but must be accurately labeled.

No promise of top-three placements, traffic, calls, customers or revenue until objectively supported (and even then describe past results rather than guaranteeing the future).

## 6. Outreach tests

- **Short owner-focused email:** a verified customized Maps observation and permission request to send a report; no invented customer-loss estimates.
- **Phone:** confirm owner/manager, explain the no-charge visibility audit in a sentence, offer to email link, end without a hard sell.
- **Short video:** 45–60 seconds walking through the prospect's actual grid/competitors.
- Keep compliance and unsubscribe/opt-out in mind for outbound campaigns.

### Draft outreach example

**Subject:** Google Maps visibility for [Business] in [City]

> I checked how [Business] appears in Google Maps for [keyword] across [area], and found a few neighborhoods where competing shops showed up ahead of you. I put together a short map report with the exact searches and locations. Would you like me to send it? No obligation.

Use only after an actual grid is measured; otherwise instead ask permission to create a free audit.

### Trial invitation example

> If your location qualifies, we can offer a limited no-cost pilot with an agreed baseline report and follow-up scan. We'll show what changed; you decide whether ongoing work makes financial sense. There's no long-term contract.

This is an **offer concept** subject to vendor trial terms and client consent, not an already available public guarantee.

## 7. Measurement + attribution

**Lead-generation funnel:** identified -> qualified -> report created -> outreach sent -> positive response -> meeting -> trial accepted -> paid customer -> retained at 30/90/180 days. Monitor reply and show rates, time to close, CAC and gross monthly contribution.

**Rank evidence:** fixed-grid top-three coverage and average rank, competitor details, keyword specificity, pre/post measurement settings.

**Business evidence:** GBP performance metrics (where owner grants access), call tracking if consented and configured, booked appointments, qualified inquiries, closed jobs, realized margin and client retention. Rank gains alone are insufficient proof of profit.

## 8. Pilot experimental discipline

If free trials are real, don't consume all 20 just acquiring customers. Reserve some for matched control or untreated comparisons and repeated scans. Record exactly what else changed (reviews, GBP categories, SEO content, site edits, competitors' status, local events) to avoid misattributing improvements to one intervention. Run baseline then check on days 7, 14 and 30 if resources permit, not only the best screenshot from a single week.

## 9. Automation plan if validated

Stage 1: manual Outscraper CSV + spreadsheet/AI scoring; stage 2: scheduled Outscraper API -> Base44 Entities -> dashboards; stage 3: optional geo-grid provider API/CSV -> trend storage -> templated personalized audit -> outreach CRM. Prioritize Place ID dedupe and explicit versioned source and rank evidence.

Avoid automating mass interactions that misrepresent genuine customer engagement. Compliant SEO services, geo-grid monitoring and business discovery should remain useful if the drive-based fulfillment partnership ends.
