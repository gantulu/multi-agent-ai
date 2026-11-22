# AI Agent Component Catalog

The 48 conceptual components are grouped into seven domains. They do not require 48 independent services or folders.

## 1. Identity & Behavior
| Component | Description |
|---|---|
| Agent | AI entity with defined identity, responsibilities, scope, and goals. |
| Instruction | Rules governing behavior, responsibilities, constraints, and methods. |
| System Prompt | Highest-level guidance supplied to the model/runtime. |
| Prompt | Task-specific input or direction for the AI. |
| Context | Relevant information needed to interpret a request. |
| Persona | Communication style and interaction characteristics. |
| Role | Functional position and responsibility in the system. |

## 2. Capabilities & Knowledge
| Component | Description |
|---|---|
| Skill | Reusable capability with domain guidance, methods, and procedures. |
| Knowledge Base | Curated collection of domain knowledge and documentation. |
| Memory | Persisted relevant information made available across tasks under policy. |
| Reference | Source material supporting work and claims. |
| Template | Reusable structure for consistent components or outputs. |
| Examples | Sample inputs, processes, and outputs showing expected behavior. |

## 3. Execution & Orchestration
| Component | Description |
|---|---|
| Workflow | Ordered process and decision points for completing work. |
| Task | Specific unit of work with an expected outcome. |
| Subtask | Smaller unit derived from or delegated by a parent task. |
| Orchestrator | Coordinates Agent selection, routing, and execution. |
| Planner | Converts a request into an execution plan. |
| Executor | Performs an approved action or workflow step. |
| Scheduler | Manages scheduled or queued execution. |
| Handoff | Transfers task ownership and context between Agents. |

## 4. Integration & Tools
| Component | Description |
|---|---|
| Tools | Callable capabilities for inspecting or changing external systems. |
| API | Contract for programmatic communication between systems. |
| MCP | Model Context Protocol for connecting AI applications to tools and context providers. |
| Connectors | Packaged integrations with external platforms. |
| Database | Structured persistence for application and operational data. |
| File System | Storage and access layer for files and artifacts. |

## 5. Governance & Security
| Component | Description |
|---|---|
| Guardrails | Policies and boundaries constraining Agent behavior and actions. |
| Permissions | Granted capabilities and access scope. |
| Authentication | Verification of a user or system identity. |
| Authorization | Decision about permitted resource/action access. |
| Validation | Checks that inputs, actions, and outputs meet requirements. |
| Approval | Human or policy gate before consequential actions. |
| Error Handling | Detection, reporting, recovery, and escalation of failures. |

## 6. Monitoring & Evaluation
| Component | Description |
|---|---|
| Evaluation | Measurement of output quality against acceptance criteria. |
| Testing | Repeatable checks for Agent, Skill, Workflow, and integrations. |
| Logging | Records of relevant events and execution outcomes. |
| Monitoring | Ongoing observation of system health and behavior. |
| Tracing | End-to-end view of a task across steps and Agent handoffs. |
| Metrics | Quantitative measures such as quality, latency, cost, and reliability. |
| Feedback | User/operator input used to improve the system. |

## 7. Configuration & Deployment
| Component | Description |
|---|---|
| Configuration | Parameters controlling system and component behavior. |
| Environment | Separation of development, test, and production settings. |
| Model | AI model selected for inference or other model tasks. |
| Model Routing | Model selection based on task needs, capabilities, and constraints. |
| Deployment | Release of an executable system into an operational environment. |
| Versioning | Identification and tracking of component revisions. |
| Documentation | Maintained explanation of architecture, usage, operations, and decisions. |

Implementation note: related components may share a service. For example, authentication and authorization may use one identity platform; logging and tracing may share an observability stack.
