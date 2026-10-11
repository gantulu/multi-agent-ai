# GEMINI CREATE MUSIC — MASTER PROMPT TEMPLATE v2.1

**Status:** Draft revisi disetujui untuk disusun
**Versi:** 2.1
**Tujuan:** Menyediakan kerangka prompt yang terstruktur, fleksibel, dan selaras dengan dokumentasi resmi pembuatan musik di aplikasi Gemini.

## Riwayat versi

- **Draft v1:** Referensi awal yang dikunci dan tidak diubah.
- **Draft v2:** Master Prompt Template yang disetujui sebelumnya dan dipertahankan sebagai arsip.
- **Draft v2.1:** Revisi berdasarkan audit dokumentasi resmi, dengan pemisahan prompt, modul lanjutan, dan pengaturan aplikasi.

***

# BAGIAN I — TUJUAN DAN PRINSIP

## 1. Tujuan

Template ini membantu pengguna mengarahkan pembuatan musik dengan menentukan:

- Genre dan identitas musik.
- Suasana dan perjalanan emosi.
- Tempo, nada dasar, dan karakter musikal.
- Instrumen, ritme, serta groove.
- Vokal dan lirik.
- Struktur lagu dan transisi.
- Dinamika, produksi, dan karakter akhir musik.
- Pengaturan aplikasi yang relevan.

Template ini merupakan kerangka kerja kreatif, bukan daftar kontrol resmi yang semuanya dijamin tersedia di aplikasi Gemini.

## 2. Prinsip penggunaan

1. Letakkan genre dan arah musik utama di awal prompt.
2. Gunakan deskripsi yang konkret dan saling mendukung.
3. Pilih modul sesuai kebutuhan; tidak semua variabel wajib digunakan.
4. Bedakan instruksi teks dengan pengaturan antarmuka aplikasi.
5. Perlakukan BPM, nada dasar, durasi, dan penanda waktu sebagai arahan, bukan jaminan presisi.
6. Jika hasil kurang sesuai, buat generasi baru dengan memperbaiki beberapa instruksi utama.
7. Hindari arahan yang bertentangan, misalnya meminta musik sangat minimalis sekaligus meminta banyak lapisan instrumen sejak awal.

***

# BAGIAN II — CORE PROMPT

## 3. Variabel inti

|Variabel|Fungsi|Contoh|
|---|---|---|
|`{{GENRE}}`|Genre utama|pop, rock, jazz, electronic|
|`{{SUBGENRE}}`|Subgenre atau pengaruh|dream pop, synthwave, jazz fusion|
|`{{MOOD}}`|Suasana musik|nostalgic, dreamy, uplifting|
|`{{MUSICAL_IDENTITY}}`|Ciri khas utama|memorable piano motif and airy synths|
|`{{BPM}}`|Tempo sasaran|around 95 BPM|
|`{{INSTRUMENTS}}`|Instrumen utama|piano, electric guitar, analog synth|
|`{{RHYTHM}}`|Ritme dan groove|relaxed half-time groove|
|`{{VOCAL_MODE}}`|Mode vokal|instrumental, lead vocals|
|`{{STRUCTURE}}`|Susunan bagian lagu|intro, verse, chorus, bridge, outro|
|`{{DYNAMICS}}`|Perkembangan energi|sparse opening, gradual build, powerful chorus|
|`{{PRODUCTION_DIRECTION}}`|Karakter produksi secara ringkas|polished, warm, spacious production|
|`{{ENDING}}`|Cara mengakhiri musik|resolved final chord, gradual fade|
|`{{RESTRICTIONS}}`|Arahan negatif opsional|no abrupt ending, no aggressive distortion|

## 4. Core Prompt Template

