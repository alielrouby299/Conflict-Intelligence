# How We Work on GitHub

Short rules, so nobody gets lost. If something is unclear, ask in the group.

## 1. Branches

- `main` = the final, working version. **Nobody commits directly to `main`.**
- Every task is done on its own branch, created from `main`.
- Branch name: `area/short-description`

| Area | Example |
|---|---|
| `docs` | `docs/requirements` |
| `pipeline` | `pipeline/cleaning-v0` |
| `notebooks` | `notebooks/eda-trends` |
| `sql` | `sql/ranking-queries` |
| `powerbi` | `powerbi/data-model` |
| `tableau` | `tableau/geo-dashboard` |
| `tests` | `tests/data-quality-checks` |

When the work is merged, delete the branch.

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

1. Push your branch, then open a Pull Request into `main`.
2. Fill in the template (what you added, which task number, how to check it).
3. Ask your reviewer (table below). The reviewer answers within 2 days.
4. After approval, merge with **Squash and merge**, then delete the branch.

| Author | Reviewer |
|---|---|
| Ali | Salma |
| Salma | Ali |
| Sara | Yasmeen |
| Yasmeen | Sara |
| Jessy | Ali |

## 4. Who owns which folder

| Member | Folders |
|---|---|
| Ali | `docs/01-planning`, `docs/02-literature-review`, `src/pipeline`, `notebooks/01…05`, `data/`, `release/` |
| Salma | `sql/`, `notebooks/06-geographic`, `validation/`, `docs/04-design/architecture`, `docs/technical-docs/sql` |
| Sara | `dashboards/powerbi`, `docs/04-design/diagrams`, `docs/technical-docs/powerbi` |
| Yasmeen | `docs/04-design/database`, `docs/technical-docs/database`, `docs/06-final` (presentation) |
| Jessy | `docs/03-requirements`, `docs/dataset`, `docs/05-testing`, `dashboards/tableau`, `docs/04-design/ui-ux`, `docs/technical-docs/tableau` |

You can read and suggest changes everywhere. Only the owner edits his or her folder.

## 5. Files and sizes

- **Raw UCDP file:** never committed (it is in `.gitignore`). Keep it locally and document it in `data/raw/README.md`.
- **Power BI (.pbix) and Tableau (.twbx):** only the owner edits the file. GitHub cannot merge these files, so two people must never edit the same one.
- GitHub refuses any file bigger than 100 MB. If a file is that large, upload it to Drive and put the link in the README.
- Never commit passwords, keys or personal data.

## 6. File names

Short, clear, no spaces: `risk_assessment.docx`, `data_dictionary.xlsx`, `er_diagram_v2.png`. Use `v1`, `v2` for versions, never `final_final`.
