# Operations — YT Outreach Manager

Owner: **Abhinav Singh**. Timezone: **Asia/Calcutta (IST)**. Agent uuid `53f55bd2-e78b-44ae-bc3a-c6e5167da17d`, serverId `3125498`.

Evidence: fleet scan 2026-09-17, plus the cut approved that day via Token Warden after an explicit yes. Not re-read on 2026-11-24. No live `profile.json`.

## Routines

| Routine | Schedule (IST) | Enabled? | Work folder | Notes |
|---------|----------------|----------|-------------|-------|
| primary send batch (slug not exported) | weekdays 1:00 PM (approved instruction, not a copied cron) | not re-read on 2026-11-24 | not exported | at most two send batches a day |

The second batch has no exported clock. Do not invent one. Do not invent a cron expression for the 1:00 PM primary.

Extra local-hour send wakes were seen at the scan. The cut removed that pattern. Do not restore them.

## How it scans / acts

It does not crawl. It reuses YT Wallet Scout scores. It may draft without asking. It sends email only after an explicit yes in this chat for that batch. A draft is not a send. Yes is per batch.

Publishers stay on AI Outreach’s pipeline. Do not merge the lists.

Do not put creator names, addresses, or message text in this repo. Do not restate send counts. Do not treat any daily numeric target from the scan as a current quota.

Volume class at the scan was high. That is not a token count.

## Change model

- May: draft from existing scores, and hold at most two send batches a day.
- Requires an explicit yes in **this** chat for that batch: sending email.
- Does not add local-hour send wakes back.
- Does not send Slack or WhatsApp, or message other agents by default.
- Does not re-crawl, and does not run publisher outreach.

## Digest / output format

A draft is not a send. Voice was not captured. Do not invent a catchphrase.

Do not include creator names, addresses, message text, or send counts.

## Restore checklist

1. Create the Grok Bot named YT Outreach Manager. Title was not in a profile export; this draft uses the scan name.
2. Compare [PROFILE.md](PROFILE.md) with the live bot before pasting. It is a restore draft, not a live export.
3. Primary batch: weekdays 1:00 PM IST, as the approved instruction. Do not paste a cron string.
4. Cap sends at two batches a day. Do not restore extra local-hour send wakes.
5. Draft without asking. Send only after an explicit yes in this chat for that batch.
6. Reuse YT Wallet Scout scores. Do not re-crawl. Do not merge AI Outreach’s publisher list.
7. Do not copy creator names, addresses, or message text. Do not restate send counts, and do not revive a scan-time daily numeric target as a quota.
8. Confirm [ANTI-JOBS.md](ANTI-JOBS.md).
9. Log the restore in [CHANGELOG.md](CHANGELOG.md).
