# Salary Tracker

A simple, single-file tracker for where a monthly salary goes: record expenses by category, see what's spent, saved and left, and compare the last 6 months.

## Use it
Open `index.html` in any browser. No build step, no dependencies, no server.

## Where data is stored
- **On claude.ai** (as a Claude artifact): saved privately to your Claude account and synced across devices, with a copy on the device.
- **Anywhere else** (GitHub Pages, opened from disk): saved in that browser's local storage only. Use ⚙ → **Backup** regularly; **Restore** moves data to another browser or device.

## Features
- Quick entry: amount, category, optional note, date
- Ring chart and category bars as a share of salary
- Savings / SIP / investments counted as saved, not spent
- **My savings**: savings you already have (bank, FD…) plus what you save/invest and unspent salary from finished months
- Per-month salary override (hike, bonus) and optional savings target with a daily allowance
- Last-6-months spent / saved / left comparison
- Light and dark mode; CSV export; JSON backup and restore

## Notes
- Amounts are stored as whole paise (integers), so totals have no rounding drift.
- The default salary (₹1,95,000) and categories are set in `freshSettings()` near the top of the script.
