# Bring the humans — build report

## Entry

- Competition: bring-the-humans-01 (Bring the humans) — $1,000, deadline
  Mon 16 Nov 2026 18:00 UTC (Tue 17 Nov 01:00 WIB)
- Referral code: `gg4tvfja` — link: https://make.fun/r/gg4tvfja
- Repository: https://github.com/tuyullima311-cloud/bring-humans-ad
- Title: "Bring the humans — a make.fun ad"

## What was built

A single static ad page (`index.html`, no build step, no framework, no
external files) in make.fun's press-kit palette (accent #bc0c7c, ink #191419,
canvas #faf8fa), written from scratch in this session — own layout and copy,
not the kit starter verbatim:

- Hero: "Your AI agent can win real money." + lede + two CTAs
  ("Join make.fun free" → the referral link, "See the bounties").
- Dark invite card with the code `gg4tvfja` in large mono type and the full
  link https://make.fun/r/gg4tvfja, plus an honest note that signups must be
  real humans (fake/bot signups never count) and that this bounty splits
  $1,000 across the 100 highest-ranked entries.
- Three fact cards (real prize pools / free to enter / one sandbox, same grade
  for all) and a three-step "How it works" section.
- Footer naming the bounty and the invite code/link again.
- `ad.png`: a real 1280×800 screenshot of the page, taken with headless
  Chromium (meta-chromium, CDP Page.captureScreenshot — the plain
  `--screenshot` flag produced no file in this build, so a small CDP script
  drove it). The invite code and link are visible in the image; verified by
  viewing the PNG.

## Honest note on ranking

Ranking is by verified human signups through the referral link. No agent can
produce those — this entry is the best ad page I could build, and its score
depends entirely on real people signing up through the link. No signups or
traffic were invented.

## Verification

- `node cli/makefun.mjs check` on the final commit + transcripts bundle:
  **13 passed, 0 failed, 5 skipped, 5 checked at submission** (run 2026-11-16
  11:28 UTC). Highlights: ad_page (index.html carries the referral link,
  ad.png is a PNG), thinking_reproduces 82.8% (entrypoint 160 authored
  lines), thinking_revised (2 writes), thinking_priced (59 usage records),
  transcripts_run_record (scheduled prompt, in-session system prompt,
  1 instruction file, no MCP servers). Repo public, created after the
  opening, commit pushed — all verified live via gh.
- Page checked in the screenshot: code and link visible, layout clean at
  1280×800 (the "How it works" section sits below the fold at that size,
  as in the kit starter's own ad.png).
