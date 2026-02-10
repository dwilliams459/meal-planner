# Integrations (GitHub + Azure DevOps)

## Goal
Support development using either (or both):
- GitHub.com (issues + PRs + Actions)
- Azure DevOps (Boards + Repos + Pipelines)

## Suggested mapping
- Requirements: PRDs in `docs/prd/`
- Decisions: ADRs in `docs/adr/`
- Delivery tracking:
  - GitHub Issues *or* Azure DevOps Boards work items
  - PRs should link to the work item/issue

## CI/CD
- GitHub Actions starter: `.github/workflows/ci.yml`
- Azure Pipelines starter: `azure-pipelines.yml`

## MCP
- Repo includes a template `.vscode/mcp.template.json`.
- Copy to `.vscode/mcp.json` locally and configure commands/auth.
- Do not commit tokens; `.vscode/mcp.json` is gitignored.

## Next decisions
- Pick the source of truth for work tracking (GitHub vs Boards).
- Choose deployment target (Azure App Service/Container Apps/AKS).
