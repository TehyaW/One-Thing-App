# One Thing

A gentle focus app built for people who have a lot going on and need to take it one step at a time.

---

## What it does

**One Thing** shows you a single task at a time — no overwhelming lists, no guilt. It intelligently schedules your day by prioritizing deadlines while weaving in lighter tasks (chores, self-care) between heavier ones (homework, work) so you don't burn out.

### Features

- **One task at a time** — the full list is hidden by default so you can focus
- **Smart scheduling** — due dates are prioritized automatically; tasks without due dates are slotted in between
- **Break it down** — split any task into smaller steps with one tap
- **Snooze** — push a task further down the list without guilt
- **Too hard today** — skip something compassionately; it moves to a separate section, not the trash
- **Quick add** — type a task directly from the focus screen and hit Enter
- **Time estimator** — context-aware questions help you figure out how long something will take, with a confirmation step and +/- adjustments
- **Recurring tasks** — set daily, weekly, custom intervals; they come back automatically
- **Overdue detection** — gently flagged in amber, never in alarming red
- **End-of-day summary** — see what you accomplished, by category, with your streak
- **Daily reset** — at midnight, recurring tasks refresh and completed tasks archive
- **Completion history** — completed tasks are grouped by date; clear today, past days, or everything
- **Edit tasks** — change the name, category, time, or recurrence from the All Tasks tab
- **Works offline** — fully cached via service worker; works without internet once loaded
- **Installable** — add to your home screen as a real app (no App Store needed)

### Categories
- 📚 School / assignments
- 💼 Work
- 🧹 Chores & cleaning
- 🌸 Self-care & hygiene
- ✨ Personal goals

---

## Getting started

### Running locally

This is a single-file static app. Just open `index.html` in any browser — no build step, no dependencies, no server required.

```bash
# Clone the repo
git clone https://github.com/YOUR_USERNAME/one-thing-app.git
cd one-thing-app

# Open directly in browser
open index.html
```

### Deploying to Vercel

1. Push this repo to GitHub
2. Go to [vercel.com](https://vercel.com) and sign in with GitHub
3. Click **Add New → Project** and import this repo
4. Leave all settings as default
5. Click **Deploy**

Vercel auto-deploys on every push to `main`.

---

## Installing on your phone

Once deployed, open your Vercel URL on your phone:

### iPhone (Safari only)
1. Open the URL in **Safari** (not Chrome)
2. Tap the **Share** button at the bottom
3. Scroll down and tap **"Add to Home Screen"**
4. Tap **Add**

### Android (Chrome)
1. Open the URL in **Chrome**
2. Tap the **three-dot menu** in the top right
3. Tap **"Add to Home Screen"** or **"Install App"**
4. Tap **Install**

The app will appear on your home screen and open fullscreen — no browser bar, no address bar. It looks and feels like a native app.

---

## File structure

```
one-thing-app/
├── index.html       # The entire app (HTML + CSS + JS in one file)
├── manifest.json    # PWA manifest — name, colors, icons
├── sw.js            # Service worker — offline support + caching
├── icons/
│   ├── icon-192.png # App icon (home screen, small)
│   └── icon-512.png # App icon (splash screen, large)
└── README.md
```

---

## Updating the app

1. Edit `index.html` (or any file) in your GitHub repo
2. Commit the change
3. Vercel automatically redeploys — usually within 30 seconds
4. On your phone, the app will update the next time you open it with a connection

---

## Data & privacy

All data is stored **locally on your device** using `localStorage`. Nothing is sent to any server. Clearing your browser data or app storage will erase your tasks — there is no cloud sync.

---

## Tech stack

- Vanilla HTML, CSS, JavaScript — no frameworks, no build tools
- Google Fonts (DM Sans + DM Serif Display)
- Web Storage API (`localStorage`) for persistence
- Service Worker API for offline support and PWA install
- Web App Manifest for home screen installation

---

## License

MIT — do whatever you want with it.
