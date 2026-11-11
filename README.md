# DEADLIGHT Core 3.2

A mobile-first, offline-capable zombie survival simulation set in Aberdeen, Scotland. Built for GitHub Pages and iPhone, with no API key, paid AI calls or backend.

## What's new in 3.2
- Compositional natural-language command grammar combines action verbs, synonyms, target objects and modifiers to cover thousands of possible phrasings without maintaining a giant brittle phrase list.
- Broader action handling for searching, inspecting, moving, manipulating, using, and interacting with environmental objects.
- Hidden survivor relationship simulation tracks private bond, affection, respect, resentment, comfort and romantic interest. These values are not shown as meters; they emerge through dialogue, shared experiences, conflict, trust and companion behaviour. Relationship actions respect boundaries and do not guarantee reciprocation.
- Companions can occasionally initiate quiet supportive moments as the relationship develops.
- Save version 13 and service-worker cache 3.2; existing saves retain the same localStorage key.

## What's new in 3.1
- Expanded natural-language command interpretation with many more synonyms and common actions: peeking, entering, closing/locking doors, taking cover, climbing, crawling, waiting, using lights, washing, filling containers and distracting infected.
- Reduced unnecessary command failures; ambiguous actions now receive a more contextual prompt without consuming time.
- Added one-tap example commands beneath the action box.
- Refined the mobile interface with cleaner spacing, typography, buttons, tabs, status cards and input focus states.

## What's new in 3.0
- Field-contract board with generated reconnaissance, supply and safehouse requests, rewards and completion tracking.
- Safehouse development: rain collectors, untreated and clean water stores, purification, gardens, food storage and structural reinforcement.
- Long-run character simulation for cold exposure, wet clothing, body temperature, morale and protective clothing.
- Survivor companion orders: ask trusted survivors to follow, keep watch, remain at the safehouse or scavenge. Outcomes depend on trust.
- Radio intercepts and persistent broadcast log, rumours and faction standing.
- 25 additional contextual story encounters with different choices and consequences.
- Expanded loot distribution for food, medical supplies, outdoor equipment and tools.
- Existing map, combat, scavenging, crafting, infection, inventory, journal, save export/import, and 2.0 systems retained.

## Important note about the "AI"
This is a procedural local game master, not a live large language model. It generates contextual situations from authored events, weighted randomness and persistent game state. It works offline and costs nothing to run, but it cannot invent unlimited dialogue with the flexibility of ChatGPT.

## Publish on GitHub Pages
1. Export a save backup in the Journal tab before updating.
2. Download and extract this ZIP on your iPhone.
3. Open `https://github.com/TyllarBarr/Deadlight/upload/main`.
4. Upload the four files at the repository root (not inside an extra folder): `index.html`, `sw.js`, `manifest.webmanifest`, and `README.md`.
5. Commit the changes to `main`.
6. Close the Home Screen app, open the site in Safari once, and reload. The service-worker cache version is bumped to 14.

## Save compatibility
The existing `deadlight-save` localStorage key is retained. Version 3.0 adds new fields during load and keeps existing inventory, location, health, journal and world state. Export a backup first as a precaution.
