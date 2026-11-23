# Operations — AEO Scout

Owner: **Abhinav Singh**. Timezone: **Asia/Calcutta (IST)**. Agent uuid `becdbf7e-437b-4bc7-9fdb-7733d8e3ac55`, serverId `2964531`. Harness: temporal.

Evidence: live profile export 2026-11-22 ([profile.json](profile.json)). The 2026-09-17 cut is labeled where it appears. It is not in the export.

## Routines

| Routine | Schedule (IST) | Enabled? | Work folder | Notes |
|---------|----------------|----------|-------------|-------|
| AI-search visibility | daily, per the export. Clock not exported. Scan saw output ~08:10 IST on 2026-09-17 | not exported | not exported | do not invent a cron |

## What the export says

Monitor Google, Bing, and other AI search engines daily. Track Cypherock’s visibility, competitor mentions, citation sources, and country-level trends. Identify cited blogs and sites. Detect meaningful changes. Build a prioritized prospect database for AI Outreach Manager.

## What the 2026-09-17 cut said (not in the export)

Via Token Warden, after an explicit yes:

- Perplexity-first daily.
- Google and Bing at most two or three times a week. Stop that engine on a challenge page or a logged-out session.
- Silent if no delta. Never send "(no change.)".
- Do not email. Do not re-research Sent or Waiting.

This folder does not claim that cut is still what the live bot does. The exported profile describes a daily Google and Bing check.

Chief BD’s export says this scout sits under Chief BD and should be throttled, per Token Warden, before outreach quotas are starved. That line is in Chief BD’s profile, not in this one.

Volume class at the scan was high. That is not a token count. Do not write prospect names into this repo.

## Change model

- May: run the check the live profile describes, and hand off a prospect database.
- The export does not grant a send. Outreach sends belong to AI Outreach Manager, after an explicit OK in that bot’s chat.
- A return to the 2026-09-17 cap, or a confirmation that the daily Google and Bing check replaced it, needs Abhinav. Do not pick one from this file.

## Digest / output format

The export says it detects meaningful changes. It does not define silent-delta. The scan cut did. Use silent-delta only if that cut is confirmed still in force. Do not send "(no change.)" in either case: that refusal is a fleet habit, and the cut stated it outright.

## Restore checklist

1. Create the Grok Bot named AEO Scout. Title and avatar were empty. Harness: temporal. `namedBy` is `user`.
2. Import [profile.json](profile.json) or paste the Canonical description from [PROFILE.md](PROFILE.md).
3. Do not invent a cron. The export says daily and does not state the hour.
4. Ask Abhinav whether the 2026-09-17 Perplexity-first cap is still in force before recreating it. The exported profile does not include it.
5. Do not email from this bot. Do not copy prospect names into the repo.
6. Confirm [ANTI-JOBS.md](ANTI-JOBS.md).
7. Log the restore in [CHANGELOG.md](CHANGELOG.md).
