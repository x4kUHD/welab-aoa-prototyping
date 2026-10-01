# welab-aoa-prototyping

A sandbox for **HTML prototyping**. It's where we quickly sketch, demo, and review feature ideas for the Parish Management System (PMS), the facility-management tool being built by the Georgia Tech WE Lab for the Archdiocese of Atlanta (AOA).

Nothing here is production code. Prototypes are disposable and meant to be easy to read, change, and show to people.

## About the project

Parishes manage large physical assets (worship spaces, schools, offices) with limited capital, aging infrastructure, and mostly volunteer, reactive maintenance. PMS aims to help parishes move from reactive to diagnostic facility management, with a simple, low-effort interface for non-technical users.

Prototypes here explore PMS features such as the dashboard, asset tracking, utility use, building valuations, active risks and backlog, finances, and history.

## How prototyping works here

- Everything lives in a single file: `prototype.html`, with inline CSS and vanilla JS.
- No frameworks, no build step, no bundlers, no package installs. A CDN `<script>` tag is fine if a prototype needs a library.
- Data is mocked in the page and resets on reload.

See `AGENT.md` for the full rules.

## Run locally

```
npm run dev
```

Serves the repo at http://localhost:3000.
