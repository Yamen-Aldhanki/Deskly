# Deskly

**Your personal digital desk.**

Notes, tasks, projects, and utilities in one focused workspace — fully offline, no account, no sync, just work.

Deskly is a productivity workspace that runs entirely in your browser. There's no backend, no API calls, and no tracking — every task, note, project, and file you create stays on your own device, stored locally via IndexedDB. Close the tab, come back next week, and it's all still there.

## Features

- **Dashboard** — an at-a-glance view of your day: pending tasks, active projects, notes, and focus time.
- **Tasks** — priorities, due dates, categories, and progress tracking.
- **Notes** — quick capture with pinning and favorites.
- **Projects** — track progress, notes, and time per project.
- **Planner & Calendar** — schedule events and link them to tasks.
- **Files** — store and organize files locally, no upload required.
- **Focus** — pomodoro/timer sessions to track deep work.
- **Analytics** — a full productivity dashboard: completion trends, focus habits, streaks, personal bests, a GitHub-style activity heatmap, custom goals, and a daily productivity score — all computed locally from your own data.
- **Drafts** — compose email drafts locally; "Send" hands them off to your default mail app via `mailto:` (Deskly itself never sends anything or talks to a server).
- **Global search** (`Cmd/Ctrl+K`) — jump to any page, task, note, project, or draft instantly.
- **Backup & restore** — export your entire workspace to a single JSON file and restore it anytime, including on a different device.
- **Light & dark themes**, with a customizable accent color.

## Privacy

Deskly has no backend. There are no API calls, no accounts, no analytics services, and no network requests of any kind once the page has loaded — it even works with your network fully disconnected. All data is stored locally in your browser via IndexedDB and never leaves your device unless you explicitly export a backup.

## Tech Stack

- [React](https://react.dev/) + [TypeScript](https://www.typescriptlang.org/)
- [Vite](https://vitejs.dev/) for building
- [Tailwind CSS](https://tailwindcss.com/) for styling
- [Dexie.js](https://dexie.org/) (IndexedDB) for local, offline-first storage
- [Recharts](https://recharts.org/) for the Analytics charts
- [Radix UI](https://www.radix-ui.com/) primitives

All fonts are embedded locally at build time — no external font requests, ever.

## Getting Started

```bash
# Install dependencies
npm install

# Run the dev server
npm run dev

# Build for production
npm run build
```

The production build outputs to `dist/` — a fully static site with no server-side requirements.

## Deployment

Since Deskly is a fully static app, it deploys anywhere that serves static files:

- **GitHub Pages** — push the contents of `dist/` to your repo and enable Pages in Settings → Pages.
- **Any static host** — Netlify, Vercel, Cloudflare Pages, or even a local file server.

## License

Add your preferred license here (e.g., MIT).
