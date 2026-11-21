# QA → SDET Roadmap

A 12-week study plan for moving from Software Quality Engineer to SDET, with full lessons,
exercises, a live SQL practice database and progress tracking.

**Live site:** https://neeragrawal.github.io/qa-sdet-roadmap/

**Offline copy:** download [`QA-Comeback-Plan-offline.html`](https://github.com/NeerAgrawal/qa-sdet-roadmap/raw/main/QA-Comeback-Plan-offline.html)
and open it in Chrome or Edge. It works with no internet.

| Phase | Weeks | Topics |
|---|---|---|
| Launch | W00 | Tools, GitHub, profiles |
| SQL | W01–W02 | Queries, joins, window functions, data validation for QA |
| Automation | W03–W06 | Python, pytest, Selenium framework, API automation, CI/CD |
| AI QA | W07–W09 | Testing LLM and RAG apps, DeepEval, RAGAS, red-teaming, Playwright |
| Interviews | W10–W12 | Coding round, testing scenarios, mock interviews |

## Features

- Lessons with explanations, interview questions and exercises with answers
- SQL lessons run live in the browser against a practice database with planted data defects
- Progress tracking: coverage gauge, pipeline stages, week status (queued, running, passed),
  study streak and an activity grid
- Reset all progress or a single week, with Undo
- Export and import progress as a JSON backup
- An offline copy (`QA-Comeback-Plan-offline.html`) that works with no internet

Progress is saved in your browser's local storage. Use the same browser each time,
and export a backup now and then.

## Related projects

Portfolio repos built while following the plan (links added as each one ships):

- `sql-for-qa`: SQL data-quality checks run by pytest (Week 3)
- `saucedemo-selenium`: Selenium + pytest Page Object framework (Week 4)
- `qa-automation-framework`: UI + API framework with CI (Week 6)
- `llm-eval-suite`: evaluation and red-teaming suite for a RAG chatbot (Week 8)

## Files

| File | Purpose |
|---|---|
| `qa-comeback-plan.html` | Source of the page. Edit this one. |
| `lessons/` | Lesson content, one file per week |
| `build.py` | Generates `index.html` and the offline copy from the source |
| `index.html` | The GitHub Pages site (generated) |
| `QA-Comeback-Plan-offline.html` | Single-file offline copy (generated) |
| `vendor/sql-asm.js` | sql.js 1.10.3 (MIT), used by the offline copy |

After changing the page or adding lessons:

```
python build.py
git add .
git commit -m "Add Week 5 lessons"
git push
```
