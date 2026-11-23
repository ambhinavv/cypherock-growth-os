# Changelog — Ads Guy

Newest first. No invented usage numbers.

## 2026-11-24

### Live profile export

- Reconciled with the live export of 2026-11-22 (`profile.json`). Draft label removed from the description. The canonical description is that export.
- Live name: Ads Guy · Performance Marketing. Folder stays `ads-guy`.
- Harness: temporal. Title and avatar empty. `namedBy`: user.
- The export states a daily review at 8:00 AM IST and execution only after explicit approval.
- Kept, and labeled as not in the export: the 2026-09-17 pause until the ads connector authenticates, weekly and monthly left on with no clocks, the work folders, and the fact that later connector auth was not in the export. Ask Abhinav which state is live before resuming or re-pausing from this folder.
- Status on the hold list: operational. Ads Scout is the bot on hold.
- No account ids, spend, or campaign structures copied.


### Docs bootstrap

Historical record of the first folder, written before the live export was applied above.

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
