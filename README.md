# Gorilla Hangout VR (WebXR)

Browser-based WebXR game for Meta Quest Browser. Also playable on desktop (mouse + keyboard) and phones (touch).

## Start screen
- **VR Mode** requests an immersive VR session (needs a WebXR headset browser over HTTPS).
- **Desktop Mode** starts playing straight away: mouse look + WASD on a computer, touch controls on a phone/tablet.
- The Esc key (desktop) or the Menu button (touch) opens the settings menu with game modes and the shop.
- When a VR session ends you return to the start screen.
- If the game engine can't load (offline / CDN blocked) the start screen says so instead of doing nothing.

## Publish with GitHub Pages
1. Create a new public repository and upload `index.html` to the top level.
2. Settings -> Pages -> Deploy from a branch -> `main` and `/(root)` -> Save.
3. Open the published HTTPS URL in Meta Quest Browser and press **VR Mode**.

Notes:
- This is a browser/WebXR game, not a native Quest APK.
- Three.js loads from a CDN unless you also upload `three.min.js` next to `index.html`.
- Online multiplayer only works in the claude.ai version; this build is single-player.
- Untested in a headset: check controls and comfort before sharing.
