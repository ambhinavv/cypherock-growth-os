# Operations — YT Outreach Manager

Owner: **Abhinav Singh**. Timezone: **Asia/Calcutta (IST)**. Agent uuid `53f55bd2-e78b-44ae-bc3a-c6e5167da17d`, serverId `3125498`. Harness: temporal. Live name: YT Outreach Manager · YouTube Outreach.

Evidence: live profile export 2026-11-22 ([profile.json](profile.json)). The 2026-09-17 cut is labeled. It is not in the export.

## Routines

| Routine | Schedule (IST) | Enabled? | Work folder | Notes |
|---------|----------------|----------|-------------|-------|
| Send batch | after approval, at local business hours (the export). Weekdays 1:00 PM IST is the 2026-09-17 primary-batch instruction, not a copied cron, and not in the export | not exported | not exported | at most two batches a day was the cut, not the export |

The second batch has no exported clock. Do not invent one. Do not invent a cron for 1:00 PM.

Extra local-hour send wakes were seen at the scan. The cut removed that pattern. The export does not mention it.

## What the export says

Enrich Scout or user leads. Find points of contact. Personalize emails. Send only after approval, at local business hours. Manage follow-ups. Keep creator relationship history.

## What the 2026-09-17 cut said (not in the export)

- At most two send batches a day. Primary batch weekdays at 1:00 PM IST.
- Reuse YT Wallet Scout scores. Do not re-crawl.
- Draft without a separate ask. Send only after an explicit yes for that batch.
- Do not restore the extra local-hour send wakes.

## Quotas named by Chief BD (not in this export)

At least 20 outreach emails sent per IST business day, still approval-limited. At least 4 follow-ups if there is no reply. Several addresses on one prospect: work them one by one. Not a measured count.

Do not treat a daily number from the scan as a quota. Do not restate send counts. Do not put creator names, addresses, or message text in this repo.

## Change model

- May: enrich, find a contact, personalize, and hold a draft.
- Requires approval before a send, and the send waits for local business hours. The export states both.
- Does not send Slack or WhatsApp, or message other agents, as part of this job.
- Does not run publisher outreach.

## Digest / output format

A draft is not a send. Voice was not captured.

## Restore checklist

1. Create the Grok Bot named YT Outreach Manager · YouTube Outreach. Title and avatar were empty. Harness: temporal. `namedBy` is `user`.
2. Import [profile.json](profile.json) or paste the Canonical description from [PROFILE.md](PROFILE.md).
3. Keep sends behind approval, at local business hours.
4. Ask Abhinav whether the two-batch cap and the weekday 1:00 PM primary batch are still in force. They are not in the export.
5. Do not copy creator names, addresses, or message text. Do not restate send counts.
6. Confirm [ANTI-JOBS.md](ANTI-JOBS.md).
7. Log the restore in [CHANGELOG.md](CHANGELOG.md).
