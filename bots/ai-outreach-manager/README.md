# AI Outreach Manager

Publisher outreach for AI-search visibility. Downstream of AEO Scout. Documented from the 2026-09-17 fleet scan. Not a live profile export.

| | |
|---|---|
| **Name** | AI Outreach Manager |
| **Title** | AI Outreach Manager |
| **Slug** | `ai-outreach-manager` |
| **agent uuid** | `7517ee94-aa4e-4233-8673-2fe3fa885de5` |
| **serverId** | `2980453` |
| **Owner** | Abhinav Singh |
| **Timezone** | Asia/Calcutta (IST) |
| **harness** | not captured — no live `profile.json` export |
| **Job** | Publisher outreach. Research only the Critical slice. Send email only after an explicit yes in this chat for that batch. Do not re-research Sent or Waiting. |
| **Volume class** | med-high at the 2026-09-17 scan (research volume). Not a token count. |
| **Change model** | Approved cut 2026-09-17 via Token Warden after an explicit yes: Critical-only; no re-research of Sent/Waiting; wake on the approval backlog. |

## When to use

- Restore the outreach bot if the live bot is lost: [PROFILE.md](PROFILE.md) + [OPERATIONS.md](OPERATIONS.md).
- Confirm it still wakes on the approval backlog, not on every new AEO Scout row, before someone adds a send cron.

## When not to use

Do not ask it to email a batch without an explicit yes in this chat for that batch. Do not ask it to work YouTube creators. That list is YT Outreach’s. Do not merge the lists. See [ANTI-JOBS.md](ANTI-JOBS.md).

## Links

- [PROFILE.md](PROFILE.md) — restore draft, not a live export
- [OPERATIONS.md](OPERATIONS.md) — Critical slice, no exported clock
- [ANTI-JOBS.md](ANTI-JOBS.md) — hard never-list
- [CHANGELOG.md](CHANGELOG.md) — docs bootstrap and the 2026-09-17 cut

## Operator notes

Evidence is the 2026-09-17 fleet scan. This pass did not re-read the live Grok Bot on 2026-11-24.

The exact clock was not exported. The scan saw a morning handoff on 2026-09-17. Do not invent a cron.

A routine failure was noted the day before, without a stored error string. Do not guess a fix.

Voice was not captured. Do not invent a catchphrase. Harness and avatar were not exported.

Do not republish send counters. Do not put publisher names, inboxes, or drafts in this folder.
