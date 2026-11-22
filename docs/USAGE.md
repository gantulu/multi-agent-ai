# Using the Multi-Agent AI Repository

## Start
Send this instruction:

```text
Gunakan AI Agent dari repository gantulu/multi-agent-ai.
```

## Discovery and selection
1. Read README.md and registry/agents.json.
2. Present available Agents with a short description.
3. Ask the user to select an Agent if the intended specialist is not obvious.
4. Read the selected Agent's README and follow its scope and constraints.
5. Load only the referenced Skills, Workflows, Instructions, Knowledge, and Tools needed.
6. If the request clearly implies one Agent, recommend it and proceed without unnecessary selection friction.

## Execution
- Define the requested outcome and acceptance criteria.
- Follow the selected Workflow where one exists.
- Respect approval gates and repository/tool permissions.
- This repository provides documented definitions and registries; it does not by itself execute Agents. An AI runtime or connector must consume these resources.

## Request examples
- "Tampilkan daftar AI Agent."
- "Gunakan AI Product Consultant untuk audit requirement."
- "Gunakan AI Coding Agent untuk review repository ini."
- "Gunakan AI Skill Architect untuk membuat Skill baru."
