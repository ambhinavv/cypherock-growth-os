# Operations — <Bot Name>

How to run this bot. Recreate routines from this file, not from memory.

## Routines

| Routine | Schedule (IST) | Enabled? | Work folder | Notes |
|---------|----------------|----------|-------------|-------|
| TODO | TODO | TODO | TODO | TODO |

Server-kept routines are often **not** mirrored under local `automations/`. Infer cadence from workdirs + this file + PROFILE if the local mirror is empty.

## How it scans / acts

TODO: paths it reads (usually under `/home/box/agent-data`), what it skips, outputs it writes.

## Change model

Default for Cypherock bots: **propose-only**.

- TODO: what this bot may do without asking
- TODO: what requires an explicit user yes in *this* bot’s chat
- TODO: whether it may message other agents (almost never, and only after yes)

## Digest / output format

TODO: length, structure, when to stay silent (`silent-delta`).

## Restore checklist

1. Create the Grok Bot with the [PROFILE.md](PROFILE.md) description (or import `profile.json`).
2. Recreate the routines in the table above.
3. Confirm anti-jobs still match [ANTI-JOBS.md](ANTI-JOBS.md).
4. Log the restore in [CHANGELOG.md](CHANGELOG.md).
