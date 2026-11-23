# Operations — Ads Guy

Owner: **Abhinav Singh**. Timezone: **Asia/Calcutta (IST)**. Agent uuid `42a6a03e-33a0-4cec-bb33-fd066665d5b7`, serverId `2945579`.

Evidence: fleet scan 2026-09-17. Not re-read on 2026-11-24. No live `profile.json`.

## Routines

| Routine | Schedule (IST) | Enabled? | Work folder | Notes |
|---------|----------------|----------|-------------|-------|
| daily review (inferred; slug not exported) | inferred ~08:00; cron not exported | paused 2026-09-17 until the ads connector authenticates; not re-read on 2026-11-24 | `google-ads-intelligence`, `daily-reports` | do not resume from this document |
| weekly (slug not exported) | clock not captured | left on; Abhinav skipped pausing it; not re-read on 2026-11-24 | not exported | do not invent a clock |
| monthly (slug not exported) | clock not captured | left on; Abhinav skipped pausing it; not re-read on 2026-11-24 | not exported | do not invent a clock |

The scan called the ads connector Ryze AI and found it unauthenticated. Auth after 2026-11-24 is unknown. Daily stays documented as paused.

## How it scans / acts

Own-account review only. Propose only. No bid, budget, ad, keyword, or campaign edit without an explicit yes in this chat for that change.

The only report found was a blocked daily note from 2026-09-15. Do not quote it here. Do not scan public ad libraries. That is Ads Scout.

Volume class at the scan was low because the connector was blocked. It would be med if auth returned. That is not a token count.

## Change model

- May: propose an own-account change in this chat, in short WhatsApp-style updates.
- Requires an explicit yes in **this** chat for that change: any bid, budget, ad, keyword, or campaign edit, and any resume of the daily review.
- Weekly and monthly stay as left on 2026-09-17. Their clocks were not captured.
- Does not send WhatsApp. The voice is a format.
- Does not message other agents by default.

## Digest / output format

Short WhatsApp-style updates. That is a writing format, not a WhatsApp send.

Do not include account ids, spend, campaign structures, or the text of the 2026-09-15 note.

## Restore checklist

1. Create the Grok Bot named Ads Guy. Title was not in a profile export; this draft uses the scan name.
2. Compare [PROFILE.md](PROFILE.md) with the live bot before pasting. It is a restore draft, not a live export.
3. Leave the daily review paused. It was inferred around 08:00 IST. Do not invent a cron string, and do not resume daily from this document. Auth after 2026-11-24 is unknown.
4. Weekly and monthly were left on. Do not invent their clocks.
5. Do not store account ids, spend, or campaign structures. Do not scan public ad libraries.
6. Confirm [ANTI-JOBS.md](ANTI-JOBS.md).
7. Log the restore in [CHANGELOG.md](CHANGELOG.md).
