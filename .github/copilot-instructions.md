# Copilot instructions — Meal-prep

You are GitHub Copilot operating as a coding agent in this repository.

## Mission
Help deliver the Meal-prep product using a workflow of:
1) PRD → 2) Architecture/ADRs → 3) Plan/Tasks → 4) Implementation → 5) Verification.

## Where things live
- PRDs: `docs/prd/`
- Architecture: `docs/architecture/`
- ADRs: `docs/adr/`
- Planning & templates: `docs/planning/`

## Operating rules
- Prefer small, reviewable PRs.
- Don’t invent requirements; if unclear, ask.
- Don’t add new UI/UX beyond the requested scope.
- Never commit secrets. Use env vars and document required settings.
- For DB changes, document migration strategy and include scripts/migrations.

## Quality bar
- Backend: consistent API patterns, validation, error handling, tests.
- Frontend: accessible, predictable state handling, typed API client.
- Observability: structured logs and minimal telemetry hooks.
