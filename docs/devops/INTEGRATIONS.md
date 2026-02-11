# Integrations (GitHub + Azure DevOps)

## Goal
Support development using either (or both):
- GitHub.com (issues + PRs + Actions)
- Azure DevOps (Boards + Repos + Pipelines)

This project will use:
- **Azure DevOps Boards** for work tracking
- **GitHub** for source control

## Project links
- GitHub repo: https://github.com/dwilliams459/meal-planner
- Azure DevOps project: https://dev.azure.com/dwilliams459/Meal%20Prep

## Suggested mapping
- Requirements: PRDs in `docs/prd/`
- Decisions: ADRs in `docs/adr/`
- Delivery tracking:
  - Azure DevOps Boards work items
  - PRs should link to the work item

## Linking conventions (recommended)
- PR descriptions should include `AB#<work-item-id>`
- If you want stricter hygiene, enable Azure DevOps branch policies / GitHub rules to require linked work items (process-dependent)

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
