# Mr. X Scraper

Cypherock brand-visibility scout on X (Twitter). Finds comment-worthy cold-wallet / hardware-wallet threads for the official account. Second documented bot in this repo.

| | |
|---|---|
| **Name** | Mr. X Scraper |
| **Title** | Mr. X Scraper |
| **Slug** | `mr-x-scraper` |
| **agent uuid** | `1a269503-bacb-4ca0-a0f7-742f89be739c` |
| **serverId** | `2642625` |
| **Owner** | Abhinav Singh |
| **Timezone** | Asia/Kolkata (IST) — same offset as fleet default Asia/Calcutta; cron uses `CRON_TZ=Asia/Kolkata` |
| **harness** | not captured — no live `profile.json` export in this repo |
| **Job** | Every day except Sunday, find X posts from roughly the last 24 hours where cold wallets / hardware wallets / self-custody are discussed, good enough for the official Cypherock account to comment. |
| **Volume class** | low (one scheduled dig/day; not a high-churn crawler) |
| **Change model** | deliver the dig in this bot’s chat without asking; do not draft/post Cypherock comments or spend X search credits unless Abhinav asks in this chat |

## When to use

- Daily (Mon–Sat) 4:00 PM IST: restore or run the Cypherock X cold-wallet dig.
- To recreate the live bot if it is deleted: [PROFILE.md](PROFILE.md) + [OPERATIONS.md](OPERATIONS.md).
- To change the free discovery path or comment-worthiness rubric — edit OPERATIONS, then log it in [CHANGELOG.md](CHANGELOG.md).

## When not to use

X comment-target dig only. Do not ask it to draft/post as Cypherock, buy X API credits, scrape YouTube (that is **YT Wallet Scout**), run ads, or do token accounting (that is **Token Warden**). See [ANTI-JOBS.md](ANTI-JOBS.md).

## Links

- [PROFILE.md](PROFILE.md) — canonical persona (voice, cadence, anti-jobs)
- [OPERATIONS.md](OPERATIONS.md) — routine, free discovery path, rubric, delivery format
- [ANTI-JOBS.md](ANTI-JOBS.md) — hard never-list
- [CHANGELOG.md](CHANGELOG.md) — 2026-09-12 job defined through 2026-09-18 docs bootstrap

## Operator notes

There is **no X search-credit budget**. Digs always use the **free path** (Startpage past-day, often via Jina reader, then FxTwitter validation). If that path is blocked, say what failed — do not silently fall back to paid X API search.

Delivery is WhatsApp-style links + one-liners in **this bot’s chat**. Cap ~10–15; if none qualify, say so — do not pad. Do not announce “routine triggered.”
