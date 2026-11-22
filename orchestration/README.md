# Orchestration

Orchestration coordinates Agent discovery, routing, task planning, execution, and handoff.

## V1 behavior contract
1. Read the user request and identify the expected outcome.
2. Discover candidates from registry/agents.json.
3. Select a clear best match or ask the user to choose when multiple Agents are similarly suitable.
4. Read the selected Agent definition and referenced components.
5. Preserve task context and acceptance criteria during handoff.
6. Enforce governance and approval requirements.
7. Return a consolidated result and disclose incomplete steps.

This directory documents the orchestration contract; it does not contain an executable runtime.
