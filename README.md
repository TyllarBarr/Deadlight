# DEADLIGHT — Survival RPG (Pre-alpha 0.2)

A mobile-first, local-first zombie survival RPG prototype set in Aberdeen, Scotland.

## Play
Open `index.html` in a modern browser. For an installable iPhone home-screen app, publish this folder to a static HTTPS host, open the URL in Safari, then Share → Add to Home Screen. Saves are stored in that browser on that device. Use Journal → Export save for backups.

## Included systems
- Local autosave, save export/import and offline service-worker cache
- Day/time progression, weather changes, hunger, thirst, energy, health, stress and noise
- Inventory quantities and approximate carried weight
- 12 locations in an Aberdeen-inspired map
- Scavenging tables by location, travel times, basic combat, stealth, barricading and crafting
- Encounter director with survivor, discovery, threat, weather and world-event scenes; encounter pool avoids immediate repeats
- Local command interpreter for common natural-language action patterns

## AI integration status
This release does **not** connect to ChatGPT. OpenAI documents a Sign in with ChatGPT route for open-source apps that can use eligible users' ChatGPT plan allowance, but it requires the app to follow its official registration/OAuth/PKCE and request contract. It is not equivalent to putting a ChatGPT login button in a static HTML file. The game must remain open source and user-controlled for this route. See: https://developers.openai.com/siwc/token-sharing-open-source

The next step is to implement the official open-source client flow and validate it on a registered app. Until then, all gameplay remains local and free, with no API key, server, subscription, or account required. AI-generated narrative and unconstrained text interpretation are not yet active.

## Notes
- This is a prototype; some actions are intentionally simplified and balancing is ongoing.
- Browser storage can be cleared by iOS/browser cleanup. Export saves regularly.
- No credentials or tokens are stored in this build.
