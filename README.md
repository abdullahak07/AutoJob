# AutoJob

AutoJob is a live dashboard for Australian academic job opportunities and applications in Computer Science, AI, Machine Learning, Data Science, Cybersecurity and related fields.

## How it works

- `data/new-opportunities.json` contains jobs that have not been confirmed as applied.
- `data/applied-jobs.json` contains the Gmail-tracked application list and current statuses.
- `index.html` loads both data files on every page load or manual refresh.
- The academic job finder updates new opportunities automatically.
- The Gmail job-status tracker updates applied jobs automatically.
- When an application is confirmed, the matching role is removed from New Opportunities.
- Every update committed to `main` triggers the GitHub Pages deployment workflow.

## Dashboard features

- New Opportunities and Applied Jobs tabs
- Search and filters
- Closing-date sorting and deadline countdowns
- Direct job links
- Application-status badges
- Local New / Interested / Ignore controls for quick browser-side triage
- Responsive desktop and mobile layout
- Refresh button that bypasses cached tracker data

## Files

- `index.html` — dashboard UI
- `data/new-opportunities.json` — live discovery data
- `data/applied-jobs.json` — live applied-job data
- `.github/workflows/pages.yml` — automatic GitHub Pages deployment

No build step or package installation is required.
