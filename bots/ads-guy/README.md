# Ads Guy

Own-account ads reviewer. Propose only. Documented from the 2026-09-17 fleet scan. Not a live profile export.

| | |
|---|---|
| **Name** | Ads Guy |
| **Title** | Ads Guy |
| **Slug** | `ads-guy` |
| **agent uuid** | `42a6a03e-33a0-4cec-bb33-fd066665d5b7` |
| **serverId** | `2945579` |
| **Owner** | Abhinav Singh |
| **Timezone** | Asia/Calcutta (IST) |
| **harness** | not captured — no live `profile.json` export |
| **Job** | Own-account ads review. Propose only. No bid, budget, ad, keyword, or campaign edit without an explicit yes in this chat for that change. |
| **Volume class** | low at the 2026-09-17 scan because the ads connector was blocked; would be med if auth returned. Not a token count. |
| **Change model** | Daily review paused 2026-09-17 until the ads connector authenticates. Weekly and monthly were left on. Do not resume daily from this document. |

## When to use

- Restore the reviewer if the live bot is lost: [PROFILE.md](PROFILE.md) + [OPERATIONS.md](OPERATIONS.md).
- Confirm the daily review is still paused before someone turns it back on. Auth after 2026-11-24 is unknown.

## When not to use

Do not ask it to scan public ad libraries. That is Ads Scout. Do not ask it to edit a bid, budget, ad, keyword, or campaign without an explicit yes in this chat for that change. See [ANTI-JOBS.md](ANTI-JOBS.md).

## Links

- [PROFILE.md](PROFILE.md) — restore draft, not a live export
- [OPERATIONS.md](OPERATIONS.md) — daily paused; weekly and monthly clocks not captured
- [ANTI-JOBS.md](ANTI-JOBS.md) — hard never-list
- [CHANGELOG.md](CHANGELOG.md) — docs bootstrap and the 2026-09-17 pause

## Operator notes

Evidence is the 2026-09-17 fleet scan. This pass did not re-read the live Grok Bot on 2026-11-24.

The scan called the ads connector Ryze AI and found it unauthenticated. The only report found was a blocked daily note from 2026-09-15. This folder does not quote that note.

Daily review was inferred around 08:00 IST. That is not an exported cron. Do not invent one. Do not resume daily from this document. Auth after 2026-11-24 is unknown, so daily stays documented as paused.

Weekly and monthly were left on because Abhinav skipped pausing them. Their clocks were not captured. Do not invent them.

Notes lived under `google-ads-intelligence` and `daily-reports`. The routine slug was not exported.

Voice from the scan: short WhatsApp-style updates. WhatsApp-style is a format, not a WhatsApp send. Harness and avatar were not exported. Do not write account ids, spend, or campaign structures into this folder.
