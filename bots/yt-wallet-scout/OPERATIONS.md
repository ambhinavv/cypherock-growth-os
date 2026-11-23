# Operations — YT Wallet Scout

Owner: **Abhinav Singh**. Timezone: **Asia/Calcutta (IST)**. Agent uuid `7bc3178d-132d-42d2-acb1-34708f32005b`, serverId `2915316`. Harness: temporal.

Evidence: live profile export 2026-11-22 ([profile.json](profile.json)). The 2026-09-17 cut is labeled. It is not in this export.

## Routines

| Routine | Schedule (IST) | Enabled? | Work folder | Notes |
|---------|----------------|----------|-------------|-------|
| New-video scan | daily, per the export. Clock not exported. Scan inferred an old hour near 08:00 | not exported | not exported | do not invent a cron |
| Full cohort | Sunday 8:15, from the 2026-09-17 cut. Not in this export. Not a copied cron | not exported | not exported | ask before restoring this as the live schedule |

Local mirrors said "No routines yet" at the scan while workdirs showed a morning rhythm. Treat that mirror as stale. It is not evidence about 2026-11-22.

## What the export says

Daily new-video scans. Creator discovery. Cypherock mentions. Competitor coverage. Outreach-ready creator scoring.

## What the 2026-09-17 cut said (not in this export)

- Weekdays: priority slice, silent-delta. Never send "(no change.)".
- Sunday 8:15 IST: full cohort.
- No same-day full rerun after a failed or partial morning.
- Do not email creators.

Chief BD’s export says: operate under Chief BD, silent-delta when empty, throttle per Token Warden before starving outreach. That is Chief BD’s instruction to the fleet, not a line in this profile.

Do not commit creator lists or score files. Volume class at the scan was high. That is not a token count.

## Change model

- May: scan and score, on the daily shape the export describes.
- Requires an explicit yes in **this** chat before emailing a creator. The export does not grant a send. YT Outreach Manager sends, after approval, at local business hours.
- Restoring the Sunday-only full cohort, or confirming that daily scans replaced it, needs Abhinav. Do not pick from this file.

## Digest / output format

The export does not define silent-delta. Chief BD’s export does, for an empty run. The 2026-09-17 cut did, for weekdays. Do not send "(no change.)".

Do not include creator names, channel URLs, or scores in this repo.

## Restore checklist

1. Create the Grok Bot named YT Wallet Scout. Do not restore the name YT Vigilante. Title and avatar were empty. Harness: temporal. `namedBy` is `user`.
2. Import [profile.json](profile.json) or paste the Canonical description from [PROFILE.md](PROFILE.md).
3. Do not invent a cron. The export says daily and does not state the hour.
4. Ask Abhinav whether the Sunday 8:15 full cohort is still the schedule before recreating it.
5. Do not email creators. Do not commit creator lists or score files.
6. Confirm [ANTI-JOBS.md](ANTI-JOBS.md).
7. Log the restore in [CHANGELOG.md](CHANGELOG.md).
