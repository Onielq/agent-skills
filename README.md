# Istighfar — Dhikr Counter

A quiet, private counter for Astaghfirullah. Tap once to add a count, set a daily intention, and view your last seven days.

## Features

- One-tap counter, undo, and a reset-today action that preserves the all-time total.
- Daily goals: 33, 100, 300, or 1,000.
- Goal progress ring, completion feedback, seven-day activity, all-time total, and completed-day streak.
- Optional gentle vibration on supported phones.
- Installable and offline-capable after the first visit on a supported HTTPS host.
- Responsive, keyboard-accessible design with no external runtime dependencies.

## Privacy

Your counter totals and preferences are stored in the current browser using `localStorage`. They are not sent to a server and are not synced across devices. Clearing browser site data will remove the locally stored counter.

## Publish with GitHub Pages

This app is isolated on the `publish/istighfar-counter` branch. The repository's `main` branch has not been changed.

1. Open [GitHub Pages settings](https://github.com/Onielq/agent-skills/settings/pages).
2. Under **Build and deployment**, select **Deploy from a branch**.
3. Select branch **`publish/istighfar-counter`** and folder **`/(root)`**.
4. Click **Save**.
5. Wait for GitHub Pages to finish building. The expected site address is [https://onielq.github.io/agent-skills/](https://onielq.github.io/agent-skills/).

The public website will not be live until the Pages source is saved in repository settings. The GitHub connector available for this build can commit files and branches but cannot change the Pages configuration itself.

## Local use

Open `index.html` in a browser for basic counting. For full PWA/offline behavior, serve it over HTTPS or localhost so the service worker can register. For example, with Python installed:

```bash
python -m http.server 8000
```

Then open http://localhost:8000.

## Design decisions

See [DESIGN.md](./DESIGN.md) for the design rationale and skill references.
