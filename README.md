# Multi-Agent AI

Repository terpusat untuk mendefinisikan, mendokumentasikan, dan mengembangkan AI Agent modular dengan spesialisasi, tanggung jawab, dan kemampuan reusable.

## Quick Start

Gunakan instruksi berikut di ChatGPT:

```text
Gunakan AI Agent dari repository gantulu/multi-agent-ai.
```

Panduan: [docs/USAGE.md](docs/USAGE.md).

## Agent Catalog

| AI Agent | Fokus |
|---|---|
| [AI Product Consultant](agents/ai-product-consultant/README.md) | Analisis kebutuhan, strategi produk, requirement, evaluasi solusi. |
| [AI Prompt Engineer](agents/ai-prompt-engineer/README.md) | Perancangan, evaluasi, dan optimasi prompt AI. |
| [AI Researcher](agents/ai-researcher/README.md) | Riset, verifikasi sumber, analisis, sintesis informasi. |
| [AI Coding Agent](agents/ai-coding-agent/README.md) | Implementasi, debugging, refactoring, verifikasi kode. |
| [AI Skill Architect](agents/ai-skill-architect/README.md) | Perancangan AI Skills dan integrasi Agent. |

Structured catalog: [registry/agents.json](registry/agents.json).

## Architecture

Arsitektur dibagi menjadi tujuh domain:

1. Identity & Behavior
2. Capabilities & Knowledge
3. Execution & Orchestration
4. Integration & Tools
5. Governance & Security
6. Monitoring & Evaluation
7. Configuration & Deployment

Baca [Architecture](docs/ARCHITECTURE.md) dan [Component Catalog](docs/COMPONENTS.md) untuk detail 48 komponen.

## Repository Structure

- `agents/` — definisi Agent.
- `instructions/` — instruksi sistem, perilaku, keamanan, dan standar kerja.
- `skills/` — kemampuan reusable.
- `workflows/` — proses kerja reusable.
- `prompts/`, `context/` — prompt dan panduan konteks.
- `knowledge/`, `memory/` — sumber pengetahuan dan kebijakan memori.
- `orchestration/`, `tasks/` — koordinasi dan unit pekerjaan.
- `tools/`, `integrations/` — kemampuan eksternal dan konektor.
- `governance/` — kontrol keamanan dan persetujuan.
- `observability/` — evaluasi, testing, dan pemantauan.
- `configuration/`, `registry/`, `schemas/` — konfigurasi, katalog, dan kontrak data.
- `templates/`, `docs/` — template dan dokumentasi.

## Principles

- Satu direktori untuk satu Agent, Skill, atau Workflow.
- Komponen reusable direferensikan, bukan diduplikasi.
- Setiap Agent memiliki scope, batasan, dan dependensi yang jelas.
- Tindakan berdampak eksternal memerlukan otorisasi dan approval yang sesuai.
- Catat asumsi, batasan, dan dependensi secara eksplisit.

## Contributing

Gunakan template di `templates/` dan ikuti [Contributing Guide](docs/CONTRIBUTING.md).
