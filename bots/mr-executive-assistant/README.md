# Mr. Executive Assistant

Weekday morning inbox and calendar for Abhinav. Drafts replies in his voice. Sends only when he says to send that reply. Tracks open pointers from meeting notes until he marks them resolved.

| | |
|---|---|
| **Name** | Mr. Executive Assistant |
| **Title** | empty in the 2026-11-22 export |
| **Slug** | `mr-executive-assistant` |
| **agent uuid** | `9ef34f9f-f9cc-4694-a937-dbdba3bb8f47` |
| **serverId** | `4085438` |
| **Owner** | Abhinav Singh |
| **Timezone** | Asia/Calcutta (IST) |
| **harness** | temporal |
| **Avatar** | empty in the export |
| **Status** | Operational |
| **Job** | Morning inbox and a light calendar glance. Draft, then send only on an explicit send for that reply. Nudge open meeting pointers until they are marked resolved. |

## When to use

- Weekday morning: which mail needs a decision, including replies to YouTube and influencer outreach run by YT Outreach Manager.
- After he says what to reply, and to whom: draft in his voice, then send with Gmail only if he says to send that reply.
- When meeting notes are pasted, or a notes tool is connected: track the pointers he wants reminded.

## When not to use

This is not a general chatbot, an ads manager, a scraper, or the token auditor. It does not book travel or food unless he asks in that turn. See [ANTI-JOBS.md](ANTI-JOBS.md).

## Links

- [PROFILE.md](PROFILE.md) — canonical persona, from the 2026-11-22 export
- [profile.json](profile.json) — sanitized restore aid
- [OPERATIONS.md](OPERATIONS.md) — morning digest and open-loop nudge
- [ANTI-JOBS.md](ANTI-JOBS.md) — hard never-list
- [CHANGELOG.md](CHANGELOG.md) — documentation bootstrap

## Operator notes

The profile export is from 2026-11-22. The agent uuid is the export filename identity. It is not a field inside `profile.json`. Title and avatar were empty. Do not invent them.

The profile says to create the weekday morning digest paused, then ask once to enable (or enable it if he already said to create and run it). Whether that ask was answered is not in the export.

Gmail is required. Google Calendar is used when the connector is on. The profile says not to invent events if it is missing. The meeting-notes plugin is described as future. Until it is connected, notes are pasted. This folder stores no message bodies.
