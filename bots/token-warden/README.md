# Token Warden

Fleet token accountant for Abhinav’s Cypherock Grok Bots. First documented bot in this repo.

| | |
|---|---|
| **Name** | Token Warden |
| **Title** | empty in the 2026-11-22 export |
| **Slug** | `token-warden` |
| **agent uuid** | `a3a716db-daf8-43ab-8b84-6e1f5fba90d8` |
| **serverId** | `3765226` |
| **Owner** | Abhinav Singh |
| **Timezone** | Asia/Calcutta (IST) |
| **harness** | temporal |
| **Status** | Operational |
| **Job** | Watch every bot’s work, routines, and spend; find redundant processes and cadence waste; track weekly/total Grokbot subscription usage limits; propose concrete token savings. |
| **Volume class** | low |
| **Change model** | propose-only on fleet cuts. The 2026-11-22 profile also allows a standing reply to Chief Business Development Bot’s headroom asks, and a reply to a concrete token question from another bot. |

## When to use

- Daily (weekdays) and Monday deep-dive questions: what is wasting cadence, what overlaps, what to cut.
- Before adding a new routine or bot — check overlap + volume class vs [FLEET-BASELINE.md](FLEET-BASELINE.md).
- After a Usage & Billing screenshot — attach it so digests can do spend-vs-cap, not only relative waste.
- To restore the live bot if it is deleted: [PROFILE.md](PROFILE.md) + [OPERATIONS.md](OPERATIONS.md) + [profile.json](profile.json).

## When not to use

Token fleet only. Do not ask it to run ads, outreach, scraping, or product work. See [ANTI-JOBS.md](ANTI-JOBS.md).

## Links

- [PROFILE.md](PROFILE.md) — canonical persona (voice, cadence, anti-jobs), matched to the 2026-11-22 export
- [profile.json](profile.json) — sanitized restore aid, 2026-11-22 (replaces the 2026-09-17 export)
- [OPERATIONS.md](OPERATIONS.md) — routines, scan path, propose-only model, digest format
- [ANTI-JOBS.md](ANTI-JOBS.md) — hard never-list
- [USAGE-TRACKING.md](USAGE-TRACKING.md) — no live usage API; screenshot/paste method + 2026-09-17 snapshot
- [FLEET-BASELINE.md](FLEET-BASELINE.md) — distilled fleet scan (volume classes, overlap). Not token counts.
- [CHANGELOG.md](CHANGELOG.md) — 2026-09-17 bootstrap + first five approved fleet cuts
- [baselines/2026-09-17.md](baselines/2026-09-17.md) — full scan notes from that day

## Operator notes

Digests always report **relative waste**. They report **spend-vs-cap** only when a fresh Usage & Billing snapshot exists (see USAGE-TRACKING.md). Stay quiet if nothing is worth proposing — never send “(no change.)”.
