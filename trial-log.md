# Trial log — Absurd Micro-Startup Pitch-Off

- Slug: `u-ricoxyz-absurd-micro-startup-pitch-off-12e33571`
- Prize: $2, top 10 (0.63/0.43/0.30/0.21/0.15/0.10/0.07/0.05/0.04/0.02)
- Deadline: 26 Nov 2026 11:25 WITA (2026-11-26T03:25:00Z)
- Gate: /output/entry.txt, 1–200 characters, one sentence
- Field (live, 24 Nov ~21:51 WITA): 434 submissions; leaderboard blind
- Judge: z-ai/glm-5.3-flash, pairwise; criteria: (1) names an absurdly
  specific micro-startup for lazy AI agents, (2) narrow/odd niche, not a
  general category + joke, (3) business sense — plausible buyer + plausible
  way to earn money, (4) lazy-agent fit — work runs with little effort,
  (5) crisp + funny in one read.

## Candidates rejected

| Candidate | Reason |
|---|---|
| Invoice-chasing agent (5% of whatever lands) | Mechanism already in field: "A debt-collection agency run by one lazy AI agent that chases unpaid invoices for other AI agents, keeping 10% of every payment it nags into existence" + "The Invoice Nag" (invoice: 3 hits) |
| Changelog ghostwriter for lazy agents | Already in field: "Changelog Ghostwriter for Lazy Agents" + "ShipNothing — the changelog for indie hackers who shipped nothing" (changelog: 2 hits) |
| Tab-closing valet (10 cents a tab) | Already in field: "A valet service that closes and files the 400 browser tabs other AI agents left open, charging 10 cents a tab" (tab: 3 hits) |
| Commit-message rewriter | Already in field: "The Commit-Message Rewriter for Lazy Agents" (commit: 1 hit) |
| Variable namer (a penny a name) | Already in field: "NameThatThing: a tireless agent names your variables, branches and files for a penny a name" (variable: 1 hit) |
| Calendar bodyguard | Already in field: "Calendar Bodyguard for Lazy Agents" (calendar: 1 hit) |
| Final_FINAL renamer | Already in field: "The Final_Final_v2 Renamer" (rename: 2 hits) |
| Newsletter unsubscriber ($4) | Already in field: "The $4 Newsletter Unsubscriber for Lazy Agents" (unsubscribe: 1 hit) |
| Queue-sitter / waitlist holder | Mechanism already in field twice: "We rent out idle AI agents as professional queue-standers… $5 a spot" + "QueueSitter… $0.20 an hour… hold their GPU queue spot" (queue: 3 hits) |
| Terms-of-service reader ($3, three killer clauses) | Already in field: "We charge $3 to have a lazy AI agent read your 400-page terms of service and send back only the three clauses that can ruin you" (terms: 1 hit) |

## Chosen entry

> PassRot rotates other agents' expiring passwords at 3 a.m. for $1 a rotation, so no agent ever wakes up to a locked account again.

- 130 characters, one sentence.
- Dup check: `python3 check_dup.py <titles> "<candidate>"` → PASS,
  max difflib 0.42 / Jaccard 0.09 (thresholds 0.75 / 0.6), field 434 titles.
- Mechanism check (manual grep in titles file): password 0, rotate 0,
  rotation 0, credential 0, login 0, expir 0. No password-rotation entry
  in the field. Nearest neighbours are different mechanisms: 3 a.m. cron
  failures / PR sighing / log butler / apology concierge / spreadsheet
  janitor (all 3 a.m. jobs, none about passwords); "Apology Texts for
  Locked-Out Airbnb Guests" is apology texts for human guests, not
  password rotation; "Overnight Memory Storage" keeps context warm while
  agents sleep, not passwords.
- Judge fit: names the startup (PassRot); niche is absurdly specific
  (expiring passwords, rotated at 3 a.m.); buyer is other lazy agents;
  payment is $1 per rotation; lazy fit is one automated rotation while
  everyone else sleeps.

## Trials

- v1: files written in this session (main.ts, README.md with 3 live
  make.fun badges, LICENSE MIT, trial-log.md, .makefun/owner.json).
  Preflight: `ENTRY_OUTPUT=/tmp/entry-test-1.txt node main.ts` (Node
  v24.22.1) → entry.txt 130 chars, 130 bytes, single line; README grep:
  3 `make.fun/badge/` lines, 0 shields.io. Committed
  `c00379874141abf78b9028f9d923936232cfe25f`.
- v1 bundle: `u-ricoxyz-absurd-micro-startup-pitch-off-12e33571-bundle-v1.tar.gz`,
  810,621 bytes, sha256
  `24513ce13b72f7b804a4aec86027cfd42274a230ad8c4a77d9fecde32dc75633`.
  Bundle warned "0 usage rows attached" (subagent rows flush only when
  the run completes — expected).
- v1 check (`--commit c0037987…`): **12 passed / 2 failed / 5 skipped /
  5 at submission**. FAILs: thinking_priced (0 usage rows, expected —
  coordinator re-bundles with --muse-usage after this run ends) and
  thinking_revised (all files written once, no revision yet). Passes
  include thinking_reproduces 95.7% (68/71 lines, main.ts 13 authored
  lines), thinking_own_work 68/71, license_osi, entrypoint node22.
  This trial-log revision is the genuine revision for thinking_revised.
- v2 bundle (after trial-log revision, commit
  `af05623d13c75fc5596c600ec5c7f0248c17ae21`):
  `u-ricoxyz-absurd-micro-startup-pitch-off-12e33571-bundle-v2.tar.gz`,
  815,606 bytes, sha256
  `baf2398b5c1674ef2b85efe9a7c33c89acb30e7b3fb90bd280f2e07af96cf5b4`.
- v2 check: **13 passed / 1 failed / 5 skipped / 5 at submission**.
  Only FAIL: thinking_priced (0 usage rows — expected, subagent rows
  flush at run end; coordinator re-bundles with --muse-usage).
  thinking_revised PASS (trial-log.md from 2 messages);
  thinking_reproduces 96.4% (82/85 lines), thinking_own_work 82/85.
- GitHub: repo `rwnliwan/u-ricoxyz-absurd-micro-startup-pitch-off-12e33571`
  created public; local branch master pushed as remote main (remote
  default is main); ls-remote HEAD = local HEAD `af05623d…`; tree clean.
  About set + verified via gh api: homepage
  `https://make.fun/c/u-ricoxyz-absurd-micro-startup-pitch-off-12e33571`,
  topics ["makefun"].
- Status: BUILD SELESAI, siap submit (menunggu ACC Septian per entry).
  TIDAK submit di sesi ini. No claim code written, no Drive folder.
