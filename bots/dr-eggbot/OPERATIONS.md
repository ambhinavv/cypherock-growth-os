# Operations — dr eggbot

Owner: **Abhinav Singh**. Timezone: **Asia/Calcutta (IST)**. Agent uuid `ed49f58e-488b-47a2-aa52-38219dec0445`, serverId `3651045`.

Evidence: fleet scan 2026-09-17 ~16:00 IST. Created that morning ~02:29 IST. Empty store, no workdir, no routines. Not re-verified on 2026-11-24.

## Routines

| Routine | Schedule (IST) | Enabled? | Work folder | Notes |
|---------|----------------|----------|-------------|-------|
| — | — | none | none at scan time | do not add a digest “so it matches the fleet” |

There is no cron to recreate. Adding one would contradict the only ops fact this repo has.

## How it scans / acts

It does not scan the fleet. Token Warden does that.

When asked to design a bot, the output is a definition: name, one job, anti-jobs, schedule (or none), and which existing bot already covers the work. Creation waits for an explicit ask.

New bots that should survive a lost computer get a folder under `bots/` in this repo, copied from `bots/_template/`, with no secrets and no contact lists.

## Change model

- May: discuss a design in this chat.
- Requires an explicit ask in **this** chat: creating a bot, skill, or routine; editing or deleting one.
- Does not message other agents by default.
- Does not run marketing jobs itself.

## Digest / output format

No standing digest. A design reply is a short spec, not a report of other bots’ work.

## Restore checklist

1. Create the Grok Bot named dr eggbot, title dr eggbot. Keep the lowercase name unless the live bot was renamed.
2. Compare [PROFILE.md](PROFILE.md) with the live bot before pasting.
3. Confirm it has **no** routines. Do not create paused digests.
4. Confirm [ANTI-JOBS.md](ANTI-JOBS.md).
5. Log the restore in [CHANGELOG.md](CHANGELOG.md).
