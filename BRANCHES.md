# Branches Guide

Each area of the project has **one branch**. Nobody creates a new branch without asking Ali.
Work is merged into `main` through a Pull Request when the owner says it is ready.

## The 17 branches

| # | Branch | Lead | Also contributes | What goes inside (folder → file names) | When |
|---|---|---|---|---|---|
| 1 | `docs/github-organization` | Ali | – | `README.md`, `CONTRIBUTING.md`, `BRANCHES.md`, `.gitignore`, `.github/`, folder structure, `data/raw/README.md` | 9 Oct |
| 2 | `docs/project-planning` | Ali | – | `docs/01-planning` → `proposal*`, `project_plan*`, `gantt*`, `task_assignment*` | 9 Oct |
| 3 | `docs/literature-review` | Ali | – | `docs/02-literature-review` → literature review, lecturer feedback, grading criteria | 16 Oct (feedback file updated until 4 Dec) |
| 4 | `docs/risk-architecture` | Salma | Sara, Yasmeen | `docs/01-planning/risk_assessment*` (Salma) · `docs/04-design/architecture` (Salma) · `docs/04-design/diagrams` → `dfd*`, `sequence*`, `activity*`, `state*`, `class*` (Sara) and `component*`, `deployment*`, deployment strategy (Yasmeen) | Risk 14 Oct · Architecture 23 Oct · Diagrams 6 Nov |
| 5 | `docs/requirements-data-dictionary` | Jessy | Yasmeen | `docs/dataset` → data dictionary, dataset documentation · `docs/03-requirements` → requirements, use case diagram and descriptions | Dictionary 14 Oct · Requirements 16 Oct · Use cases 27 Oct |
| 6 | `docs/kpis-analytics-design` | Sara | Yasmeen | `docs/01-planning/project_kpis*` · `docs/analysis` → `analytical_questions_kpis*` (Sara), `business_rules_kpi_definitions*` (Yasmeen) | KPIs 14 Oct · Questions 30 Oct · Rules 30 Oct |
| 7 | `analysis/python` | Ali | – | `src/pipeline` · `notebooks/01-data-quality` … `05-time-series` · `data/interim`, `data/processed` (small files) · `docs/analysis/data_quality_report*` · `docs/technical-docs/python` | v0 16 Oct · v1 23 Oct · final data 30 Oct · analysis 13 Nov |
| 8 | `database/modeling` | Yasmeen | – | `docs/04-design/database` → ER diagram, schema · `sql/schema` → table creation and loading · `docs/technical-docs/database` · database validation | ER 23 Oct · validation 13 Nov · docs 20 Nov |
| 9 | `sql/analysis-geospatial` | Salma | – | `sql/analysis`, `sql/views`, `sql/validation` · `notebooks/06-geographic` · `docs/technical-docs/sql` | SQL 13 Nov · views, geo 20 Nov |
| 10 | `powerbi/modeling` | Sara | Yasmeen | Power Query (M code as text), DAX measures (text files), data model notes, in `dashboards/powerbi/model-notes` | 13–20 Nov |
| 11 | `powerbi/dashboard` | Sara | Jessy | `dashboards/powerbi` → `.pbix` (Sara only) · `docs/04-design/ui-ux` → wireframes, mockups, guidelines (Jessy) · `docs/technical-docs/powerbi` | Wireframes 30 Oct · dashboard 20 Nov |
| 12 | `tableau/dashboard` | Jessy | – | `dashboards/tableau` → `.twbx` · `docs/technical-docs/tableau` | 20 Nov |
| 13 | `qa/validation` | Jessy | Salma, Yasmeen (and Ali, Sara for their own results) | `docs/05-testing` → `test_plan*`, `test_cases*`, `bug_log*`, `end_to_end*`, `usability*`, `reproducibility*`, `test_results_*` · `validation/` → cross-tool validation matrix and discrepancy log (Salma) · `docs/analysis/analytical_results*` validation (Yasmeen) | Plan 30 Oct · cross-tool 27 Nov · tests 2 Dec |
| 14 | `docs/documentation` | Ali | Whole team | `README.md` (final) · `docs/06-final/technical_documentation*` (Salma, structure by Jessy) · `docs/06-final/user_manual*` (Sara) · each owner's file in `docs/technical-docs/` | 25 Nov – 2 Dec |
| 15 | `final/video-demo` | Salma | Sara, Jessy | `docs/06-final/video*` (a link, the video itself goes on Drive) | 4 Dec |
| 16 | `final/presentation` | Yasmeen | Whole team (own slides) | `docs/06-final/presentation*` | 4 Dec |
| 17 | `final/integration` | Ali | Jessy | `release/` packaged final files · `docs/06-final/final_report*` (Jessy) · consistency check notes · final merge | 4 Dec |

## How work reaches GitHub

1. Do your work in your folder and name the file as in the table (file names matter, CODEOWNERS uses them).
2. Upload it to **your branch** (GitHub: switch to the branch, **Add file → Upload files**), or send it to Ali, who uploads it.
3. Commit message: `type(scope): message`, for example `docs(planning): add risk assessment`.
4. When a branch is ready, Ali opens a Pull Request into `main`. The reviewer checks it, then it is merged.

## Rules for shared branches

- A branch can have several contributors, but **a file has one owner**. Do not change someone else's file.
- `.pbix` and `.twbx` files cannot be merged by GitHub: only one person edits each file, and each new version is saved with a number (`dashboard_v1`, `dashboard_v2`).
- The raw UCDP dataset is never uploaded. Files larger than 100 MB are shared by link.
