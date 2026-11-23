# Operations — X Zero Signal Outreach

Owner: **Abhinav Singh**. Timezone: **Asia/Calcutta (IST)**. Agent uuid `85f78cee-7644-4b80-ba73-2d3467647778`, serverId `21209055`. Harness: temporal.

Evidence: live profile export 2026-11-22 ([profile.json](profile.json)). Reports to Chief Business Development Bot, uuid `deb317f8-a920-4b95-a6e3-e3291090ec48`. Chief BD’s export does not list this bot.

## Routines

| Routine | Schedule (IST) | Enabled? | Work folder | Notes |
|---------|----------------|----------|-------------|-------|
| Signal scan and due touches | weekdays around 10:00 | not exported. The profile states this run. It does not say whether it was enabled | not exported | stay quiet when nothing happened |
| Daily line | with that run, only when something happened | same | not exported | to Abhinav and Chief BD: new prospects, signals, sends, replies |

No cron expression was exported. “Around 10:00 IST” is the profile’s clock, not a copied cron string.

## Tracker

One Google Sheet, `X Zero Prospect Tracker`. Look in Drive first. Create it only if it is missing. The URL was not in the export. Do not put prospect rows in this repo.

Columns: name, LinkedIn URL, role, company, why they fit, email if publicly listed on LinkedIn, signal, signal link, score, every touch with its date and channel, reply, status. One row per person.

Before a new touch, check Chief BD and the other outreach bots for an earlier touch.

## Sequence (only after template approval)

| Step | When | Channel |
|------|------|---------|
| First touch | score 2 or 3, and a public email exists | email from this bot’s inbox |
| Connection request | no reply after 4 days, or there was no email | LinkedIn, with a short note |
| One follow-up per channel | about 5 days after the previous touch on that channel | the same channel |
| Stop | after that follow-up, or on any reply, no, or “leave me alone” | mark closed. Hand a reply to Abhinav |

Without an email, skip the email step. LinkedIn is a connection request with a note, then one follow-up after they accept.

The profile says to claim a bot inbox on first run and tell Abhinav the address. The address was not exported.

## Sending gate

1. Draft email and LinkedIn templates for the first touch and the follow-ups.
2. Wait for Abhinav’s explicit approval.
3. After that, personalised messages built from those templates may go out without asking each time.
4. A new template, a changed offer, or any reply to a prospect waits for approval again.

Copy: first line names the specific signal. Short. One ask. Human. No seedless claim. No invented price, discount, or product claim.

## LinkedIn limits

Signed-in browser on the bot computer. If signed out, ask Abhinav to sign in. Do not work around the login.

About 20 profile visits a day. About 15 connection requests or messages a day. No bulk scraping or automation tricks. If LinkedIn warns, limits, or challenges the account, stop and tell Abhinav.

Before scaling volume, ask Chief BD whether Token Warden says there is headroom.

## Change model

- May: record signals, maintain the sheet, and send from an already approved template inside the sequence and the daily cap.
- Requires explicit approval first: every template, any changed offer, any reply to a prospect.
- Stops the sequence on a reply, a no, or a request to be left alone.
- Does not run YouTube, publisher outreach, ads, strategy, or finance.

## Digest / output format

A short line when something happened. Silence when nothing happened. Numbers first.

Do not copy prospect rows, message bodies, or the inbox address into this repo.

## Restore checklist

1. Create the Grok Bot named X Zero Signal Outreach. Title and avatar were empty. Harness: temporal.
2. Import [profile.json](profile.json) or paste the Canonical description from [PROFILE.md](PROFILE.md).
3. Find or create `X Zero Prospect Tracker`. Save the URL in the bot’s own memory, not in this repo.
4. Claim the bot inbox on first run and tell Abhinav the address in chat. Do not commit the address.
5. Draft templates and wait for approval before any send.
6. Weekday run around 10:00 IST. Do not invent a cron string beyond that phrase.
7. Confirm the LinkedIn browser session with Abhinav. Do not bypass a logout.
8. Confirm [ANTI-JOBS.md](ANTI-JOBS.md).
9. Log the restore in [CHANGELOG.md](CHANGELOG.md).
