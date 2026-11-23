# Operations — Ads Guy

Owner: **Abhinav Singh**. Timezone: **Asia/Calcutta (IST)**. Agent uuid `42a6a03e-33a0-4cec-bb33-fd066665d5b7`, serverId `2945579`. Harness: temporal. Live name: Ads Guy · Performance Marketing.

Evidence: live profile export 2026-11-22 ([profile.json](profile.json)). Earlier cadence notes are from the 2026-09-17 fleet scan and are marked as not exported.

## Routines

| Routine | Schedule (IST) | Enabled? | Work folder | Notes |
|---------|----------------|----------|-------------|-------|
| Daily account review | 8:00 AM, stated in the 2026-11-22 profile. Cron expression not exported | not exported. The 2026-09-17 scan had recorded this review paused until the ads connector authenticates. The export does not restate that pause | `google-ads-intelligence`, `daily-reports` (scan paths, not in the export) | execute only after explicit approval |
| Weekly | clock not captured | left on at the 2026-09-17 scan. Not mentioned in the export | not exported | do not invent a clock |
| Monthly | clock not captured | left on at the 2026-09-17 scan. Not mentioned in the export | not exported | do not invent a clock |

## How it scans / acts

Own-account Google Ads review. Recommend profitable changes (ROAS, CPA, wasted spend). Execute only after explicit approval.

The scan called the ads connector Ryze AI and found it unauthenticated on 2026-09-17. The export does not mention the connector. Do not guess whether auth has returned.

The scan's only stored report was a blocked daily note from 2026-09-15. Do not quote it. Do not copy account ids, spend, or campaign structures into this repo.

Public ad-library monitoring was Ads Scout's lane at the scan. The export does not mention that split.

## Change model

- May: monitor the account and recommend a change, in plain-text WhatsApp-style updates.
- Requires explicit approval before execution. The export states that gate. It does not define a separate channel for the approval. Treat it as a yes in this chat for that change, which is the fleet rule, and say so when asking.
- Does not send WhatsApp. The voice is a format.
- Weekly and monthly clocks were not exported. Do not invent them.

## Digest / output format

Plain text, WhatsApp-style, aimed at profitable growth rather than vanity metrics.

Do not include account ids, spend, or campaign structures.

## Restore checklist

1. Create the Grok Bot named Ads Guy · Performance Marketing. Title and avatar were empty. Harness: temporal. `namedBy` in the export is `user`.
2. Import [profile.json](profile.json) or paste the Canonical description from [PROFILE.md](PROFILE.md).
3. Daily review at 8:00 AM IST is the exported clock. Do not invent a cron string.
4. Do not decide, from this folder, whether the 2026-09-17 pause is still on. Ask Abhinav.
5. Do not invent weekly or monthly clocks.
6. Confirm [ANTI-JOBS.md](ANTI-JOBS.md).
7. Log the restore in [CHANGELOG.md](CHANGELOG.md).
