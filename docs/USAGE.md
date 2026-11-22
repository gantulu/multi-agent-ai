# Menggunakan AI Agent

Dokumen ini menjelaskan cara memanggil katalog AI Agent dari ChatGPT menggunakan GitHub connector.

## Perintah Sederhana

Kirim instruksi ini di ChatGPT:

```text
Gunakan AI Agent dari repository gantulu/multi-agent-ai.
```

## Perilaku yang Diharapkan

Saat menerima perintah tersebut, ChatGPT harus:

1. Membuka repository `gantulu/multi-agent-ai` pada branch `main` melalui GitHub connector.
2. Membaca `README.md` untuk mendapatkan katalog agent.
3. Membaca README setiap agent di dalam direktori `agents/` agar daftar dan spesialisasinya berdasarkan dokumentasi terbaru.
4. Menampilkan nama, spesialisasi, deskripsi singkat, dan tautan dokumentasi setiap agent.
5. Meminta pengguna memilih agent. Jika pengguna belum yakin, rekomendasikan agent berdasarkan tugas yang ingin dikerjakan.
6. Setelah pengguna memilih, membaca kembali dokumentasi agent tersebut dan menerapkan identitas, misi, tanggung jawab, workflow, serta batasannya selama percakapan.
7. Jika pengguna sudah menyebut nama agent secara langsung, muat dokumentasi agent tersebut tanpa harus menampilkan seluruh katalog terlebih dahulu.

## Contoh Perintah Lanjutan

Setelah katalog ditampilkan, pengguna cukup menyebut nama agent, misalnya:

```text
Gunakan AI Product Consultant.
```

Atau langsung jelaskan tugasnya:

```text
Pilih AI Agent yang paling sesuai untuk membantu saya merancang aplikasi.
```

## Aturan Penting

- Gunakan isi repository sebagai sumber instruksi agent; jangan mengarang agent atau tanggung jawab yang tidak terdokumentasi.
- Selalu baca versi terbaru dari branch `main` sebelum menggunakan agent.
- Jika GitHub connector tidak tersedia atau akses repository gagal, jelaskan kendalanya dan jangan berpura-pura telah memuat instruksi.
- Pertahankan batasan dan workflow yang tertulis pada dokumentasi agent.
- Perubahan pada repository, database, deployment, atau sistem eksternal tetap memerlukan persetujuan eksplisit pengguna.
- Agent yang dimuat dengan cara ini berjalan sebagai **mode kerja dalam percakapan ChatGPT**. Ini bukan eksekusi agent terpisah atau sistem multi-agent runtime.

## Sumber

- [Repository](https://github.com/gantulu/multi-agent-ai)
- [Agent Catalog](../README.md)
- [Agent directories](../agents/)
