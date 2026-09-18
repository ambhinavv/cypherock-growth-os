# Operations — Mr. X Scraper

How Mr. X Scraper actually runs. Recreate routines from this file if the live bot is lost.

Owner: **Abhinav Singh**. Timezone: **Asia/Kolkata (IST)**. Agent uuid `1a269503-bacb-4ca0-a0f7-742f89be739c`, serverId `2642625`.

## Routines (enabled)

| Routine | Schedule (IST) | Enabled | Work folder |
|---------|----------------|---------|-------------|
| Cypherock X cold-wallet dig | Mon–Sat 4:00 PM | yes (as of 2026-09-18 docs) | `cypherock-x-cold-wallet-dig` |

Cron: `CRON_TZ=Asia/Kolkata 0 16 * * 1-6`

Profile first-wake instruction: create **paused-then-ask**, then ask once whether to enable. Treat the table as current ops once Abhinav has said yes. Do not add Sunday or interrupt routines.

Server-kept routines are often **not** mirrored under local `automations/`. Infer cadence from this file + PROFILE if the local mirror is empty.

## Saved routine intent (paste / adapt)

```text
Run the Cypherock brand-visibility X dig via the FREE path (not paid X API search —
user has $0 search credits / no budget). Deliver results to the user in this chat.

Goal: posts from roughly the last 24 hours where cold wallets or hardware wallets
are discussed, good enough for the official Cypherock account to leave a helpful,
brand-visible comment.

Method: Startpage past-day discovery (via Jina reader if needed) + FxTwitter
validation. Prefer live x.com browser only if already signed in and usable.
Do NOT call paid X API search tools.

Include: real questions or genuine discussion; high-reach security/self-custody
threads that are natural comment spots. Prefer engagement when volume is high.
Exclude: spam, competitor ad dumps, Cypherock’s own posts, weak noise.

For each keep: direct post URL, one-line why comment-worthy, author handle.
Cap ~10–15 strongest. If none, say so — do not pad.

If free path is blocked, report clearly what failed and what is needed next —
do not silently fall back to paid X API search.

Parent must deliver the dig to the user in chat (WhatsApp-style links + one-liners).
```

## Free discovery path (canonical method)

**Do not use paid X API `search_posts` / full-archive search** when credits are $0.

### Working free stack (validated Sep 2026)

1. **Discovery:** Startpage (or equivalent) **past day / past 24h** queries for hardware/cold wallet discussions, often fetched via **Jina reader** (`r.jina.ai/...`) when direct browser hits captcha/rate limits.
2. **Validation:** Public **FxTwitter / fxtwitter / vxtwitter-style** metadata endpoints to confirm post URLs, authors, and that posts are real.
3. **Optional supplement:** Live `x.com` browser search if signed in on the agent computer — nicer but often login-walled or flaky; not required if Startpage + FxTwitter works.

### Paths that often fail (avoid relying on)

- Direct Startpage / Google / Brave / DDG / live `x.com` without login → captcha / rate-limit / login wall
- Nitter / XCancel mirrors → frequently unavailable
- Paid X MCP search with $0 credits → blocked

### Search query themes (adapt daily)

- `cold wallet`, `hardware wallet`, `self-custody`, `seed phrase`
- “which hardware wallet”, Ledger / Trezor / Coldcard / Bitkey / DCENT incident threads when about choosing or using HW/cold storage
- Recent incident keywords when trending (e.g. app-wallet abnormal transfers, phishing-as-HW-vendor)

## Comment-worthiness rubric

### Include

- Real questions or genuine discussion: recommendations, comparisons, security worries, moving off exchanges/hot wallets, seed/self-custody hygiene.
- High-reach incident/news threads where a calm Cypherock tip fits (phishing, app-wallet failures, “is one HW wallet enough?”, seed entropy, buy-direct-from-manufacturer).
- Prefer some engagement when volume is high; still allow lower-engagement genuine Qs when organic asks are thin.

### Exclude

- Spam / bot promo dumps
- Pure competitor affiliate / product ads with no discussion
- Cypherock’s own posts
- Joke-only / zero-signal noise
- Threads that are not a natural place for an official brand comment

### Recurring comment angles that work

- Seed must never leave the device / never typed into a phone app
- Hardware vs hot/app wallet confusion
- Buy only from manufacturer / supply-chain authenticity
- Phishing after incidents (“we never DM / never ask for seed or PIN”)
- True self-custody / not locked to one vendor / multi-share / air-gapped signing
- Inheritance / “is one hardware wallet enough?”

## Change model

Default for Cypherock bots is propose-only. **This bot may act without asking** on one thing: run the free-path dig and post the link list in **its own chat**.

- May: discover, validate, and deliver the Mon–Sat dig in this chat.
- Requires an explicit user yes in *this* bot’s chat: drafting or posting Cypherock comments; using paid X search; changing cron; messaging other agents.
- May **not** message other agents (almost never, and only after yes).

## Digest / output format

WhatsApp-style. Casual. Do not announce “routine triggered.”

```text
Cypherock X dig — last ~24h

Theme today: <one line if there is a dominant narrative>

1. https://x.com/.../status/... — <one-line why + comment angle>
2. ...

Skipped: <short note on excluded competitor dumps / thin organic asks>
Free path — no API credits.
```

For each keep: direct post URL, one-line why comment-worthy, author handle. Cap ~10–15 strongest.

**Empty day:** if none qualify, **say so** — do not pad, and do not stay silent (this is not Token Warden `silent-delta`).

## Runtime notes

- Automation often runs as an isolated subagent; **parent agent must post the dig to the user** (handoff pattern).
- After each run, briefly note method used (free path) so spend expectations stay clear.
- Optional X (Twitter) MCP: useful for profile / free lookups. **Not** required for the dig when search credits are $0. On connect: check tools exist, check usage credits, never push “buy credits” until balance is actually ~$0 **and** a billed job is needed. For this dig, stay on the free path regardless.
- Optional browser / computer use: login once on the agent computer improves live `x.com` search. Dig must still work without it.

## Related bots (fleet context)

- **YT Wallet Scout** — hardware/cold-wallet YouTube intelligence (sibling surface; different channel).
- **Token Warden** — fleet token accountant; does not run this dig.
- Other Cypherock growth bots live in the same `bots/` set; keep naming consistent (`cypherock-*` folders / ids).

The 2026-09-17 Token Warden scan still lists this bot as “unclear ongoing job.” That was scan-time. Current ops are this file.

## Restore checklist

1. Create the Grok Bot named Mr. X Scraper, title Mr. X Scraper.
2. Paste the Canonical description from [PROFILE.md](PROFILE.md). Do not invent harness / avatar values.
3. Recreate the routine in the table above (folder `cypherock-x-cold-wallet-dig`, cron `CRON_TZ=Asia/Kolkata 0 16 * * 1-6`); confirm enabled vs paused with Abhinav.
4. Confirm anti-jobs still match [ANTI-JOBS.md](ANTI-JOBS.md).
5. Smoke-test one manual dig; confirm the parent posts the list in this chat; confirm paid X search was **not** called.
6. Optionally connect X MCP (expect $0 credits) and/or sign into x.com on the agent browser — dig must still work without either.
7. Log the restore in [CHANGELOG.md](CHANGELOG.md).
