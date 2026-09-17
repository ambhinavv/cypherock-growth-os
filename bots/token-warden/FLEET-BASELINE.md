# Fleet baseline (distill) — Token Warden

Working copy of the 2026-09-17 fleet scan. Full notes: [baselines/2026-09-17.md](baselines/2026-09-17.md).

**Snapshot time:** 2026-09-17 ~16:00 IST (Asia/Calcutta)  
**Scope:** `/home/box/agent-data` (= `/home/box/sand-data`); skip `sand-subagent-*` (none present that day)  
**Method:** profiles/settings + local FS work products + scarce transcript/store signals. Routines are **server-kept**; local `automations/` mirrors were empty / “No routines yet.”

**Do not treat volume classes as token counts.** Evidence is file activity, digests, and stated cadences only. Per-bot token counters were unavailable.

Same-day **approved cuts** (after this scan, via SendToAgent) are in [CHANGELOG.md](CHANGELOG.md). This file keeps the scan-time picture so Monday deep dives can see what changed.

## Subscription usage / limits (as of the scan)

Weekly and total Grokbot subscription limits/usage were **unavailable on the box**. Digests could only flag **relative waste** until a Usage & Billing paste existed.

A Usage & Billing snapshot from the same calendar day is recorded in [USAGE-TRACKING.md](USAGE-TRACKING.md) (plan Pro, weekly usage 32%, resets in 5 days ~Sep 22, on-demand monthly limit None). That is a settings-screen paste, not box telemetry.

## Volume classes (9 bots)

| Bot | Volume class | Key routines (inferred at scan) | Notes from scan |
|-----|--------------|---------------------------------|-----------------|
| AEO Scout | **high** | daily morning AI visibility | Biggest known waste: daily Google/Bing cells while CAPTCHA / logged-out |
| YT Wallet Scout | **high** | daily ~08:00 IST digest (+ weekly template) | feeds YT Outreach; make-up double-run risk |
| YT Outreach Manager | **high** | daily ops + local-hour send windows | daily_target 20; multi-wake sends |
| AI Outreach Manager | **med-high** | daily AEO handoff + timed sends | high research/draft volume; send throughput still 0 at scan |
| Ads Scout | **med Mon / low else** | weekly Mon 08:00 IST silent-delta | already cut daily→weekly on 2026-09-16 |
| Ads Guy | **low** (would be med if auth restored) | daily ~08:00 IST account review | daily paused after approved cut (Ryze auth dead); weekly+monthly left on |
| Mr. X Scraper | **low** | unknown | one-day screenshot dump 2026-09-14; unclear ongoing job |
| dr eggbot | **low** | none (on-demand) | do not add crons |
| Token Warden | **low** | weekday 08:30 digest; Mon 09:00 deep dive | new that day; see OPERATIONS for current enablement |

Ads Guy row includes the later 2026-09-17 pause on daily (user skipped pausing weekly/monthly). Other volume classes are scan-time.

## Identity index (from scan)

| Bot | agent uuid | serverId |
|-----|------------|----------|
| Mr. X Scraper | `1a269503-bacb-4ca0-a0f7-742f89be739c` | 2642625 |
| Ads Guy | `42a6a03e-33a0-4cec-bb33-fd066665d5b7` | 2945579 |
| YT Outreach Manager | `53f55bd2-e78b-44ae-bc3a-c6e5167da17d` | 3125498 |
| Ads Scout | `70b9e7e7-5a5c-487f-885e-b9ee6a6f633d` | 3120543 |
| AI Outreach Manager | `7517ee94-aa4e-4233-8673-2fe3fa885de5` | 2980453 |
| YT Wallet Scout | `7bc3178d-132d-42d2-acb1-34708f32005b` | 2915316 |
| Token Warden | `a3a716db-daf8-43ab-8b84-6e1f5fba90d8` | 3765226 |
| AEO Scout | `becdbf7e-437b-4bc7-9fdb-7733d8e3ac55` | 2964531 |
| dr eggbot | `ed49f58e-488b-47a2-aa52-38219dec0445` | 3651045 |

## Overlap map

```
[YouTube intel]     YT Wallet Scout ──leads──► YT Outreach Manager
                         RISK: both re-scrape same channels / re-enrich

[Ads]               Ads Scout (library, weekly)  ≠  Ads Guy (own account)
                         complementary if scopes hold
                         RISK: both browser-heavy; don’t both go daily

[AEO / publishers]  AEO Scout ──prospects──► AI Outreach Manager
                         RISK: AEO deep-research + AI Outreach re-research same domains

[Outreach process]  AI Outreach Manager  ≈  YT Outreach Manager
                         same approval/send/follow-up pattern, different ICP
                         RISK: duplicate send-infrastructure wakes

[Unscoped]          Mr. X Scraper — marketing generalist; unclear vs above fleet
[Meta]              Token Warden — watches all; no product overlap
[Factory]           dr eggbot — creates bots; no scheduled overlap
```

Named pairs:

- **Marketing outreach:** AI Outreach vs YT Outreach — parallel pipelines (publishers vs YT creators); process overlap, audience distinct.
- **Ads:** Ads Guy vs Ads Scout — account vs competitive library; good split; Ads Guy auth-blocked at scan.
- **YouTube:** YT Wallet Scout vs YT Outreach — scout→outreach handoff working; watch double enrichment.
- **AEO:** AEO Scout vs AI Outreach — scout→outreach handoff working; watch double research on Critical batch.

## Ranked waste at scan (propose-only at the time)

1. **AEO Scout** — failed Google/Bing cells every morning. Fix proposed: Perplexity-first daily; Google/Bing 2–3×/week; skip until session healthy; silent if no delta. **Approved 2026-09-17** (CHANGELOG).
2. **YT Wallet Scout** — full daily yt-dlp/WebSearch sweep; make-up double-run risk. Fix proposed: silent-delta daily; priority-only weekdays; full cohort weekly; no same-day make-up full rerun. **Approved 2026-09-17**.
3. **Ads Guy** — daily wake while connector dead. Fix proposed: pause daily until Ryze auth. **Approved for daily pause**; user skipped further pause (weekly+monthly left on).
4. **AI Outreach** — high research volume, zero sends. Fix proposed: Critical-only; no re-research Sent/Waiting; wake on approval backlog. **Approved 2026-09-17**.
5. **YT Outreach** — multi-wake local send windows. Fix proposed: fewer send batches; reuse Scout scores; no re-crawl. **Approved 2026-09-17** (≤2 send batches/day, primary weekdays 1:00 PM IST).
6. **Mr. X Scraper** — unclear ongoing role. Still propose-only; not in the first five cuts.
7. **Ads Scout** — already weekly silent-delta. No further cut unless Monday runs are empty-noisy.
8. **Token Warden digests** — scan said don’t enable until usage readable. Usage paste now exists; routines are enabled per OPERATIONS.

## Explicit gaps (still true unless a later baseline says otherwise)

- Server-side routine list (names, cron, enabled/paused, last_run) — **not on box**
- Per-bot token counters — **unavailable** (do not invent)
- Weekly/total usage on the box — **unavailable**; settings-screen paste only
