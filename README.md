# green-squares

Automated commits at random times to keep the GitHub contribution graph green.

## How it works

A GitHub Actions workflow runs every hour. A Python script (`commit.py`) picks
3–5 random days per week to commit, generates 3–15 commits on those days, and
sleeps a random amount before each commit so timestamps land at random minutes
throughout the day.

## Setup

1. Push this repo to GitHub
2. Enable GitHub Actions (Settings > Actions > General)
3. That's it — the workflow runs automatically

## Customization

- `.github/workflows/activity.yml` — schedule and git identity
- `commit.py` — quotes, commit messages, and randomization logic
- `.commit_tracker.json` — per-day and per-week commit tracking (auto-generated)
