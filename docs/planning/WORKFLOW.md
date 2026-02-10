# Workflow

## Canonical flow
1. Write/iterate PRD in `docs/prd/`.
2. Capture key decisions as ADRs in `docs/adr/`.
3. Break PRD into tasks (use `docs/planning/TASK_TEMPLATE.md`).
4. Implement in small PRs.
5. Verify: tests + acceptance checks.

## Linking
- Prefer linking PRs to a single issue/work item.
- If using Azure DevOps Boards, include the work item ID in PR title/body.

## Repository conventions
- No secrets in repo.
- DB changes must include migration scripts and rollout notes.
