# Operations — Ads Scout

Owner: **Abhinav Singh**. Timezone: **Asia/Calcutta (IST)**. Agent uuid `70b9e7e7-5a5c-487f-885e-b9ee6a6f633d`, serverId `3120543`.

Evidence: fleet scan 2026-09-17. Not re-read on 2026-11-24. No live `profile.json`.

## Routines

| Routine | Schedule (IST) | Enabled? | Work folder | Notes |
|---------|----------------|----------|-------------|-------|
| not exported | Mondays 08:00 (status note; cron expression not copied) | not re-read on 2026-11-24 | `competitor-ads-intel` (routine folder slug not exported) | weekly silent-delta; daily removed 2026-09-16 |

A local snapshot said "No routines yet". Treat that as a stale mirror. Routines are server-kept. Do not invent a cron string from the Monday 08:00 clock.

## How it scans / acts

Public competitive ad-library monitor only. Weekly, not daily. Known mode is silent-delta.

It does not change the company's ads. That is Ads Guy, after approval in that bot's chat.

Do not copy library captures or competitor names into this repo.

Volume class at the scan: med on Mondays, low otherwise. Not a token count.

## Change model

- May: run the Monday public-library check on the weekly silent-delta cadence.
- Daily was removed 2026-09-16. No further cut on 2026-09-17. Leave weekly unless a Monday run is empty noise.
- Requires an explicit yes in **this** chat before changing cadence, or before messaging anyone.
- Does not edit the company's ads, and does not edit Ads Guy.

## Digest / output format

Silent-delta. That is the known mode: speak only when there is a material change. Do not send "(no change.)".

Do not paste library captures or competitor names into this repo.

## Restore checklist

1. Create the Grok Bot named Ads Scout. Title was not in a profile export; this draft uses the scan name.
2. Compare [PROFILE.md](PROFILE.md) with the live bot before pasting. It is a restore draft, not a live export.
3. Weekly, Mondays 08:00 IST, silent-delta. Do not paste a cron expression. It was not copied.
4. Do not recreate a daily routine. Daily was removed 2026-09-16.
5. Work lived under `competitor-ads-intel`. The routine folder slug was not exported. "No routines yet" on a local snapshot is a stale mirror.
6. Do not change the company's ads.
7. Do not copy library captures or competitor names into the repo.
8. Confirm [ANTI-JOBS.md](ANTI-JOBS.md).
9. Log the restore in [CHANGELOG.md](CHANGELOG.md).
