# YT Outreach Manager

YouTube influencer outreach for Cypherock. The live name is **YT Outreach Manager · YouTube Outreach**. The folder stays `yt-outreach-manager`.

| | |
|---|---|
| **Live name** | YT Outreach Manager · YouTube Outreach |
| **Title** | empty in the 2026-11-22 export |
| **Slug** | `yt-outreach-manager` |
| **agent uuid** | `53f55bd2-e78b-44ae-bc3a-c6e5167da17d` |
| **serverId** | `3125498` |
| **Owner** | Abhinav Singh |
| **Timezone** | Asia/Calcutta (IST) |
| **harness** | temporal |
| **Avatar** | empty in the export |
| **namedBy** | user |
| **Status** | Operational |
| **Job** | Enrich leads from YT Wallet Scout or from Abhinav, find a point of contact, personalize the email, and send only after approval at local business hours. Manage follow-ups and the creator history. |

## When to use

- A scored creator is ready for a draft.
- Abhinav has approved a batch, and the send falls at the creator’s local business hours.

## When not to use

Publishers are AI Outreach Manager’s pipeline. The scan said not to merge the lists. That sentence is not in this export. See [ANTI-JOBS.md](ANTI-JOBS.md).

## Links

- [PROFILE.md](PROFILE.md) — live description, plus the 2026-09-17 cut labeled as not exported
- [profile.json](profile.json) — sanitized restore aid, 2026-11-22
- [OPERATIONS.md](OPERATIONS.md) — approval at local business hours; the 1:00 PM clock was not in the export
- [ANTI-JOBS.md](ANTI-JOBS.md) — hard never-list
- [CHANGELOG.md](CHANGELOG.md) — export reconciliation

## Operator notes

The export’s send rule is approval, then local business hours. “Local” is the creator’s hours, as Chief BD’s profile also states it (“creator-local business hours”).

The 2026-09-17 cut said at most two send batches a day, with the primary batch on weekdays at 1:00 PM IST, and it removed extra local-hour send wakes. That 1:00 PM clock is the approved instruction from the cut. It is not in the export, and it is not a copied cron. The cut also said to reuse YT Wallet Scout scores and not re-crawl. The export says “enrich Scout/user leads” and does not say “do not re-crawl.”

Chief BD’s profile sets a target of at least 20 outreach emails sent per IST business day, still approval-limited, and at least 4 follow-ups when there is no reply. That target is not a measured count. Do not treat any daily number from the 2026-09-17 scan as a current quota either. No send counts are stored here.

Do not put creator names, addresses, or message text in this folder.