```text
Create a music track in the style of {{GENRE}},
incorporating elements of {{SUBGENRE}}.

Mood and atmosphere: {{MOOD}}.

Musical identity: {{MUSICAL_IDENTITY}}.

Tempo: {{BPM}} BPM.

Instrumentation: {{INSTRUMENTS}}.

Rhythm and groove: {{RHYTHM}}.

Vocal mode: {{VOCAL_MODE}}.

Arrangement and structure: {{STRUCTURE}}.

Energy development: {{DYNAMICS}}.

Production direction: {{PRODUCTION_DIRECTION}}.

Ending: {{ENDING}}.

Restrictions: {{RESTRICTIONS}}.

Maintain a coherent musical identity throughout the track.
Ensure that the genre, instrumentation, rhythm, arrangement,
and production work together naturally.
```

Gunakan bagian ini sebagai dasar. Tambahkan modul lanjutan hanya jika diperlukan.

***

# BAGIAN III — CREATIVE DIRECTION

## 5. Arah kreatif dan emosi

|Variabel|Fungsi|Contoh|
|---|---|---|
|`{{EMOTIONAL_DIRECTION}}`|Perjalanan emosi|starts lonely, gradually becomes hopeful|
|`{{MUSICAL_IDENTITY}}`|Ciri khas musikal|recurring piano motif, shimmering synths|
|`{{VISUAL_DESCRIPTION}}`|Inspirasi visual dalam bentuk teks|cinematic night drive through a rainy city|

Contoh:

```text
Creative direction:
{{EMOTIONAL_DIRECTION}}

Musical identity:
{{MUSICAL_IDENTITY}}

Visual atmosphere described in words:
{{VISUAL_DESCRIPTION}}
```

`{{VISUAL_DESCRIPTION}}` hanya merupakan deskripsi teks. Jika ingin menggunakan gambar atau video sebagai input, unggah media tersebut melalui fitur aplikasi yang mendukungnya.

## 6. Tempo, nada dasar, melodi, dan harmoni

|Variabel|Fungsi|Contoh|
|---|---|---|
|`{{BPM}}`|Tempo sasaran|around 95 BPM|
|`{{KEY}}`|Nada dasar atau karakter tonal|A minor, warm major tonality|
|`{{MELODY_STYLE}}`|Karakter melodi|flowing, memorable, gently rising|
|`{{HARMONY_STYLE}}`|Karakter harmoni|rich extended chords, simple pop harmony|

Template:

```text
Tempo: {{BPM}} BPM.

Key and tonality: {{KEY}}.

Melody style: {{MELODY_STYLE}}.

Harmony style: {{HARMONY_STYLE}}.
```

Nilai BPM dan nada dasar dapat dicoba sebagai arahan musikal, tetapi hasilnya tidak dijamin tepat secara teknis.

## 7. Instrumen, tekstur, dan groove

|Variabel|Fungsi|Contoh|
|---|---|---|
|`{{INSTRUMENTS}}`|Instrumen utama|electric piano, bass, drums|
|`{{SUPPORTING_TEXTURES}}`|Lapisan pendukung|ambient pads, soft strings|
|`{{DRUM_STYLE}}`|Karakter drum|tight kick, soft snare, restrained hi-hats|
|`{{BASS_STYLE}}`|Karakter bass|warm rounded bass, melodic movement|
|`{{RHYTHM}}`|Groove|relaxed half-time groove|

Template:

```text
Main instruments: {{INSTRUMENTS}}.

Supporting textures: {{SUPPORTING_TEXTURES}}.

Drum and percussion style: {{DRUM_STYLE}}.

Bass character: {{BASS_STYLE}}.

Rhythm and groove: {{RHYTHM}}.
```

Pilih instrumen yang mendukung genre. Jika menginginkan suara yang minimalis, batasi jumlah instrumen dan jelaskan kapan lapisan tambahan mulai masuk.

***

# BAGIAN IV — VOKAL DAN LIRIK

## 8. Modul vokal

