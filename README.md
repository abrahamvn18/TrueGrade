# TrueGrade

Tells parents whether their kid is actually learning — or just letting AI do the homework.

## The idea

**Learning debt** = homework average − exam average, per subject, from Canvas gradebooks. Homework is AI-doable; in-person exams aren't. A big gap means the homework is being completed but the learning isn't.

- Under 10 → LOW · 10–20 → WATCH · over 20 → HIGH
- A widening trend matters more than one snapshot.
- "Worth a conversation," never proof of cheating.

## Demo (90 seconds)

1. Paste a Canvas token (or tap "use demo student").
2. Debt cards render: "Math — homework 94%, exams 61% — DEBT: HIGH".
3. Tap a course → trend lines splitting apart: "The homework is being completed. The learning isn't."
4. Parent view: "3 subjects to watch. Worth a conversation this week — not an accusation."

## Run it

Open `index.html` in a browser. Paste your Canvas token when prompted (Canvas → Account → Settings → New Access Token) — it stays in your browser and only talks to Canvas's API. No token? Tap "use demo student" for the offline fixture.

## How it works

- `data.js` — pulls courses, assignment groups, and submissions from the Canvas API (or loads the offline fixture)
- `engine.js` — classifies groups (homework vs exam), computes debt scores + trends
- `dashboard.js` / `parent.js` — the two views

## Built at

Ensign Build 2026 — Ensign College, Oct 9–10, 2026.

## AI disclosure

Built with AI coding assistance (Muse). All project code was written during the event.
