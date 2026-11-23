# Changelog — YT Outreach Manager

Newest first. No invented usage numbers.

## 2026-11-24

### Docs bootstrap

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