|Variabel|Fungsi|Contoh|
|---|---|---|
|`{{VOCAL_MODE}}`|Vokal atau instrumental|lead vocals, instrumental only|
|`{{VOCAL_PROFILE}}`|Karakter suara|soft airy voice, warm mid-range timbre|
|`{{VOCAL_DELIVERY}}`|Cara bernyanyi|restrained verses, expressive chorus|
|`{{BACKING_VOCALS}}`|Vokal latar|subtle harmonies in the final chorus|
|`{{LANGUAGE}}`|Bahasa lirik|Indonesian, English|

Template:

```text
Vocal mode: {{VOCAL_MODE}}.

Vocal profile and timbre: {{VOCAL_PROFILE}}.

Vocal delivery: {{VOCAL_DELIVERY}}.

Backing vocals: {{BACKING_VOCALS}}.

Lyrics language: {{LANGUAGE}}.
```

### Aturan untuk musik instrumental

Jika menginginkan musik tanpa vokal, gunakan instruksi eksplisit:

```text
Instrumental only. No vocals or lyrics.
```

Untuk musik instrumental, variabel profil vokal, penyampaian vokal, backing vocals, dan bahasa lirik tidak perlu diisi.

## 9. Modul lirik

|Variabel|Fungsi|Contoh|
|---|---|---|
|`{{LYRICS_MODE}}`|Cara menangani lirik|generate original lyrics, use provided lyrics, instrumental|
|`{{LYRICS_THEME}}`|Tema cerita|remembering someone while learning to move forward|
|`{{LYRICS_CONTENT}}`|Lirik yang disediakan pengguna|teks lirik lengkap dengan penanda bagian|

### A. Lirik dibuat oleh model

```text
Lyrics mode: generate original lyrics.

Lyrics language: {{LANGUAGE}}.

Theme: {{LYRICS_THEME}}.

The lyrics should have a clear emotional arc and a memorable
chorus. Keep the wording natural and appropriate for the genre.
```

### B. Menggunakan lirik yang diberikan pengguna

```text
Lyrics mode: use the provided lyrics.

Lyrics language: {{LANGUAGE}}.

Lyrics:
{{LYRICS_CONTENT}}
```

Jika fitur mendukungnya, gunakan penanda bagian untuk menunjukkan susunan lirik:

```text
[Verse 1]
...

[Pre-Chorus]
...

[Chorus]
...

[Verse 2]
...

[Bridge]
...

[Final Chorus]
...

[Outro]
...
```

Pisahkan instruksi musikal dari teks lirik agar struktur dan isi lebih mudah dipahami.

### C. Musik instrumental

```text
Lyrics mode: instrumental.

Instrumental only. No vocals or lyrics.
```

Ketersediaan metode input lirik tertentu bergantung pada mode atau antarmuka yang digunakan.

***

# BAGIAN V — STRUKTUR, WAKTU, DAN DINAMIKA

## 10. Struktur lagu

Variabel: `{{STRUCTURE}}`

### A. Pop dengan vokal

```text
Intro → Verse 1 → Pre-Chorus → Chorus →
Verse 2 → Chorus → Bridge → Final Chorus → Outro
```

### B. Instrumental sinematik

```text
Ambient Intro → Main Theme → Gradual Build →
Emotional Peak → Breakdown → Final Theme → Outro
```

### C. Musik elektronik

```text
Intro → Build-up → Drop → Main Groove →
Breakdown → Second Build-up → Final Drop → Outro
```

### D. Musik ambient

```text
Atmospheric Opening → Gradual Texture Development →
Harmonic Evolution → Peak Texture → Fade Out
```

Pilih satu struktur utama dan sesuaikan dengan genre serta durasi sasaran.

## 11. Timing markers

Variabel: `{{TIMING_MARKERS}}`

Gunakan penanda waktu untuk mengarahkan perubahan instrumen, masuknya vokal, atau perkembangan energi.

Contoh:

```text
[0:00–0:10] Intro:
Soft piano and ambient textures.

[0:10–0:30] Verse:
Introduce lead vocals and a gentle beat.

[0:30–0:50] Chorus:
Fuller drums, wider instrumentation, and stronger melody.

[0:50–1:00] Outro:
Return to piano and resolve naturally.
```

