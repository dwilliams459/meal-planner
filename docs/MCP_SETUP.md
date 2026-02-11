# MCP setup (GitHub + Azure DevOps)

This repo is intended to work well with Copilot Chat tooling and Model Context Protocol (MCP) servers.

## Goals
- Use MCP servers to interact with GitHub.com and Azure DevOps from your dev environment.
- Keep secrets out of the repo.

Work tracking source of truth: **Azure DevOps Boards**.
See `docs/devops/INTEGRATIONS.md` for the repo/project links and conventions.

## GitHub
- Install/enable the GitHub Pull Requests extension.
- Sign into GitHub in VS Code.
- Ensure the repo remote points at GitHub.

## Azure DevOps
- Install the Azure Repos / Azure Pipelines / Azure Boards extensions as needed.
- Sign into Azure DevOps in VS Code.

## MCP configuration
MCP server definitions are environment-specific (paths, auth, tenant/org). If your VS Code supports `mcp.json`, you can place a local config under `.vscode/mcp.json`.

This repo includes a template `.vscode/mcp.template.json` that you can copy to `.vscode/mcp.json` and customize locally.

## Security
- Use device code / OAuth login flows when available.
- Prefer per-user auth caches; do not store tokens in files.
