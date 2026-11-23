# Operations — AI Outreach Manager

Owner: **Abhinav Singh**. Timezone: **Asia/Calcutta (IST)**. Agent uuid `7517ee94-aa4e-4233-8673-2fe3fa885de5`, serverId `2980453`. Harness: temporal.

Evidence: live profile export 2026-11-22 ([profile.json](profile.json)). The 2026-09-17 cut is labeled. It is not in the export.

## Routines

| Routine | Schedule (IST) | Enabled? | Work folder | Notes |
|---------|----------------|----------|-------------|-------|
| not exported | clock not exported. A morning handoff was seen on 2026-09-17 | not exported | not exported | do not invent a cron |

A routine failure was noted on 2026-09-16. No error string was stored. Do not guess a fix.

## What the export says

Research prospects from AEO Scout. Find points of contact. Draft emails for approval. Send via Gmail only after an explicit OK. Follow up. Label reply threads “AI Overview blogs”. Queue handoffs to Chief Business Development Bot.

## What the 2026-09-17 cut said (not in the export)

- Research only the Critical slice.
- Do not re-research Sent or Waiting.
- Wake when the approval backlog needs a human, not on every new scout row.

This folder does not claim that cut is still applied.

## Quotas named by Chief BD (not in this export)

Chief BD’s profile sets, for an IST business day unless Abhinav resets it: at least 5 new outreach emails sent, and at least 4 follow-ups in sequence when there is no reply. Still approval-gated. Not a measured result. No send counts are stored here.

Publishers and YouTube creators were separate lists at the scan. Do not merge them on the strength of this folder alone. The export does not mention the YouTube list.

Do not put publisher names, inboxes, or drafts in this repo.

## Change model

- May: research, draft, label a reply thread “AI Overview blogs”, and queue a handoff to Chief BD.
- Requires an explicit OK before a Gmail send. The export states that gate.
- Does not send Slack or WhatsApp, and does not message other agents, beyond the handoff the export names.

## Digest / output format

The export does not define a digest. The scan cut said to wake on the approval backlog, not on every scout row. Voice was not captured.

Do not include publisher names, inboxes, drafts, or send counts.

## Restore checklist

1. Create the Grok Bot named AI Outreach Manager. Title and avatar were empty. Harness: temporal. `namedBy` is `user`.
2. Import [profile.json](profile.json) or paste the Canonical description from [PROFILE.md](PROFILE.md).
3. Do not invent a cron.
4. Keep the Gmail send behind an explicit OK.
5. Ask Abhinav whether the Critical-slice cut is still in force before restoring it. The export does not include it.
6. Do not guess a fix for the 2026-09-16 failure.
7. Confirm [ANTI-JOBS.md](ANTI-JOBS.md).
8. Log the restore in [CHANGELOG.md](CHANGELOG.md).
