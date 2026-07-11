# Agent Cron Timeline & Health Monitor — Implementation Spec

## Overview

A Next.js web GUI that visualizes all scheduled jobs (Hermes cron, system crontab,
systemd timers) on a Gantt-style timeline, with health status, run history,
and output preview. Reads from real infrastructure — no mocks.

## Data Sources

1. **Hermes cron jobs** — `~/.hermes/cron/jobs.json`
   - 19 YouTube watcher jobs, each with:
     - id, name, schedule (cron expr), enabled, state, paused_at/reason
     - last_run_at, next_run_at, last_status, last_error, last_delivery_error
     - deliver targets (origin, email, telegram)
     - model, provider, script
   - Schedule format: `{"kind": "cron", "expr": "1 3 * * *", "display": "1 3 * * *"}`

2. **Hermes cron output** — `~/.hermes/cron/output/<job_id>/<timestamp>.md`
   - One file per job run, named `YYYY-MM-DD_HH-MM-SS.md`
   - Most files are 0 bytes (empty output = agent ran successfully but produced
     no stdout to save). Some have markdown content.
   - File count per job = total run count
   - File modification time = run completion time

3. **System crontab** — `crontab -l`
   - Currently 2 entries: heartbeat (5min), email-to-wiki (10min)
   - Parse with cron expression parser

4. **Systemd user timers** — `systemctl list-timers --user --all --output json`
   - Currently 1 timer: launchpadlib cache clean
   - Has NEXT/LAST/PASSED timing data

## Architecture

```
agent-cron-monitor/
├── src/
│   ├── app/
│   │   ├── layout.tsx
│   │   ├── page.tsx                # Main view: timeline + job list + detail
│   │   └── api/
│   │       ├── jobs/
│   │       │   └── route.ts        # GET: list all jobs (Hermes + crontab + systemd)
│   │       ├── jobs/[id]/
│   │       │   └── route.ts        # GET: job detail + run history from output dir
│   │       └── runs/
│   │           └── route.ts        # GET: all recent runs across all jobs
│   ├── components/
│   │   ├── TimelineView.tsx        # Gantt-style timeline (horizontal time axis)
│   │   ├── JobList.tsx             # Scrollable job list with health badges
│   │   ├── JobDetail.tsx           # Expanded job view: schedule, history, output
│   │   ├── HealthBadge.tsx         # Color-coded status (green/yellow/red)
│   │   └── StatsBar.tsx            # Summary stats (total jobs, healthy, stale, failed)
│   ├── lib/
│   │   ├── db.ts                   # Read jobs.json, scan output dirs, parse crontab
│   │   ├── types.ts                # Job, Run, CronEntry, SystemdTimer types
│   │   ├── paths.ts                # File paths
│   │   └── cron-parser.ts          # Parse cron expressions to human-readable + next run
│   └── hooks/
│       ├── useJobs.ts              # Fetch + filter jobs
│       └── useJobDetail.ts         # Fetch job detail + run history
├── next.config.ts
├── tailwind.config.ts
├── package.json
└── README.md
```

## Tech Stack

- Next.js 15 (App Router, TypeScript)
- Tailwind CSS v4 + shadcn/ui (dark theme, same palette)
- better-sqlite3 not needed — data comes from JSON + filesystem
- cron-parser (npm package for human-readable cron expressions)
- lucide-react (icons)

## Key Design

### Timeline View
- Horizontal time axis (24h or 7d toggle)
- Each job is a row
- Dots/bars on the timeline show actual run times (from output file timestamps)
- Color: green (ok), yellow (stale > 2x interval), red (failed/error)
- Hover shows job name + run time + status
- Click a dot to open job detail

### Job List
- Cards/rows with: name, schedule (human-readable), next run (relative), last status badge
- Filter by: source (Hermes/crontab/systemd), status (all/healthy/stale/failed), enabled
- Sort by: next run, last run, name
- Click to expand detail

### Job Detail
- Schedule (cron expr + human-readable)
- Last run time + status + error if any
- Next run time
- Run history: list of output files with timestamps, file size (0 = empty/no output, >0 = has content)
- Click a run to preview its markdown output
- Delivery targets (origin, email, telegram)
- Model/provider info

### Health Logic
- **green**: last_status === "ok" AND last_run within expected interval
- **yellow**: last_status === "ok" BUT last_run > 2x expected interval (stale)
- **red**: last_status === "error" OR last_error is set
- **gray**: disabled/paused

## Task Breakdown (10 tasks)

| # | Task | Depends On |
|---|------|------------|
| 1 | Scaffold Next.js 15 + shadcn/ui + Tailwind | — |
| 2 | Types + paths + cron parser + job reader (db.ts) | 1 |
| 3 | Jobs API route (list all: Hermes + crontab + systemd) | 2 |
| 4 | Job detail API route (history from output dir) | 2 |
| 5 | Timeline view component (Gantt-style horizontal timeline) | 3 |
| 6 | Job list + health badges + stats bar | 3 |
| 7 | Job detail panel (run history + output preview) | 4 |
| 8 | Main page wiring (timeline + list + detail) | 5,6,7 |
| 9 | README + GitHub repo | 8 |
| 10 | Deploy (Vercel or local production) | 9 |