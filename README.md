# DEADLIGHT Core 3.8

A mobile-first, local-first zombie survival RPG set in Aberdeen. No paid API, API key or external AI service is used.

## 3.8 behemoth action-language expansion

This release adds a very large bank of colloquial phrases and additional regional variants, UK/US wording, verb inflections, typo corrections, slang, target aliases and reference carry-over. A compositional grammar combines those vocabularies with action targets and modifiers, creating a large number of combinations without storing 100,000 brittle fixed sentences.

It improves action chaining to up to eight clauses, carries referenced objects/items, including plural references like “put them in the torch”, through phrases such as “open the door, then close it”, and adds persistent actions for holding/releasing a door, dismantling a barricade, checking/disarming traps, lowering readied weapons, planning, calming breathing and listening closely through a barrier.

The existing simulation mechanics remain responsible for travel, searching, doors and containers, combat, stealth, inventory, survival needs, medical care, crafting, barricades, vehicles, radio, shelter projects and survivor relationships. Unsupported actions are not falsely reported as successful. This is still a local rule-based system, not a live language model; it cannot understand every possible sentence or perform actions absent from the simulation.

## Install / update

Upload `index.html`, `sw.js`, `manifest.webmanifest` and `README.md` directly into the root of the GitHub Pages repository, replacing the existing files, then commit to `main`. Open the Pages URL in Safari after deployment. If the Home Screen app remains cached, close it and refresh the Safari website first.

## Files

- `index.html` — game, simulation and action interpreter
- `sw.js` — offline cache / update strategy
- `manifest.webmanifest` — Home Screen app metadata
- `README.md` — release notes

Additional 3.8 coverage in the final pass includes more slang and regional phrasings for scavenging, food/drink, movement, stealth, combat, container operations, inventory, wound care, shelter work, vehicles, radios, survivor requests, waiting/resting, journaling and roleplay. Follow-up references now carry plural items such as “them” into later clauses. New stateful actions include phone photographs, checking for active bleeding, shoving a nearby infected back, crawling through an already-open window, and listening through barriers. Pronouns without a remembered target now ask for clarification instead of being sent to a generic fallback.


3.8 fixes target-aware combat so striking a wall or object cannot hit an infected, and adds a general check-in action for flatmates/housemates/friends/survivors without requiring a named NPC. Save migration retains existing progress.


3.8 fix: beverage actions now require the exact named drink to exist in inventory. No drink is created, no substitute is consumed, and thirst is unchanged when the requested drink is absent.
