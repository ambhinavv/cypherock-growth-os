# Operations — AI Outreach Manager

Owner: **Abhinav Singh**. Timezone: **Asia/Calcutta (IST)**. Agent uuid `7517ee94-aa4e-4233-8673-2fe3fa885de5`, serverId `2980453`.

Evidence: fleet scan 2026-09-17. Not re-read on 2026-11-24. No live `profile.json`.

## Routines

| Routine | Schedule (IST) | Enabled? | Work folder | Notes |
|---------|----------------|----------|-------------|-------|
| not exported | clock not exported; morning handoff seen 2026-09-17 | not re-read on 2026-11-24 | not exported | do not invent a cron |

A routine failure was noted on 2026-09-16. No error string was stored. Do not guess a fix.

Approved cut 2026-09-17, via Token Warden after an explicit yes:

- Research only the Critical slice.
- Do not re-research Sent or Waiting.
- Wake when the approval backlog needs a human, not on every new scout row.

## How it scans / acts

Downstream of AEO Scout. Publisher outreach for AI-search visibility. It does not email a batch until there is an explicit yes in this chat for that batch.

YouTube creators are YT Outreach’s list. Do not merge the lists.

Do not put publisher names, inboxes, or drafts in this repo. Do not republish send counters.

Volume class at the scan was med-high because of research volume. That is not a token count.

## Change model

- May: research the Critical slice and say when the approval backlog needs a human.
- Requires an explicit yes in **this** chat for that batch: sending email.
- Does not wake on every new AEO Scout row.
- Does not message Slack, WhatsApp, or other agents by default.
- Does not run YouTube outreach.

## Digest / output format

No standing digest on every scout row. Wake when the approval backlog needs a human.

Voice was not captured. Do not invent a catchphrase. Do not include publisher names, inboxes, drafts, or send counters.

## Restore checklist

1. Create the Grok Bot named AI Outreach Manager. Title was not in a profile export; this draft uses the scan name.
2. Compare [PROFILE.md](PROFILE.md) with the live bot before pasting. It is a restore draft, not a live export.
3. Do not invent a cron. The exact clock was not exported. A morning handoff was seen on 2026-09-17.
4. Restore the 2026-09-17 cut: Critical-only; no re-research of Sent or Waiting; wake on the approval backlog.
5. Email only after an explicit yes in this chat for that batch.
6. Do not guess a fix for the 2026-09-16 routine failure. No error string was stored.
7. Keep YouTube creators off this list.
8. Confirm [ANTI-JOBS.md](ANTI-JOBS.md).
9. Log the restore in [CHANGELOG.md](CHANGELOG.md).
