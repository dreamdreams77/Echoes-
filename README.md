# Echoes of the Forgotten Kingdom

A browser-based 3D stealth/action adventure built with three.js. No build step: open `index.html`, or serve the repo root (for example with GitHub Pages) and play.

Controls and goals are in the in-game **How to play** screen. Press **X** for the Echo Burst once the violet meter is full.

Everything (three.js, post-processing, font) is bundled in `lib/`, so the game runs fully offline. When served over http(s) it also registers a service worker and can be installed as an app.
