# Operations — AEO Scout

Owner: **Abhinav Singh**. Timezone: **Asia/Calcutta (IST)**. Agent uuid `becdbf7e-437b-4bc7-9fdb-7733d8e3ac55`, serverId `2964531`.

Evidence: fleet scan 2026-09-17. Not re-read on 2026-11-24. No live `profile.json`.

## Routines

| Routine | Schedule (IST) | Enabled? | Work folder | Notes |
|---------|----------------|----------|-------------|-------|
| not exported | clock not exported; output seen ~08:10 IST on 2026-09-17 | not re-read on 2026-11-24 | not exported | morning AI-search visibility. Do not invent a cron string. |

There is no exported cron expression to recreate.

Approved cut 2026-09-17, via Token Warden after an explicit yes:

- Perplexity-first daily.
- Google/Bing at most 2-3 times a week, and stop on a challenge page or logged-out session.
- Silent if no delta. Never send "(no change.)".

## How it scans / acts

Perplexity is the daily check. Google and Bing are not a daily crawl. Stop that engine on a challenge page or a logged-out session. Do not keep crawling a blocked engine.

Handoff is a prospect queue for AI Outreach. Do not email anyone. Do not re-research Sent or Waiting. Do not invent citations or prospect records. Do not write prospect names into this repo.

Volume class at the scan was high. That is not a token count.

## Change model

- May: run the approved morning check and hand off a prospect queue.
- Requires an explicit yes in **this** chat: Google/Bing every day; email, Slack, WhatsApp, or messaging other agents.
- Silent if no delta.
- Does not run ads, YouTube, X, or token accounting.

## Digest / output format

Silent if no delta. Never send "(no change.)".

When there is a delta, the handoff is a prospect queue for AI Outreach, not an email.

## Restore checklist

1. Create the Grok Bot named AEO Scout. Title was not in a profile export; this draft uses the scan name.
2. Compare [PROFILE.md](PROFILE.md) with the live bot before pasting. It is a restore draft, not a live export.
3. Do not invent a cron string. The clock was not exported. The scan saw output around 08:10 IST on 2026-09-17.
4. Restore the 2026-09-17 cut: Perplexity-first daily; Google/Bing at most 2-3 times a week; stop on a challenge page or logged-out session; silent if no delta.
5. Confirm it does not email, and does not re-research Sent or Waiting.
6. Confirm [ANTI-JOBS.md](ANTI-JOBS.md).
7. Log the restore in [CHANGELOG.md](CHANGELOG.md).
