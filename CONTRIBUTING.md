# Contributing Guidelines

## 1. Branching Rules

The `main` branch is the protected and stable branch of the project.

Team members should create a separate branch before working on a new feature, analysis, data preparation, dashboard, or documentation.

### Branch Naming Convention

Use the following format:

`type/short-description`

Examples:

* `feature/conflict-analysis`
* `data/data-cleaning`
* `analysis/conflict-trends`
* `dashboard/powerbi-dashboard`
* `docs/project-documentation`
* `fix/missing-values`

Direct changes to the `main` branch should be avoided.

All changes should be merged into `main` through a Pull Request.

---

## 2. Commit Message Rules

All team members should use clear and meaningful commit messages.

### Format

`type: short description`

### Allowed Types

* `feat` — New feature or functionality
* `fix` — Bug fix or correction
* `docs` — Documentation changes
* `data` — Data cleaning or preparation
* `analysis` — Data analysis or EDA
* `dashboard` — Power BI or Tableau changes
* `refactor` — Code restructuring or improvement
* `test` — Testing and validation

### Examples

`feat: add conflict trend analysis`

`data: clean missing event locations`

`analysis: analyze yearly conflict events`

`dashboard: add conflict severity KPI`

`docs: update project README`

`fix: handle missing values`

### Commit Guidelines

* Keep commit messages clear and concise.
* Use the appropriate type.
* Keep each commit focused on one logical change.
* Avoid vague messages such as `update`, `changes`, `final`, or `stuff`.
* Write commit messages in English.

---

## 3. Pull Request Rules

All changes intended for the `main` branch must be submitted through a Pull Request.

Each Pull Request should:

1. Have a clear and descriptive title.
2. Explain what was changed.
3. Explain why the change was made.
4. Include relevant screenshots or evidence when applicable.
5. Be reviewed by at least one team member.
6. Resolve all review conversations before merging.
7. Ensure that the branch is up to date before merging when required.

The `main` branch should not be modified directly.

---

## 4. Code and Data Guidelines

* Keep files organized according to the project structure.
* Do not commit sensitive information such as passwords, API keys, or private credentials.
* Do not upload unnecessary large temporary files.
* Keep data processing and analysis steps reproducible whenever possible.
* Use clear and meaningful file names.
* Avoid committing generated or temporary files unless they are required by the project.

---

## 5. Team Workflow

The standard workflow is:

`Create Branch → Work → Commit → Push → Pull Request → Review → Approval → Merge`

All team members should follow this workflow to maintain a clean and organized project repository.

