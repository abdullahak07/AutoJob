# AutoJob

AutoJob is a live dashboard for Australian academic job opportunities and applications in Computer Science, AI, Machine Learning, Data Science, Cybersecurity and related fields.

## Live data flow

- `data/new-opportunities.json` contains jobs that have not been confirmed as applied.
- `data/applied-jobs.json` contains the Gmail-tracked application list and current statuses.
- `index.html` loads both files whenever the dashboard opens or Refresh is pressed.
- The academic job finder keeps New Opportunities synchronized.
- The Gmail tracker keeps Applied Jobs synchronized.
- When an application is confirmed, the matching role is removed from New Opportunities so it does not reappear.
- The Excel trackers remain the master/audit copies while this repository provides the website data layer.

## Dashboard features

- New Opportunities and Applied Jobs tabs
- Search and filters
- Closing-date sorting and deadline countdowns
- Direct job links
- Application-status badges
- Local New / Interested / Ignore controls for quick browser-side triage
- Responsive desktop and mobile layout
- Cache-bypassing Refresh button

## Repository structure

- `index.html` — dashboard UI
- `data/new-opportunities.json` — synchronized discovery data
- `data/applied-jobs.json` — synchronized application-status data

No build step or package installation is required.
