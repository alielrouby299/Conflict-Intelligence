# How We Work on GitHub

Short rules, so nobody gets lost. If something is unclear, ask in the group.

## 1. Branches

- `main` = the final, working version. **Nobody commits directly to `main`.**
- The project has **17 fixed branches**, one per area. The full list, with the owner and what goes in each one, is in **BRANCHES.md**.
- Do not create new branches without asking Ali.
- Upload your work to your branch (or send it to Ali). Branches are merged into `main` through a Pull Request.

## 2. Commit messages

Format: `type(scope): short message` (present tense, under 70 characters).

| Type | Use for | Example |
|---|---|---|
| `docs` | documents | `docs(planning): add risk assessment` |
| `data` | dataset versions | `data(interim): add dataset v0` |
| `feat` | new code or analysis | `feat(pipeline): add coordinate validation` |
| `fix` | fixing a mistake | `fix(sql): correct civilian deaths total` |
| `test` | tests | `test(checks): add duplicate check` |
| `chore` | folders, small cleanups | `chore: add folder structure` |

Bad: `update`, `final`, `new file`, `asdf`.

## 3. Pull Requests

1. When a branch is ready, open a Pull Request from that branch into `main`.
2. Fill in the template (what you added, which task number, how to check it).
3. The reviewer (table below) checks it within 2 days.
4. After approval, Ali merges it with **Squash and merge**.

| Author | Reviewer |
|---|---|
| Ali | Salma |
| Salma | Ali |
| Sara | Yasmeen |
| Yasmeen | Sara |
| Jessy | Ali |

## 4. Who owns which file

Every document and every piece of code has **one owner**. You edit only your own files. Some folders hold files of several people: add your own file there, and never change someone else's.

Use these file-name starts, so GitHub knows the owner (CODEOWNERS uses them):

| Folder | File name starts with | Owner |
|---|---|---|
| `docs/01-planning` | `proposal`, `project_plan`, `gantt`, `task_assignment` | Ali |
| `docs/01-planning` | `risk_assessment` | Salma |
| `docs/01-planning` | `project_kpis` | Sara |
| `docs/02-literature-review` | everything | Ali |
| `docs/03-requirements` | `requirements`, `use_case` | Jessy |
| `docs/dataset` | everything (data dictionary, dataset documentation) | Jessy |
| `docs/analysis` | `data_quality_report` | Ali |
| `docs/analysis` | `analytical_questions_kpis` | Sara |
| `docs/analysis` | `business_rules_kpi_definitions`, `analytical_results` | Yasmeen |
| `docs/04-design/architecture` | everything (architecture, technology stack) | Salma |
| `docs/04-design/database` | everything (ER diagram, schema) | Yasmeen |
| `docs/04-design/diagrams` | `dfd`, `sequence`, `activity`, `state`, `class` | Sara |
| `docs/04-design/diagrams` | `component`, `deployment` | Yasmeen |
| `docs/04-design/ui-ux` | everything (wireframes, mockups, guidelines) | Jessy |
| `docs/05-testing` | `test_plan`, `test_cases`, `bug_log`, `end_to_end`, `usability`, `reproducibility` | Jessy |
| `docs/05-testing` | `test_results_python` / `_sql_geographic` / `_powerbi` / `_database` / `_tableau` | Ali / Salma / Sara / Yasmeen / Jessy |
| `docs/06-final` | `final_report` | Jessy |
| `docs/06-final` | `presentation` | Yasmeen |
| `docs/06-final` | `user_manual` | Sara |
| `docs/06-final` | `technical_documentation`, `video` | Salma |
| `docs/technical-docs/python` | everything | Ali |
| `docs/technical-docs/sql` | everything | Salma |
| `docs/technical-docs/powerbi` | everything | Sara |
| `docs/technical-docs/database` | everything | Yasmeen |
| `docs/technical-docs/tableau` | everything | Jessy |
| `src/`, `data/`, `release/`, `notebooks/01` to `05` | code and datasets | Ali |
| `notebooks/06-geographic`, `sql/`, `validation/` | | Salma |
| `dashboards/powerbi` | | Sara |
| `dashboards/tableau`, `tests/` | | Jessy |

You can read and suggest changes everywhere. If you want to change someone else's file, ask the owner or open a Pull Request and tag the owner.

## 5. Files and sizes

- **Raw UCDP file:** never committed (it is in `.gitignore`). Keep it locally and document it in `data/raw/README.md`.
- **Power BI (.pbix) and Tableau (.twbx):** only the owner edits the file. GitHub cannot merge these files, so two people must never edit the same one.
- GitHub refuses any file bigger than 100 MB. If a file is that large, upload it to Drive and put the link in the README.
- Never commit passwords, keys or personal data.

## 6. File names

Short, clear, no spaces: `risk_assessment.docx`, `data_dictionary.xlsx`, `er_diagram_v2.png`. Use `v1`, `v2` for versions, never `final_final`.
