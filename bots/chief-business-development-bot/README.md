# Chief Business Development Bot

Runs the outreach and scout fleet for Cypherock. Sets daily send quotas, protects approval gates, and checks Token Warden before it throttles a lane. It does not send the outreach itself.

| | |
|---|---|
| **Name** | Chief Business Development Bot |
| **Title** | empty in the 2026-11-22 export |
| **Slug** | `chief-business-development-bot` |
| **agent uuid** | `deb317f8-a920-4b95-a6e3-e3291090ec48` |
| **serverId** | `4087835` |
| **Owner** | Abhinav Singh |
| **Timezone** | Asia/Calcutta (IST) |
| **harness** | temporal |
| **Avatar** | empty in the export |
| **Status** | Operational |
| **Job** | Run YT Outreach Manager, AI Outreach Manager, AEO Scout, and YT Wallet Scout. Keep their approval gates. Ask Token Warden before a throttle. Ask Abhinav when headroom is tight. |

## When to use

- Weekday scoreboard: which lane is behind its quota, which scout to throttle first, what to ask Abhinav.
- Before changing which lane or scout stays alive.
- When a fleet bot looks expensive or hung, after a Token Warden check.
- Gmail label “Influencers” on cold-outreach reply threads. That label stays here, not with Mr. Executive Assistant.

## When not to use

It does not send outreach email. It does not run ads, diagnose hung bots (that is Bot Doctor), or act as the general executive assistant. See [ANTI-JOBS.md](ANTI-JOBS.md).

## Links

- [PROFILE.md](PROFILE.md) — canonical persona, from the 2026-11-22 export
- [profile.json](profile.json) — sanitized restore aid
- [OPERATIONS.md](OPERATIONS.md) — quotas, gates, Token Warden checks
- [ANTI-JOBS.md](ANTI-JOBS.md) — hard never-list
- [CHANGELOG.md](CHANGELOG.md) — documentation bootstrap

## Operator notes

The profile names four fleet bots by server id, plus Token Warden (`3765226`) as the standing headroom partner:

- YT Outreach Manager — serverId `3125498`
- AI Outreach Manager — serverId `2980453`
- AEO Scout — serverId `2964531`
- YT Wallet Scout — serverId `2915316`

X Zero Signal Outreach’s own profile says it reports to this bot (uuid `deb317f8-a920-4b95-a6e3-e3291090ec48`). This bot’s export does not list X Zero. Both facts are recorded. Neither file was edited to hide the gap.

The export names a weekday scoreboard and does not give it a clock. Do not invent one. Quotas below are the profile’s daily targets, not a measured result. This repo has no send counts.

No seedless product claims. Cypherock is not described as seedless.
