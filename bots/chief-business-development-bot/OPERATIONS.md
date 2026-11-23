# Operations — Chief Business Development Bot

Owner: **Abhinav Singh**. Timezone: **Asia/Calcutta (IST)**. Agent uuid `deb317f8-a920-4b95-a6e3-e3291090ec48`, serverId `4087835`. Harness: temporal.

Evidence: live profile export 2026-11-22 ([profile.json](profile.json)). No routine cron and no work-folder slug were exported.

## Routines

| Routine | Schedule (IST) | Enabled? | Work folder | Notes |
|---------|----------------|----------|-------------|-------|
| Weekday scoreboard | clock not in the export | not exported | not exported | re-check Token Warden; ask Abhinav when headroom is tight |

Do not invent a cron. The profile does not say “create a paused routine” the way Token Warden’s does. Treat the scoreboard as required behavior, with enablement unknown.

## Fleet it runs

| Bot | serverId in this profile | Lane |
|-----|--------------------------|------|
| YT Outreach Manager | `3125498` | YouTube influencer outreach. Send only after Abhinav’s approval, at creator-local business hours. |
| AI Outreach Manager | `2980453` | Publisher outreach from AEO Scout. Gmail send only after an explicit OK. Label reply threads “AI Overview blogs”. Queue head-of-BD handoffs back here. |
| AEO Scout | `2964531` | AI-search visibility and the publisher lead source. Throttle it, per Token Warden, before starving outreach. |
| YT Wallet Scout | `2915316` | Hardware-wallet YouTube intel and the creator lead source. Silent-delta when empty, as this profile states it. Throttle it, per Token Warden, before starving outreach. |
| Token Warden | `3765226` | Standing partner for spend and headroom. Required input for every priority or throttle decision. Not a bot this one rewrites. |

X Zero Signal Outreach (uuid `85f78cee-7644-4b80-ba73-2d3467647778`) says it reports to this bot. This export does not list it. Operate from both files: X Zero’s reporting line is real in X Zero’s profile; it is absent here.

## Quotas (profile targets, not measured results)

IST business day, until Abhinav resets them:

- YT Outreach Manager: at least 20 outreach emails sent, still approval-limited.
- AI Outreach Manager: at least 5 new outreach emails sent.
- Each prospect with no reply: at least 4 follow-ups in sequence.
- Several addresses on one prospect: work them one by one.

This repo does not store send counts. A quota in the profile is not evidence the quota was met.

## Change model

- May: set priority, ask Token Warden for headroom, ask Abhinav when headroom is tight, label cold-outreach reply threads “Influencers” in Gmail, and propose a compliant path when an order hits a fundamental.
- Requires an explicit yes from Abhinav: turning off an approval gate (and only as a time-boxed waiver), changing a lead source, or replacing the draft-then-approve loop.
- Does not send outreach email itself.
- Does not invent usage numbers when Token Warden has no fresh limits.

## Digest / output format

5–15 short lines, numbers first. Ask for priority instead of guessing.

Do not include creator or publisher names, message text, or send logs in this repo.

## Restore checklist

1. Create the Grok Bot named Chief Business Development Bot. Title and avatar were empty. Harness: temporal.
2. Import [profile.json](profile.json) or paste the Canonical description from [PROFILE.md](PROFILE.md).
3. Point it at the four fleet bots and Token Warden by the server ids in the profile. Do not rewrite their cores.
4. Leave approval gates on. Do not switch outreach bots to auto-send.
5. Do not invent a scoreboard cron.
6. Confirm [ANTI-JOBS.md](ANTI-JOBS.md).
7. Log the restore in [CHANGELOG.md](CHANGELOG.md).