Sesuaikan waktu dengan durasi sasaran. Penanda waktu merupakan arahan kreatif dan tidak menjamin setiap bagian dimulai tepat pada detik yang ditentukan.

## 12. Dinamika dan perkembangan energi

Variabel: `{{DYNAMICS}}`

Contoh:

```text
Start with minimal instrumentation.
Gradually introduce rhythmic and harmonic layers.
Make the chorus wider and more energetic.
Create a quieter bridge.
Build toward an emotionally strong final chorus.
End with a controlled, natural resolution.
```

Gunakan dinamika untuk mengarahkan perubahan energi dari awal hingga akhir, bukan hanya untuk meminta musik terdengar “lebih megah” atau “lebih emosional”.

***

# BAGIAN VI — PRODUKSI DAN EFEK

## 13. Production direction

Untuk prompt sederhana, gunakan:

`{{PRODUCTION_DIRECTION}}`

Contoh:

```text
Warm, organic production with clear vocals, a defined bass,
spacious synthesizers, and balanced instrumentation.
```

Untuk kebutuhan lebih terperinci, pecah menjadi modul berikut.

|Variabel|Fungsi|Contoh|
|---|---|---|
|`{{PRODUCTION}}`|Karakter produksi|polished modern production|
|`{{MIX_STYLE}}`|Karakter keseimbangan suara|clear vocals, defined bass|
|`{{SPACE_AND_AMBIENCE}}`|Ruang dan ambience|intimate verses, wide chorus|
|`{{EFFECTS}}`|Efek dan transisi|subtle risers, reverb tails|

Template lanjutan:

```text
Overall production: {{PRODUCTION}}.

Mix characteristics: {{MIX_STYLE}}.

Space and ambience: {{SPACE_AND_AMBIENCE}}.

Effects and transitions: {{EFFECTS}}.
```

Modul-modul ini merupakan deskripsi sonik, bukan kontrol mixing terpisah yang dijamin tersedia di aplikasi.

## 14. Ending

Variabel: `{{ENDING}}`

Contoh:

- Resolve with a warm final chord.
- Fade out gradually with lingering ambient textures.
- End with a short instrumental tail.
- Return to the main motif for a reflective ending.

Pilih satu arahan akhir yang sesuai dengan struktur musik.

## 15. Restrictions

Variabel: `{{RESTRICTIONS}}`

Contoh:

```text
Avoid aggressive distortion, overly busy percussion,
abrupt transitions, and an excessively cheerful mood.
```

Arahan negatif dapat membantu memperjelas tujuan, tetapi tidak menjamin semua karakter yang dilarang akan sepenuhnya dihilangkan.

***

# BAGIAN VII — PENGATURAN APLIKASI GEMINI

## 16. Prompt versus kontrol aplikasi

|Kebutuhan|Di dalam prompt|Pengaturan aplikasi|
|---|---|---|
|Genre|Jelaskan genre dan pengaruhnya|Gunakan pilihan genre jika tersedia|
|Mood|Jelaskan suasana dan emosi|Tidak selalu berupa kontrol terpisah|
|Vokal|Jelaskan mode dan karakter vokal|Pilih opsi vokal jika tersedia|
|Lirik|Tentukan tema atau sediakan teks|Gunakan kolom lirik khusus jika tersedia|
|Durasi|Sebutkan durasi sasaran bila relevan|Pilih opsi durasi yang benar-benar tersedia|
|Gambar atau video|Deskripsikan suasana visual dalam teks|Unggah media jika didukung|
|BPM dan nada dasar|Cantumkan sebagai arahan kreatif|Jangan menganggap tersedia sebagai kontrol khusus|
|Struktur dan transisi|Jelaskan urutan bagian dan perubahan musik|Biasanya berupa arahan prompt|

### Variabel untuk pencatatan pengaturan

Variabel berikut adalah metadata untuk pengguna atau dokumentasi, bukan instruksi yang harus selalu disertakan di prompt musik.

