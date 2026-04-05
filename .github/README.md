# 🎮 Game Story — VS Code Copilot Setup

Sistem narasi berbasis GitHub Copilot Instructions untuk membangun game story yang konsisten, imersif, dan emosional.

---

## 📁 Struktur File

```
.github/
├── copilot-instructions.md              ← Aturan global (selalu aktif)
└── instructions/
    ├── progress.instructions.md         ← Tracking arc & progress cerita
    ├── characters.instructions.md       ← Profil & suara karakter
    ├── world.instructions.md            ← Lore, setting & aturan dunia
    ├── dialogue.instructions.md         ← Standar penulisan dialogue
    ├── branching.instructions.md        ← Sistem pilihan & konsekuensi
    ├── pacing.instructions.md           ← Tempo & ketegangan narasi
    ├── tone.instructions.md             ← Gaya bahasa & nuansa cerita
    └── quest.instructions.md            ← Desain quest, tipe & registry
```

---

## 🚀 Cara Menggunakan

### 1. Setup VS Code Copilot
Pastikan ekstensi **GitHub Copilot** sudah terinstall dan aktif di VS Code.

### 2. File `copilot-instructions.md` (Global Rules)
File ini **selalu aktif** untuk seluruh project. Berisi:
- Filosofi narasi
- Aturan penulisan global
- Standar format output

### 3. File `*.instructions.md` (Contextual Rules)
File ini aktif berdasarkan file yang sedang dibuka (via `applyTo` di header).

| Kamu sedang edit... | Instruction aktif |
|--------------------|-------------------|
| File di `/scenes/` | `progress` + `pacing` + `tone` |
| File di `/characters/` | `characters` + `dialogue` |
| File di `/world/` | `world` |
| File di `/branches/` | `branching` |
| File di `/quests/` atau `/missions/` | `quest` + `branching` + `characters` |

---

## ✍️ Workflow Membuat Cerita

### Langkah 1 — Isi World Bible
Buka `world.instructions.md` → Isi bagian **World Overview** dan **Prime Directives**.

### Langkah 2 — Buat Karakter
Buat file `characters/protagonist.character.md` menggunakan template dari `characters.instructions.md`.

### Langkah 3 — Susun Story Arc
Update `progress.instructions.md` → Isi bagian **Story Arc Structure** dengan rencana cerita kamu.

### Langkah 4 — Tulis Scenes
Buat file `scenes/act1/scene-01-hook.scene.md` dan minta Copilot membantu dengan konteks lengkap.

### Langkah 5 — Desain Quest
Buat file `quests/main/Q001-nama-quest.quest.md` menggunakan template dari `quest.instructions.md`. Setiap quest butuh: hook emosional, komplikasi di tengah, dan pilihan di klimaks.

### Langkah 6 — Buat Branching
Untuk setiap keputusan besar, buat `branches/choice-[nama].branch.md`.

---

## 💡 Tips Menggunakan Copilot

### Prompt yang Bagus
```
Tulis scene pembuka di lokasi [X], dengan karakter [Y] dalam kondisi [Z].
Mood: tegang. Ini adalah scene pertama dalam ACT 1.
```

```
Buat quest side untuk NPC seorang pedagang yang kehilangan anaknya.
Quest harus punya twist di tengah dan satu pilihan moral di akhir.
```

```
Buat dialogue antara [Karakter A] dan [Karakter B] di mana A menyembunyikan 
informasi tentang [X] sementara B mencoba mencari tahu.
```

```
Buat 3 opsi pilihan untuk player di titik ini: protagonis baru saja menemukan 
bahwa sekutunya berbohong. Setiap opsi harus mencerminkan nilai yang berbeda.
```

### Copilot Chat Commands
- `@workspace` — Copilot membaca seluruh project context
- Tambahkan `#file:characters.instructions.md` untuk referensi spesifik
- Gunakan `/explain` untuk memahami keputusan narasi

---

## 🔄 Maintenance

### Setelah Setiap Writing Session
- [ ] Update `progress.instructions.md` → `scenes_completed`
- [ ] Log foreshadowing baru di `foreshadowing_planted`
- [ ] Update relationship flags jika ada perubahan signifikan
- [ ] Review `pending_payoffs` — ada yang terlupa?

### Tanda Bahaya 🚩
- Character berbicara tidak sesuai suaranya → Review `characters.instructions.md`
- Scene terasa lambat → Review `pacing.instructions.md`
- Dialogue terasa hambar → Review `dialogue.instructions.md`
- Pilihan terasa tidak bermakna → Review `branching.instructions.md`

---

## 📖 Referensi Cepat

| Kebutuhan | File |
|-----------|------|
| Desain quest (main/side/hidden/faction) | `quest.instructions.md` |
| Nuansa & gaya bahasa | `tone.instructions.md` |
| Struktur pilihan player | `branching.instructions.md` |
| Cara karakter bicara | `characters.instructions.md` + `dialogue.instructions.md` |
| Progress & struktur cerita | `progress.instructions.md` |
| Fakta dunia & lore | `world.instructions.md` |
| Ritme & ketegangan | `pacing.instructions.md` |
