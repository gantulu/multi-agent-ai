# Contributing Guide

Panduan ini menetapkan cara menambahkan dan memelihara AI Agent di repository.

## Directory Convention

- Setiap agent harus memiliki direktori sendiri di `agents/`.
- Gunakan nama direktori lowercase dan kebab-case.
- Setiap direktori agent minimal memiliki `README.md`.
- Gunakan `templates/agent-template/README.md` sebagai kerangka awal.

## Required Documentation

Setiap profil agent harus menjelaskan:
1. Identity dan Mission.
2. Core Responsibilities.
3. Inputs dan Outputs.
4. Workflow.
5. Boundaries dan aturan keamanan.
6. Dependencies, jika ada.
7. Evaluation criteria.

## Catalog Maintenance

Saat menambahkan agent:
- Tambahkan tautan dan deskripsi singkat ke tabel Agent Catalog di root `README.md`.
- Pastikan nama dan path pada katalog sesuai dengan direktori agent.
- Perbarui dokumentasi bila tanggung jawab agent berubah secara signifikan.

## Quality Guidelines

- Satu agent harus memiliki fokus dan tanggung jawab yang jelas.
- Hindari duplikasi fungsi tanpa alasan yang terdokumentasi.
- Gunakan istilah dan format yang konsisten.
- Tandai asumsi dan kemampuan yang belum diverifikasi.
- Jangan menyimpan API keys, passwords, tokens, atau secrets di repository.
- Jangan memasukkan data pribadi atau rahasia ke dokumentasi publik.

## Changes and Review

Sebelum perubahan dianggap selesai:
- Periksa struktur dan tautan Markdown.
- Pastikan dokumentasi sesuai dengan implementasi aktual.
- Tinjau dampak perubahan terhadap agent lain dan katalog.
- Jalankan pemeriksaan otomatis jika tersedia.

## Scope

Panduan ini berlaku untuk seluruh direktori agent, template, dan dokumentasi di repository.
