# Using the Multi-Agent AI Repository

## Start

Send this instruction in ChatGPT:

```text
Gunakan AI Agent dari repository gantulu/multi-agent-ai.
```

The assistant should read the current `README.md` and `registry/agents.json`, then display the available active Agents for selection.

## Discovery and selection

1. Read `registry/agents.json`; do not rely on a hardcoded or remembered Agent list.
2. Validate registry metadata against `schemas/agent-registry.schema.json` and `schemas/agent.schema.json`.
3. For a list request, show every active Agent with its category and short description.
4. For a task request, match the user's intent against Agent ID/name, category, tags, keywords, and description.
5. Prefer exact ID/name matches, followed by category/tag/keyword matches.
6. Recommend one clear match and proceed. Ask the user to choose only when multiple candidates are similarly suitable.
7. Read the selected Agent's registered `path`; never guess a path.
8. Apply shared instructions and load only the Skills, Workflows, Knowledge, and Tools required by that task.

Detailed contract: [Agent Discovery V1](AGENT-DISCOVERY.md).

## Example requests

- "Tampilkan daftar AI Agent."
- "Gunakan AI Product Consultant untuk audit requirement."
- "Pakai AI Researcher untuk riset kompetitor."
- "Gunakan AI Coding Agent untuk review repository ini."
- "Pilih AI Skill Architect untuk merancang Skill baru."

## Execution boundaries

- Define the requested outcome and acceptance criteria.
- Follow the selected Agent's scope, boundaries, and Workflow.
- Respect governance, security, tool permissions, and approval gates.
- Distinguish verified facts, assumptions, recommendations, and incomplete work.
- This repository provides documented definitions, metadata, and contracts. It does not by itself execute Agents; an AI assistant or external runtime must read and apply these resources.
