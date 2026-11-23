# Changelog — AI Outreach Manager

Newest first. No invented usage numbers.

## 2026-11-24

### Docs bootstrap

- Registered in `bots/ai-outreach-manager/` from the 2026-09-17 fleet scan.
- Identity: uuid `7517ee94-aa4e-4233-8673-2fe3fa885de5`, serverId `2980453`.
- No live `profile.json`. This profile is a restore draft, not a live export.
- Harness, avatar, cron expression, and profile text were not exported. Voice was not captured.
- Live Grok Bot account was not re-listed for this commit.
- Publisher names, inboxes, drafts, and send counters were not copied.

## 2026-09-17

### Approved cut

- Via Token Warden, after an explicit yes: Critical-only; no re-research of Sent or Waiting; wake on the approval backlog, not on every new scout row.
- Send email only after an explicit yes in this chat for that batch.
- Exact clock was not exported. The scan saw a morning handoff that day.
- A routine failure was noted on 2026-09-16 without a stored error string. No fix is guessed here.
- Volume class at the scan: med-high (research volume). Not a token count.

Historical picture: `bots/token-warden/baselines/2026-09-17.md`.
