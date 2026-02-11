# Agents

This folder contains reusable role prompts for Copilot/LLM-assisted work.

Suggested flow:
1. Start with `docs/prd/PRD_TEMPLATE.md` (or a real PRD).
2. Record key decisions in `docs/adr/`.
3. Break work into tasks using `docs/planning/TASK_TEMPLATE.md`.

Agents:
- `tech-lead.md`
- `business-analyst.md`
- `dotnet-api.md`
- `react-frontend.md`
- `sqlserver-data.md`
- `devops-ci-cd.md`

## Starter prompts (copy/paste into Copilot Chat)

### Requirements (Business Analyst)
- “Act as the Business Analyst agent in `agents/business-analyst.md`. Ask me one question at a time to complete a PRD for Meal-prep. Don’t propose solutions yet. Stop when the PRD template can be fully filled.”
- “Using my answers, create `docs/prd/PRD_001_mvp.md` based on `docs/prd/PRD_TEMPLATE.md`. Keep language business-friendly and list assumptions + open questions.”
- “Turn `docs/prd/PRD_001_mvp.md` into 10–25 user stories with Given/When/Then acceptance criteria. Group by epic, and tag each story with a short priority (MVP/Next/Later).”

### Planning (Tech Lead)
- “Act as `agents/tech-lead.md`. Propose the minimal set of ADRs we need from `docs/prd/PRD_001_mvp.md` and draft them under `docs/adr/`.”
- “Break `docs/prd/PRD_001_mvp.md` into implementation tasks using `docs/planning/TASK_TEMPLATE.md`. Keep tasks small and verifiable.”

### Implementation (Engineers)
- “Act as `agents/dotnet-api.md`. Propose the API endpoints + DTOs implied by the PRD and outline a test plan.”
- “Act as `agents/react-frontend.md`. Propose the UI routes/screens and component boundaries implied by the PRD.”
- “Act as `agents/sqlserver-data.md`. Propose the core entities and draft a normalized SQL Server schema (tables + keys + indexes) implied by the PRD.”

### Delivery (DevOps)
- “Act as `agents/devops-ci-cd.md`. Update CI to build/test both .NET and React once they exist, and document required secrets without committing them.”
