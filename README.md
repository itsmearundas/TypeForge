# TypeForge

A precision typing trainer — live WPM, accuracy, consistency scoring, WPM-over-time chart, personal bests, and session history, all saved locally in your browser. No backend, no build step, no dependencies to install.

**[Live demo →](#)** *(link will work once GitHub Pages is enabled — see below)*

## Features

- Time modes: 15s / 30s / 60s / 120s, plus custom pasted text
- Live WPM, accuracy, mistake count, and timer while typing
- Character-level highlighting (correct / incorrect / current)
- Results screen with a WPM-over-time line chart and a consistency score
- Personal best tracking and a 10-session history, saved via `localStorage`
- Dark / light theme toggle and optional keystroke sound
- Keyboard-first: press **Tab** to restart anytime
- Fully responsive, no external JS frameworks

## Run locally

Just open `index.html` in any browser — double-click it, or:

```bash
open index.html        # macOS
start index.html        # Windows
xdg-open index.html      # Linux
```

## Deploy to GitHub Pages

1. **Create a new repository** on GitHub (e.g. `typeforge`), don't initialize it with a README since you already have one here.

2. **Push this folder to it:**

   ```bash
   cd typeforge-repo
   git init
   git add .
   git commit -m "Initial commit: TypeForge typing trainer"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/typeforge.git
   git push -u origin main
   ```

3. **Enable GitHub Pages:**
   - Go to your repo on GitHub → **Settings** → **Pages**
   - Under "Build and deployment", set **Source** to `Deploy from a branch`
   - Set **Branch** to `main` and folder to `/ (root)`
   - Click **Save**

4. **Visit your site** — GitHub will give you a URL like:

   ```
   https://YOUR_USERNAME.github.io/typeforge/
   ```

   It can take a minute or two for the first deploy to go live.

That's it — since this is a single static `index.html` file with no build step, GitHub Pages will serve it exactly as-is. Any time you push changes to `main`, the live site updates automatically within a minute or so.

## Project structure

```
typeforge-repo/
├── index.html      # the entire app (HTML, CSS, JS)
├── README.md       # this file
└── .gitignore
```

## Tech

Vanilla HTML/CSS/JS. Fonts loaded from Google Fonts (Space Grotesk, JetBrains Mono). No React, no build tooling, no npm install required.
