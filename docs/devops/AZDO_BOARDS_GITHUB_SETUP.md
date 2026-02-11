# Azure DevOps Boards + GitHub repo setup

## Goal
Use Azure DevOps Boards for work tracking while hosting code on GitHub.

## Links
- GitHub repo: https://github.com/dwilliams459/meal-planner
- Azure DevOps project: https://dev.azure.com/dwilliams459/Meal%20Prep

## One-time setup (manual)
1. In Azure DevOps, open the project settings and connect the GitHub repository so Boards can surface PR/commit development links.
2. Ensure your team members are authenticated to both Azure DevOps and GitHub.

## Day-to-day conventions
- Create a work item in Azure DevOps Boards first.
- Create a branch for the work item (recommended): `feat/<id>-short-title`.
- In GitHub PR descriptions, include the work item reference: `AB#<id>`.
- Keep PRs small and link them to exactly one work item when possible.

## Optional enforcement (later)
- Enable policies/rules that require work items to be linked to PRs before merge (capability depends on your exact setup and whether you use GitHub branch protection, Azure Repos policies, or additional tooling).
