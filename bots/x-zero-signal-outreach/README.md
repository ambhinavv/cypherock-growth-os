# X Zero Signal Outreach

Finds people on LinkedIn who hold crypto and may need a cold wallet, watches them for a buying signal, and reaches out by email and LinkedIn when the signal scores 2 or higher. Sells Cypherock X Zero, Cypherock’s cold wallet. Reports to Chief Business Development Bot.

| | |
|---|---|
| **Name** | X Zero Signal Outreach |
| **Title** | empty in the 2026-11-22 export |
| **Slug** | `x-zero-signal-outreach` |
| **agent uuid** | `85f78cee-7644-4b80-ba73-2d3467647778` |
| **serverId** | `21209055` |
| **Owner** | Abhinav Singh |
| **Timezone** | Asia/Calcutta (IST) |
| **harness** | temporal |
| **Avatar** | empty in the export |
| **Status** | Operational |
| **Reports to** | Chief Business Development Bot, uuid `deb317f8-a920-4b95-a6e3-e3291090ec48` |
| **Job** | Signal-scored LinkedIn and email outreach for Cypherock X Zero. Templates need Abhinav’s approval before the first send. A reply, a new template, or a changed offer waits again. |

## When to use

- Weekday run, around 10:00 IST: scan for signals and send the touches that are due under an already approved template.
- Before the first send: draft the email and LinkedIn templates (first touch and follow-ups) and wait for explicit approval.
- A daily line to Abhinav and to Chief BD when there are new prospects, signals, sends, or replies. Stay quiet when nothing happened.

## When not to use

YouTube and publisher outreach, ads, strategy, and finance are other bots. See [ANTI-JOBS.md](ANTI-JOBS.md).

## Links

- [PROFILE.md](PROFILE.md) — canonical persona, from the 2026-11-22 export
- [profile.json](profile.json) — sanitized restore aid
- [OPERATIONS.md](OPERATIONS.md) — signals, sequence, approval, daily cap
- [ANTI-JOBS.md](ANTI-JOBS.md) — hard never-list
- [CHANGELOG.md](CHANGELOG.md) — documentation bootstrap

## Operator notes

Cypherock is not seedless. The profile forbids saying or implying that it is, and forbids invented product claims, prices, or discounts.

LinkedIn uses the signed-in browser on the bot computer. The profile caps the day at about 20 profile visits and 15 connection requests or messages, and says to stop if LinkedIn warns, limits, or challenges the account.

The tracker is one Google Sheet named `X Zero Prospect Tracker`, created only if Drive does not already have it. The sheet URL was not in the export. This folder stores no prospect rows.

Chief BD’s own profile does not list this bot. This profile does name Chief BD. Both are true of the exports.

The profile says to claim a bot inbox on first run and tell Abhinav the address. No address was in the export, and none is written here.
