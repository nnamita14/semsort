# SemSort

Built by Team Stalwarts Coder: Namita Tiwari and Karan Upadhyay.

Sort your semester around real workload, not just due dates.

Students' assignments, internal tests, lab submissions and registrations have deadlines in different places, so conflicts only show up at the last moment. SemSort combines deadlines, workload and available study time into a realistic schedule.

## Features
- Task planner (assignments, internal tests, labs, registrations)
- Deadline calendar with crunch days highlighted
- Workload heatmap: "if you leave it late" vs "balanced plan"
- Priority engine: score = type weight x (hours left + 2) / (days left + 1)
- Conflict detection (3+ deadlines on one day, or more hours due than your daily limit) with an alternate schedule
- Rescheduling: earliest-deadline-first, capped by your daily study hours; log progress with +1h
- Class sharing with a class code
- Export deadlines as .ics

## Run locally
Open `index.html` in any browser. No build step, no dependencies.

## Tech stack
HTML, CSS and vanilla JavaScript in one file. Data is saved in the browser (localStorage). When hosted as a Claude artifact it also syncs to a database for private accounts and class sharing; outside that environment the app falls back to local storage and the Class tab is hidden behind a sign-in message.

## Files
- `index.html`: the whole app
- `docs/SemSort.pptx`: prototype presentation

## Demo
Open the app, tap "Load sample semester" and check the Overview tab: three deadlines on one day trigger a conflict card with an alternate plan.
