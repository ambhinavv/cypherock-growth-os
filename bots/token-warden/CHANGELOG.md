# Changelog — Token Warden

Newest first. No invented usage numbers.

## 2026-11-24

### Live profile export

- Replaced `profile.json` and the canonical description with the live export from 2026-11-22.
- The new text adds a standing reply path for Chief Business Development Bot (serverId `4087835`): headroom and outreach-spend asks are answered, and a concrete token question from another bot may be answered. Fleet cuts stay propose-only until Abhinav says yes.
- Anti-jobs wording in the export now says “outreach execution” rather than “outreach”, and it states the messaging exception above.
- Title and avatar are empty in this export. The bootstrap note below that said to set the title to “Token Warden” is withdrawn. Harness remains temporal. Status: operational.
- No usage numbers in the export. The 2026-09-17 Usage & Billing snapshot is unchanged and is not refreshed here.

## 2026-09-17

### Docs bootstrap

- First Grok Bot documented in `cypherock-growth-os`.
- Laid `bots/` conventions + `_template/` for later bots.
- Captured live profile export as `profile.json` (title empty in export; live title Token Warden).
- Fleet scan ~16:00 IST saved as `baselines/2026-09-17.md` and distilled in `FLEET-BASELINE.md`.
- Usage & Billing paste recorded in `USAGE-TRACKING.md`: plan Pro, weekly usage 32%, resets in 5 days (~Sep 22), on-demand monthly limit None.

### Routines

- Daily token digest — weekdays 8:30 AM IST — folder `daily-token-digest` — enabled.
- Weekly token deep dive — Mondays 9:00 AM IST — folder `weekly-token-deep-dive` — enabled.

### First five approved fleet cuts

Applied **via SendToAgent after explicit yes from Abhinav** in Token Warden’s chat. Token Warden did not edit the other bots’ routines directly.

1. **AEO Scout** — Perplexity-first daily; Google/Bing ≤2–3×/week + stop on CAPTCHA/logout; silent if no delta.
2. **YT Wallet Scout** — silent-delta daily; priority-only weekdays; full cohort → Sun 8:15 weekly; no same-day make-up full rerun.
3. **Ads Guy** — daily Google Ads Review paused until Ryze auth; weekly+monthly left on (user skipped further pause).
4. **AI Outreach** — Critical-only; no re-research Sent/Waiting; wakes on approval backlog.
5. **YT Outreach** — ≤2 send batches/day (primary weekdays 1:00 PM IST); reuse Scout scores; no re-crawl.

Not in this batch (still propose-only as of this changelog): park/define Mr. X Scraper; further Ads Scout cuts.
