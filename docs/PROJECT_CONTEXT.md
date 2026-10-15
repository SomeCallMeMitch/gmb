# Project Context: Google Maps / GBP Visibility Agency

Updated 2026-10-14 PT. This document consolidates the user's stated requirements and research discussion, **not** a claim that the vendor or economics have been independently validated.

## Vision

Launch a low-overhead, repeatable agency selling improved visibility in Google's local/Maps search results to established owner-operated local businesses. Use a compelling grid-based baseline report to demonstrate currently missed search visibility; test results rapidly; convert interested owners to monthly recurring retainers. Scale through systematic lead discovery, rank analysis, proof and outreach rather than relying on networking alone.

The owner's edge is marketing/sales experience and practical familiarity with local SEO, GBP optimization and credible service-business marketing. The proposed vendor only provides a rank-related service; our business would control sales, prospecting, customer management, reporting and complementary on-site SEO / GBP work.

## User's hypothesis about fulfillment

- An **unnamed** white-label vendor has relationships with game companies and uses gamified local Google Guides / participants to drive to business locations, creating physical presence/engagement signals intended to influence local ranking.
- They say this can improve position on a timescale of about **one week** and have reportedly offered **20 free trials** initially, potentially increasing later.
- They **do not** handle on-page SEO or Google Business Profile optimization, leaving a significant opportunity for complementary agency services.
- Vendor cost is reportedly **$300 per location per month**, with **$500 per month** recommended retail price.
- Vendor has restrictions around address eligibility; a home-based handyman hiding their private address would not qualify for this vendor's offering. Hidden-address service-area businesses can still have legitimate GBPs and can still be served by conventional local SEO solutions.
- The owner considers the driving tactic proven based on personal experience and believes the risk of detection is low. The method may violate Google policies or lose effectiveness due to platform changes; business continuity plans should not require the tactic to remain permanently effective.

## The strategic difference: ranking vs. commercial outcomes

The owner specifically highlighted that a shop with **15 reviews** rising above competitors with **300–500 reviews** may not gain much incremental traffic/calls because consumers favor listings with greater review social proof. Thus, *ability to rank* is not the same as *ability to generate a return*. The target prospect should have enough review credibility and a good customer experience, not simply the lowest current position.

Qualification should consider:

- Review rating (e.g. 4.6–5.0), review count relative to rivals, and evidence of a strong actual business. More reviews do not automatically imply a better fit; compare within vertical and market.
- Current proximity-dependent ranking / average top-3 coverage on a grid for valuable terms.
- Physical customer-facing location suitability for the vendor and user experience; assess eligibility rather than incorrectly assuming any hidden-address business cannot rank.
- High-value, high-margin jobs / recurring customer economics. A single additional roofing or collision job may cover several months' retainer; low-ticket services need more volume.
- Website/GBP quality and opportunities for legitimate optimization.
- Independent owner decision-maker, realistic budget, manageable competition, and geographically relevant demand.
- Avoid clients with consistently poor ratings, obvious service-quality problems or misleading listings.

## Candidate verticals

### Highest interest (first-wave tests)
- Auto repair, auto body/collision, transmission, tire and specialty auto services: publicly visitable locations, review-heavy consumer decision processes, active Maps demand.
- Roofers, HVAC contractors, plumbing, garage door services, tree removal, water damage restoration: high customer value, but some are service-area businesses with no publicly visible staffed location and must be checked for vendor fit.

### Additional verticals to test
- Pest control, electricians, flooring contractors and stores, appliance repair, locksmiths, landscapers, auto glass, detailing/ceramic coating, oil change/brake specialists.
- Dentists / cosmetic dentistry, chiropractors, veterinarians, self-storage and other physical-location verticals.
- Attorneys and realtors were considered but were not selected as first tests; verify economics, buying journey and local-search importance by specialty rather than assuming they are unsuitable.

### Initial exact Outscraper category strings discussed
`auto repair shop`, `auto body shop`, `roofing contractor`, `hvac contractor`, `plumber`. Expansion categories discussed: `transmission shop`, `tire shop`, `car detailing service`, `electrician`, `garage door supplier`, `tree service`, `water damage restoration service`, `pest control service`, `flooring contractor`, `flooring store`, `appliance repair service`, `locksmith`, `heating contractor`, `air conditioning contractor`, `air conditioning repair service`, `landscaper`, `auto glass repair service`, `dentist`, `cosmetic dentist`, `chiropractor`, `veterinarian`, `self-storage facility`, `oil change service`, `brake shop`.

These were drawn from a user-supplied category workbook in the originating conversation. Check category availability and synonyms in the live Outscraper UI.

## Target geography

Initial focus: **Benicia, Vallejo, Fairfield, Concord**, expanding to **Napa** and adjoining Northern California markets. The first real export accidentally or deliberately used Concord and Vallejo zip-filtered queries, not Benicia; future query design should explicitly define city/catchment and avoid misinterpreting returned business city vs query text.

## Positioning and offer

Lead with a useful **free Maps visibility diagnostic**, showing where a company ranks across the area vs competitors for economically important phrases. If qualified and with written permission, offer a limited-time no-cost pilot where possible; use a matched pre/post baseline, avoid overclaiming causation, and make continuation **month-to-month** with uncomplicated cancellation.

Illustrative positioning, not approved final copy:

> See where your business is being missed on Google Maps. We'll map the neighborhoods where competitors appear ahead of you, then show you what a measured improvement effort looks like. No long-term contract; continue only if the service earns its place in your marketing budget.

Do not present artificial user interactions as organic customer traffic, conceal material fulfillment information if asked, or describe rankings / revenue as guaranteed.

## Commercial channels

- Highly targeted direct email with one verified, personalized observation and a link to a report. Follow legal and deliverability rules.
- Short telephone outreach to smaller owner-operated shops; first goal is permission to show an audit, not a hard sell.
- 45–60 second customized screen recording of a live geo-grid report versus direct competitors.
- Track contact -> response -> conversation -> pilot -> paid; benchmark in market instead of relying on general conversion claims.

## Sources of uncertainty

**Known:** Outscraper account created; actual auto-repair export produced; business model price/terms described by owner; proposed free-trial availability described by owner; 12 leads preliminarily scored.

**Claims not independently confirmed:** vendor's mechanism, ability to guarantee rapid lifts, undetectability, real conversion from lifts to customer calls, vendor trial and refund terms, whether all listed shops qualify, current API capabilities/prices.

**Important platform distinction:** Google business discovery endpoints/providers and geo-grid rank tracking solve distinct problems. Google Places API can discover businesses but does not provide a turnkey fixed-size multi-coordinate geo-grid ranking API equivalent to specialized rank trackers.
