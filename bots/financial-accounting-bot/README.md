# Financial Accounting Bot

Keeps one Google Sheet of every paid marketing activity Cypherock pays for: how much, which month, which channel. Records what Abhinav supplies. Does not move money, and does not message partners.

| | |
|---|---|
| **Name** | Financial Accounting Bot |
| **Title** | empty in the 2026-11-22 export |
| **Slug** | `financial-accounting-bot` |
| **agent uuid** | `59c87f5b-5ade-43db-8483-9acc62698ea2` |
| **serverId** | `20258512` |
| **Owner** | Abhinav Singh |
| **Timezone** | Asia/Calcutta (IST) |
| **harness** | temporal |
| **Avatar** | empty in the export |
| **Status** | Operational |
| **Job** | One ledger sheet for paid marketing. Ask until the row is complete or he says to leave a gap on Open Items. Monday 10:00 IST nudge when something is still open. Quiet when nothing is. |

## When to use

- A payment went out, or a commitment was made: influencers, paid media, paid blogs, Meta Ads, Google Ads, Amazon Ads, partnerships, or a channel he names.
- Monday 10:00 IST: open items and live links still missing.
- A strategy, ads, or outreach question: point it at Cypherock Marketing Strategist, Ads Guy, or Chief Business Development Bot. This bot does not answer those.

## When not to use

It does not send, move, or approve money. It does not message partners. It does not give tax advice. See [ANTI-JOBS.md](ANTI-JOBS.md).

## Links

- [PROFILE.md](PROFILE.md) — canonical persona, from the 2026-11-22 export
- [profile.json](profile.json) — sanitized restore aid
- [OPERATIONS.md](OPERATIONS.md) — one sheet, the Monday nudge
- [ANTI-JOBS.md](ANTI-JOBS.md) — hard never-list
- [CHANGELOG.md](CHANGELOG.md) — documentation bootstrap

## Operator notes

The sheet name in the profile is `Cypherock Paid Marketing Ledger`. On first chat, look in Google Drive and create it only if it is missing. The URL was not in the export. It stays in the bot’s memory, not in this repo. One file. Extra structure is tabs, not new files.

No amounts, wallet addresses, transaction hashes, partner names, or invoice links are stored here. The profile’s column list is the schema. It is not a ledger.

The Monday nudge is the only routine the profile allows, unless he asks for another. Stay quiet when Open Items is empty.
