Ali Hamdy +MIN5_DATA3_S1

# Conflict Intelligence – Global Conflict and Violence Analysis

DEPI Data Analyst track – final project.

We break wars down into thousands of individual events and analyze each one by place, time, parties, type of violence and deaths, to find where and when violence is concentrated, how its intensity changes over time, and which geographic and time patterns repeat.

## Dataset

- **Name:** UCDP Georeferenced Event Dataset (GED), Uppsala Conflict Data Program
- **Source:** https://ucdp.uu.se/downloads/#ged_global
- **Version:** _(fill in, e.g. 26.1)_
- **Period covered:** _(fill in after checking the file)_
- The original file is **never edited and never committed**. See `data/raw/README.md`.

## Team

| Member | Main role |
|---|---|
| Ali | Team Lead + Python / Data Analysis |
| Salma | SQL + Geographic Analysis + Data Validation |
| Sara | Power BI + KPI & Dashboard Analytics |
| Yasmeen | Database Design + BI Data Modeling + Analytical Results |
| Jessy | Tableau + Requirements + QA & Documentation |

## Official deadlines

| Date | What |
|---|---|
| 16 Oct 2026 | Planning, Literature Review, Requirements |
| 6 Nov 2026 | System Analysis & Design |
| 30 Nov 2026 | Implementation (source code & execution) |
| 4 Dec 2026 | Final presentation, testing & reports |

## Repository structure

```
docs/
  01-planning/            proposal, project plan, task assignment, risks, KPIs
  02-literature-review/   literature review, lecturer feedback, grading criteria
  03-requirements/        requirements gathering
  04-design/              architecture, database, diagrams, ui-ux
  05-testing/             test plan, test cases, bug log, reproducibility, usability
  06-final/               final report, presentation, user manual, video
  dataset/                dataset documentation and data dictionary
  technical-docs/         python, sql, powerbi, database, tableau
data/
  raw/                    original UCDP file (local only, not committed)
  interim/                dataset versions v0 and v1
  processed/              final analysis-ready dataset
src/pipeline/             data quality and cleaning code
notebooks/                01-data-quality ... 06-geographic
sql/                      database scripts, queries, analytical views
dashboards/               powerbi/ and tableau/
tests/                    automated data checks
validation/               cross-tool validation (SQL = Python = Power BI = Tableau)
release/                  final packaged files
```

## How we work

Read **CONTRIBUTING.md** (5 minutes). The short version:

1. Never work directly on `main`. Create your own branch.
2. Small commits with clear messages: `type(scope): message`.
3. Open a Pull Request. One teammate reviews it, then it is merged.
4. Every document goes in its folder, with a clear file name.

## Installation and execution

_To be completed by the README owner before 25 Nov: installation steps, system requirements, configuration instructions, execution guide._
