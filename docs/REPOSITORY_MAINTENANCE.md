# Repository Maintenance Protocol — AI Research and Project Continuity

**Effective:** 2026-10-15. **Repository:** https://github.com/SomeCallMeMitch/gmb (**public**, main branch). This is the authoritative, human-reviewable **project knowledge base**, not an automatic transcript mirror.

## Critical limitation — no automatic cross-chat synchronization

A file in GitHub cannot monitor and ingest private ChatGPT conversations by itself. Reading `AGENTS.md` also does not automatically cause every new chat to connect to GitHub or write files. A future assistant must have an **authorized, connected GitHub tool** and the user must direct it to the repo (or use an equivalent attached workflow). The process below makes updates routine **when the tool is available**, but **does not promise automatic updates to the repo without an active, authorized session**.

A scheduled GitHub Action also cannot access ChatGPT chat content merely by running on a timer. Full unattended synchronization would require an intentionally deployed integration with approved data access and secrets, outside the scope of this documentation change.

## New-chat start protocol

1. Access GitHub with the connected tool; confirm `SomeCallMeMitch/gmb` exists and the correct `main` branch.
2. Read `README.md`, `AGENTS.md`, `docs/NEXT_STEPS.md`, `docs/DEEP_RESEARCH_REPORT.md` (or its executive section), plus topic-specific docs. Do **not** rely solely on an earlier message or cached copy.
3. Check `docs/RESEARCH_CHANGELOG.md` for latest changes/decisions, and follow dated sources in current topic file.
4. Summarize active strategy, hypotheses, constraints and data gaps succinctly before making new plans; prefer current owner directives over older frozen research.
5. For a topic already researched, update the relevant document instead of starting a competing unsourced summary.

## In-session documentation and end-of-session GitHub sync

When the owner authorizes or asks to keep the project repo updated:

1. **Capture important new information as it is decided or verified**, including:
   - Newly discovered services/vendors/tools, exact price, plan, observed limitations, official source URL and check date.
   - Pilot scans: keyword, Place ID, 5x5 grid center/spacing/radius, date/time, raw/aggregate result reference, and any observed rank changes. Keep identifiable client records private.
   - Provider terms and trial constraints; distinguish vendor claim, actual contract, user report, experiment and independent evidence.
   - Revised unit economics, pricing decisions, lead scoring, scripts/offer changes and retention measurements.
   - Relevant discussion/review consensus, with dates, URLs and explicit bias/small-sample caveats.
   - Owner decisions and actions taken (including no-action blockers).
2. **Before writing, fetch the current GitHub file and its SHA**; preserve all relevant existing material and update rather than overwrite newer decisions. Avoid conflicting parallel updates to the same file.
3. Store **stable evergreen facts** in topic files. For new major dated research, add a separate `docs/<TOPIC>_YYYY-MM-DD.md`; link it from `README.md` and `AGENTS.md`. Only add new docs if they improve findability.
4. Add an entry to `docs/RESEARCH_CHANGELOG.md` with date, subject, source, major findings, files changed, outstanding verification items.
5. Update `docs/NEXT_STEPS.md` only when actual priorities shift and `AGENTS.md` only when handoff/owner instructions materially change. Prevent stale or mutually inconsistent handoffs.
6. Use concise commit messages. **Verify each affected GitHub file can be fetched after the write**, and disclose any failed writes or missing original binary/attachments.
7. At the end of a substantial research session, tell the owner **exactly which repo files were updated** and which research remains provisional. If no GitHub connector is available, say explicitly that nothing was committed; provide the text or ask for an authorized connection rather than claiming success.

## Information hierarchy (avoid stale assumptions)

1. **Latest explicit owner direction** and actually observed outcomes/contractual terms.
2. `AGENTS.md` for the current operating handoff, `docs/NEXT_STEPS.md` for next actions.
3. Newest topic-specific dated reports and `docs/RESEARCH_CHANGELOG.md`.
4. `docs/DEEP_RESEARCH_REPORT.md` for the completed October 15 business opportunity study; **do not downgrade its updated $697/$597 trial recommendations to old $500-only assumptions.**
5. Historical `BUSINESS_MODEL.md`, `TOOLS_AND_SOURCES.md`, `SALES_RESEARCH.md` and older briefs remain as references; note historical status where assumptions conflict.

## Evidence and formatting conventions

Use labels:
- **Observed/confirmed:** tool outputs, actual owner data, verified subscription checkout or committed trial outcomes; include date/measurement protocol.
- **Vendor-advertised:** pricing, trial, product feature or claim from its site/marketing materials; add source URL and checked date.
- **User-reported:** statements about provider demos, relationships, trial promises, costs or results not independently verified.
- **Third-party/anecdotal:** forum impressions/reviews with dates and bias caveats.
- **Planning assumption:** illustrative pricing, funnel conversion, score weighting and retention, with no claim it has happened.

Each research note should include: `Updated`, `Scope`, `Executive recommendation`, `Evidence table`, `Sources (direct links)`, `Unknowns`, `Owner decisions`, and `Next test` when relevant.

## Safety and data privacy

This GitHub repository is **public**. Do **not** commit:
- raw prospect exports with private contact/person details, user-provided proprietary sheets, confidential vendor PDFs or agreements, API tokens, credentials, billing details, personally identifying customer outcomes;
- full private chat transcripts or emails, or information from integrations beyond what's approved for public publication;
- unlicensed third-party article/forum copies in place of short sourced summaries.

The **150-business Outscraper pilot** is summarized in `docs/OUTSCRAPER_PILOT.md`; raw spreadsheets and provider PDF remain outside this repo. Keep future client grids, identifiers and lead contact CRM in restricted/private storage unless the owner explicitly authorizes publication.

## Suggested GitHub issue workflow (optional)

If a future chat lacks GitHub write permission, prepare a concise issue-ready summary or Markdown patch for the owner to post. A future authorized chat can pick up tracked items and commit them. Don't create an issue for every trivial conversation.

## Copy/paste prompt to open a new chat

> Work on my GMB Rank Improvements project in GitHub at https://github.com/SomeCallMeMitch/gmb. Read README.md, AGENTS.md, docs/NEXT_STEPS.md and the research changelog first, then topic-specific files. Treat this repo as our knowledge base. When we establish new findings or make decisions, update the relevant Markdown documents and changelog through the connected GitHub tool, verify your commits, and tell me what changed. The repo is public: don't upload private files or contact lists. If GitHub write access is unavailable, say so.

## Copy/paste end-of-chat sync request

> Sync the useful new research, decisions, testing notes and next steps from this conversation to SomeCallMeMitch/gmb. Update existing files rather than replacing useful information, append the changelog, verify GitHub writes, and list any items not saved.
