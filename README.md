# Water Polo Live Match Stat-Tracker

A phone-friendly page for logging stats during a water polo match. Tap a button next to a cap number to record a goal, shot, steal or exclusion, and see a live team table. When the match ends, download the whole sheet as a CSV file for Excel or Google Sheets.

**Live:** https://kontraf.github.io/waterpolo-tracker/

## What it does

- Tracks 13 players (caps 1 to 13) with goals, shots, steals and exclusions.
- A goal also counts as a shot, and shot percentage is calculated for you.
- Shows a warning if you try to add an exclusion to a player who already has 3.
- **Undo last** reverses the most recent tap, in case of a mis-tap.
- **New match** clears everything, after asking for confirmation.
- Stats are saved in the browser automatically, so a refresh or an accidental close does not lose the match.
- **Download CSV** exports one row per player.

## Run it

No build step. Open `index.html` in a browser, or serve the folder with any static server.

## Built with

HTML, JavaScript and Tailwind CSS (loaded from a CDN).

## Notes

Stats are stored with `localStorage`, so they stay on the device and browser you used. Download the CSV if you need to keep a match or move it to another device.
