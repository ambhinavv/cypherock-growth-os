# Changelog — YT Wallet Scout

Newest first. No invented usage numbers.

## 2026-11-24

### Live profile export

- Reconciled with the live export of 2026-11-22 (`profile.json`). Draft label removed from the description. The canonical description is that export.
- Harness: temporal. Title and avatar empty. `namedBy`: user. Name in the export: YT Wallet Scout.
- The export says daily new-video scans, creator discovery, Cypherock mentions, competitor coverage, and outreach-ready scoring. It does not mention a weekday slice, a Sunday cohort, or email.
- The 2026-09-17 cut (weekday priority slice, silent-delta, Sunday 8:15 IST full cohort, no same-day full rerun) is kept and labeled as not in this export.
- Chief BD’s export says this scout uses silent-delta when empty and sits under Chief BD. That line is recorded in OPERATIONS. It was not copied into this bot’s canonical description.
- Status: operational.
- Creator lists and score files were not copied.


### Docs bootstrap

Historical record of the first folder, written before the live export was applied above.

- Registered in `bots/yt-wallet-scout/` from the 2026-09-17 fleet scan.
- Identity: uuid `7bc3178d-132d-42d2-acb1-34708f32005b`, serverId `2915316`.
- No live `profile.json`. This profile is a restore draft, not a live export.
- Harness, avatar, cron expression, and profile text were not exported. Voice was not captured.
- Live Grok Bot account was not re-listed for this commit.
- Creator lists and score files were not copied.

## 2026-09-17

### Approved cut

- Via Token Warden, after an explicit yes: weekday runs are a priority slice and silent-delta. Never send "(no change.)".
- Full cohort is Sunday 8:15 IST. That clock is the approved instruction, not a copied cron string.
- No same-day full rerun after a failed or partial morning.
- The old daily digest hour was inferred near 08:00 IST, with output around 08:15 that day. Local mirrors said "No routines yet" while workdirs showed a morning rhythm.
- The earlier name YT Vigilante was already renamed before the scan. This folder does not restore it.
- Volume class at the scan: high. Not a token count.

Historical picture: `bots/token-warden/baselines/2026-09-17.md`.
