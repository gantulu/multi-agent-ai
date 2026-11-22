# Multi-Agent AI

Repository terpusat untuk menyimpan, mendokumentasikan, dan mengembangkan berbagai AI Agent dengan spesialisasi, tanggung jawab, dan instruksi yang berbeda.

## Agent Catalog

| AI Agent | Fokus |
|---|---|
| [AI Product Consultant](agents/ai-product-consultant/README.md) | Analisis kebutuhan, strategi produk, requirement, dan evaluasi solusi. |
| [AI Prompt Engineer](agents/ai-prompt-engineer/README.md) | Perancangan, evaluasi, dan optimasi prompt AI. |
| [AI Researcher](agents/ai-researcher/README.md) | Riset, verifikasi sumber, analisis, dan sintesis informasi. |
| [AI Coding Agent](agents/ai-coding-agent/README.md) | Implementasi, debugging, refactoring, dan verifikasi kode. |
| [AI Skill Architect](agents/ai-skill-architect/README.md) | Perancangan dan pengembangan AI Skills serta integrasi agent. |

## Quick Start

Untuk menampilkan katalog dan memilih AI Agent melalui ChatGPT, gunakan satu instruksi:

```text
Gunakan AI Agent dari repository gantulu/multi-agent-ai.
```

ChatGPT akan membaca katalog dan dokumentasi agent melalui GitHub connector, menampilkan daftar agent, lalu meminta pengguna memilih. Setelah dipilih, dokumentasi agent digunakan sebagai panduan kerja dalam percakapan.

Panduan lengkap: [Menggunakan AI Agent](docs/USAGE.md).

## Repository Structure

```text
multi-agent-ai/
├── README.md
├── agents/
│   ├── ai-product-consultant/
│   │   └── README.md
│   ├── ai-prompt-engineer/
│   │   └── README.md
│   ├── ai-researcher/
│   │   └── README.md
│   ├── ai-coding-agent/
│   │   └── README.md
│   └── ai-skill-architect/
│       └── README.md
├── templates/
│   └── agent-template/
│       └── README.md
└── docs/
    └── CONTRIBUTING.md
```

## Menambahkan Agent

1. Buat folder baru di dalam `agents/` menggunakan nama yang deskriptif dan konsisten.
2. Tambahkan `README.md` yang menjelaskan identitas, tujuan, ruang lingkup, instruksi, dan batasan agent.
3. Gunakan [Agent Template](templates/agent-template/README.md) sebagai titik awal.
4. Tambahkan agent baru ke tabel Agent Catalog di atas.

## Prinsip

- Satu direktori untuk satu AI Agent.
- Setiap agent memiliki spesialisasi dan instruksi yang jelas.
- Dokumentasi agent dikelola secara independen.
- Hindari duplikasi tanggung jawab antar-agent.
- Catat asumsi, batasan, dan dependensi secara eksplisit.

Lihat [Contributing Guide](docs/CONTRIBUTING.md) untuk aturan kontribusi.
