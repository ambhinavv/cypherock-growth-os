# dr eggbot

On-demand Grok Bot designer. Builds a bot when asked. No schedule. Documented from the 2026-09-17 fleet scan. Not a live profile export.

| | |
|---|---|
| **Name** | dr eggbot |
| **Title** | dr eggbot |
| **Slug** | `dr-eggbot` |
| **agent uuid** | `ed49f58e-488b-47a2-aa52-38219dec0445` |
| **serverId** | `3651045` |
| **Owner** | Abhinav Singh |
| **Timezone** | Asia/Calcutta (IST) |
| **harness** | not captured — no live `profile.json` export |
| **Job** | Design or create a Grok Bot when Abhinav asks in this chat. Do not grow a cron, and do not run the marketing fleet. |
| **Volume class** | low at the 2026-09-17 scan (new that morning, no workdir) |
| **Change model** | on demand — create a bot only after an explicit ask in this chat |

## When to use

- Restore the designer if the live bot is lost: [PROFILE.md](PROFILE.md) + [OPERATIONS.md](OPERATIONS.md).
- Confirm it still has **no** routines before someone “helpfully” adds a morning digest.

## When not to use

Do not ask it to run ads, outreach, scraping, or token accounting. Those bots already exist. See [ANTI-JOBS.md](ANTI-JOBS.md).

## Links

- [PROFILE.md](PROFILE.md) — restore draft, not a live export
- [OPERATIONS.md](OPERATIONS.md) — no routines
- [ANTI-JOBS.md](ANTI-JOBS.md) — hard never-list
- [CHANGELOG.md](CHANGELOG.md) — docs bootstrap

## Operator notes

The scan found this bot created 2026-09-17 ~02:29 IST, with an empty store and no workdir. Role recorded then: on-demand designer (`CreateAgent`), not a scout.

The display name in the scan is lowercase **dr eggbot**. Keep that spelling unless a later live export shows a rename.

This pass did not re-read the live Grok Bot on 2026-11-24. If it has since grown routines, this folder is behind the live bot on that point, on purpose: the last known instruction was “do not add crons.”
