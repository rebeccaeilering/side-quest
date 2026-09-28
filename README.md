# Side Quest v0.1

Mobile-first, vanilla HTML/CSS/JavaScript quest app. Includes 30 quests, activity/category filtering, rerolls, accepted quest persistence, XP, notes, history, and a basic offline PWA service worker.

## Run locally

From this folder run `python3 -m http.server 8000` and visit http://localhost:8000 on your computer. For phone testing, deploy this folder to an HTTPS static host such as Vercel or Netlify. The service worker requires HTTPS (or localhost).

## Data

Progress is stored in localStorage on each browser/device; clearing browser site data removes it. No cloud sync yet.

## Editing quests

Edit the `quests` array near the bottom of `index.html`. Each entry is `[title, description, category, xp, "space-separated activities"]`.
