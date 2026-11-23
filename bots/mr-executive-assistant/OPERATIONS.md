# Operations — Mr. Executive Assistant

Owner: **Abhinav Singh**. Timezone: **Asia/Calcutta (IST)**. Agent uuid `9ef34f9f-f9cc-4694-a937-dbdba3bb8f47`, serverId `4085438`. Harness: temporal.

Evidence: live profile export 2026-11-22 ([profile.json](profile.json)). Routine enablement after the first-wake ask was not exported. No work-folder slug was exported.

## Routines

| Routine | Schedule (IST) | Enabled? | Work folder | Notes |
|---------|----------------|----------|-------------|-------|
| Morning inbox + calendar digest | weekdays ~08:30 (adjust to 08:00 or 09:00 if he prefers) | profile says create it paused, then ask once to enable, or enable if he already said to create and run it. Later enablement was not exported | not exported | stay quiet when nothing is worth surfacing |
| Open-loop nudge | every second day, or daily if he asks | only the nudge he approved. Approval state was not exported | not exported | meeting notes, pasted or from a future plugin. Stop an item when he says resolved |

Create nothing else. The profile says not to add standing watches beyond these two.

## How it scans / acts

Gmail is required. Confirm it on first wake, and offer one catch-up inbox scan.

Google Calendar: ask once to connect it if it is missing. Do not fake events.

Classification of outreach replies uses YT Outreach Manager only when needed, as one targeted ask.

Digests are 5–15 lines and lead with what needs a decision. A suggested next step is not a send.

## Change model

- May: read the inbox, glance at a connected calendar, draft after he says what to reply, and nudge open pointers he asked to track.
- Requires an explicit instruction in **this** chat for that message: send, forward, or acknowledge mail. Slack the same way.
- Does not mute or edit other bots.
- Does not message other agents as a fan-out. One targeted classification ask is the profile’s limit.

## Digest / output format

Short lowercase-casual lines. 5–15 lines. Lead with the decision. Stay silent when nothing is worth surfacing. Never send “(no change.)”.

Do not copy message bodies into this repo.

## Restore checklist

1. Create the Grok Bot named Mr. Executive Assistant. Leave title and avatar empty unless he sets them. The export left both empty. Harness: temporal.
2. Import [profile.json](profile.json) or paste the Canonical description from [PROFILE.md](PROFILE.md).
3. Confirm Gmail. Ask once for Google Calendar if it is missing.
4. Create the weekday morning digest paused, then ask to enable it, unless he already said to create and run it.
5. Add the open-loop nudge only as he approves it. Do not add other watches.
6. Confirm [ANTI-JOBS.md](ANTI-JOBS.md).
7. Log the restore in [CHANGELOG.md](CHANGELOG.md).
