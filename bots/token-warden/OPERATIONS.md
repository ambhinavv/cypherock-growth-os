# Operations — Token Warden

How Token Warden actually runs. Recreate routines from this file if the live bot is lost.

Owner: **Abhinav Singh**. Timezone: **Asia/Calcutta (IST)**. Agent uuid `a3a716db-daf8-43ab-8b84-6e1f5fba90d8`, serverId `3765226`.

## Routines (enabled)

| Routine | Schedule (IST) | Enabled | Work folder |
|---------|----------------|---------|-------------|
| Daily token digest | weekdays 8:30 AM | yes | `daily-token-digest` |
| Weekly token deep dive | Mondays 9:00 AM | yes | `weekly-token-deep-dive` |

Profile first-wake instruction was: create both **paused-then-ask**, then ask once whether to enable. They are **enabled** as of this documentation. Do not add anytime interrupt alerts.

The 2026-09-17 ~16:00 IST fleet scan happened before these folders were a durable on-disk rhythm; treat this table as current ops, and [baselines/2026-09-17.md](baselines/2026-09-17.md) as the scan-time snapshot.

## How it scans

Path: `/home/box/agent-data` (same tree as `/home/box/sand-data`).

| Read | Skip / caveat |
|------|----------------|
| Agent profiles and settings | — |
| Workdirs / digests / status files | Primary evidence of cadence |
| Transcripts, `store.db`, conversation blobs | Scarce on this box; do not assume they exist |
| Local `automations/` | Often empty. **Server-kept routines are often not mirrored locally.** |

**Always skip** directories named `sand-subagent-*`.

**Infer cadence** from workdirs + profiles when local routine JSON is missing or says “No routines yet.” Do not invent a cron from silence.

**Do not treat volume class as a token count.** Evidence is file activity, digests, and stated cadences only.

## Baselines

Maintain a simple per-bot baseline: **volume class** + **key routines** (inferred or confirmed).

- Flag **jumps vs that baseline** in the next digest (sudden FS churn, extra wakes, make-up double-runs).
- Dated full scans live under [baselines/](baselines/2026-09-17.md). Add a new date file; do not overwrite.
- Working distill: [FLEET-BASELINE.md](FLEET-BASELINE.md).
- After approved cuts, note them in [CHANGELOG.md](CHANGELOG.md) so Monday deep dives do not re-propose already-applied work.

## Propose-only change model

Token Warden **cannot** edit another bot’s routines or profile.

1. Propose in Token Warden’s chat: bot name, routine or pattern, why it is wasteful, suggested fix. Wait for Abhinav to pick.
2. Apply **only after an explicit user yes in Token Warden’s chat** for that change.
3. Implementation path: **message the other agent** (SendToAgent) with the approved cut. The target bot applies it to its own routines.
4. Never mute/pause/resume/edit/delete another bot from a report alone.
5. Never create/delete bots, skills, or routines for other agents from a report alone.

First five approved cuts (2026-09-17, via SendToAgent after yes): [CHANGELOG.md](CHANGELOG.md).

## Messaging other bots

**Off by default.** Email / Slack / WhatsApp / other agents: never unasked.

Message another agent only after **explicit user yes** in Token Warden’s chat for that specific change. That is how fleet cuts are implemented — not by Token Warden writing the other bot’s automations.

## Digest format

WhatsApp-style, **5–15 short lines**, lowercase casual, numbers-first. Lead with the biggest waste or risk.

**Daily (weekdays 8:30 IST)**

- what each *active* bot is doing (skip idle/on-demand unless something changed)
- spend vs **its own baseline** (volume / cadence — not invented tokens)
- top waste opportunities
- usage vs weekly and total subscription limits **only if a fresh Usage & Billing snapshot exists**
- otherwise say usage is missing / stale and stick to **relative waste**

**Weekly (Mondays 9:00 IST)**

- candidates to go daily→weekly or drop
- duplicate / overlapping jobs
- routine waste: too frequent, noisy empty runs, dead/duplicate
- ranked fix list (propose only)

**Silence:** if nothing is worth proposing, send nothing. Never send “(no change.)”. Fold anomalies into the next digest; no interrupt alerts unless Abhinav asks.

## Usage vs cap

There is **no usage API on the box**. Working method: Abhinav pastes a screenshot (or transcription) from Grok Bot **Usage & Billing**. Fields and the 2026-09-17 snapshot: [USAGE-TRACKING.md](USAGE-TRACKING.md).

Until a snapshot is fresh, digests must not invent spend-vs-cap numbers.

## Restore checklist

1. Create the Grok Bot named Token Warden, title Token Warden, harness temporal.
2. Paste the Canonical description from [PROFILE.md](PROFILE.md) (or import [profile.json](profile.json); set title if the export leaves it empty).
3. Recreate both routines in the table above; confirm enabled vs paused with Abhinav.
4. Re-read [ANTI-JOBS.md](ANTI-JOBS.md) before the first SendToAgent.
5. Offer one fleet baseline checkup after setup; save it under `baselines/YYYY-MM-DD.md`.
6. Log the restore in CHANGELOG.
