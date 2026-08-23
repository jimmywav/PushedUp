# PushedUp

A daily pushup tracker PWA — progressive weekly goals, 2 rest days per week, streaks, and a full calendar view. No backend; all data lives in your browser via `localStorage`, with export/import for backup.

## Deploying to GitHub Pages

1. Push these files to the root of `https://github.com/jimmywav/PushedUp`.
2. In the repo, go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`.
4. Save. Your app will be live at `https://jimmywav.github.io/PushedUp/` within a minute or two.
5. Open that URL on your Nothing Phone (4a) Pro in Chrome, then use **Add to Home screen** to install it as a standalone app.

## How it works

- **Logging**: adjust the rep counter on the home screen or tap **Log today**. Reaching the day's goal marks it Complete (green); otherwise it's a Skip (red) once the day has passed.
- **Rest days**: tap **Use a rest day** — capped at 2 per Monday–Sunday week, hard limit, even when editing past days.
- **Retroactive editing**: tap any past (or today's) date on the calendar to change its state or reps.
- **Weekly goal increase**: the goal only increases the week after a fully completed week (every required day either Complete at/above goal, or a used Rest day).
- **Settings** (gear icon): starting goal, weekly increase amount, and tracking start date. Also export/import a JSON backup, and a full reset.

## Notes for next steps

- Push notification reminders aren't wired up yet — that needs a decision on timing/type before building.
- Icons are simple placeholders (`icons/*.png`) — swap them for your own art whenever you like, same filenames.
