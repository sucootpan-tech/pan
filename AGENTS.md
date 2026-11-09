# Repository Guidelines

## Project Structure & Module Organization

This project currently contains one requirements document, `報修需求筆記.txt`, describing a small repair-request registration demo. Treat it as the source of truth for scope. No application source, tests, assets, dependency manifests, or build configuration exist yet.

Planned deliverables include a web form and request list, Supabase schema and access rules, an Excel field dictionary with sample data, a six-slide PowerPoint proposal, and a Word user guide. When implementation begins, group application code, database migrations, tests, and deliverables in clearly named directories, and update this guide with their actual paths.

## Build, Test, and Development Commands

No build, development, lint, or test commands are currently configured. Do not assume `npm test` or other framework commands are available. To review the requirements in PowerShell, run:

```powershell
Get-Content -LiteralPath '報修需求筆記.txt' -Raw
```

When adding a technology stack, document its prerequisites and exact installation, local development, build, and verification commands here.

## Coding Style & Naming Conventions

Preserve UTF-8 encoding and the Traditional Chinese terminology used in the requirements. Use descriptive names and consistent indentation within each file. Once a language or framework is selected, configure its formatter and linter and record those conventions here. Avoid introducing unrelated tooling before implementation needs it.

## Testing Guidelines

There is no testing framework or coverage target yet. Future checks should verify required fields, category and urgency choices, automatic registration timestamps, successful submission, and list display. Database checks must confirm that anonymous users can insert and read requests but cannot update or delete them. Document test locations and naming conventions when tests are introduced.

## Commit & Pull Request Guidelines

This folder has no Git metadata, so no existing commit convention can be inferred. Use concise, imperative commit subjects, such as `Add repair request form`. Pull requests should explain scope, reference applicable requirements, list validation performed, and include screenshots for visible interface changes.

## Security & Scope

Use fictional names and locations only. Enable Supabase row-level security before exposing data through the frontend. Never commit privileged keys or credentials. The current demo supports creation and listing only; login, status updates, and notifications remain unresolved and require an explicit scope decision.
