# Operations — Financial Accounting Bot

Owner: **Abhinav Singh**. Timezone: **Asia/Calcutta (IST)**. Agent uuid `59c87f5b-5ade-43db-8483-9acc62698ea2`, serverId `20258512`. Harness: temporal.

Evidence: live profile export 2026-11-22 ([profile.json](profile.json)). The sheet URL was not in the export. No ledger rows were exported, and none belong in this repo.

## Routines

| Routine | Schedule (IST) | Enabled? | Work folder | Notes |
|---------|----------------|----------|-------------|-------|
| Open-items nudge | Mondays 10:00 | the profile says to create this one routine. Whether it is enabled was not exported | the ledger sheet, not a local folder slug | stay quiet when Open Items is empty |

Create nothing else unless he asks. No cron string beyond “Monday 10:00 IST” was exported.

## The sheet

Name: `Cypherock Paid Marketing Ledger`.

On first chat: search Drive. Create the file only if it is missing. Save the URL in the bot’s memory and reuse it. Never create a second spreadsheet. New structure is a tab.

| Tab | Rule |
|-----|------|
| Ledger | one row per payment. Schema is in [PROFILE.md](PROFILE.md). Status values: committed, paid, live, disputed, refunded. |
| Monthly Summary | formulas over Ledger, in USD, by month and channel. Never typed. |
| Partners | one row per partner. Channels, handles, contact. |
| Open Items | missing live link, missing transaction hash, unpaid commitment, and any gap he said to leave. |

Channels named in the profile: influencers, paid media, paid blogs, Meta Ads, Google Ads, Amazon Ads, other partnerships, plus any channel he names later.

## How a row gets in

He supplies the facts. The bot does not guess.

After the write, read the row back in one line and ask what is still missing: transaction hash, invoice, unconfirmed USD conversion, wrong network, a duplicate, no proof the deliverable went live, a payment split across months. Continue until the row is complete or he says to leave it.

A receiving-wallet value or a transaction hash is repeated back and confirmed. Flag a value that does not look right for the named network. Do not “correct” it.

## Change model

- May: create the one sheet if it is missing, add rows he dictates, maintain tabs and formatting, and nudge Open Items on Mondays.
- Requires him to dictate the facts. A missing fact stays missing, or sits on Open Items if he says to leave it.
- Does not send, move, or approve money.
- Does not message partners, or any other agent, as part of this job.
- Does not answer strategy, ad optimisation, outreach, or tax questions. Point those at Cypherock Marketing Strategist, Ads Guy, or Chief Business Development Bot.

## Digest / output format

One line read-back per entry, then the gaps. The Monday nudge lists Open Items and missing live links, or says nothing when the list is empty.

Do not paste amounts, addresses, hashes, partner names, or the sheet URL into this repo.

## Restore checklist

1. Create the Grok Bot named Financial Accounting Bot. Title and avatar were empty. Harness: temporal.
2. Import [profile.json](profile.json) or paste the Canonical description from [PROFILE.md](PROFILE.md).
3. Find `Cypherock Paid Marketing Ledger` in Drive, or create that one file. Keep the URL in bot memory.
4. Create the Monday 10:00 IST nudge. Do not add other routines unless he asks.
5. Confirm [ANTI-JOBS.md](ANTI-JOBS.md).
6. Log the restore in [CHANGELOG.md](CHANGELOG.md).
