# Usage tracking — Token Warden

There is **no live usage API** on the box. Weekly and total Grokbot subscription usage/limits are **not** in `/home/box/agent-data` telemetry, agent `store.db`, or local workflow files (confirmed on the 2026-09-17 fleet scan).

Do **not** invent token counts, dollar spend, or remaining quota.

## Working method

1. Abhinav opens Grok Bot **Usage & Billing** (settings).
2. Pastes a **screenshot** into Token Warden’s chat, or transcribes the visible fields here.
3. Token Warden records a dated snapshot in this file (newest first) and may use it for **spend-vs-cap** in digests until it goes stale.
4. If the snapshot is missing or older than the current weekly window, digests report **relative waste only** and say usage is unavailable.

## Fields to capture

Copy what the screen actually shows. Leave a field blank rather than guessing.

| Field | Why |
|-------|-----|
| **Captured at** | Date/time + timezone (IST) of the screenshot, not of the digest |
| **Source** | “Usage & Billing screenshot” or paste |
| **Plan** | e.g. Pro |
| **Weekly usage** | Percent or amount as shown |
| **Weekly reset** | “resets in N days” and/or calendar date if stated or clearly implied |
| **On-demand monthly limit** | As shown (may be `None`) |
| **Any other visible cap** | Total remaining, period, etc. — only if on screen |
| **Notes** | Cropped UI, unclear digits, timezone caveats |

Never derive a token count from volume class or from workdir file counts.

## Snapshot — 2026-09-17

Captured from Usage & Billing (user paste/screenshot). Use these figures only as of that day; do not roll them forward as if they were live.

| Field | Value |
|-------|--------|
| **Captured at** | 2026-09-17 (IST) |
| **Source** | Usage & Billing screenshot / paste |
| **Plan** | Pro |
| **Weekly usage** | 32% |
| **Weekly reset** | resets in 5 days (~Sep 22) |
| **On-demand monthly limit** | None |

No per-bot token counters were available. Do not backfill them.