|Variabel|Fungsi|
|---|---|
|`{{APP_DURATION_SETTING}}`|Opsi durasi yang dipilih di aplikasi|
|`{{APP_VOCAL_SETTING}}`|Pengaturan vokal yang dipilih jika tersedia|
|`{{APP_GENRE_SETTING}}`|Pilihan genre di aplikasi jika tersedia|
|`{{VISUAL_INPUT}}`|Gambar atau video yang benar-benar diunggah|
|`{{MODEL_OR_MODE}}`|Model atau mode yang digunakan, jika terlihat|

## 17. Alur penggunaan Create Music

1. Buka fitur Create Music atau Buat musik di aplikasi Gemini.
2. Periksa opsi model, durasi, vokal, dan genre yang tersedia.
3. Pilih pengaturan aplikasi yang sesuai dengan kebutuhan.
4. Isi Core Prompt dengan genre, mood, instrumen, groove, struktur, dan arahan produksi.
5. Tambahkan modul vokal, lirik, timing, atau referensi visual bila diperlukan.
6. Buat musik dan evaluasi hasilnya.
7. Jika hasil belum sesuai, ubah beberapa arahan utama lalu buat generasi baru.

Nama, posisi, dan ketersediaan kontrol dapat berubah mengikuti versi aplikasi dan akses pengguna. Proses ini tidak menjanjikan pengeditan langsung terhadap audio yang sudah dihasilkan.

***

# BAGIAN VIII — MASTER PROMPT LENGKAP

## 18. Master Prompt Template

Bagian ini menggabungkan modul-modul utama. Hapus bagian yang tidak relevan sebelum menggunakannya.

```text
Create a {{DURATION_REQUEST}} music track in the style of
{{GENRE}}, incorporating elements of {{SUBGENRE}}.

CREATIVE DIRECTION
Mood and atmosphere: {{MOOD}}.
Emotional direction: {{EMOTIONAL_DIRECTION}}.
Musical identity: {{MUSICAL_IDENTITY}}.
Visual description, if relevant: {{VISUAL_DESCRIPTION}}.

TEMPO AND MUSICAL FOUNDATION
Tempo: {{BPM}} BPM.
Key and tonality: {{KEY}}.
Melody style: {{MELODY_STYLE}}.
Harmony style: {{HARMONY_STYLE}}.

INSTRUMENTATION AND RHYTHM
Main instruments: {{INSTRUMENTS}}.
Supporting textures: {{SUPPORTING_TEXTURES}}.
Rhythm and groove: {{RHYTHM}}.
Drum and percussion style: {{DRUM_STYLE}}.
Bass character: {{BASS_STYLE}}.

VOCALS
Vocal mode: {{VOCAL_MODE}}.
Vocal profile and timbre: {{VOCAL_PROFILE}}.
Vocal delivery: {{VOCAL_DELIVERY}}.
Backing vocals: {{BACKING_VOCALS}}.
Lyrics language: {{LANGUAGE}}.

LYRICS
Lyrics mode: {{LYRICS_MODE}}.
Lyrics theme: {{LYRICS_THEME}}.
Lyrics content, if provided:
{{LYRICS_CONTENT}}

ARRANGEMENT
Song structure: {{STRUCTURE}}.
Timing and transitions: {{TIMING_MARKERS}}.
Energy development: {{DYNAMICS}}.

PRODUCTION
Production direction: {{PRODUCTION_DIRECTION}}.
Optional detailed production: {{PRODUCTION}}.
Mix characteristics: {{MIX_STYLE}}.
Space and ambience: {{SPACE_AND_AMBIENCE}}.
Effects and transitions: {{EFFECTS}}.

ENDING
{{ENDING}}

RESTRICTIONS
{{RESTRICTIONS}}

Maintain a coherent musical identity throughout the track.
Ensure that the genre, instrumentation, rhythm, melody, vocals,
arrangement, and production work together naturally.
Prioritize the main creative direction and avoid unnecessary
stylistic changes.
```

