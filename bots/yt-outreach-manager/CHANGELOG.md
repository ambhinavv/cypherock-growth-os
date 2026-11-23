# Changelog — YT Outreach Manager

Newest first. No invented usage numbers.

## 2026-11-24

### Live profile export

- Reconciled with the live export of 2026-11-22 (`profile.json`). Draft label removed from the description. The canonical description is that export.
- Live name: YT Outreach Manager · YouTube Outreach. Folder stays `yt-outreach-manager`.
- Harness: temporal. Title and avatar empty. `namedBy`: user.
- The export states the gate: enrich Scout or user leads, find a point of contact, personalize, send only after approval at local business hours, follow up, keep creator history.
- The 2026-09-17 cut (at most two batches a day, primary weekdays 1:00 PM IST, no re-crawl, extra local-hour wakes removed) is kept and labeled as not in the export.
- Chief BD’s export restates creator-local business hours and a target of at least 20 sends a day, still approval-limited. Not copied as a result.
- Status: operational.
- Creator names, addresses, message text, and send counts were not copied.


### Docs bootstrap

Historical record of the first folder, written before the live export was applied above.

- Registered in `bots/yt-outreach-manager/` from the 2026-09-17 fleet scan.
- Identity: uuid `53f55bd2-e78b-44ae-bc3a-c6e5167da17d`, serverId `3125498`.
- No live `profile.json`. This profile is a restore draft, not a live export.
- Harness, avatar, cron expression, and profile text were not exported. Voice was not captured.
- Live Grok Bot account was not re-listed for this commit.
- Creator names, addresses, message text, and send counts were not copied.

## 2026-09-17

### Approved cut

- Via Token Warden, after an explicit yes: at most two send batches a day. Primary batch weekdays 1:00 PM IST. That clock is the approved instruction, not a copied cron.
- Extra local-hour send wakes were seen at the scan. The cut removed that pattern. Do not restore them.
- Reuse YT Wallet Scout scores. Do not re-crawl. Draft without asking. Send email only after an explicit yes in this chat for that batch.
- Do not treat any daily numeric target from the scan as a current quota. Send counts are not restated here.
- Publishers stay on AI Outreach’s pipeline.
- Volume class at the scan: high. Not a token count.

Historical picture: `bots/token-warden/baselines/2026-09-17.md`.
