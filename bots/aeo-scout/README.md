# AEO Scout

Daily AI-search visibility for Cypherock. Tracks citations and builds a prospect list for AI Outreach Manager.

| | |
|---|---|
| **Name** | AEO Scout |
| **Title** | empty in the 2026-11-22 export |
| **Slug** | `aeo-scout` |
| **agent uuid** | `becdbf7e-437b-4bc7-9fdb-7733d8e3ac55` |
| **serverId** | `2964531` |
| **Owner** | Abhinav Singh |
| **Timezone** | Asia/Calcutta (IST) |
| **harness** | temporal |
| **Avatar** | empty in the export |
| **namedBy** | user |
| **Status** | Operational |
| **Job** | Monitor Google, Bing, and other AI search engines daily for Cypherock’s visibility, competitor mentions, citation sources, and country-level trends. Hand a prioritized prospect database to AI Outreach Manager. |

## When to use

- The daily visibility check described in the live profile.
- A prospect handoff for AI Outreach Manager. Chief Business Development Bot’s profile says this scout operates under Chief BD, and that it should be throttled, per Token Warden, before outreach is starved.

## When not to use

Sending the outreach is AI Outreach Manager, and only after an explicit OK in that bot’s chat. See [ANTI-JOBS.md](ANTI-JOBS.md).

## Links

- [PROFILE.md](PROFILE.md) — live description, plus the 2026-09-17 cut labeled as not exported
- [profile.json](profile.json) — sanitized restore aid, 2026-11-22
- [OPERATIONS.md](OPERATIONS.md) — what the export says, and what the scan cut said
- [ANTI-JOBS.md](ANTI-JOBS.md) — hard never-list
- [CHANGELOG.md](CHANGELOG.md) — export reconciliation

## Operator notes

The live profile says Google, Bing, and other AI search engines, daily. It does not mention Perplexity, a weekly cap, or silent-delta.

The 2026-09-17 approved cut said the opposite about frequency: Perplexity-first daily, Google and Bing at most two or three times a week, stop on a challenge page or a logged-out session, silent if there is no delta. That cut is not in the export. This folder does not claim it is still applied, and it does not delete the record of the cut.

The clock was not exported. The scan saw output around 08:10 IST on 2026-09-17. Do not invent a cron. Do not put prospect names in this folder.
