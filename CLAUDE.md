# CLAUDE.md — fmai-landingpage-proto
- Before acting, read: the header comments in index.html and fmai-lp-t1-exec.html (this
  repo has no docs; the pages self-document via HTML comments).
- Protocol: ~/code/working-style/WORKING-STYLE.md. PART A always; PART B (FMAI) applies
  here. That file wins over this one.
- Autonomy in this repo: propose-only — show diffs and stop. Sole exception per PART A:
  append-only pushes to WORKING-STYLE RECENT LESSONS, both-sides SHA check.
- Deploys/publishes run via the deployall and lpnew zsh functions (defined in ~/.zshrc);
  Josh runs them — manual and gated.
- Every LP carries the /request-demo form's 7 hidden UTM fields (utm_source, utm_medium,
  utm_campaign, utm_term, utm_content, referrer, landing_page) plus the UTM-capture
  script. Canonical example: fmai-lp-t1-exec.html.
- FMAI content rules (PART B) apply to all copy in these pages.
- Josh runs commits unless a one-time authorization in the session prompt says otherwise.

## Doc hygiene
- Durable docs record STATE, not PATH: current facts, ratified decisions, open questions. No
  "this session", no who-suggested-what, no correction history.
- Superseded before commit = delete. Superseded after commit = edit the entry in place to state
  what's now true — EXCEPT in DECISIONS.md, where a committed entry is immutable: the correction
  is a new entry, and the old one gets exactly one head-line, `SUPERSEDED IN PART by D<n>:
  <clause>` (or `SUPERSEDED by D<n>` for a whole-entry replacement). Policy: working-style
  playbooks/durable-records-playbook.md, DECISIONS.md LEDGER POLICY (D27).
- Provenance = one dated line per number. No epistemics paragraphs.
- Intake (meeting notes / transcripts) is a transform: keep decisions, facts, open questions;
  drop attribution, ordering, rejected options (park or drop).
- Method lessons about the assistant go to working-style RECENT LESSONS, never here (ONE EVENT,
  TWO RECORDS).
- Volatile numbers (prices, counts, statuses) live in WORKING.md with a date — never in
  DECISIONS.md; durable docs point at the source of truth instead.
- DECISIONS entry template: Decision / Reasons / Provenance line / Open questions. Nothing else.
