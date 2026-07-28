# 20-Day Lifestyle Challenge

A self-contained web app for tracking a 20-day lifestyle challenge running **Aug 2–21, 2026**, with a bonus reflection day on Aug 22.

**Live site:** https://owro172.github.io/20-Day-Lifestyle-Challenge/

## What it does

- **Today** — the seven daily habits (9 hours sleep, exercise, 15,000+ steps, eat clean, screen limits, reading, journaling) plus cold showers on the three days a week they belong. Each day also shows a schedule shaped to that day's training type, and names the specific session or routes.
- **Workout** — the two lift-day sessions with sets, reps and form cues, the weight guide, and the bike and run routes with door-to-door distances.
- **Progress** — streak, full-day count, a 20-day heatmap, per-habit completion rates, the Day 1 / 8 / 15 measurement and photo check-ins, and the closing reflection questions.
- **Guide** — daily schedule, the 7-day training cycle, nutrition timing, sleep protocol, skincare routine, starting budget, and breakfast ideas.

## How it's built

One file, `index.html`, with all styles and logic inline. No build step, no dependencies, no network calls. It runs the same opened from disk as it does hosted.

Layout adapts to the device: a bottom tab bar and full-bleed cards on phones, a sidebar and two-column dashboard on laptops. Light and dark themes both follow the system setting.

## Your data

Everything is stored in the browser's `localStorage` on the device you're using — nothing is uploaded anywhere. Because of that it does not sync between devices on its own. The Progress tab has a **Move Your Data** section for that:

- **Sync code** — copy on one device, paste on the other. Carries checkmarks, notes, measurements and reflections.
- **Download backup** — a JSON file that also includes the progress photos, which are too large to fit in a paste-able code.

Clearing your browser data for this site erases your log, so export a backup before doing that.

## Deployment

GitHub Pages serves `main` from the repository root. Pushing to `main` redeploys the live site automatically.
