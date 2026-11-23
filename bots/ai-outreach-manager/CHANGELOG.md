# Changelog — AI Outreach Manager

Newest first. No invented usage numbers.

## 2026-11-24

### Live profile export

- Reconciled with the live export of 2026-11-22 (`profile.json`). Draft label removed from the description. The canonical description is that export.
- Harness: temporal. Title and avatar empty. `namedBy`: user.
- The export states the approval gate: draft, then Gmail only after an explicit OK. It also states the “AI Overview blogs” label and the handoff to Chief BD.
- The 2026-09-17 cut (Critical-only, no re-research of Sent or Waiting, wake on the approval backlog) is kept and labeled as not in the export.
- Chief BD’s export adds a target of at least 5 new sends a day and at least 4 follow-ups. Not copied as a result. No send counts were available.
- Clock still not exported. The 2026-09-16 failure still has no stored error string.
- Status: operational.
- Publisher names, inboxes, and drafts were not copied.


### Docs bootstrap

Historical record of the first folder, written before the live export was applied above.

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