**Catatan penggunaan:** `{{DURATION_REQUEST}}` adalah arahan teks. Pengaturan durasi aplikasi dicatat secara terpisah melalui `{{APP_DURATION_SETTING}}`. Jangan mengisi semua variabel secara otomatis; gunakan hanya bagian yang dibutuhkan.

***

# BAGIAN IX — CONTOH PENGGUNAAN

## 19. Contoh A: Dream Pop Indonesia

```text
Create a longer Indonesian dream-pop track with subtle
synthwave influences.

Mood and atmosphere: nostalgic, dreamy, intimate, and quietly
hopeful.

Emotional direction: begin with loneliness and gradually move
toward acceptance.

Musical identity: a memorable electric-piano motif, shimmering
synthesizers, and a warm melodic bass line.

Tempo: around 95 BPM.
Key and tonality: minor-key atmosphere with moments of
harmonic warmth.

Instrumentation: electric piano, soft analog synthesizers,
clean electric guitar, warm bass, restrained drums, and
subtle ambient textures.

Rhythm and groove: relaxed, steady half-time groove with
soft kick drums, restrained snare, and delicate hi-hats.

Vocal mode: lead vocals.
Vocal profile: intimate, soft, airy timbre.
Vocal delivery: restrained verses and more expressive choruses.
Backing vocals: subtle harmonies in the final chorus.

Lyrics language: Indonesian.
Lyrics mode: generate original lyrics.
Lyrics theme: remembering someone while learning to move forward.

Structure: atmospheric intro, verse, pre-chorus, chorus,
second verse, chorus, bridge, final chorus, reflective outro.

Energy development: begin sparsely, gradually introduce
rhythmic and harmonic layers, open up the chorus, create
an intimate bridge, and make the final chorus the emotional peak.

Production direction: polished dream-pop production with
organic warmth, clear vocals, defined bass, spacious
synthesizers, and a wide stereo image.

Ending: resolve gently with the main electric-piano motif
and lingering ambient textures.

Restrictions: avoid aggressive drums, heavy distortion,
abrupt transitions, and an excessively cheerful mood.

Maintain a consistent dream-pop identity throughout the track.
```

## 20. Contoh B: Instrumental sinematik

```text
Create an instrumental cinematic ambient track with a
reflective, mysterious, and gradually uplifting atmosphere.

Musical identity: a recurring piano motif supported by
evolving orchestral textures.

Tempo: slow to moderate.
Key and tonality: minor-key foundation with a hopeful
harmonic resolution.

Instrumentation: piano, soft strings, atmospheric pads,
low cinematic percussion, and subtle sound textures.

Rhythm and groove: restrained, spacious, and deliberate.

Instrumental only. No vocals or lyrics.

Structure: atmospheric intro, main theme, gradual build,
emotional peak, breakdown, final theme, and gentle outro.

Energy development: begin quietly, gradually expand
the orchestral layers, reach a restrained emotional climax,
then return to a spacious final passage.

Production direction: cinematic, detailed, spacious,
and emotionally focused.

Mix characteristics: clear melodic focus and controlled
low frequencies.

Space and ambience: wide, soft, and atmospheric.

Ending: let the main theme resolve naturally with lingering
ambient textures.

Restrictions: no vocals, no abrupt ending, no aggressive
dance beat, and no excessive percussion.
```

## 21. Contoh C: Musik elektronik

```text
Create an energetic melodic electronic track with a modern
synthwave influence.

Mood and atmosphere: futuristic, confident, and uplifting.

Musical identity: a memorable synthesizer lead over a
driving bass line.

Tempo: around 120 BPM.

Instrumentation: analog-style synthesizers, electronic bass,
punchy kick, snare, hi-hats, and atmospheric pads.

Rhythm and groove: steady four-on-the-floor pulse with
a controlled, danceable groove.

Vocal mode: instrumental only. No vocals or lyrics.

Structure: intro, build-up, first drop, main groove,
breakdown, second build-up, final drop, outro.

Energy development: begin with a restrained synth motif,
gradually introduce percussion, build tension before each drop,
and finish with a concise instrumental outro.

Production direction: clean, punchy electronic production
with defined bass and bright but controlled high frequencies.

Ending: resolve the lead motif and end cleanly.

Restrictions: avoid muddy bass, excessive distortion,
and abrupt changes in genre.
```

