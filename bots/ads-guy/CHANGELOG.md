# Changelog — Ads Guy

Newest first. No invented usage numbers.

## 2026-11-24

### Docs bootstrap

- Registered in `bots/ads-guy/` from the 2026-09-17 fleet scan.
- Identity: uuid `42a6a03e-33a0-4cec-bb33-fd066665d5b7`, serverId `2945579`.
- No live `profile.json`. This profile is a restore draft, not a live export.
- Harness, avatar, routine slug, weekly clock, and monthly clock were not exported.
- Auth after this date is unknown. Daily stays documented as paused.
- Live Grok Bot account was not re-listed for this commit.
- Account ids, spend, campaign structures, and the 2026-09-15 note text were not copied.

## 2026-09-17

### Daily pause

- Daily review paused until the ads connector authenticates. The clock was inferred around 08:00 IST, not exported as a cron.
- The scan called that connector Ryze AI and found it unauthenticated.
- Weekly and monthly were left on because Abhinav skipped pausing them. Their clocks were not captured.
- The only report found was a blocked daily note from 2026-09-15.
- Volume class at the scan: low because the connector was blocked; would be med if auth returned. Not a token count.

Historical detail: `bots/token-warden/baselines/2026-09-17.md`.
