# Operations — Ads Scout

Owner: **Abhinav Singh**. Timezone: **Asia/Calcutta (IST)**. Agent uuid `70b9e7e7-5a5c-487f-885e-b9ee6a6f633d`, serverId `3120543`. Harness: temporal. Live name: Ads Scout · Competitive Ads.

**On hold since 2026-09-22 23:51 IST.** Source: operator hold list. Reason recorded there: Abhinav said to stop operations until further notice. Resume when he says resume. The 2026-11-22 profile export shows the bot still exists.

## Routines

| Routine | Schedule (IST) | Enabled? | Work folder | Notes |
|---------|----------------|----------|-------------|-------|
| Google ads library check | Mondays 08:00, from the 2026-09-17 status note. Not in the profile export. Cron expression not copied | on hold since 2026-09-22. Do not enable from this document | `competitor-ads-intel` (scan path; routine folder slug not exported) | silent-delta at the scan. Daily removed 2026-09-16 |

A local snapshot said "No routines yet". The scan treated that as a stale mirror. The hold is the current operations order, whatever the mirror says.

## How it scans / acts

The export: watch the Google ads library.

The scan: weekly, not daily, silent-delta. It does not change the company's ads. No further cut on 2026-09-17. Leave the weekly shape alone unless a Monday run is empty noise, and do not make that judgment while the hold stands.

Do not copy library captures or competitor names into this repo.

Volume class at the scan: med on Mondays, low otherwise. Not a token count.

## Change model

- While the hold stands: do not run the check, and do not recreate a daily routine.
- Resume only when Abhinav says so.
- Own-account edits are Ads Guy, after approval in that bot's chat. That split is from the scan. The export does not name Ads Guy.
- Requires an explicit yes in **this** chat before a cadence change.

## Digest / output format

Silent-delta was the known mode at the scan: speak only on a material change. Do not send "(no change.)". The export does not restate that mode.

## Restore checklist

1. Create the Grok Bot named Ads Scout · Competitive Ads. Avatar: pebble, brown. Title was empty. Harness: temporal. `namedBy` is `user`.
2. Import [profile.json](profile.json) or paste the Canonical description from [PROFILE.md](PROFILE.md).
3. Leave operations stopped. The hold dates from 2026-09-22 23:51 IST and ends when Abhinav says to resume.
4. If he resumes: weekly, Mondays 08:00 IST, is the scan's clock, not a copied cron. Do not recreate the daily run unless he says yes to that.
5. Do not copy library captures or competitor names into the repo.
6. Confirm [ANTI-JOBS.md](ANTI-JOBS.md).
7. Log the restore in [CHANGELOG.md](CHANGELOG.md).