***

# BAGIAN X — TROUBLESHOOTING

## 22. Jika hasil musik tidak sesuai

|Masalah|Arahan revisi|
|---|---|
|Genre tidak terasa jelas|Perjelas genre utama dan kurangi pengaruh yang bertentangan|
|Musik terlalu ramai|Kurangi instrumen dan lapisan pendukung|
|Chorus kurang menonjol|Jelaskan perbedaan energi antara verse dan chorus|
|Vokal kurang sesuai|Perjelas timbre, cara bernyanyi, dan intensitas|
|Lirik tidak sesuai tema|Perjelas cerita, sudut pandang, bahasa, dan emosi|
|Musik terlalu pendek atau panjang|Periksa opsi durasi aplikasi serta revisi arahan durasi|
|Struktur tidak konsisten|Sederhanakan urutan bagian dan gunakan penanda yang lebih jelas|
|Ending terasa mendadak|Jelaskan jenis penutupan dan ruang yang diperlukan sebelum berakhir|
|Produksi terasa terlalu padat|Kurangi lapisan, efek, dan instruksi produksi yang berulang|

Perubahan prompt tidak menjamin hasil tertentu. Evaluasi audio yang dihasilkan dan sesuaikan instruksi berdasarkan perbedaan yang benar-benar terdengar.

***

# BAGIAN XI — BATASAN DAN REFERENSI

## 23. Batasan penggunaan

- Tidak semua variabel merupakan parameter teknis yang dapat dikunci oleh generator.
- BPM, nada dasar, durasi, dan penanda waktu dapat berfungsi sebagai arahan, tetapi tidak selalu dipatuhi secara persis.
- Pengaturan aplikasi bergantung pada versi, model, ketersediaan fitur, dan jenis akses pengguna.
- Deskripsi visual dalam teks tidak sama dengan mengunggah gambar atau video.
- Arahan negatif membantu memperjelas kebutuhan, tetapi tidak menjamin semua elemen yang tidak diinginkan akan hilang.
- Prompt ini merupakan kerangka kreatif yang disusun berdasarkan dokumentasi; bukan prompt resmi yang diterbitkan Google.

## 24. Referensi resmi

1. **Dokumentasi bantuan aplikasi Gemini — Create Music**
   https://support.google.com/gemini/answer/16901237?hl=id

2. **Pengumuman resmi Google — Create your best tracks yet with Lyria in Gemini**
   https://blog.google/innovation-and-ai/products/gemini-app/better-tracks-lyria-gemini/

3. **Gemini API — Music Generation**
   https://ai.google.dev/gemini-api/docs/music-generation

4. **Panduan prompt Lyria**
   https://ai.google.dev/gemini-api/docs/lyria-prompt-guide

Dokumentasi aplikasi Gemini menjadi rujukan utama untuk alur dan kontrol aplikasi. Dokumentasi API dan panduan Lyria digunakan sebagai rujukan tambahan untuk teknik penulisan prompt serta kemampuan generasi musik. Keduanya tidak boleh dianggap identik dalam setiap detail fitur.

***

# BAGIAN XII — STATUS VERSI

## 25. Riwayat dan tata kelola dokumen

- **Draft v1:** tetap dikunci sebagai referensi awal.
- **Draft v2:** dipertahankan sebagai versi arsip.
- **Draft v2.1:** revisi berdasarkan hasil audit dokumentasi resmi dan rekomendasi terstruktur.
- Revisi berikutnya harus dibahas terlebih dahulu sebelum diterapkan pada versi aktif.

**Akhir dokumen — Gemini Create Music: Master Prompt Template v2.1**
