# Project Plan — Meal-prep

## Goal
Establish a predictable workflow from requirements → design → implementation → verification.

## Deliverables (initial)
- PRD template and first PRD
- Architecture overview + ADR process
- Backlog workflow (issues/work items) and sprint cadence
- CI scaffolding for .NET + React

## Workflow
1. **Discover**: Create/extend a PRD in `docs/prd/`.
2. **Decide**: Capture key decisions as ADRs in `docs/adr/`.
3. **Plan**: Break into epics/stories in `docs/planning/ROADMAP.md`.
4. **Deliver**: Implement via small PRs.
5. **Verify**: Tests + acceptance checks.

## Definition of Ready (DoR)
- Clear user value
- Acceptance criteria
- Data implications understood (tables/PII)
- Dependencies identified

## Definition of Done (DoD)
- Code merged
- Tests and lint pass
- Migration/script checked in for DB changes
- PRD/ADR updated if needed

## Open questions
- Auth strategy (Entra ID? local accounts?)
- Hosting target (Azure App Service / Container Apps / AKS?)
- Deployment pipeline: GitHub Actions, Azure DevOps, or both?
