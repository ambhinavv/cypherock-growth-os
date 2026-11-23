# Operations — YT Wallet Scout

Owner: **Abhinav Singh**. Timezone: **Asia/Calcutta (IST)**. Agent uuid `7bc3178d-132d-42d2-acb1-34708f32005b`, serverId `2915316`.

Evidence: fleet scan 2026-09-17, plus the cut approved that day via Token Warden after an explicit yes. Not re-read on 2026-11-24. No live `profile.json`.

## Routines

| Routine | Schedule (IST) | Enabled? | Work folder | Notes |
|---------|----------------|----------|-------------|-------|
| weekday priority slice (slug not exported) | silent-delta; old hour inferred near 08:00; cron not exported | not re-read on 2026-11-24 | not exported | never send "(no change.)" |
| full cohort (slug not exported) | Sunday 8:15 (approved instruction, not a copied cron) | not re-read on 2026-11-24 | not exported | not a weekday run |

Local mirrors said "No routines yet" while workdirs showed a morning rhythm. Treat that mirror as stale. Do not invent a cron expression from the inferred 08:00 hour or from Sunday 8:15.

Output around 08:15 on 2026-09-17 was scan evidence of the old morning rhythm, not a cron string.

## How it scans / acts

Hardware-wallet YouTube intel only. Weekdays are a priority slice and silent-delta. Sunday 8:15 IST is the full cohort.

No same-day full rerun after a failed or partial morning. Do not email creators. That is YT Outreach.

Do not commit creator lists or score files. Volume class at the scan was high. That is not a token count.

## Change model

- May: run the weekday priority slice, stay silent when there is no delta, and run the full cohort on Sunday at the approved 8:15 IST instruction.
- Requires an explicit yes in **this** chat: emailing creators, restoring a full daily cohort, or a same-day full rerun.
- Does not send Slack, WhatsApp, or message other agents by default.

## Digest / output format

Silent-delta on weekdays. Never send "(no change.)".

Do not include creator names, channel URLs, or scores in this repo.

## Restore checklist

1. Create the Grok Bot named YT Wallet Scout. Do not restore the earlier name YT Vigilante.
2. Compare [PROFILE.md](PROFILE.md) with the live bot before pasting. It is a restore draft, not a live export.
3. Weekdays: priority slice, silent-delta. Do not invent a cron. The old hour was only inferred near 08:00 IST.
4. Full cohort: Sunday 8:15 IST, as the approved instruction. Do not paste a cron string.
5. Do not add a same-day full rerun after a failed or partial morning.
6. Do not email creators. Do not commit creator lists or score files.
7. Confirm [ANTI-JOBS.md](ANTI-JOBS.md).
8. Log the restore in [CHANGELOG.md](CHANGELOG.md).
