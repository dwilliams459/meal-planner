# Workflow

## Canonical flow
1. Write/iterate PRD in `docs/prd/`.
2. Capture key decisions as ADRs in `docs/adr/`.
3. Break PRD into tasks (use `docs/planning/TASK_TEMPLATE.md`).
4. Implement in small PRs.
5. Verify: tests + acceptance checks.

## Linking
- Work tracking source of truth: **Azure DevOps Boards**.
- Prefer linking PRs to a single work item.
- Include the work item in PR description using the `AB#<id>` convention.
- Prefer branch naming that includes the work item id, e.g. `feat/123-short-title`.

## Repository conventions
- No secrets in repo.
- DB changes must include migration scripts and rollout notes.
