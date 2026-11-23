# Ads Scout

Public competitive ad-library monitor. Mondays 08:00 IST, silent-delta. Weekly, not daily. Documented from the 2026-09-17 fleet scan. Not a live profile export.

| | |
|---|---|
| **Name** | Ads Scout |
| **Title** | Ads Scout |
| **Slug** | `ads-scout` |
| **agent uuid** | `70b9e7e7-5a5c-487f-885e-b9ee6a6f633d` |
| **serverId** | `3120543` |
| **Owner** | Abhinav Singh |
| **Timezone** | Asia/Calcutta (IST) |
| **harness** | not captured — no live `profile.json` export |
| **Job** | Public competitive ad-library monitor. Mondays 08:00 IST, silent-delta. Weekly, not daily. Do not change the company's ads. |
| **Volume class** | med on Mondays, low otherwise, at the 2026-09-17 scan. Not a token count. |
| **Change model** | Daily removed 2026-09-16. No further cut on 2026-09-17. Leave weekly unless a Monday run is empty noise. Own-account changes are Ads Guy, after approval in that bot's chat. |

## When to use

- Restore the weekly monitor if the live bot is lost: [PROFILE.md](PROFILE.md) + [OPERATIONS.md](OPERATIONS.md).
- Confirm it is still weekly and still silent-delta before someone adds the daily run back.

## When not to use

Do not ask it to change the company's ads. That is Ads Guy, after approval in that bot's chat. See [ANTI-JOBS.md](ANTI-JOBS.md).

## Links

- [PROFILE.md](PROFILE.md) — restore draft, not a live export
- [OPERATIONS.md](OPERATIONS.md) — weekly Monday clock, no copied cron
- [ANTI-JOBS.md](ANTI-JOBS.md) — hard never-list
- [CHANGELOG.md](CHANGELOG.md) — docs bootstrap and the 2026-09-16 cut

## Operator notes

Evidence is the 2026-09-17 fleet scan. This pass did not re-read the live Grok Bot on 2026-11-24.

The Monday 08:00 IST clock is from the bot's status note at scan time. The cron expression was not copied. Do not invent one.

Work lived under `competitor-ads-intel`. The routine folder slug was not exported. A local snapshot said "No routines yet"; treat that as a stale mirror.

Do not copy library captures or competitor names into this folder. Harness, avatar, and profile text were not exported. Known mode is silent-delta. Voice was not captured.
