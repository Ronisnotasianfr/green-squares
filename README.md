# green-squares

Automated daily commits to keep the GitHub contribution graph green.

## How it works

A GitHub Actions workflow runs daily, updates a log file with the current date, and commits the change. A random delay is added so commits happen at different times each day.

## Setup

1. Push this repo to GitHub
2. Enable GitHub Actions (Settings > Actions > General)
3. That's it — the workflow runs automatically

## Customization

Edit `.github/workflows/daily-commit.yml` to change the schedule or commit message format.
