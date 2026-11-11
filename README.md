# DEADLIGHT Core 5.0

A mobile-first, local-first zombie survival RPG set in Aberdeen. No paid API, API key or external AI service is used.

## 5.0 — playthrough readiness update

- Routes improvised environmental actions through the environmental resolver before the legacy action handlers. This is important for object-targeted actions such as striking a wall, moving furniture, climbing onto objects and breaking windows.
- Keeps the fictional starting location **Marlowe Court**; no reference to the player's real street is intended.
- Updates the visible build label and service-worker cache key so browsers request the new release rather than reusing the previous cached shell.
- Clarifies the command prompt: use one or two actions at a time, and the local resolver checks state rather than promising unrestricted natural-language understanding.
- Preserves the existing local save format and game data. Existing saves are not deliberately reset by this update.

## Important limitations

DEADLIGHT is a local procedural/rule-based simulation, not a live language model. It does not understand every possible sentence. The action engine is still a mixture of specialised handlers and a legacy fallback, so unfamiliar commands may need rephrasing. No browser-based end-to-end playtest was available during this build; the JavaScript syntax and ZIP integrity were checked.

## Install / update

Upload `index.html`, `sw.js`, `manifest.webmanifest` and `README.md` directly into the root of the GitHub Pages repository, replacing the existing files, then commit to `main`. Open the Pages URL in Safari after deployment. If the Home Screen app remains cached, close it and refresh the Safari website first.

## Files

- `index.html` — game, simulation and action interpreter
- `sw.js` — offline cache / update strategy
- `manifest.webmanifest` — Home Screen app metadata
- `README.md` — release notes
