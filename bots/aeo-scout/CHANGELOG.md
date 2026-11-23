# Changelog — AEO Scout

Newest first. No invented usage numbers.

## 2026-11-24

### Live profile export

- Reconciled with the live export of 2026-11-22 (`profile.json`). Draft label removed from the description. The canonical description is that export.
- Harness: temporal. Title and avatar empty. `namedBy`: user.
- The export says Google, Bing, and other AI search engines, daily, with a prospect database for AI Outreach Manager. It does not mention Perplexity, a weekly cap, or silent-delta.
- The 2026-09-17 cut (Perplexity-first, Google/Bing two or three times a week, silent if no delta, no email, no re-research of Sent or Waiting) is kept and labeled as not in the export. This folder does not claim the cut is still applied.
- Clock still not exported. Scan output was seen around 08:10 IST on 2026-09-17.
- Status: operational.
- Prospect names were not copied.


### Docs bootstrap

Historical record of the first folder, written before the live export was applied above.

- Registered in `bots/aeo-scout/` from the 2026-09-17 fleet scan.
- Identity: uuid `becdbf7e-437b-4bc7-9fdb-7733d8e3ac55`, serverId `2964531`.
- No live `profile.json`. This profile is a restore draft, not a live export.
- Harness, avatar, cron expression, and profile text were not exported.
- Live Grok Bot account was not re-listed for this commit.

## 2026-09-17

### Approved cut

- Via Token Warden, after an explicit yes: Perplexity-first daily; Google/Bing at most 2-3 times a week and stop on a challenge page or logged-out session; silent if no delta.
- Never send "(no change.)". Do not email anyone. Handoff is a prospect queue for AI Outreach. Do not re-research Sent or Waiting.
- Clock was not exported. The scan saw output around 08:10 IST. Volume class at that scan: high. Not a token count.

Historical detail: `bots/token-warden/baselines/2026-09-17.md`.
