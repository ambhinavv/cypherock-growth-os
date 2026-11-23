# YT Wallet Scout

Hardware-wallet and cold-wallet YouTube intelligence. Daily new-video scans, creator discovery, Cypherock mentions, competitor coverage, and scores meant for outreach.

| | |
|---|---|
| **Name** | YT Wallet Scout |
| **Title** | empty in the 2026-11-22 export |
| **Slug** | `yt-wallet-scout` |
| **agent uuid** | `7bc3178d-132d-42d2-acb1-34708f32005b` |
| **serverId** | `2915316` |
| **Owner** | Abhinav Singh |
| **Timezone** | Asia/Calcutta (IST) |
| **harness** | temporal |
| **Avatar** | empty in the export |
| **namedBy** | user |
| **Status** | Operational |
| **Job** | Daily YouTube scans of the hardware-wallet and cold-wallet space, plus creator discovery, Cypherock mentions, competitor coverage, and outreach-ready scores. |

## When to use

- The daily new-video scan the live profile describes.
- A creator score for YT Outreach Manager. Sending the email is that bot’s job, after approval.

## When not to use

It does not send creator email. Chief BD’s profile, not this one, says this scout operates under Chief BD, stays on silent-delta when a run is empty, and is throttled per Token Warden before outreach is starved. See [ANTI-JOBS.md](ANTI-JOBS.md).

## Links

- [PROFILE.md](PROFILE.md) — live description, plus the 2026-09-17 cut labeled as not exported
- [profile.json](profile.json) — sanitized restore aid, 2026-11-22
- [OPERATIONS.md](OPERATIONS.md) — daily scans in the export; Sunday cohort not in it
- [ANTI-JOBS.md](ANTI-JOBS.md) — hard never-list
- [CHANGELOG.md](CHANGELOG.md) — export reconciliation

## Operator notes

The live profile says daily new-video scans. It does not mention a weekday priority slice, silent-delta, or a Sunday full cohort.

The 2026-09-17 cut said weekdays are a priority slice and silent-delta, and the full cohort is Sunday 8:15 IST, with no same-day full rerun after a failed or partial morning. That cut is not in this export. Chief BD’s export does say “silent-delta when empty” for this scout. Both are recorded. This folder does not claim the Sunday cohort is still the live schedule.

The earlier name YT Vigilante was already renamed before the 2026-09-17 scan. Do not restore it. The export’s name is YT Wallet Scout.

Do not commit creator lists or score files. The old morning hour was inferred near 08:00 IST. Do not invent a cron.
