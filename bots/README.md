# Grok Bots

This folder is the durable source of truth for Cypherock Grok Bots: who each bot is, how it runs, what it must never do, and what changed.

Live bots on the box can be lost, renamed, or recreated. Docs here should be enough for another human or agent to **restore**, **operate**, and **audit** them without relying on chat memory.

There is no marketing-automation code in this tree. Personas and ops notes only.

## Why this structure exists

1. **Recreate / restore** a bot from `PROFILE.md` + `OPERATIONS.md` (and `profile.json` when present) if the live bot is lost.
2. **Onboard the next bot** by copying `_template/` instead of reinventing file names and sections.
3. **Audit trail** of fleet cuts and dated baselines for Monday deep dives.
4. **Shared vocabulary** (`volume class`, `silent-delta`, `propose-only`) so marketing bots describe waste the same way.
5. **Handoff:** someone else can operate Token Warden or Mr. X Scraper from these files alone.
6. **Later (optional):** a CI/lint check that every `bots/<slug>/` has the required files. Not implemented in this commit.

## Documented bots

Every bot named in the 2026-09-17 fleet scan has a folder. Token Warden and Mr. X Scraper were registered from live material (a profile export, and an operating playbook). The other seven were registered on 2026-11-24 from that scan plus the cuts already written in Token Warden’s changelog. Their `PROFILE.md` files are restore drafts, not live exports. A live re-list of the Grok Bot account was not available for that pass, so bots created, renamed, or deleted after 2026-09-17 are not in this table.

| Bot | Folder | Role |
|-----|--------|------|
| Token Warden | [token-warden/](token-warden/README.md) | Fleet token accountant |
| Mr. X Scraper | [mr-x-scraper/](mr-x-scraper/README.md) | Cypherock X cold-wallet dig (brand-visibility comment targets) |
| AEO Scout | [aeo-scout/](aeo-scout/README.md) | AI-search visibility; prospect queue for AI Outreach |
| AI Outreach Manager | [ai-outreach-manager/](ai-outreach-manager/README.md) | Publisher outreach, send only after approval |
| YT Wallet Scout | [yt-wallet-scout/](yt-wallet-scout/README.md) | Hardware-wallet YouTube intel |
| YT Outreach Manager | [yt-outreach-manager/](yt-outreach-manager/README.md) | YouTube creator outreach, send only after approval |
| Ads Scout | [ads-scout/](ads-scout/README.md) | Weekly public ads-library monitor |
| Ads Guy | [ads-guy/](ads-guy/README.md) | Own-account ads review; changes only after approval |
| dr eggbot | [dr-eggbot/](dr-eggbot/README.md) | On-demand bot designer; no routines |

Do not create a folder for a bot that is only a rumor. Identity (name plus agent uuid, or a live profile export) has to be in hand first. Do not create empty stub folders.

Scan-time volume classes and overlap stay in Token Warden’s [FLEET-BASELINE.md](token-warden/FLEET-BASELINE.md). Those rows are historical. Per-bot folders hold the later cuts.

## How to add a bot

1. Copy `bots/_template/` → `bots/<slug>/`. Slug is kebab-case of the live bot name (`token-warden`, `mr-x-scraper`).
2. Fill every required file. Do not merge leftover `TODO` placeholders.
3. Add a row to the table above.
4. Log the documentation bootstrap in that bot’s `CHANGELOG.md`.
5. Extra files are allowed when the role needs them (Token Warden’s `USAGE-TRACKING.md`, `FLEET-BASELINE.md`, `baselines/`).

## Required files (every bot)

| File | Purpose |
|------|---------|
| `README.md` | One-pager: purpose, owner, when to use, links |
| `PROFILE.md` | Canonical persona — voice, cadence, anti-jobs |
| `OPERATIONS.md` | How it runs: schedules (IST unless PROFILE says otherwise), folders, scan paths, propose vs execute |
| `ANTI-JOBS.md` | Hard never-list (ops-facing; must match PROFILE) |
| `CHANGELOG.md` | Dated decisions and applied changes |

Recommended extras:

| File | When |
|------|------|
| `profile.json` | Live Grok Bot profile export — restore aid |
| `baselines/YYYY-MM-DD.md` | Dated scans; do not overwrite, add a new date |

## Conventions

- **Timezone:** IST (`Asia/Calcutta`) unless the bot’s PROFILE says otherwise.
- **No secrets:** never commit API keys, cookies, session tokens, or third-party credentials.
- **No personal or account data:** never commit contact lists, message bodies, ad-account ids, spend, campaign structures, or connector tokens. Role, cadence, and anti-jobs belong here. Operating data stays on the bot computer.
- **No invented identity:** if harness, cron expression, avatar, or profile text was not exported, say so. A restore draft must be labeled as a draft.
- **No invented usage numbers:** if Usage & Billing / telemetry is missing, say what is missing and what you need.
- **Volume class is not a token count.** It is qualitative activity (workdir churn + stated cadence).
- **Propose-only** unless that bot’s OPERATIONS says it may act after an explicit user yes in *its* chat.
- Update `CHANGELOG.md` the same day a live change is approved.

## Shared vocabulary

| Term | Meaning |
|------|---------|
| **volume class** | Activity band (`high` / `med-high` / `med` / `low`) from workdir + cadence evidence. Not tokens. |
| **silent-delta** | Speak only when there is a material change vs baseline. Never send “(no change.)”. |
| **propose-only** | Recommend a cut; do not mute/pause/edit/message other bots until explicit user yes in that bot’s chat. |
| **relative waste** | Cadence / overlap / empty-run waste you can flag without a usage API. |
| **spend-vs-cap** | Usage vs weekly/total subscription limits — only with a fresh Usage & Billing snapshot. |
| **SendToAgent** | After user yes, Token Warden messages the target bot to apply a cut. It cannot edit other bots’ routines directly. |
