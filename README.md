# GZ-Diplomacy Support

A small public support page for reporting bugs, crashes, desyncs, confusing UI behavior, and multiplayer edge cases in **GZ-Diplomacy**.

GZ-Diplomacy is a multiplayer team-start and diplomacy mod for **Factorio 2.0**. It is designed to support Oarc-style separate team starts while adding a cleaner team flow, prepared spawn previews, admin tools, basic diplomatic stances, and GIZMOD-powered debug reporting.

---

## What this form is for

Use this support form for problems related to **GZ-Diplomacy**, especially:

- Creating a new team
- Joining, leaving, or switching teams
- Prepared starts and spawn preview
- Keep / Pass spawn selection
- Admin teleport or team-management tools
- Hostile / Neutral / Friendly diplomacy stances
- Flags, team colors, or team identity UI
- Multiplayer crashes, desyncs, or force/team weirdness
- GIZMOD debug output related to GZ-Diplomacy

The form is meant to collect useful bug reports without needing a GitHub account.

---

## What makes a good report?

A good report does not need to be long. It just needs to explain what happened clearly enough that the bug can be reproduced.

The most useful reports include:

```text
1. What you clicked or did.
2. What happened.
3. What you expected instead.
4. Whether this was singleplayer, multiplayer, or a dedicated server.
5. Your GZ-Diplomacy version.
6. Any relevant debug/log output.
```

Example:

```text
I was admin on a multiplayer save.
I clicked Join on team_002 from the Diplomacy panel.
It moved me to the team, but did not teleport me to the team's spawn.
Expected: join team and teleport to the team spawn.
GZ-Diplomacy: 0.3.14
Factorio: 2.0.76
```

That is enough to start investigating.

---

## Logs are extremely helpful

For simple UI bugs, logs are optional.

For crashes, desyncs, broken team state, spawn-preview bugs, or anything involving multiplayer force behavior, logs are very helpful.

Useful files:

```text
Factorio/factorio-current.log
Factorio/script-output/GIZMOD_logs/current_gz-diplomacy.json
Factorio/script-output/GIZMOD_logs/previous_gz-diplomacy.json
Factorio/script-output/GIZMOD_logs/session_gz-diplomacy.jsonl
```

If the game crashed, copy `factorio-current.log` before restarting Factorio. Restarting can replace or change the useful log contents.

---

## What is GZ-Diplomacy trying to do?

GZ-Diplomacy lets multiplayer maps start with separate player teams instead of forcing everyone into one shared force.

The basic flow is:

```text
Host/admin prepares start locations.
Players create a team or join an existing team.
New teams scout a prepared start.
Players Keep the start to found their team there, or Pass and continue the preview flow.
Teams can set basic relations with each other.
Admins can move around quickly to help test or fix player state.
```

The current public beta focuses on the foundation:

- Safe team creation
- Separate Factorio forces
- Prepared start buffering
- Spawn preview
- Team joining and switching
- Basic relation stances
- Admin mobility
- Debug reporting

Planned or experimental areas may include war declarations, congress/council mechanics, embargoes, sanctions, team chat controls, shared vision rules, and deeper economy integration.

---

## Before submitting

Please check:

- You are using the latest public beta build.
- The issue is actually related to GZ-Diplomacy.
- You included the GZ-Diplomacy version.
- For crashes/desyncs, you included the relevant log text.
- For multiplayer bugs, you described who was admin, who was on which team, and what button was clicked.

Reports do not need to be perfect. Clear beats long.

---

## Privacy note

Bug reports are sent by email to the maintainer. Do not paste private information, server passwords, private Discord links, personal tokens, or anything else you do not want sent in an email.

Factorio logs can contain file paths, usernames, mod lists, and system details. Trim them if needed, but keep the relevant error/debug section.

---

## Translation notes

GZ-Diplomacy may include first-pass locale files for major UI flows, settings, and commands. If a translated label is awkward or wrong, please report it through the form and mention the language.

Helpful translation reports include:

```text
Language:
Current text:
Suggested text:
Where it appears:
```

---

## Links

- Factorio mod portal: add the public mod URL here
- Bug report form: add the GitHub Pages URL here
- GIZMOD core: add the Gizmod mod URL here

---

## Status

This support page is intentionally small and static. It exists so players and testers can report GZ-Diplomacy issues without needing to understand GitHub, mod internals, or the debug system.

If something broke, describe it. If something desynced, send logs. If a button let you do something absurd but the game survived, that is still useful.
