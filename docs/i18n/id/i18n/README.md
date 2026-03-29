# 🚀 OmniRute — Pintu Masuk AI GRATIS

### Teruslah koding. Routing cerdas untuk **MODEL AI GRATIS & murah** dengan fallback otomatis.

_Proxy API universal Anda — satu endpoint, 67+ penyedia, tidak ada downtime.
Sekarang dengan agen orkestrasi MCP & A2A._

**Penyelesaian percakapan • Embeddings • Pembaruan Citra • Video • Musik • Suara
• Reranking • **Cari di Web** • Server MCP • Protokol A2A • 100% TypeScript**

---

<div align="center">

[![versi
npm](https://img.shields.io/npm/v/omniroute?color=cb3837&logo=npm)](https://www.npmjs.com/package/omniroute)
[![unduh
npm](https://img.shields.io/npm/dm/omniroute?color=cb3837&logo=npm&label=npm%20downloads)](https://www.npmjs.com/package/omniroute)
[![Docker
Hub](https://img.shields.io/docker/v/diegosouzapw/omniroute?label=Docker%20Hub&logo=docker&color=2496ED)](https://hub.docker.com/r/diegosouzapw/omniroute)
[![Docker
Pulls](https://img.shields.io/docker/pulls/diegosouzapw/omniroute?logo=docker&color=2496ED&label=docker%20pulls)](https://hub.docker.com/r/diegosouzapw/omniroute)
[![Lisensi](https://img.shields.io/github/license/diegosouzapw/OmniRoute)](https://github.com/diegosouzapw/OmniRoute/blob/main/LICENSE)
[![Website](https://img.shields.io/badge/Website-omniroute.online-blue?logo=google-chrome&logoColor=white)](https://omniroute.online)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-Community-25D366?logo=whatsapp&logoColor=white)](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

[🌐 Website](https://omniroute.online) • [🚀 Aktivitas Cepat](#-quick-start) • [💡
Fitur](#-key-features) • [📖 Dokumentasi](#-documentation) • [💰
Pricing](#-pricing-at-a-glance) • [💬
WhatsApp](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

</div>

🌐 **Tersedia dalam:** 🇺🇸 [Bahasa Inggris](README.md) | 🇧🇷 [Portugis
(Brasil)](docs/i18n/pt-BR/README.md) | 🇪🇸 [Spanyol](docs/i18n/es/README.md) | 🇫🇷
[Prancis](docs/i18n/fr/README.md) | 🇮🇹 [Italia](docs/i18n/it/README.md) | 🇷🇺
[Rusia](docs/i18n/ru/README.md) | 🇨🇳 [Hanzi
Sederhana](docs/i18n/zh-CN/README.md) | 🇩🇪 [Jerman](docs/i18n/de/README.md) | 🇮🇳
[Hindi](docs/i18n/in/README.md) | 🇹🇭 [Thai](docs/i18n/th/README.md) | 🇺🇦
[Ukraina](docs/i18n/uk-UA/README.md) | 🇸🇦 [Arab](docs/i18n/ar/README.md) | 🇯🇵
[Jepang](docs/i18n/ja/README.md) | 🇻🇳 [Vietnam](docs/i18n/vi/README.md) | 🇧🇬
[Bulgaria](docs/i18n/bg/README.md) | 🇩🇰 [Denmark](docs/i18n/da/README.md) | 🇫🇮
[Finlandia](docs/i18n/fi/README.md) | 🇮🇱 [Ibrani](docs/i18n/he/README.md) | 🇭🇺
[Hongaria](docs/i18n/hu/README.md) | 🇮🇩 [Indonesia](docs/i18n/id/README.md) | 🇰🇷
[Korea](docs/i18n/ko/README.md) | 🇲🇾 [Melayu](docs/i18n/ms/README.md) | 🇳🇱
[Belanda](docs/i18n/nl/README.md) | 🇳🇴 [Norwegia](docs/i18n/no/README.md) | 🇵🇹
[Portugis (Portugal)](docs/i18n/pt/README.md) | 🇷🇴
[Rumania](docs/i18n/ro/README.md) | 🇵🇱 [Polandia](docs/i18n/pl/README.md) | 🇸🇰
[Slovak](docs/i18n/sk/README.md) | 🇸🇪 [Swedia](docs/i18n/sv/README.md) | 🇵🇭
[Filipina](docs/i18n/phi/README.md) | 🇨🇿 [Ceko](docs/i18n/cs/README.md)

---

## 🆕 Apa Baru di v3.0.0

> ** Mengganti dari v2.9.5?** — Lihat [CHANGELOG
> lengkap](CHANGELOG.md#300--2026-03-22-release-candidate--not-yet-merged-to-main)
> untuk semua perubahan.

| Area                                 | Perubahan                                                                                                                                                        |
| ------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🔒 **Keamanan CodeQL**                | Telah memperbaiki 10+ peringatan CodeQL: polynomial-redos, keamanan random yang salah, remediasi Shell-injection                                                 |
| ✅ **Validasi Jalur**                 | Semua 176 jalur API sekarang diverifikasi dengan skema Zod + `validateBody()` — `check:route-validation:t06` berhasil                                            |
| 🐛 **omniModel Tanda Rusak**          | Tag Internal `<omnimodel>` tidak lagi menyebarkan ke klien dalam respons streaming SSE (#585)</omnimodel>                                                        |
| 🔑 **Kunci Terdaftar API**            | Mengatur kunci API otomatis melalui `POST /api/v1/registered-keys` dengan Kuota per-penyedia/ akun, imanen, penyimpanan SHA-256, dan laporan isu GitHub opsional |
| 🎨 **Ikon Penyedia**                  | 130+ logo provider via `@lobehub/icons` (format SVG) dengan fallback untuk PNG                                                                                   |
| 🔄 **Mimiliki Otomatis **             | Jadwal 24 jam pengatur pengulangan model untuk daftar penyedia bawaan dan khusus kompatibel dengan OpenAI                                                        |
| 🌐 **OpenCode Zen/Go **               | Dua penyedia baru dari @kang-heewon melalui PR #530: penyedia gratis + penyedia langganan via `OpencodeExecutor`                                                 |
| 🐛 **CLI Otoritas Gemn **             | Kerusakan yang dapat diatasi ketika `GEMINI_OAUTH_CLIENT_SECRET` tidak ada di Docker (sebelumnya kesalahan Google yang kabur)                                    |
| 🐛 **Konfigurasi OpenCode **          | `saveOpenCodeConfig()` sekarang menulis TOML yang benar ke `XDG_CONFIG_HOME`                                                                                     |
| 🐛 **Penyimpanan model yang diping ** | `body.model` sekarang diatur ke `pinnedModel` untuk perlindungan kinerja cache                                                                                   |
| 🐛 **Lampiran/Claude loop **          | `tool_result` sekarang diubah ke teks untuk menghentikan loop tak berhentinya                                                                                    |
| 🐛 **Pindah ke login **               | Tidak adanya penangguhan setelah mengabaikan setup password                                                                                                      |
| 🐛 **Jalur Windows **                 | Path pada MSYS2/Git-Bash (`/c/...`) yang diatur ke `C:\...` secara otomatis                                                                                      |

---

## 🖼️ Dashboard Utama

<div align="center">
  <img src="./docs/screenshots/MainOmniRoute.png" alt="OmniRoute Dashboard" width="800"/>
</div>

---

## 📸 Previw Dashboard

<details>
<summary><b>Click to see dashboard screenshots</b></summary>

| Halaman                | Tampilan Layar                                          |
| ---------------------- | ------------------------------------------------------- |
| **Penyedia**           | ![Penyedia](docs/screenshots/01-providers.png)          |
| **Kombinasi**          | ![Kombinasi](docs/screenshots/02-combos.png)            |
| **Analisis**           | ![Analisis](docs/screenshots/03-analytics.png)          |
| **Kesehatan**          | ![Kesehatan](docs/screenshots/04-health.png)            |
| **Penerjemah**         | ![Penerjemah](docs/screenshots/05-translator.png)       |
| **Pengaturan**         | ![Pengaturan](docs/screenshots/06-settings.png)         |
| **Alat Perintah CLI**  | ![Alat Perintah CLI](docs/screenshots/07-cli-tools.png) |
| **Catatan Penggunaan** | ![Penggunaan](docs/screenshots/08-usage.png)            |
| ** Endpoint**          | ![Endpoint](docs/screenshots/09-endpoint.png)           |

</details>

---

### Robot AI Gratis untuk coding agent kegemaran Anda

_Konek IDE atau CLI yang berkekuatan AI melalui OmniRoute — pengganti API gratis
untuk coding tak terbatas._

  <table>
    <tr>
      <td align="center" width="110">
        <a href="https://github.com/openclaw/openclaw">
          <img src="./public/providers/openclaw.png" alt="OpenClaw" width="48"/><br/>
          <b>OpenClaw</b>
        </a><br/>
        <sub>⭐ 205K</sub>
      </td>
      <td align="center" width="110">
        <a href="https://github.com/HKUDS/nanobot">
          <img src="./public/providers/nanobot.png" alt="NanoBot" width="48"/><br/>
          <b>NanoBot</b>
        </a><br/>
        <sub>⭐ 20.9K</sub>
      </td>
      <td align="center" width="110">
        <a href="https://github.com/sipeed/picoclaw">
          <img src="./public/providers/picoclaw.jpg" alt="PicoClaw" width="48"/><br/>
          <b>PicoClaw</b>
        </a><br/>
        <sub>⭐ 14.6K</sub>
      </td>
      <td align="center" width="110">
        <a href="https://github.com/zeroclaw-labs/zeroclaw">
          <img src="./public/providers/zeroclaw.png" alt="ZeroClaw" width="48"/><br/>
          <b>ZeroClaw</b>
        </a><br/>
        <sub>⭐ 9.9K</sub>
      </td>
      <td align="center" width="110">
        <a href="https://github.com/nearai/ironclaw">
          <img src="./public/providers/ironclaw.png" alt="IronClaw" width="48"/><br/>
          <b>IronClaw</b>
        </a><br/>
        <sub>⭐ 2.1K</sub>
      </td>
    </tr>
    <tr>
      <td align="center" width="110">
        <a href="https://github.com/anomalyco/opencode">
          <img src="./public/providers/opencode.svg" alt="OpenCode" width="48"/><br/>
          <b>OpenCode</b>
        </a><br/>
        <sub>⭐ 106K</sub>
      </td>
      <td align="center" width="110">
        <a href="https://github.com/openai/codex">
          <img src="./public/providers/codex.png" alt="Codex CLI" width="48"/><br/>
          <b>Codex CLI</b>
        </a><br/>
        <sub>⭐ 60.8K</sub>
      </td>
      <td align="center" width="110">
        <a href="https://github.com/anthropics/claude-code">
          <img src="./public/providers/claude.png" alt="Claude Code" width="48"/><br/>
          <b>Claude Code</b>
        </a><br/>
        <sub>⭐ 67.3K</sub>
      </td>
      <td align="center" width="110">
        <a href="https://github.com/google-gemini/gemini-cli">
          <img src="./public/providers/gemini-cli.png" alt="Gemini CLI" width="48"/><br/>
          <b>Gemini CLI</b>
        </a><br/>
        <sub>⭐ 94.7K</sub>
      </td>
      <td align="center" width="110">
        <a href="https://github.com/Kilo-Org/kilocode">
          <img src="./public/providers/kilocode.png" alt="Kilo Code" width="48"/><br/>
          <b>Kilo Code</b>
        </a><br/>
        <sub>⭐ 15.5K</sub>
      </td>
    </tr>
  </table>

<sub>📡 Semua agen terhubung melalui <code>http://localhost:20128/v1</code> atau
<code>http://cloud.omniroute.online/v1</code> — satu konfigurasi, kodifikasi tak
terbatas, dan kuota</sub>

---

## 🤔 Mengapa OmniRoute?

**Hentikan pengeluaran uang dan batas setiap bulan:**

- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Kuota langganan tidak digunakan akan habis setiap bulan
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Batas akses mengganggu sedang coding
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  API yang mahal ($20-50/bulan per penyedia)
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Pelelangan manual antara penyedia

**OmniRoute menyelesaikan masalah ini:**

- ✅ **Maksimalkan langganan** - Pantau kuota, gunakan setiap bit sebelum reset
- ✅ **Jatuhkan balik otomatis** - Langganan → Kunci API → Murah → Gratis, tanpa
  ganggu
- ✅ **Multi-akun** - Rotasi antar akun per penyedia
- ✅ **Universal** - Bekerja dengan Claude Code, Codex, Gemini CLI, Cursor,
  Cline, OpenClaw, alat CLI apa saja

---

## 📧 Bantuan

> 💬 **Join our komunitas!** [WhatsApp
> Group](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t) — Dapatkan
> bantuan, berbagi tips, dan tetap diperbarui.

- **Website**: [omniroute.online](https://omniroute.online)
- **GitHub**:
  [github.com/diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute)
- **Isu**:
  [github.com/diegosouzapw/OmniRoute/issues](https://github.com/diegosouzapw/OmniRoute/issues)
- **WhatsApp**: [Kumpulan
  Komunitas](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)
- **Kontribusi**: Lihat [CONTRIBUTING.md](CONTRIBUTING.md), buka PR, atau pilih
  `masalah pertama baik`
- **Proyek Asli **: [9router by decolua](https://github.com/decolua/9router)

### 🐛 Meminta Bantuan?

Saat membuka isu, silakan jalankan perintah system-info dan taruh file yang
dihasilkan:

```bash
npm run system-info
```

Perintah ini menghasilkan sebuah `system-info.txt` dengan informasi Node.js,
versi OmniRoute, detail sistem operasi, alat CLI yang terinstal (iflow, gemini,
klaude, codex, antigravitasi, droid, dll.), status Docker/PM2, dan paket sistem
— segalanya yang dibutuhkan untuk mengulangi masalah Anda dengan cepat. Sambung
file tersebut langsung ke isu GitHub Anda.

---

## Cara Kerjanya

```
┌─────────────┐
│  Alat CLI   │  (Kode Claude, Codex, Gemini CLI, OpenClaw, Cursor, Cline...)
│   Alat      │
└──────┬──────┘
       │ http://localhost:20128/v1
       ↓
┌─────────────────────────────────────────┐
│           OmniRoute (Router Cerdas)        │
│  • Konversi Format (OpenAI ↔ Claude) │
│  • Pemantauan Kuota + Embeddings + Gambar │
│  • Perbaruan Otomatis Token               │
└──────┬──────────────────────────────────┘
       │
       ├─→ [Tingkat 1: SUBSKRIPSI] Kode Claude, Codex, Gemini CLI
       │   ↓ kuota habis
       ├─→ [Tingkat 2: API KEY] DeepSeek, Groq, xAI, Mistral, NVIDIA NIM, dll.
       │   ↓ limit anggaran
       ├─→ [Tingkat 3: MURAH] GLM ($0,6/1JUTA), MiniMax ($0,2/1JUTA)
       │   ↓ limit anggaran
       └─→ [Tingkat 4: GRATIS] iFlow, Qwen, Kiro (tidak terbatas)

Hasil: Teruslah coding dengan biaya minimal
```

---

## 🎯 Apa yang Dihapus oleh OmniRoute — 30 Masalah Nyata & Kasus Penggunaan

> **Setiap pengembang menggunakan alat AI menghadapi masalah-masalah ini setiap
> hari.** OmniRoute dibangun untuk menjawab semua masalah mereka — dari biaya
> yang melambung hingga pembatasan di tingkat regional, dari protokol pengalaman
> jaringan hingga observasi kinerja bisnis.

<details>
<summary><b>💸 1. "I pay for an expensive subscription but still get interrupted by limits"</b></summary>

Pengembang membayar $20–200/bulan untuk Claude Pro, Codex Pro, atau GitHub
Copilot. Bahkan membayar, kuota memiliki titik akhir — 5 jam penggunaan,
pembatasan mingguan, atau pembatasan per-menit. Di tengah sesi pengembangan,
penyedia berhenti menjawab dan pengembang kehilangan alur dan produktivitas.

**Mengapa OmniRoute dapat menjawabnya:**

- **Falling Back Smart 4-Tingkat** — Jika kuota subsripsi habis, secara otomatis
  beralih ke API Key → Murah → Gratis Tanpa Intervensi Manusia
- **Pantauan Kuota Siswa** — Menunjukkan penggunaan token secara real-time
  dengan hitung mundur (5 jam, harian, mingguan)
- **Dukungan Multi-Akun** — Akun multi per penyedia dengan auto switching —
  Ketika satu habis, beralih ke akun yang lain
- **Kombinasi Sendiri** — Rantai beralih yang dapat disesuaikan dengan 6
  strategi penyeimbang (fill-first, round-robin, P2C, random, least-used,
  cost-optimized)
- **Biaya Quota Bisnis Claude** — Monitoring kuota bagi kantor/kelompok bisnis
  di dashboard

</details>

<details>
<summary><b>🔌 2. "I need to use multiple providers but each has a different API"</b></summary>

OpenAI menggunakan satu format, Claude (Anthropic) menggunakan format lain,
Gemini lagi-lagi menggunakan format berbeda. Jika seorang pengembang ingin makan
model dari penyedia-penyedia berbeda atau beralih di antara mereka, mereka harus
merekonfigurasi SDK, mengganti endpoint, menangani format yang tidak kompatibel.
Penyedia custom (FriendLI, NIM) mempunyai endpoint model yang tidak standar.

**Mengapa OmniRoute dapat menjawabnya:**

- **Endpoint Bersatu** — Satu `http://localhost:20128/v1` memadankan 67+
  penyedia
- **Pengubahan Format** — Otomatis dan transparan: OpenAI ↔ Claude ↔ Gemini ↔
  Responses API
- **Pengisian Tanda Tangan Kembali** — Menghilangkan bidang tidak standar
  (`x_groq`, `penggunaan_breakdown`, `kelas_pelayanan`) yang dapat memecahkan
  OpenAI SDK v1.83+
- **Normalisasi Peran** — Mengubah `pengembang` → `sistem` untuk penyedia
  non-OpenAI; `sistem` → `pengguna` untuk GLM/ERNIE
- **Ekstraksi Penanda Tag Pemikir** — Meningkatkan `` bloks dari model seperti
  DeepSeek R1 ke konten `konten_pemikiran` berstandar
- **Keluaran Terstruktur untuk Gemini** — `json_schema` →
  `MimeType_respon`/`Schema_respon` konversi otomatis
- **'stream' default ke 'false' ** — Sesuai dengan spesifikasi OpenAI,
  menghindari SSE tak terduga dalam SDK Python/Rust/Go

</details>

<details>
<summary><b>🌐 3. "My AI provider blocks my region/country"</b></summary>

Penyedia seperti OpenAI/Codex mengblokir akses dari wilayah geografis tertentu.
Pengguna mendapatkan eror seperti `wilayah_tanah_teritori_Tidak_dukungan` selama
Otentikasi OAuth dan koneksi API. Ini sangat mengganggu bagi pengembang dari
negara berkembang.

**Mengapa OmniRoute dapat menjawabnya:**

- **Konfigurasi Proxy 3 Tingkatan** — Memungkinkan konfigurasi proxy pada 3
  tingkatan: global (semua lalu lintas), per-penyedia (satu penyedia saja), dan
  per-koneksi/kunci
- **Identifikator Biru Proxy Warna** — Indikator visual: 🟢 proxy global, 🟡 proxy
  penyedia, 🔵 proxy koneksi, selalu menampilkan IP
- **Tukar Token OAuth Melalui Proxy** — Aliran OAuth juga melalui proxy,
  memecahkan `wilayah_tanah_teritori_Tidak_dukungan`
- **Pemantauan Koneksi melalui Proxy** — Pemantauan koneksi menggunakan proxy
  yang dikonfigurasikan (tidak ada lagi kelebihan secara langsung)
- **Dukungan SOCKS5** — Dukungan proxy SOCKS5 penuh untuk routing keluar
- **Palsuje Tanda Sidik TLS** — Sidik jari browser seperti TLS melalui `wreq-js`
  untuk menghindari deteksi robot
- **Matematika Finger Print CLI** — Mereorder header dan field tubuh untuk
  menyesuaikan tanda sidik asli sinyal CLI native, drastis mengurangi risiko
  flagging akun. IP proxy dipelihara - Anda mendapatkan kedua kehalusan **dan**
  pemuteusel IP secara bersamaan

</details>

<details>
<summary><b>🆓 4. "I want to use AI for coding but I have no money"</b></summary>

Bukan semua orang dapat membayar $20–200/bulan untuk langganan AI. Siswa,
pengembang dari negara berkembang, hobi, dan freelancer membutuhkan akses ke
model berkualitas tanpa biaya

**Mengapa OmniRoute dapat menjawabnya:**

- **Penyedia Tunggal Gratis Dikonfigurasi** — Dukungan asli untuk penyedia 100%
  gratis: iFlow (5 model tanpa batas melalui Otentikasi OAuth: kimi-k2-pemikir,
  qwen3-pembuat-plus, deepseek-r1, minimax-m2, kimi-k2), Qwen (4 model tanpa
  batas: qwen3-pembuat-plus, qwen3-pembuat-flash, qwen3-pembuat-berikutnya,
  model visi), Kiro (Claude + ID Pembuat AWS untuk gratis), Gemini CLI (180K
  token/bulan gratis)
- **Ollama Cloud** — Ollama model yang dihoskan di cloud di `api.ollama.com`
  dengan tingkat "Penggunaan Ringan" gratis; gunakan `ollamacloud/<model>`
  prefix</model>
- **Kombinasi Hanya-Gratis** — Menggandung `gc/gemini-3-tersembunyi →
  jika/kimi-k2-pemikir → qw/qwen3-pembuat-plus` = $0/bulan dengan tidak ada
  gangguan waktu
- **NVIDIA NIM Akses Gratis** — ~40 RPM pengembang kekal akses gratis ke 70+
  model di build.nvidia.com (bertransisi dari kredit ke larangan tingkat)
- Strategi Optimasi Biaya **— Rute strategi yang secara otomatis memilih
  penyedia terjangkau tersedia

</details>

<details>
<summary><b>🔒 5. "I need to protect my AI gateway from unauthorized access"</b></summary>

Ketika mengekspos gateway AI ke jaringan (LAN, VPS, Docker), siapa saja yang
memiliki alamat dapat mengonsumsi kunci pengembang/takannya/kuota. Tanpa
perlindungan, API rentan terhadap penyalahgunaan, penyuntikan prompt, dan
penyalahgunaan.

**Mengapa OmniRoute dapat menjawabnya:**

- **Manajemen Kunci API** — Pengembangan, rotasi, dan skoping per penyedia
  dengan halaman `/dashboard/api-manager` yang dedikasi
- **Kewenangan Model Tingkat Tinggi** — Batasi kunci API ke model tertentu
  (`openai/*`, pola bintangwildcard), dengan tombol Izinkan Semua/Keterbatasan
  toggle
- **Perlindungan Endpoint API** — Minta kunci untuk `/v1/models` dan blokir
  penyedia tertentu dari daftar
- **Penjaga Autentikasi + Proteksi CSRF** — Semua rute halaman dashboard
  dilindungi dengan `withAuth` middleware + token CSRF
- **Pemeteran Waktu** — Pemeteran waktu IP dengan jendela yang dapat disesuaikan
- **Pengaturan IP** — whitelist/blocklist untuk kontrol akses
- **Penjaga Pelufukan Prompt** — Pembersihan terhadap pola pelufukan malfungsi
- **Enkripsi AES-256-GCM** — Kredensial dienkripsi di tempat

</details>

<details>
<summary><b>🛑 6. "My provider went down and I lost my coding flow"</b></summary>

Penyedia AI dapat menjadi tidak stabil, mengembalikan kesalahan 5xx, atau
mengenai batasan waktu sementara. Jika pengembang tergantung pada penyedia
tunggal, mereka terganggu. Tanpa pemutus sirkuit, ulang retry dapat membuat
aplikasi hancur.

**Mengapa OmniRoute dapat menjawabnya:**

- **Pemutus Sirkuit per-model** — Auto-buka/tutup dengan prasyarat yang dapat
  disesuaikan dan cooldown (Tutup/Buka/Sementara Terbuka), dikoletifasikan
  per-model untuk menghindari blok yang menyambung
- **Mengulang Mundur Eksponensial** — Mengulang mundur sembari menunda ulang
  dengan perintang yang meningkat
- **Penjaga Hujan Anti-Gempa** — Mutex + semaphore perlindungan terhadap badai
  retry yang berkonkurensi
- **Rantai Cadangan Kombo** — Jika penyedia utama gagal, secara otomatis jatuh
  melalui rantai dengan tidak ada intervensi
- **Pemutus Sirkuit Combo** — Auto-mengaktifkan penyedia yang gagal dalam rantai
  combo
- **Papan Indikator Kesehatan** — Pengawasan waktu yang berlangsung, status
  pemutus sirkuit, pembatasan yang mematikan, statistik cache, kecepatan laten
  p50/p95/p99

</details>

<details>
<summary><b>🔧 7. "Configuring each AI tool is tedious and repetitive"</b></summary>

Pengembang menggunakan Cursor, Claude Code, Codex CLI, OpenClaw, Gemini CLI,
Kilo Code... Setiap tool membutuhkan konfigurasi yang berbeda (endpoint API,
kunci, model). Mengulangi konfigurasi ketika beralih penyedia atau model
merupakan pemborosan waktu.

**Mengapa OmniRoute dapat menjawabnya:**

- **Tampilan Bantuan CLI** — Halaman dedikasi dengan satu-klik yang siap untuk
  Claude Code, Codex CLI, OpenClaw, Kilo Code, Antigravity, Cline
- **Generator Pengaturan Copilot GitHub** — Menghasilkan
  `chattLanguageModels.json` untuk VS Code dengan seleksi model bulk
- **Wizard Penyambutan** — Pendampingan 4 langkah untuk pengguna baru pertama
  kali
- **Satu endpoint, semua model** — Konfigurasi `http://localhost:20128/v1`
  sekali, akses lebih dari 67 penyedia

</details>

<details>
<summary><b>🔑 8. "Managing OAuth tokens from multiple providers is hell"</b></summary>

Claude Code, Codex, Gemini CLI, Copilot — semua menggunakan OAuth 2.0 dengan
token yang akan kedaluwarsa. Para pengembang perlu untuk mensyahkan ulang secara
terus-menerus, menghadapi `client_secret hilang`, `redirect_uri_match_mismatch`,
dan kegagalan di server jarak jauh. OAuth di LAN/VPS sangat ber(problematik)

**Mengapa OmniRoute dapat menjawabnya:**

- **AUTO REFRESH TOKEN** — Token OAuth diperbarui di latar sambil berlangsungnya
  kedaluwarsa
- **OAuth 2.0 (PKCE) Built-in** — Aliran otomatis untuk Claude Code, Codex,
  Gemini CLI, Copilot, Kiro, Qwen, iFlow
- **OAuth Multi-Akun** — Berbagai akun per penyedia melalui JWT/ID token
  ekstraksi
- **Pemecahan OAuth LAN/Remote** — Deteksi IP pribadi untuk `redirect_uri` +
  mode URL manual untuk server jaringan
- **Pemecahan OAuth di balik Nginx** — Menggunakan `window.location.origin`
  untuk kemampuan reverse proxy
- **Panduan OAuth Jarak Jauh** — Panduan langkah-demi-langkah untuk kredential
  Google Cloud di VPS/Docker

</details>

<details>
<summary><b>📊 9. "I don't know how much I'm spending or where"</b></summary>

Para pengembang menggunakan penyedia berbayar beberapa tetapi tidak memiliki
tampilan yang terintegrasi akan pengeluaran. Setiap penyedia memiliki dashboard
billing sendiri, tetapi tidak ada alur keluaran yang disatukan. Pengeluaran tak
terduga akan menumpuk

**Mengapa OmniRoute dapat menjawabnya:**

- **Tampilan Analisis Biaya** — Track biaya per-token dan pengelolaan anggaran
  per penyedia
- **Pengaturan Batas Biaya per Peringkat** — Jumlah untuk tier berskala yang
  menyebabkan beralih otomatis fallback
- **Konfigurasi Harga per Model** — Harga yang dapat diatur per model
- **Statistik Penggunaan per API Key** — Hitungan permintaan dan timestamp
  terakhir digunakan per kunci
- **Tampilan Analisis** — Carta statistik, penggunaan model, tabel penyedia
  dengan tingkat kesuksesan dan latar belakang latency

</details>

<details>
<summary><b>🐛 10. "I can't diagnose errors and problems in AI calls"</b></summary>

Logika Falha Panggilan : Pengembang tidak tahu jika gagalnya panggilan
dikarenakan ratelimit, token kadaluarsa, formatkah, atau kesalahan layanan
pengaturan. Log yang terfragmentasi di berbagai terminal. Tanpa observabilitas,
debugging bergantung pada pengujian melalui pengalaman.

**Mengapa OmniRoute dapat menjawabnya:**

- **Dashboard Log Terintegrasi** — 4 tab: Log Panggilan, Proxy Log, Log Audit,
  Konsole
- **Pengelihat Log Konsole** — Penyambung konsole secara real-time dengan
  tingkat kode warna berbeda, auto-scroll, pencarian, penyaringan
- **SQLite Log PengaturanProxy** — Log yang berkelanjutan yang dapat bertahan
  setelah server di-restart
- **Lahan Uji Percobaan** — 4 mode pengujian: Lahan (penerjemahan format),
  Pengeleher Pergulatan (sunting balik), Meja Pengujian (grup), Pengawas Hidup
  (real-time)
- **Telemetri Pengiriman Request** — Latensi p50/p95/p99 + ID Permintaan Pencari
  Tracing
- **Pengaturan Log Berdasarkan File dengan Rotasi** — Penyambung konsole
  mengarahkan semua ke dalam log JSON dengan rotasi berdasarkan ukuran
- **Laporan Info Sistem** — `npm run system-info` menghasilkan `system-info.txt`
  dengan lingkungan yang komprehensif (Versi Node, Versi OmniRoute, OS, alat
  CLI, status Docker/PM2). Hubungkan ketika melaporkan masalah untuk menunjukkan
  tugas instan

</details>

<details>
<summary><b>🏗️ 11. "Deploying and maintaining the gateway is complex"</b></summary>

Menginstal, mengkonfigurasi, dan memelihara pengaturan proxy AI di berbagai
lingkungan (lokal, VPS, Docker, cloud) sangat berat. Masalah seperti jalan kode
yang tertanam, `EACCES` pada direktori, konflik porta, serta build yang berbeda
antar platform memungkinkan gesekan

**Mengapa OmniRoute dapat menjawabnya:**

- **Penginstallan Global NPM** — `npm install -g omniroute &amp;&amp; omniroute`
  — selesai
- **Docker Multi-Platform** — AMD64 + ARM64 asli (Apple Silicon, AWS Graviton,
  Raspberry Pi)
- **Profildesktop Docker** — `base` (tidak ada alat CLI) dan `cli` (dengan Kode
  Claude, Codex, OpenClaw)
- **Aplikasi Desktop Elektron** — Aplikasi asli untuk Windows/macOS/Linux dengan
  troya sistem, menjalankan ulang otomatis, mode Offline
- **Modus Jendela Segment** — API dan Dashboard di port yang berbeda untuk
  skenario canggih (proxy balik, jaringan kontainer)
- **SINKronisasi Cloud** — sinkronisasi pengaturan melalui Pekerja Cloudflare
- **Backup Basis Data** — Back-up otomatis, mengembalikan, menskala dan
  memasukkan semua pengaturan

</details>

<details>
<summary><b>🌍 12. "The interface is English-only and my team doesn't speak English"</b></summary>

Tim di negara non-bhs Inggris, terutama di Amerika Latin, Asia, dan Eropa,
mengalami kesulitan dengan antarmuka yang hanya Inggris. Kendala bahasa
memperkecil adopsi dan meningkatkan kesalahan pengaturan

**Mengapa OmniRoute dapat menjawabnya:**

- **Dashboard i18n — 30 Bahasa** — Semua 500+ kunci telah diterjemahkan,
  termasuk Arab, Bulgaria, Denmark, Jerman, Spanyol, Finlandia, Perancis,
  Ibrani, Hindi, Hungarian, Indonesia, Italia, Jepang, Korea, Melayu, Belanda,
  Norwegia, Polandia, Portugis (PT/BR), Rumania, Rusia, Slowak, Swedia, Thai,
  Ukraina, Vietnam, Cina, Filipina, Inggris
- **Dukungan RTL** — Dukungan kanan-ke-kiri untuk Arab dan Ibrani
- **Baca PETUNJUK MULTIBAHASA** — 30 Dokumentasi terjemahan lengkap
- **Pilihan Bahasa** — Gloficon dalam header untuk beralih real-time

</details>

<details>
<summary><b>🔄 13. "I need more than chat — I need embeddings, images, audio"</b></summary>

AI bukan hanya selesai pengarahan percakapan. Para pengembang perlu menghasilkan
gambar, merekam audio, membuat embeddings untuk RAG, menyusun kembali dokumen,
dan mengawasi konten. Setiap API memiliki akhiran endpoint yang berbeda dan
formatnya.

**Mengapa OmniRoute dapat menjawabnya:**

- **Embeddings** — `/v1/embeddings` dengan 6 penyedia dan 9+ model
- **Pengembangan Citra** — `/v1/images/generations` dengan 10 penyedia dan 20+
  model (OpenAI, xAI, Together, Fireworks, Nebius, Hyperbolic, NanoBanana,
  Antigravity, SD WebUI, ComfyUI)
- **Pengarangan Teks ke Video** — `/v1/videos/generations` — ComfyUI
  (AnimateDiff, SVD) dan SD WebUI
- **Pengarangan Teks ke Musik** — `/v1/music/generations` — ComfyUI (Stable
  Audio Open, MusicGen)
- **Pengiktisiran Audio** — `/v1/audio/transcriptions` — Whisper + Nvidia NIM,
  HuggingFace, Qwen3
- **Pengucapan Teks** — `/v1/audio/speech` — ElevenLabs, Nvidia NIM,
  HuggingFace, Coqui, Tortoise, Qwen3, **Inworld**, **Cartesia**, **PlayHT**, +
  penyedia eksisting
- **Pengawasan Konten** — `/v1/moderations` — Periksa keamanan konten
- **Kemungkinkan Ulang** — `/v1/rerank` — Perankingan relevansi dokumen
- **API Respons** — Dukungan penuh `/v1/responses` untuk Codex

</details>

<details>
<summary><b>🧪 14. "I have no way to test and compare quality across models"</b></summary>

Para pengembang ingin tahu mana model yang terbaik untuk kasus guna mereka —
kode, terjemahan, logika — tetapi membandingkan secara manual membutuhkan waktu.
Tidak adanya alat evaluasi terintegrasi.

**Mengapa OmniRoute dapat menjawabnya:**

- **Evaluasi LLM** — Pengujian setemas dengan 10 kasus pra-dibungkus yang
  meliputi selamat, matematika, geografi, pembangunan kode, konsisten JSON,
  terjemahan, markdown, ke tolak aman
- **4 Strategi Match** — `akurat`, `mengandung`, `regular expression`, `kustom`
  (fungsi JS)
- **Testan Playground Translator** — Pengujian batch dengan input beragam dan
  hasil yang diharapkan, perbandingan penyedia silang
- [TesT[0] Catur] — Proses lindung sepanjang dengan menampilkan responsoris
  visual
- [TesT[13] Mengawasi Langsung] — Tampilan waktu nyata dari semua permintaan
  yang mengalir melalui proxy

</details>

<details>
<summary><b>📈 15. "I need to scale without losing performance"</b></summary>

Saat permintaan tumbuh, tanpa caching pertanyaan yang sama menghasilkan biaya
tambahan. Tanpa idempotensi, permintaan yang sama akan menyia-nyiakan proses.
Batasan per-tangkalan wajib dipatuhi

**Mengapa OmniRoute dapat menjawabnya:**

- [TesT[0] Caching Semantis] — Caching dua tingkat (tanda tangan + semantis)
  menurunkan biaya dan latenensi
- [TesT[0] Idempotensi Permintaan] — Jendela deduplikasi 5s untuk permintaan
  yang sama
- [TesT[0] Pengendalian Batas Laju] — Melacak batas per-tangkalan, jarak
  minimum, dan maksimum concurrent
- [TesT[0] Pengaturan Laju Edabel] — Pengaturan default yang konfigurabel di
  Pengaturan → Kekacaan dengan persistensi
- [TesT[0] Validasi API Key Caching] — Caching tiga tingkat untuk kinerja
  produksi
- [TesT[0] Dasbor Kesehatan dengan Telemetri] — Latensi p50/p95/p99, statistik
  caching, dan waktu waktu

</details>

<details>
<summary><b>🤖 16. "I want to control model behavior globally"</b></summary>

Para pengembang yang ingin semua respons dalam bahasa tertentu, nada tertentu,
atau ingin membatasi token logika. Mengonfigurasi ini di setiap alat/perintah
adalah praktis

**Mengapa OmniRoute dapat menjawabnya:**

- [TesT[0] Penyuntikan Semangat Sistem] — Semangat global diterapkan pada semua
  permintaan
- [TesT[0] Validasi Anggaran Berpikir] — Pengalokasian token logika pengaturan
  per permintaan (passthrough, auto, custom, adaptive)
- [TesT[0] Strategi Penerbitan 6] — Strategi global yang menentukan bagaimana
  permintaan di distribusikan
- [TesT[0] Penerbit Wildcard] — Pola [X22]provider/*[X33]_patterns menyalurkan
  secara dinamik ke penyedia apapun
- [TesT[0] Tombol Opsi Kombinasi] — Matikan/matikan kombinasi langsung dari
  dashboard
- [TesT[0] Tombol Toggle Penyedia] — Aktifkan/Nonaktifkan semua koneksi untuk
  penyedia dengan satu klik
- [TesT[0] Penyedia yang Diblokir] — Tolak penyedia spesifik dari
  [X56]/v1/models[X67] tampilan

</details>

<details>
<summary><b>🧰 17. "I need MCP tools as first-class product capabilities"</b></summary>

Banyak penyedia AI mengungkap MCP hanya sebagai rincian implementasi yang
disembunyikan. Tim butuh suatu lapisan operasi yang kelihatan, dapat diaturnya.

**Mengapa OmniRoute dapat menjawabnya:**

- Dashboard navigasi dan tab protokol endpoint MCP
- Halaman pengelolaan MCP dedikasi dengan proses, alat, lingkup, dan audit
- Pengaturan cepat-instal untuk `omniroute --mcp` dan penggunaan klien

</details>

<details>
<summary><b>🧠 18. "I need A2A orchestration with sync + stream task paths"</b></summary>

Proses kerja agen memerlukan balasan langsung dan eksekusi langganan yang
berjalan lama dengan kontrol siklus hidup.

**Mengapa OmniRoute dapat menjawabnya:**

- Endpoint JSON-RPC A2A (`POST /a2a`) dengan fungsi `kirim pesan` dan `stream
  pesan`
- Stream SSE dengan penyebaran status terminal
- API siklus tugas untuk `tugas/get` dan `tugas/batal`

</details>

<details>
<summary><b>🛰️ 19. "I need real MCP process health, not guessed status"</b></summary>

Tim operasional perlu tahu jika MCP masih aktif, bukan hanya apakah API dapat
dicapai.

**Mengapa OmniRoute dapat menjawabnya:**

- File getar waktu waktu eksekusi dengan PID, periode waktu, transportasi,
  hitungan alat, dan mode domain
- API status MCP yang menggabungkan getar waktu + kegiatan baru-baru ini
- Kartu status UI untuk proses/jumlah waktu/harga kebaruan getar

</details>

<details>
<summary><b>📋 20. "I need auditable MCP tool execution"</b></summary>

Ketika alat menyesuaikan konfigurasi atau mengaktifkan aksi operasional, tim
perlu kejelasan forensik.

**Mengapa OmniRoute dapat menjawabnya:**

- Perekaman audit SQLite untuk panggilan alat MCP
- Pengaturan filter berdasarkan alat, kesuksesan/fail, kunci API, dan paginasi
- Tabel audit dashboard + endpoint statis otomatisasi untuk penggunaan

</details>

<details>
<summary><b>🔐 21. "I need scoped MCP permissions per integration"</b></summary>

Klien berbeda harus memiliki akses yang paling privasi rendah ke kategori alat.

**Mengapa OmniRoute dapat menjawabnya:**

- 9 skala kehalusan MCP (Multiple Control Plane) untuk akses kontrol perangkat
  terkendali
- Pengaktifan dan visibilitas scope di antarmuka pengguna MCP (Management User
  Interface)
- Postur baku aman untuk peralatan operasional

</details>

<details>
<summary><b>⚙️ 22. "I need operational controls without redeploying"</b></summary>

Tim membutuhkan perubahan runtime cepat selama insiden atau kejadian biaya.

**Mengapa OmniRoute dapat menjawabnya:**

- Aktivasi pilihan kombinasi langsung dari antarmuka MCP (dashboard)
- Penerapan profil ketahanan dari paket politi yang sudah ditetapkan
- Pengaturan kembali state breaker sirkuit dari panel operasi yang sama

</details>

<details>
<summary><b>🔄 23. "I need live A2A task lifecycle visibility and cancellation"</b></summary>

Tanpa visibilitas siklus, insiden tugas menjadi sulit untuk ditriage.

**Mengapa OmniRoute dapat menjawabnya:**

- Daftar tugas/pengaturan berdasarkan status/hard skill dengan pagination
- Penyinaran ke metadata tugas, event, dan artefak
- Endpoint pembatalkan tugas dan aksi UI dengan konfirmasi

</details>

<details>
<summary><b>🌊 24. "I need active stream metrics for A2A load"</b></summary>

Arus kerja streaming memerlukan wawasan operasional ke concurrency dan koneksi
yang berlangsung.

**Mengapa OmniRoute dapat menjawabnya:**

- Sistem penunjuk aktif stream terintegrasi ke status A2A
- Timestamp tugas terakhir dan perhitungan jumlah per-saat
- Kartu A2A dashboard untuk pemantauan opersional waktu nyata

</details>

<details>
<summary><b>🪪 25. "I need standard agent discovery for clients"</b></summary>

Klien eksternal dan pengatur harus memiliki metadata yang bisa dibaca mesin
untuk proses onboarding.

**Mengapa OmniRoute dapat menjawabnya:**

- Agent Card terbuka di `/.well-known/agent.json`
- Kemampuan dan keterampilan ditampilkan di UI manajemen
- Status API A2A termasuk metadata pencarian untuk otomatisasi

</details>

<details>
<summary><b>🧭 26. "I need protocol discoverability in the product UX"</b></summary>

Jika pengguna tidak dapat menemukan permukaan protokol, kualitas pengadopsi dan
dukungan akan menurun

**Mengapa OmniRoute dapat menjawabnya:**

- Halaman Endpoint ** yang disatukan dengan tab untuk Proxy, MCP, A2A, dan API
  Endpoints
- Tombol status layanan Inline (Online/Offline) untuk MCP dan A2A
- Tautan dari ringkasan ke tab manajemen dedikasi

</details>

<details>
<summary><b>🧪 27. "I need end-to-end protocol validation with real clients"</b></summary>

Pengujian palsu tidak cukup untuk mengvalidasi konsisten protokol sebelum rilis

**Mengapa OmniRoute dapat menjawabnya:**

- Paket uji E2E yang menyala aplikasi dan menggunakan transport MCP SDK real
- Pengujian klien A2A untuk pencarian, kirim, strim, get, dan batalkan alir
- Mengecek asersi melawan MCP audit dan tugas A2A API

</details>

<details>
<summary><b>📡 28. "I need unified observability across all interfaces"</b></summary>

Membagi observabilitas berdasarkan protokol menciptakan spot blind dan waktu
MTTR yang lebih lama

**Mengapa OmniRoute dapat menjawabnya:**

- Dashboard yang terpadu/logs/anlaysis dalam satu produk
- Kesehatan + audit + telemetri request untuk tingkat OpenAI, MCP, dan A2A
- API operasional untuk status dan otomatisasi

</details>

<details>
<summary><b>💼 29. "I need one runtime for proxy + tools + agent orchestration"</b></summary>

Mengoperasikan banyak layanan terpisah meningkatkan biaya operasional dan mode
kegagalan

**Mengapa OmniRoute dapat menjawabnya:**

- Proksi yang kompatibel dengan OpenAI, server MCP, dan server A2A di satu stack
- Authologi yang bersamaan, kebugaran, penyimpanan data, dan teliti
- Model kebijakan yang konsisten di semua permukaan interaksi

</details>

<details>
<summary><b>🚀 30. "I need to ship agentic workflows without glue-code sprawl"</b></summary>

Tim kehilangan kecepatan ketika menggabungkan banyak layanan dan skrip yang
ad-hoc

**Mengapa OmniRoute dapat menjawabnya:**

- Strategi endpoint yang bersamaan untuk klien dan agen
- Pengelolaan protokol bawaan dan pintasan pengadaan asap
- Dasar produksi yang siap (keamanan, pemantauan, kebugaran, backup)

</details>

### Contoh Buku Kerja (Kasus Pengguna yang Terintegrasi)

**Buku Kerja A: Maksimalkan langganan yang dibayar + cadangan murah**

```txt
Kombinasi: "maksimalkan-claude"
  1. cc/claude-opus-4-6
  2. glm/glm-4.7
  3. if/kimi-k2-pikiran

Biaya per bulan: $20 + pengeluaran kecil untuk cadangan
Hasil: kualitas yang lebih tinggi, gangguan hampir nol
```

**Buku Kerja B: Stack kode tanpa biaya**

```txt
Kombinasi: "gratis-forever"
  1. gc/gemini-3-flash
  2. if/kimi-k2-pikiran
  3. qw/qwen3-coder-plus

Biaya per bulan: $0
Hasil: alur kerja coding yang stabil tanpa biaya
```

**Buku Kerja C: Jaringan cadangan selalu berlangsung 24/7**

```txt
Kombinasi: "selalu-berlangsung"
  1. cc/claude-opus-4-6
  2. cx/gpt-5.2-codex
  3. glm/glm-4.7
  4. minimax/MiniMax-M2.1
  5. if/kimi-k2-pikiran

Hasil: kealamatan cadangan yang dalam untuk kerja keras yang menentukan waktu
```

**Buku Kerja D: Operasional agen dengan MCP + A2A**

```txt
1) Jalankan transportasi MCP (`omniroute --mcp`) untuk operasi yang dikemudikan alat
2) Jalankan tugas A2A melalui `message/send` dan `message/stream`
3) Amati via /dashboard/endpoint (tab MCP dan A2A)
4) Nyalakan/matikan layanan via kontrol status inline
```

---

## 🆓 Mulai Gratis — Biaya Konfigurasi Nol

> Tetapkan pengembangan AI dalam waktu beberapa menit pada **$0/bulan**.
> Hubungkan akun-akun gratis ini dan gunakan konsinyir **Stack Gratis** yang
> bawaan.

| Langkah | Tindakan                                                             | Pemasok Ditamatkan                                                  |
| ------- | -------------------------------------------------------------------- | ------------------------------------------------------------------- |
| 1       | Hubungkan **Kiro** (OAuth ID Pembangun AWS)                          | Sonnet Claude 4.5, Haiku 4.5 — **tanpa batas**                      |
| 2       | Hubungkan **iFlow** (OAuth Google)                                   | kimi-k2-pikiran, qwen3-coder-plus, deepseek-r1... — **tanpa batas** |
| 3       | Hubungkan **Qwen** (Kode Perangkat)                                  | qwen3-coder-plus, qwen3-coder-flicker... — **tanpa batas**          |
| 4       | Hubungkan **Gemini CLI** (OAuth Google)                              | gemini-3-flicker, gemini-2.5-pro — **-180K per bulan gratis**       |
| 5       | `/tampilan dashboard/senyawa` → **Kolom bebas (gratis $0)** template | Mulai secara otomatis semua pemasok gratis yang tersedia            |

**Arahkan IDE/KLI mana saja ke: `http://localhost:20128/v1` · Kunci API:
`apa-uniknya` · Selesai.

> **Koverase ekstensi opsional (juga gratis): **Kunci API Groq (30 RPM gratis),
> NVIDIA NIM (40 RPM gratis, 70+ model), Cerebras (1M tok/day), Kunci API
> LongCat (50M token/day!), Cloudflare Workers AI (10K Nefron/day, 50+ model).

## Mulai Cepat

### 1. Instal dan jalankan

```bash
npm install -g omniroute
omniroute
```

> **pnpm pengguna:** Jalankan `pnpm approbasi-builds -g` setelah pemasangan
> untuk mengaktifkan skrip build asli yang diperlukan oleh `better-sqlite3` dan
> `@swc/core`:
> 
> ```bash
> pnpm install -g omniroute
> pnpm approbasi-builds -g   # Pilih semua paket → approve
> omniroute
> ```

Dashboard membuka di `http://localhost:20128` dan URL basis API adalah
`http://localhost:20128/v1`.

| Perintah                | Pengenalan                                                        |
| ----------------------- | ----------------------------------------------------------------- |
| `omniroute`             | Mulai server (`PORT=20128`, API dan dashboard di porta yang sama) |
| `omniroute --port 3000` | Tetapkan porta canonical/API ke 3000                              |
| `omniroute --mcp`       | Mulai server MCP (transport stdio)                                |
| `omniroute --no-open`   | Jangan buka browser secara otomatis                               |
| `omniroute --help`      | Tampilkan informasi bantuan                                       |

Mode opsi pangkah-port:

```bash
PORT=20128 DASHBOARD_PORT=20129 omniroute
# API:       http://localhost:20128/v1
# Dashboard: http://localhost:20129
```

### 2) Hubungi penyedia dan buat API Key Anda

1. Buka Dashboard → `Penyedia` dan hubungi setidakkan satu penyedia (OAuth atau
   API Key).
2. Buka Dashboard → `Endpoint` dan buat API Key.
3. (opsional) Buka Dashboard → `Kombinasi` dan atur rantai fallback Anda.

### 3) Hubungkan alat pengembangan Anda ke OmniRoute

```txt
URL dasar: http://localhost:20128/v1
API Key:  [Salin dari halaman Endpoint]
Model:    jika/kimi-k2-pikiran (atau prefix penyedia/model mana pun)
```

Kompatibel dengan Claude Code, Codex CLI, Gemini CLI, Cursor, Cline, OpenClaw,
OpenCode, dan SDK konsultan yang kompatibel dengan OpenAI.

### 4) Aktifkan dan validasi protokol (v2.0)

**MCP (untuk operasi tool-driven):**

```bash
omniroute --mcp
```

Kemudian hubungkan klien MCP Anda melalui `stdio` dan tes alat seperti:

- `omniroute_get_health`
- `omniroute_list_combos`

**A2A (untuk alur kerja agen-ke-agen):**

```bash
curl http://localhost:20128/.well-known/agent.json
```

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: aplikasi/json' \
  -d '{"jsonrpc":"2.0","id":"quickstart","method":"pesan/kirim","params":{"skill":"manajemen kuota","messages":[{"peran":"pengguna","konten":"Berikan ringkasan kuota singkat."}]}}'
```

### 5) Validasi semua secara end-to-end (direkomendasikan)

```bash
npm run tes:protokol:e2e
```

Suite ini mengvalidasi alur klien MCP dan A2A yang asli terhadap aplikasi yang
berjalan.

### Alternatif: jalankan dari sumber

```bash
cp .env.example .env
npm install
PORT=20128 DASHBOARD_PORT=20129 NEXT_PUBLIC_BASE_URL=http://localhost:20129 npm run dev
```

---

## Container Docker

OmniRoute dapat diakses sebagai gambar Docker publik di [Docker Hub].

**Jalankan cepat:**

```bash
docker run -d \
  --name omniroute \
  --restart tidak terkalahkan \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:latest
```

**Dengan berkas lingkungan:**

```bash
# Salin dan edit .env terlebih dahulu
cp .env.example .env

docker run -d \
  --name omniroute \
  --restart tidak terkalahkan \
  --env-file .env \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:latest
```

**Menggunakan Docker Compose:**

```bash
# Profil dasar (tidak ada alat CLI)
docker compose --profile base up -d

# Profil CLI (Claude Code, Codex, Claw Terbuka)
docker compose --profile cli up -d
```

| Gambar                   | Label      | Ukuran | Pengenalan            |
| ------------------------ | ---------- | ------ | --------------------- |
| `diegosouzapw/omniroute` | `terakhir` | ~250MB | Versi stabil terakhir |
| `diegosouzapw/omniroute` | `1.0.3`    | ~250MB | Versi saat ini        |

---

## Komputer desktop — Offline dan Selalu On 👩‍💻

> 🆕 **BARU!** OmniRoute sekarang tersedia sebagai aplikasi desktop native **X
> desktop asli** untuk Windows, macOS, dan Linux.

Jalankan OmniRoute sebagai sebuah aplikasi desktop berdiri — tanpa terminal,
tanpa web browser, tanpa koneksi internet diperlukan untuk model lokal. Aplikasi
desktop berbasis Electron yang termasuk:

- 🖥️ **Jendela X Native** — Jendela aplikasi yang dedikasi dengan integrasi tray
  sistem
- 🔄 **Mulai Otomatis** — Jalankan OmniRoute pada log masuk sistem
- 🔔 **Pemberitahuan X Asli** — Dapatkan pemberitahuan untuk habis kuota atau
  masalah penyedia
- ⚡ **Pasang Sekali Klik** — NSIS (Windows), DMG (macOS), AppImage (Linux)
- 🌐 **Mode X Offline** — Berjalan penuh offline dengan server yang dibundel

### Mulai Cepat

```bash
# Modus pengembangan
npm run electron:dev

# Bangun untuk platform
npm run electron:build        # Platform saat ini
npm run electron:build:win    # Windows (.exe)
npm run electron:build:mac    # macOS (.dmg) — x64 &amp; arm64
npm run electron:build:linux  # Linux (.AppImage)
```

### Tray Sistem

Saat diminimalkan, OmniRoute tinggal di tray sistem Anda dengan tindakan cepat:

- Buka Dasbor
- Ubah port server
- Keluar aplikasi

📖 Dokumentasi lengkap: [`electron/README.md`](electron/README.md)

---

## Tarif dengan Cepat

| Tingkat             | Provider                   | Biaya                                  | Reset Quota               | Saat Terbaik                                      |
| ------------------- | -------------------------- | -------------------------------------- | ------------------------- | ------------------------------------------------- |
| **💳 SUBSCRIPSI**    | Claude Kode (Pro)          | $20/bulan                              | 5 jam + mingguan          | Already subscribed                                |
|                     | Codex (Plus/Pro)           | $20-200/bulan                          | 5 jam + mingguan          | Pengguna OpenAI                                   |
|                     | Gemini CLI                 | **gratis**                             | 180K/bulan + 1K/hari      | Orang semua!                                      |
|                     | Kopilot GitHub             | $10-19/bulan                           | Bulanannya                | Pengguna GitHub                                   |
| **🔑 API KEY**       | NVIDIA NIM                 | **gratis** (developer selamanya)       | 20 RPM                    | 70+ model pembuka                                 |
|                     | Cerebras                   | **Gratis** (1juta tok/day)             | 60R TPM / 30 RPM          | Paling cepat di dunia                             |
|                     | Groq                       | **Gratis** (30 RPM)                    | 14.400 RPM                | Llama/Gemma yang sangat cepat                     |
|                     | DeepSeek V3.2              | $0,27/$1,10 per 1juta                  | Tidak ada                 | Alasan harga/kualitas terbaik                     |
|                     | xAI Grok-4 Cepat           | **$0,20/$0,50 per 1juta** 🆕            | Tidak ada                 | Paling cepat + panggilan instrumen, rendah sekali |
|                     | xAI Grok-4 (standar)       | $0,20/$1,50 per 1juta 🆕                | Tidak ada                 | Flagship alasan dari xAI                          |
|                     | Mistral                    | Free trial + pembayaran berlangganan   | Tarif terbatas            | AI Eropa                                          |
|                     | OpenRouter                 | Bayar sesuai penggunaan                | Tidak ada                 | Integrasi +100 model                              |
| ** 💰 HARGA MURAH ** | GLM-5 (via Z.AI) 🆕         | $0,5/1 juta                            | Setiap hari, 10 pagi      | 128K keluaran, flagship terbaru                   |
|                     | GLM-4,7                    | $0,6/1 juta                            | Setiap hari, 10 pagi      | Cadangan anggaran                                 |
|                     | MiniMax M2,5 🆕             | $0,3/1 juta (masukan)                  | Aktifitas 5 jam (berlalu) | Tugas alur kelanjutan + aksinya                   |
|                     | MiniMax M2,1               | $0.2/1Juta                             | Aktifitas 5 jam (berlalu) | Pilihan Termurah                                  |
|                     | Kimi K2.5 (API Moonshot) 🆕 | Bayar sesuai penggunaan                | Tidak ada                 | Akses Langsung ke API Moonshot                    |
|                     | Kimi K2                    | $9/bulan biaya tetap                   | 10Juta token/bulan        | Biaya yang dapat diprediksi                       |
| **🆓 GRATIS**        | iFlow                      | **$0**                                 | Tidak Terbatas            | 5 model tidak terbatas                            |
|                     | Qwen                       | **$0**                                 | Tidak Terbatas            | 4 model tidak terbatas                            |
|                     | Kiro                       | **$0**                                 | Tidak Terbatas            | Claude Sonnet/Haiku (AWS Builder)                 |
|                     | LongCat Flash-Lite 🆕       | **$0** (50Juta tok/hari 🔥)             | 1 RPS                     | Kuota tertinggi gratis di Bumi                    |
|                     | Pollinations AI 🆕          | **$0** (tidak ada key yang diperlukan) | 1 permintaan/15s          | GPT-5, Claude, DeepSeek, Llama 4                  |
|                     | Cloudflare Workers AI  🆕   | **$0** (10K neuron/hari)               | ~150 respon/hari          | 50+ model, edge global                            |
|                     | Scaleway AI 🆕              | **$0** (1M token total)                | Tarif terbatas            | UE/GDPR, Qwen3 235B, Llama 70B                    |

> 🆕 **Model baru yang ditambahkan (Mar 2026):** Keluarga Grok-4 Fast pada
> $0,20/$0,50/M (didemonstrasikan sebanyak 1143ms — 30% lebih cepat daripada
> Gemini 2.5 Flash), GLM-5 melalui Z.AI dengan 128K keluaran, MiniMax M2.5
> rasio, DeepSeek V3.2 harga yang diupdate, Kimi K2.5 melalui Moonshot API
> langsung.

**💡 $0 Stack Kombo Lengkap — Setup Gratis yang Lengkap:**

```
# 🆓 Stack Gratis Ultimate 2026 — 11 Pengembang, $0 Forever
Kiro (kr/)             → Claude Sonnet/Haiku TANPA BATAS
iFlow (if/)            → kimi-k2-pikiran, qwen3-peserta-coder-plus, deepseek-r1 TANPA BATAS
LongCat Lite (lc/)     → LongCat-Flash-Lite — 50M token/hari 🔥
Pollinations (pol/)    → GPT-5, Claude, DeepSeek, Llama 4 — tidak ada key yang diperlukan
Qwen (qw/)             → qwen3-peserta-coder-plus, qwen3-peserta-coder-Flash, qwen3-peserta-coder-turut TANPA BATAS
Gemini (gemini/)       → Gemini 2.5 Flash — 1.500 permintaan/bebas API key gratis
Cloudflare AI (cf/)    → Llama 70B, Gemma 3, Mistral — 10K neuron/hari
Scaleway (scw/)        → Qwen3 235B, Llama 70B — 1M token gratis (UE)
Groq (groq/)           → Llama/Gemma tercepat — 14.4K permintaan/hari
NVIDIA NIM (nvidia/)   → 70+ model terbuka — 40 RPM selamanya
Cerebras (cerebras/)   → Llama/Qwen paling cepat di dunia — 1M tok/hari
```

** Gratis. Tidak pernah berhenti menerjemahkan.** Konfigurasi ini sebagai satu
combo OmniRoute dan semua fallback terjadi secara otomatis — tidak perlu memilih
manualpun.

---

---

## 🆓 Model Gratis — Apa yang Anda Sebenarnya Dapatkan

> Semua model di bawah ini adalah ** 100% gratis dengan tidak memerlukan kartu
> kredit**. OmniRoute memanfaatkan model lain ketika quota satu model habis —
> kombinasikan mereka semua untuk kombo $0 yang tak terpecahkan.

### 🔵 CLAUDE MODELS (via Kiro — AWS Pembangun ID)

| Model               | Awalan | limit              | Batas Nilai                   |
| ------------------- | ------ | ------------------ | ----------------------------- |
| `Claude-Sonnet-4.5` | `kr/`  | ✨ Tidak Terbatas** | Tidak ada batasan sehari-hari |
| `Claude-Haiku-4.5`  | `kr/`  | ✨ Tidak Terbatas** | Tidak ada batasan sehari-hari |
| `Claude-Opus-4.6`   | `kr/`  | ✨ Tidak Terbatas** | Opu Terakhir melalui Kiro     |

### 🟢 IFlow MODELS (OAuth Gratis — Tidak Membayar Kartu Kredit)

| Model                        | Awalan | limit              | Batas Nilai                       |
| ---------------------------- | ------ | ------------------ | --------------------------------- |
| `Kimi-K2-Pikiran`            | `if/`  | ✨ Tidak Terbatas** | Tidak Ada Batasan yang Dilaporkan |
| Pencarian PWWEN3-coder-plus` | `if/`  | ✨ Tidak Terbatas** | Tidak Ada Batasan yang Dilaporkan |
| Pencarian Mendalam-r1`       | `if/`  | ✨ Tidak Terbatas** | Tidak Ada Batasan yang Dilaporkan |
| Pencarian Minimalis-m2.1`    | `if/`  | ✨ Tidak Terbatas** | Tidak Ada Batasan yang Dilaporkan |
| Pencarian Kimi-k2`           | `if/`  | ✨ Tidak Terbatas** | Tidak Ada Batasan yang Dilaporkan |

### 👻 MODELS PWWEN (Kode Perangkat Auth)

| Model                         | Awalan            | limit              | Batas Nilai                       |
| ----------------------------- | ----------------- | ------------------ | --------------------------------- |
| Pencarian PWWEN3-coder-plus`  | Pencarian PWWEN/` | ✨ Tidak Terbatas** | Tidak Ada Batasan yang Dilaporkan |
| Pencarian PWWEN3-coder-flash` | Pencarian PWWEN/` | ✨ Tidak Terbatas** | Tidak Ada Batasan yang Dilaporkan |
| Pencarian PWWEN3-coder-next`  | Pencarian PWWEN/` | ✨ Tidak Terbatas** | Tidak Ada Batasan yang Dilaporkan |
| Pencarian Model Penglihatan`  | Pencarian PWWEN/` | ✨ Tidak Terbatas** | Multimodal (gambar)               |

### 🔵 CLI GEMINI (Auth Google OAuth)

| Model                    | Awalan | limit                                 | Batas Nilai          |
| ------------------------ | ------ | ------------------------------------- | -------------------- |
| `Gemini-3 Flash Preview` | `gc/`  | **180K token/month** + 1K/hari        | Lewat bulan          |
| `Gemini-2,5 pro`         | `gc/`  | 180K/token/bulan (benjolan bersamaan) | Kualitas yang tinggi |

### NVIDIA NIM (API Kunci Gratis — build.nvidia.com)

| Tingkat      | Batas Harian                 | Batas Nilai | Catatan                                                                |
| ------------ | ---------------------------- | ----------- | ---------------------------------------------------------------------- |
| Gratis (Dev) | Tidak ada pengecualian token | **~40 RPM** | 70+ mode; sementara bertransisi ke batasan kecepatan purna, paruh-2025 |

Model gratis populer: `moonshotai/kimi-k2.5` (Kimi K2.5), `z-ai/glm4.7` (GLM
4.7), `deepseek-ai/deepseek-v3.2` (DeepSeek V3.2),
`nvidia/llama-3.3-70b-instruct`, `deepseek/deepseek-r1`

### CEREBRAS (API Kunci Gratis — inference.cerebras.ai)

| Tingkat | Batas Harian      | Batas Nilai      | Catatan                                                              |
| ------- | ----------------- | ---------------- | -------------------------------------------------------------------- |
| Gratis  | **1M token/hari** | 60R TPM / 30 RPM | Inferensi LLM yang paling cepat di dunia; mengatur ulang setiap hari |

Tersedia gratis: `llama-3.3-70b`, `llama-3.1-8b`,
`deepseek-r1-distill-llama-70b`

### 🔴 GROQ (Kunci API Gratis — console.groq.com)

| Tingkat | Batas Harian  | Batas Nilai      | Catatan                                                                |
| ------- | ------------- | ---------------- | ---------------------------------------------------------------------- |
| Gratis  | **14.4K RPD** | 30 RPM per model | Tidak diperlukan kartu kredit; 429 ketika batas, tidak dikenakan biaya |

Tersedia gratis: `llama-3.3-70b-versatile`, `gemma2-9b-it`, `mixtral-8x7b`,
`whisper-large-v3`

### 🔴 LONGCAT AI (Kunci API Gratis — longcat.chat) 🆕

| Model                         | Awalan | Hari Bebas Quota | Catatan                          |
| ----------------------------- | ------ | ---------------- | -------------------------------- |
| `LongCat-Flash-Lite`          | `lc/`  | **50M token** 💥  | Quota gratis terbesar sejauh ini |
| `LongCat-Flash-Chat`          | `lc/`  | 500K token       | Chat multi-turn                  |
| `LongCat-Flash-Thinking`      | `lc/`  | 500K token       | Pikiran / CoT                    |
| `LongCat-Flash-Thinking-2601` | `lc/`  | 500K token       | Versi Januari 2026               |
| `LongCat-Flash-Omni-2603`     | `lc/`  | 500K token       | Multimodal                       |

> 100% gratis selama beta publik. Daftar di [longcat.chat](https://longcat.chat)
> dengan email atau telepon. Reset harian pukul 00:00 UTC.

### 🟢 POLLINATIONS AI (Tidak Diperlukan API Key) 🆕

| Model      | Awalan | Batas Nilai      | Penyedia di Balik  |
| ---------- | ------ | ---------------- | ------------------ |
| `openai`   | `pol/` | 1 permintaan/15s | GPT-5              |
| `claude`   | `pol/` | 1 permintaan/15s | Anthropic Claude   |
| `gemini`   | `pol/` | 1 permintaan/15s | Google Gemini      |
| `deepseek` | `pol/` | 1 permintaan/15s | DeepSeek V3        |
| `llama`    | `pol/` | 1 permintaan/15s | Meta Llama 4 Scout |
| `mistral`  | `pol/` | 1 permintaan/15s | Mistral AI         |

> ✨ Tidak adanya gesekan:** Tidak ada pendaftaran, tidak ada API key. Tambahkan
> penyedia Pollinations dengan bidang kunci kosong dan bekerja langsung.

### 🟠 PENYEDIA KEPERCAYAAN KEPABEANAN CLOUDFLARE (API Key Gratis — cloudflare.com) 🆕

| Tingkat | Siklus Sinar Harian | Penggunaan Equivalen                                          | Catatan                |
| ------- | ------------------- | ------------------------------------------------------------- | ---------------------- |
| Gratis  | 10.000**10.000**    | ~ 150 LLM per permintaan / 500 detik audio / 15.000 embedding | Edge Global, 50+ model |

Model bebas populer: `@cf/meta/llama-3.3-70b-instruct`,
`@cf/google/gemma-3-12b-it`, `@cf/openai/whisper-large-v3-turbo` (audio
gratis!), `@cf/qwen/qwen2.5-coder-15b-instruct`

> Memerlukan Token API + ID Akun dari
> [dash.cloudflare.com](https://dash.cloudflare.com). Simpan ID Akun di
> pengaturan penyedia.

### 🟣 INTI SKALA AI (1M Token Gratis — scaleway.com) 🆕

| Tingkat | Kuantitas Gratis                   | Lokasi       | Catatan                                    |
| ------- | ---------------------------------- | ------------ | ------------------------------------------ |
| Gratis  | 1.000.000 token**1.000.000 token** | 🇫🇷 Paris, EU | Tidak perlu kartu kredit dalam batas limit |

Tersedia gratis: `qwen3-235b-a22b-instruct-2507` (Qwen3 235B!),
`llama-3.1-70b-instruct`, `mistral-small-3.2-24b-instruct-2506`,
`deepseek-v3-0324`

> Tunduk GDPR/EU. Dapatkan kunci API di
> [console.scaleway.com](https://console.scaleway.com).

> ** 💡 Stok Bebas Ultimate (11 Penyedia, $0 Abadi):**
> 
> ```
> Kiro (kr/)             → Claude Sonnet/Haiku SERBAGA UNTERBATAS
> iFlow (if/)            → kimi-k2-thinking, qwen3-coder-plus, perdeep-mengembara-1 UNTERBATAS
> LongCat Lite (lc/)     → LongCat-Flash-Lite — 50Juta Token/hari 🔥
> Pollinations (pol/)    → GPT-5, Claude, DeepSeek, Llama 4 — tidak perlu kunci
> Qwen (qw/)             → qwen3-coder perangkat UNTERBATAS
> Gemini (gemini/)       → Gemini 2.5 Flash — 1.500 permintaan/hari gratis
> Cloudflare AI (cf/)    → 50+ perangkat — 10Ribu Sinar/Hari
> Scaleway (scw/)        → Qwen3 235M, Llama 70M — 1Juta Token gratis (EU)
> Groq (groq/)           → Llama/Gemma — 14.4Ribuan permintaan/hari super-cepat
> NVIDIA NIM (nvidia/)   → 70+ model terbuka — 40 RPM selamanya
> Cerebras (cerebras/)   → Llama/Qwen tercepat di dunia — 1Juta tok/hari
> ```

## 🎙️ Kombo Transkripsi Gratis

> Transkripsi audio/video apa saja untuk [X312X] $0** — Deepgram mendapatkan
> utang $200, AssemblyAI $50 penyimpanan, Groq Whisper sebagai cadangan darurat
> tanpa batas.

| Provider         | Sisa Kredit                    | Model Terbaik                            | Batas Nilai                        |
| ---------------- | ------------------------------ | ---------------------------------------- | ---------------------------------- |
| 🟢 **Deepgram**   | ** $200 gratis** (tanda ulang) | ` nova-3` — ketepatan tinggi, 30+ bahasa | Tanpa Batas RPM pada kredit gratis |
| 🔵 **AssemblyAI** | ** $50 gratis** (tanda ulang)  | ` universal-3-pro` — bab, sentiment, PII | Tanpa Batas RPM pada kredit gratis |
| 🔴 **Groq**       | ** selamanya gratis**          | ` whisper-large-v3` — OpenAI Whisper     | 30 RPM (terbatas kecepatan)        |

** Kombinasi yang disarankan di `/dashboard/combos`:**

```
Nama: kiro-transkripsi gratis
 Strategi: Prioritas
 Node:
  [1] deepgram/nova-3          → menggunakan $200 free pertama
  [2] assemblyai/universal-3-pro → alternatif ketika kredit Deogram habis
  [3] groq/whisper-large-v3    → gratis selamanya, cadangan darurat
```

Dalam `/dashboard/media` → **Transkripsi** tab: unggah berkas audio atau video
mana saja → pilih endpoint combo Anda → dapatkan transkripsi dalam format yang
didukung.

## 💡 Fitur Utama

OmniRoute v2.0 dibangun sebagai platform operasional, bukan hanya relay proxy.

### 🆕 Baru — Perbaikan-Inspired ClawRouter (Mar 2026)

| Fitur                                    | Apa Kegunannya                                                                                                      |
| ---------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| ⚡ **Grok-4 Fast Family**                 | Model AI pada $0.20/$0.50/Juta — teruji 1143ms (30% lebih cepat dari Gemini 2.5 Flash)                              |
| 🧠 **GLM-5 melalui Z.AI**                 | Konteks keluaran 128K, $0.5/1Juta — flagship terbaru dari keluarga GLM                                              |
| 🔮 **MiniMax M2.5**                       | Tugas penalaran + agen pada $0.30/1Juta — upgrade signifikan dari M2.1                                              |
| 🎯 **flag Panggilan Model per Model**     | Panggilan per model `toolCalling: true/false` dalam registry — AutoCombo melompati model non-cahut yang tidak mampu |
| 🌍 **Deteksi Niat Berbahasa Multibahasa** | Kata kunci PT/ZH/ES/AR dalam scoring AutoCombo — pemilihan model yang lebih baik untuk konten non-Bahasa Inggris    |
| 📊 **Fallback Terbangun dari Benchmark**  | Laju nyata p95 dari permintaan hidup sebagai umpan balik scoring Combo — AutoCombo belajar dari data nyata          |
| 🔁 **Deduplikasi Permintaan**             | Jendela dedup berdasarkan hash konten — aman multi-agency, mencegah biaya berulang                                  |
| 🔌 **Router Strategi Pluggable **         | Extensible `Router Strategi` interface — tambahkan logika routing kustom sebagai plugin                             |

### 🚀 Sebelumnya v2.0.9+ — Playground, CLI Fingerprint Matching & ACP

| Fitur                                      | Apa Kegunannya                                                                                                                                                                                                                                                                               |
| ------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🎮 **Model Playground**                     | Halaman dashboard untuk menguji model apa saja secara langsung — pengilih provider/model/endpoint, Editor Monaco, streaming, abort, timing                                                                                                                                                   |
| 🔏 **Matching Fingerprint CLI **            | Urutan header/body per-provider untuk menyesuaikan tanda tangan CLI alami — nonaktifkan per provider di Pengaturan > Keamanan. **Alamat IP proxy Anda tetap dipertahankan**                                                                                                                  |
| 🤝 **Dukungan ACP (Protocol Client Agent)** | Pengenalan agen CLI (Codex, Claude, Goose, Gemini CLI, OpenClaw + 9 lebih lagi), pengganti proses, endpoint `/api/acp/agen`                                                                                                                                                                  |
| 🤖 **DASHBOARD AGEN ACP **                  | Uji coba › Halaman Agent — grid dari 14 agen dengan status instalasi, versi, formulir agen kustom untuk alat CLI apa saja. **Pengguna OpenCode** mendapatkan tombol "Unduh opencode.json" yang secara otomatis menghasilkan konfigurasi yang siap digunakan dengan semua model yang tersedia |
| 🔧 **Model Model `apiFormat` Routing **     | Model kustom dengan `apiFormat: "responses"` sekarang secara benar menyeting ke Translator API Respons                                                                                                                                                                                       |
| 🏢 **Isolasi Workspace Codex **             | Banyaknya workspace Codex per email — OAuth memisahkan koneksi dengan ID workspace yang benar                                                                                                                                                                                                |
| 🔄 **Update Otomatis Electron **            | Aplikasi desktop memeriksa update + menginstal secara otomatis saat restart                                                                                                                                                                                                                  |

### 🤖 Operasi Agenta & Protokol (v2.0)

| Fitur                                       | Apa Kegunannya                                                                                  |
| ------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| 🔧 **Server MCP (16 alat)**                  | IDE/agen alat via 3 transport: stdio, SSE (`/api/mcp/sse`), Streamable HTTP (`/api/mcp/stream`) |
| 🤝 **Server A2A (JSON-RPC + SSE)**           | Eksekusi tugas antar-agen dengan aliran sinkronisasi dan streaming                              |
| 🧭 **Halaman Endpoint Terpadu**              | Halaman manajemen yang beralur, Endpoint Proxy, MCP, A2A, dan API Endpoints                     |
| 🎚️ **Tombol Untuk Menyala/Menindas Servis** | Tombol ON/OFF untuk MCP dan A2A dengan penyimpanan pengaturan (ataran: OFF)                     |
| 🛰️ **Detak Hati Nurani MCP**                | Status proses nyata (pid, waktu, usia detak, transport, mode lingkup)                           |
| 📋 **Jejak Pengauditan MCP**                 | Cari/berdasarkan jejak log pengauditan dengan kesuksesan/gagal dan atribusi kunci               |
| 🔐 **Pengamanan Lingkup MCP**                | 9 izin keamanan lingkup yang teliti untuk akses alat terkontrol                                 |
| 📡 **Manajemen Hidup Tugas A2A**             | Tampilkan/mencari tugas, menginspeksi acara/artikel, batalkan tugas berjalan                    |
| 📋 **Penemuan Kardus Agent**                 | `/.well-known/agent.json` untuk auto-pengenalan klien                                           |
| 🧪 **Protokol E2E Uji Harness**              | Nyata SDK MCP + A2A client flows di protokol `uji:protokol:e2e`                                 |
| ⚙️ **Kontrol Operasional**                  | Ganti combo, aplikasikan profil ketahanan, dan atur reset breaker dari satu permukaan kontrol   |

### 🧠 Routing & Intelligence

| Fitur                                          | Apa Kegunannya                                                                              |
| ---------------------------------------------- | ------------------------------------------------------------------------------------------- |
| 🎯 **Fallas Inteligen 4-Tier**                  | Merekam secara otomatis: Subskripsi → Kunci API → Murah → Gratis                            |
| 📊 **Pantauan Kuota Sederhana Muka waktu Real-X | Tokennya beredar langsung + hitung mundur reset per penyedia                                |
| 🔄 **Translasi Format**                         | OpenAI ↔ Claude ↔ Gemini ↔ Respons dengan konversi yang aman skema                          |
| 👥 **Dukungan Akun Menggunakan Banyak Akun**    | Banyak akun per penyedia dengan seleksi yang pintar                                         |
| 🔄 **Penghapusan Otomatis Token**               | Tokennya menerima penghapusan secara otomatis dengan ulangi                                 |
| 🎨 **Kombinasi Kustom**                         | Strategi keseimbangan 6 + kontrol rantai fallback                                           |
| 🌐 **Router Jalan-Jalan**                       | Pengguna ` provider/*` routing dinamis                                                      |
| 🧠 Pengaturan Anggaran **Pikiran **             | Telaah otomatis, auto, kustom, dan batasan adaptif                                          |
| 🔀 Penggandaan **Alias Model **                 | Penggandaan model yang dibangun sendiri dan aman untuk migrasi                              |
| ⚡ **Degradasi Latar **                         | routing tugas berkepentingan rendah ke model yang lebih murah                               |
| 🧪 Rute Pengambilan Tugas yang Bijak **         | mengambil model yang sesuai dengan jenis konten (pengkodean/penglihatan/analisis ringkasan) |
| 💬 Penginjeksian Prompt Sitem **                | pengontrol perilaku yang konsisten                                                          |
| 📄 Kompatibilitas API Tanggapan **              | support lengkap `/v1/responses` untuk Codex dan alur kerja agen yang canggih                |

### 🎵 API Multimodal

| Fitur                       | Apa Kegunannya                                                                                                                                                             |
| --------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🖼️ Generasi **Gambar **     | generasi `/v1/images/generations` dengan backend cloud dan lokale                                                                                                          |
| 📐 Pencarian **Pengukuran ** | pencarian `/v1/embeddings` untuk alur pipeline RAG                                                                                                                         |
| 🎤 **Transkripsi Audio**     | `/v1/audio/transcriptions` — 7 penyedia (Deepgram Nova 3, AssemblyAI, Groq Whisper, HuggingFace, ElevenLabs, OpenAI, Azure), deteksi otomatis bahasa, dukungan MP4/MP3/WAV |
| 🔊 **Text-to-Speech**        | `/v1/audio/speech` — 10 penyedia (ElevenLabs, OpenAI, Deepgram, Cartesia, PlayHT, HuggingFace, Nvidia NIM, Inworld, Coqui, Tortoise) dengan pesan kesalahan yang akurat    |
| 🎬 **Pembuatan Video**       | `/v1/videos/generations` (ComfyUI + SD WebUI workflow)                                                                                                                     |
| 🎵 **Pembuatan Musik**       | `/v1/music/generations` (ComfyUI workflow)                                                                                                                                 |
| 🛡️ **Pengaturan Keamanan**  | `/v1/moderations` periksa keselamatan                                                                                                                                      |
| 🔀 **Reranking**             | `/v1/rerank` untuk skor relevansi                                                                                                                                          |
| 🔍 **Pencarian Web** 🆕       | `/v1/search` — 5 penyedia (Serper, Brave, Perplexity, Exa, Tavily), 6.500+ gratis/bulan, otomatis failover, cache                                                          |

### 🛡️ Keamanan, Keselamatan & Penggabungan Data

| Fitur                              | Apa Kegunannya                                                                         |
| ---------------------------------- | -------------------------------------------------------------------------------------- |
| 🔌 **Circuit Breakers**             | Pengulangan model/recover dengan kontrol ambang batas                                  |
| 🎯 **Model yang Sadar Endpoint**    | Custom models declare supported endpoints + API format                                 |
| 🛡️ **Anti-Thundering Herd**        | Mutex + semaphore protections on retry/rate events                                     |
| 🧠 **Semantic + Signature Cache**   | Cost/latency reduction with two cache layers                                           |
| ⚡ **Request Idempotency**          | Duplicate protection window                                                            |
| 🔒 **TLS Fingerprint Spoofing**     | Browser-like TLS fingerprint — **reduces bot detection and account flagging**          |
| 🔏 **Matching Fingerprint CLI **    | Matches native CLI request signatures — **reduces ban risk while preserving proxy IP** |
| 🌐 **IP Filtering**                 | Allowlist/blocklist control for exposed deployments                                    |
| 📊 **Editable Rate Limits**         | Configurable global/provider-level limits with persistence                             |
| 🔑 **API Key Management + Scoping** | Secure key issuance/rotation and model/provider controls                               |
| 🛡️ **Protected `/models`**         | Optional auth gating and provider hiding for model catalog                             |

### 📊 Observability & Analytics

| Fitur                                     | Apa Kegunannya                                                        |
| ----------------------------------------- | --------------------------------------------------------------------- |
| 📝 Catatan **Permintaan + Logging Proxy**  | Pencatatan permintaan dan respon serta logging proxy                  |
| 📋 **Tampilan Dashboard Log Terintegrasi** | Penglihatan request, proxy, audit, dan console dalam satu halaman     |
| 🔍 **Teliti Teknologi Permintaan**         | Keterlambatan p50/p95/p99 dan kemahiran tracing permintaan            |
| 🏥 **Tampilan Dashboard Kesehatan**        | Aktivitas waktu, kondisi rusak, pemblokiran, statistik cache          |
| 💰 **Pantauan Biaya**                      | Pengendalian anggaran dan visibilitas harga per-model                 |
| 📈 **Visualisasi Hasil Analitik**          | Wawasan penggunaan model/provider dan tampilan tren                   |
| 🧪 **Semenanjung Evaluator**               | Pengujian set emas dengan strategi pencocokan yang dapat dikonfigurir |

### ☁️ Penyebaran & Platform

| Fitur                           | Apa Kegunannya                                                    |
| ------------------------------- | ----------------------------------------------------------------- |
| 🌐 **Tegangkan Mana Saja**       | Lokal, VPS, Docker, Lingkungan cloud                              |
| 💾 **Sink **                     | Sink konfigurasi melalui pekerja cloud                            |
| 🔄 **Backup/Restore**            | Alur ekspor/impot dan recovery bencana                            |
| 🧙 **Wizard Penggunaan[Berisi]** | Pengaturan dasar tugasnya pertama                                 |
| 🔧 **Instrumen CLI Pita(X23X]    | Penyiapan satu-klik perangkat lunak perkalian populer             |
| 🎮 **Model Playground**          | Jalankan uji dari dashboard pada penyedia/model/endpoint apa saja |
| 🔏 **Toggle Jari CLI (X26X]      | Matching jari penyedia per penyedia di Pengaturan > Keamanan      |
| 🌐 **I18n (30 bahasa)**          | Dukungan bahasa penuh + dokumen plus penutupan RTL                |
| 🧹 **Hapus Semua Model**         | Menghapus daftar model dengan sekali-klik di detail penyedia      |
| 📋 **Template Masalah**          | Template GitHub baku untuk masalah dan fitur                      |
| 📂 **Direktori Data Kustom**     | `DIREKTORI_DATA` override untuk lokasi penyimpanan                |

### Penjelasan Fitur Deep Dive

#### Pengalihan cerdas dengan pengendalian biaya praktis

```txt
Kombinasi: "kode-saya-stack"
  1. cc/claude-opus-4-6
  2. nvidia/llama-3.3-70b
  3. glm/glm-4.7
  4. jika/kimi-k2-pengemudi
```

Jika kuota, tarif, atau kesehatan gagal, OmniRoute secara otomatis Bergerak ke
kandidat berikutnya tanpa switching manual.

#### Manajemen protokol yang terlihat dan beroperasi

- MCP + A2A dapat ditemukan di UI dan dokumentasi (tidak disembunyikan)
- API status protokol mengungkapkan data operasional hidup (`/api/mcp/*`,
  `/api/a2a/*`)
- Dahsboard mencakup aksi untuk operasional hari ke-2 (combo toggle, breaker
  reset, pembatalan tugas)

#### Alur kerja penerjemah + validasi

Area Penerjemah termasuk:

- **Lahan main**: periksa pengecekan transformasi
- **Coba-basa: tugas permintaan/keluaran 1 rute penuh
- **Meja Uji**: kasus-kasus multiple dalam 1 lari
- **Pantau secara langsung**: pandangan real-time traffic

Pengujian protokol validasi dengan klien pengguna via `npm run
test:protocols:e2e`.

> 📖 **[Baca README MCP Server (open-sse/mcp-server/README.md)** — Referensi
> alat, konfigurasi IDE, dan contoh klien
> 
> 📖 **[Baca README A2A Server (src/lib/a2a/README.md)** — Kemampuan, metode
> JSON-RPC, aliran, dan jadwal hidup tugas

## 🧪 Evaluasi (Evals)

OmniRoute menyediakan kerangka evaluasi bawaan untuk menguji kualitas respons
LLM melawan set emas. Akses melalui **Analisis → Evals** di dashboard.

### Paket Standar Emas

Paket pra-loader "OmniRoute Golden Set" berisi kasus peraturan untuk:

- Selamat Datang, matematik, geografi, kode penghasilan
- Komitmen dengan JSON, terjemahan, generasi markdown
- Kehilangan keamanan (konten berbahaya), komputeran bilangan, logika boolean

### Strategi Evaluasi

| Strategi     | Pengenalan                                                      | Contoh                                             |
| ------------ | --------------------------------------------------------------- | -------------------------------------------------- |
| `tepat`      | Keluarannya harus cocok secara tepat                            | `"4"`                                              |
| `mengandung` | Keluaran harus mengandung substring (tanpa memperhatikan kasus) | `"Paris"`                                          |
| `regex`      | Keluarannya harus cocok dengan pola regex                       | `"1.*2.*3"`                                        |
| `custom`     | Fungsi JS custom mengembalikan true/false                       | `(hasil output) =&gt; hasil output.length &gt; 10` |

---

## Panduan Pengaturan 📖

### Pengaturan Protokol (MCP + A2A)

<details>
<summary><b>🧩 MCP Setup (Model Context Protocol)</b></summary>

Mulai transport MCP dalam mode stdio:

```bash
omniroute --mcp
```

Aliran validasi yang disarankan:\
==

1. Hubungkan klien MCP Anda melalui stdio.
2. Jalankan `omniroute_get_health`.
3. Jalankan `omniroute_list_combos`.
4. Buka `/dashboard/mcp` untuk memastikan detak jantung, kegiatan, dan audit.

API yang bermanfaat untuk otomatisasi:

- `GET /api/mcp/status`
- `GET /api/mcp/tools`
- `GET /api/mcp/audit`
- `GET /api/mcp/audit/stats`

</details>

<details>
<summary><b>🤝 A2A Setup (Agent2Agent)</b></summary>

Tentukan agen:

```bash
curl http://localhost:20128/.well-known/agent.json
```

Kirim tugas:

```bash
curl -X POST http://localhost:20128/a2a 
  -H 'content-type: application/json' 
  -d '{"jsonrpc":"2.0","id":"setup-a2a","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"Ringkasan status kuota."}]}}'
```

Manajemen siklus kehidupan:

- GET /api/a2a/status
- GET /api/a2a/tasks
- GET /api/a2a/tasks/:id
- POST /api/a2a/tasks/:id/cancel

Beranda UI:

- `/dashboard/a2a` untuk memantau tugas/keadaan/ aliran dan aksi keluaran

</details>

<details>
<summary><b>🧪 End-to-end protocol validation</b></summary>

Validasi kedua protokol dengan klien nyata:

```bash
npm run tes:protokol:e2e
```

Hal ini memverifikasi:

- Klient SDK MCP koneksi/list/panggilan
- Pengungkapan A2A ketahui/berbagi/ aliran/batalkan
- Perluasan data dalam audit MCP dan API manajemen tugas A2A

</details>

<details>
<summary><b>💳 Subscription Providers</b></summary>

### Claude Code (Pro/Maks)

```bash
Beranda → Pengada → Hubungkan Claude Code
→ Login OAuth → Perbarui token otomatis
→ Pemantauan kuota 5 jam + mingguan

Model :
  cc/claude-opus-4-6
  cc/claude-sonnet-4-5-20250929
  cc/claude-haiku-4-5-20251001
```

**Tusunan Utama :** Gunakan Opus untuk tugas kompleks, Sonnet untuk kecepatan.
OmniRoute melacak kuota per model!

### OpenAI Codex (Plus/Pro)

```bash
Beranda → Pengada → Hubungkan Codex
→ Login OAuth (port 1455)
→ Pemantauan 5 jam + mingguan reset

Model :
  cx/gpt-5.2-codex
  cx/gpt-5.1-codex-max
```

#### Pengelolaan Batas Akun Codex (5h + Mingguan)

Setiap akun Codex sekarang memiliki toggle kebijakan di `Beranda -&gt; Pengada
`:

- `5 Jam` (ON/OFF): mengaktifkan kebijakan jendela waktu ambang batas 5 jam.
- `Mingguan` (MENGIKUTI/ MATI): implement kebijakan jendela Mingguan.
- Siklus batas: ketika jendela yang diaktifkan mencapai >=90% penggunaan, akun
  tersebut dilewati.
- Siklus rotasi: OmniRoute mengarahkan ke akun Codex yang layak berikutnya
  secara otomatis.
- Pengaktifan ulang: ketika waktu `resetAt` penyedia melewati waktu tertentu,
  akun tersebut kembali layak secara otomatis.

Scenariio:

- `5 jam ON` + `Mingguan ON`: akun dilewati ketika jendela mana pun mencapai
  ambang batas.
- `5 jam OFF` + `Mingguan ON`: hanya penggunaan mingguan yang dapat menghalangi
  akun.
- `5 jam ON` + `Mingguan OFF`: hanya penggunaan 5 jam yang dapat menghalangi
  akun.
- `resetAt` lewati: akun kembali masuk ke rotasi secara otomatis (tidak perlu
  diaktifkan manual).

### CLI Gemini (BEBAS 180K/month!)

```bash
Dashboard → Penyedia → Hubungkan CLI Gemini
→ Google OAuth
→ 180K penghantaran lengkap/month + 1K/hari

Model:
  gc/gemini-3-preview-terbakar
  gc/gemini-2.5-pro
```

**Nilai Terbaik:** Membawa tipe gratis yang besar! Gunakan hal ini sebelum
tingkat pembayaran.

### Kopilot GitHub

```bash
Dashboard → Penyedia → Hubungkan GitHub
→ OAuth melalui GitHub
→ Reset bulanan (1 Januari)

Model:
  gh/gpt-5
  gh/claude-4.5-sonnet
  gh/gemini-3-pro
```

</details>

<details>
<summary><b>🔑 API Key Providers</b></summary>

### NVIDIA NIM (Akses pengembang gratis — 70+ model)

1. Daftar: [build.nvidia.com](https://build.nvidia.com)
2. Dapatkan akses API gratis (1000 kredit inferensi termasuk)
3. Dashboard → Tambah Penyedia → NVIDIA NIM:
   - Kunci API: `nvapi-kunci-anda`

**Model:** `nvidia/llama-3.3-70b-instruct`, `nvidia/mistral-7b-instruct`, dan
50+ lebih banyak

[Tips Pro:][Tip10] API Kompatibel OpenAI — berjalan lancar dengan format
pengubahan OmniRoute!

### DeepSeek

1. Daftar: [platform.deepseek.com](https://platform.deepseek.com)
2. Dapatkan Kunci API
3. Dashboard → Tambah Provider → DeepSeek

[Tips Pro:][Tip0] Model:[Tip9] [Tip12]deepseek/deepseek-chat[Tip35],
[Tip38]deepseek/deepseek-coder[Tip62]

### Groq (Tingkat Gratis Tersedia!)

1. Daftar: [console.groq.com](https://console.groq.com)
2. Dapatkan Kunci API (tingkat gratis tercakup)
3. Dashboard → Tambah Provider → Groq

[Tips Pro:][Tip0] Model:[Tip9] [Tip12]groq/llama-3.3-70b[Tip31],
[Tip34]groq/mixtral-8x7b[Tip52]

[Tips Pro:][Tip10] Inferensi Cepat — Terbaik untuk Koding Real-Time!

### OpenRouter (100+ Model)

1. Daftar: [openrouter.ai](https://openrouter.ai)
2. Dapatkan Kunci API
3. Dashboard → Tambah Provider → OpenRouter

[Tips Pro:][Tip0] Model:[Tip9] Akses 100+ model dari semua penyedia utama
melalui kunci API tunggal.

</details>

<details>
<summary><b>💰 Cheap Providers (Backup)</b></summary>

### GLM-4.7 (Reset Harian, $0,6/1M)

1. Daftar: [Zhipu AI](https://open.bigmodel.cn/)
2. Dapatkan Kunci API dari Coding Plan
3. Petaan Dashboard → Tambah Kunci API:
   - Pembuat: `glm`
   - Kunci API: `kunci-api`

**Gunakan:** `glm/glm-4.7`

**Tips Pro:** Rencana Koding menawarkan 3× kuantitas dengan 1/7 biaya! Reset
setiap hari 10:00 AM.

### MiniMax M2.1 (5 jam reset, $0,20/1M)

1. Daftar: [MiniMax](https://www.minimax.io/)
2. Dapatkan Kunci API
3. Petaan Dashboard → Tambah Kunci API

**Gunakan:** `minimax/MiniMax-M2.1`

**Tips Pro:** Opsi termurah untuk konteks panjang (1M token)!

### Kimi K2 ($9/bulan flat)

1. Daftar: [Moonshot AI](https://platform.moonshot.ai/)
2. Dapatkan Kunci API
3. Petaan Dashboard → Tambah Kunci API

**Gunakan:** `kimi/kimi-latest`

**Tips Pro:** $9/bulan tetap untuk 10M token = $0,90/1M biaya efektif!

</details>

<details>
<summary><b>🆓 FREE Providers (Emergency Backup)</b></summary>

### iFlow (5 model gratis via OAuth)

```bash
Petaan Dashboard → Hubungkan iFlow
→ Login OAuth iFlow
→ Akses yang tidak terbatas

Model:
  if/kimi-k2-pikiran
  if/qwen3-coder-plus
  if/glm-4.7
  if/minimax-m2
  if/deepseek-r1
```

### Qwen (4 model gratis via Kode Perangkat)

```bash
Dashboard → Hub Qwen
→ Kode device autentikasi
→ Penggunaan tak terbatas

Models:
  qw/qwen3-coder-plus
  qw/qwen3-coder-flash
```

### Kiro (Claude GRATIS)

```bash
Dashboard → Hub Kiro
→ ID Pengembang AWS atau Google/GitHub
→ Penggunaan tak terbatas

Models:
  kr/claude-sonnet-4.5
  kr/claude-haiku-4.5
```

</details>

<details>
<summary><b>🎨 Create Combos</b></summary>

### Contoh 1: Maksimalkan Subskripsi → Backup Sederhana

```
Dashboard → Kombinasi → Buat Baru

Nama: pengkodean-premium
Models:
  1. cc/claude-opus-4-6 (Subskripsi utama)
  2. glm/glm-4.7 (Backup murah, $0,6/1M)
  3. minimax/MiniMax-M2.1 (Fallback termurah, $0,20/1M)

Gunakan di CLI: pengkodean-premium
```

### Contoh 2: Hanya Gratis (Tanpa Biaya)

```
Nama: kombinasi gratis
Models:
  1. gc/gemini-3-flash-preview (180K gratis/bulan)
  2. if/kimi-k2-pikiran (tak terbatas)
  3. qw/qwen3-kode-plus (tak terbatas)

Biaya: $0 selamanya!
```

</details>

<details>
<summary><b>🔧 CLI Integration</b></summary>

### IDE kursor

```
Pengaturan → Model → Lanjutan:
  URL Base API OpenAI: http://localhost:20128/v1
  Kunci API OpenAI: [dari dashborad OmniRoute]
  Model: cc/claude-opus-4-6
```

### Kode Claude

Gunakan halaman **Pembaruan CLI** di dasbor untuk pengaturan satu kali klik,
atau edit `~/.claude/settings.json` secara manual.

### CLI Codex

```bash
export URL_BASE_API_OPENAI="http://localhost:20128"
export API_KEY_OPENAI="kunci-api-omniroute-mu"

codex "promptmu"
```

### OpenClaw

**Pilihan 1 — Dasbor (direkomendasikan):**

```
Dasbor → Pembaruan CLI → OpenClaw → Pilih Model → Terapkan
```

**Pilihan 2 — Manual:** Edit `~/.openclaw/openclaw.json`:

```json
{
  "models": {
    "providers": {
      "omniroute": {
        "baseUrl": "http://127.0.0.1:20128/v1",
        "apiKey": "sk_omniroute",
        "api": "openai-completions"
      }
    }
  }
}
```

> [X0X Catatan:]** OpenClaw hanya bekerja dengan OmniRoute lokal. Gunakan
> `127.0.0.1` daripada `localhost` untuk menghindari masalah resolusi IPv6.

### Cline / Teruskan / RooCode

```
Pengaturan → Konfigurasi API:
  Provider: Kompatibel dengan OpenAI
  URL Dasar: http://localhost:20128/v1
  API Key: [dari OmniRoute dashboard]
  Model: jika/kimi-k2-pikiran
```

### OpenCode

**Langkah 1:** Tambahkan OmniRoute sebagai penyedia kustom:

```bash
opencode
/konek
# Pilih "Lainnya" → Masukan ID: "omniroute" → Masukan API Key OmniRoute Anda
```

**Langkah 2:** Buat atau edit `opencode.json` di root proyek Anda:

```json
{
  "$schema": "https://opencode.ai/config.json",
  "provider": {
    "omniroute": {
      "npm": "@ai-sdk/openai-compatible",
      "name": "OmniRoute",
      "options": {
        "baseURL": "http://localhost:20128/v1"
      },
      "models": {
        "cc/claude-sonnet-4-20250514": { "name": "Claude Sonnet 4" },
        "gg/gemini-2.5-pro": { "name": "Gemini 2.5 Pro" },
        "if/kimi-k2-pikiran": { "name": "Kimi K2 (Gratis)" }
      }
    }
  }
}
```

**Langkah 3:** Pilih model di OpenCode:

```bash
/model
# Pilih apapun model OmniRoute dari daftar
```

> **Tip:** Tambahkan model apa pun tersedia di endpoint `/v1/models` Anda
> OmniRoute ke bagian `models`. Gunakan format `provider/model-id` dari
> dashboard OmniRoute Anda.

</details>

---

## Pemecahan masalah

<details>
<summary><b>Click to expand troubleshooting guide</b></summary>

** "Model Bahasa Tidak Membagikan Pesan"**

- Kuota Penyediaan habis → Periksa tracker kuota dashboard
- Solusi: Gunakan fallback kombinasi atau beralih ke tipe yang lebih mahal

**Pemberlakuan Suara **

- Kuota langganan habis → Beralih ke GLM/MiniMax
- Tambahkan kombinasi: `cc/claude-opus-4-6 → glm/glm-4.7 → if/kimi-k2-pikiran`

**"Token Oauth Masa Aktif Habis"**

- Dicabut secara otomatis oleh OmniRoute
- Jika masalah tetap berlanjut: Dashboard → Penyedia → Rekonnect

**Biaya Tinggi**

- Cek statistik pengguna di Dashboard → Biaya
- Ubah model utama menjadi GLM/MiniMax
- Gunakan kinerja gratis (Gemini CLI, iFlow) untuk tugas yang tidak kritikal

[ X0X ]Dashboard / API Ports Tidak Benar [ X31X ]

- [ X0X ]PORT ` adalah basis port standar (dan port API default)
- [ X0X ]API_PORT ` hanya mengatasi pengiriman API yang kompatibel dengan OpenAI
- [ X0X ]DASHBOARD_PORT ` hanya mengatasi pengguna / Next.js peramban
- Atur ` NEXT_PUBLIC_BASE_URL ` ke URL public dashboard Anda (untuk panggilan
  OAuth)

[ X0X ]Kesalahan sinkronisasi awan **

- Periksa ` BASE_URL ` menunjuk ke instance yang berjalan
- Periksa ` CLOUD_URL ` menunjuk ke endpoint awan yang diharapkan
- Tetapkan ` NEXT_PUBLIC_* ` nilai sesuai dengan nilai server

[ X0X ]Login pertama tidak berhasil **

- Periksa ` INITIAL_PASSWORD ` di `. env [ X33X ]
- Jika tidak ada, password default adalah ` 123456 `

[ X0X ]Tidak ada log permintaan **

- Atur ` ENABLE_REQUEST_LOGS=true ` di `. env [ X39X ]

[ X0X ]Uji koneksi menunjukkan "Invalid" untuk penyedia OpenAI yang kompatibel
**

- Banyak penyedia tidak mengekspos endpoint ` / models `
- OmniRoute v1.0.6+ mencakup validasi fallback melalui kelanjutan obrolan
- Pastikan URL dasar termasuk `/v1` suffix

### 🔐 OAuth di Server Jarak Jauh

<a name="oauth-on-a-remote-server"></a> <a name="oauth-em-servidor-remoto"></a>

> **⚠️ Penting untuk pengguna yang menjalankan OmniRoute di VPS, Docker, atau
> server jarak jauh**

#### Mengapa CLI OAuth Antigravity / Gemini gagal di server online?

Pemberi **Antigravity** dan **Gemini CLI** menggunakan **OAuth Google 2.0**.
Google memerlukan `redirect_uri` dalam aliran OAuth untuk sesuai persis dengan
salah satu URI yang sudah terdaftar dalam konsol Google Cloud.

Kredensial OAuth yang dibundel dalam OmniRoute sudah terdaftar **hanya untuk
`localhost`**. Saat Anda mengakses OmniRoute di server jarak jauh (misal
`https://omniroute.myserver.com`), Google menolak autentikasi dengan:

```
Error 400: redirect_uri_mismatch
```

#### Solusi: Konfigurasi kredensial OAuth sendiri

Anda membutuhkan **Klien ID OAuth 2.0** di konsol Google Cloud dengan URI server
Anda.

#### Langkah demi langkah

**1. Buka konsol Google Cloud**

Klik:
[https://console.cloud.google.com/apis/credentials](https://console.cloud.google.com/apis/credentials)

**2. Buat Klien ID OAuth 2.0 baru**

- Klik **"+" Buat Kredensial"** → **"Klien ID OAuth"**
- Tipe aplikasi: **"Aplikasi web"**
- Nama: apa saja yang Anda sukai (misal `OmniRoute Jarak Jauh`)

**3. Tambahkan URI Otorisasi Redirect**

Di bidang **"URI Otorisasi Redirect"**, tambahkan:

```
https://server-pribadi.co.id/callback
```

> Ganti `server-pribadi.co.id` dengan domain atau IP server Anda (termasuk port
> jika diperlukan, contoh `http://45.33.32.156:20128/callback`).

**4. Simpan dan salin kredential**

Setelah membuat, Google akan menampilkan **ID Klien** dan **Rahasia Klien**.

**5. Setel variabel lingkungan**

Pada file `.env` (atau variabel lingkungan Docker):

```bash
# Untuk Antigravity:
ANTIGRAVITY_OAUTH_CLIENT_ID=your-client-id.apps.googleusercontent.com
ANTIGRAVITY_OAUTH_CLIENT_SECRET=GOCSPX-your-secret

# Untuk Gemini CLI:
GEMINI_OAUTH_CLIENT_ID=your-client-id.apps.googleusercontent.com
GEMINI_OAUTH_CLIENT_SECRET=GOCSPX-your-secret
GEMINI_CLI_OAUTH_CLIENT_SECRET=GOCSPX-your-secret
```

**6. Mulai ulang OmniRoute**

```bash
# npm:
npm run dev

# Docker:
docker restart omniroute
```

**7. Coba terhubung lagi**

Dashboard → Provedor → Antigravity (atau Gemini CLI) → OAuth

Google akan dialihkan dengan benar ke `https://your-server.com/callback`.

---

#### Kerja sementara (tanpa kredential kustom)

Jika Anda tidak ingin mengatur kredential sendiri sekarang, Anda masih dapat
menggunakan **aliran URL manual**:

1. OmniRoute membuka URL autorisasi Google
2. Setelah mensetujui, Google mencoba dialihkan ke `localhost` (yang gagal pada
   server jarak jauh)
3. **Salin URL penuh** dari alamat URL browser Anda (bahkan jika halaman tidak
   dimuat)
4. Salin URL itu ke bidang yang ditunjukkan di model koneksi OmniRoute
5. Klik **"Hubungkan"**

> Hal ini berhasil karena kode otorisasi di URL masih valid tidak peduli halaman
> pemindahan dimuat atau tidak.

---

<details>
<summary><b>🇧🇷 Versão em Português</b></summary>

#### Mengapa OAuth dari Antigravity / Gemini CLI gagal di server jarak jauh?

Provedor **Antigravity** dan **Gemini CLI** menggunakan **OAuth 2.0 Google**
untuk autentikasi. Google mengharuskan `redirect_uri` digunakan pada aliran
OAuth adalah **satu kemungkinan** yang sudah terdaftar di Google Cloud Console
dari aplikasi tersebut.

As kreditensi OAuth terintegrasi di OmniRoute hanya untuk `localhost`** saja.
Ketika Anda mengakses OmniRoute di server jarak jauh (contoh:
`https://omniroute.meuservidor.com`), Google menolak autentifikasi dengan:

```
Error 400: redirect_uri_mismatch
```

#### Solusi: Konfigurasi kreditensi OAuth Anda sendiri

Anda butuh membuat **OAuth 2.0 Client ID** di Google Cloud Console dengan URI
server Anda.

#### Langkah-Langkah

**1. Akses Google Cloud Console**

Buka:
[https://console.cloud.google.com/apis/credentials](https://console.cloud.google.com/apis/credentials)

**2. Buat kreditensi OAuth 2.0 Client ID**

- Klik **"+" Buat Kreditensi Baru"** → **"OAuth client ID"**
- Tipe aplikasi: **"Aplikasi Web"**
- Nama: Pilih nama apa saja (contoh: `OmniRoute Jarak Jauh`)

**3. Tambahkan Redirect URIs yang Diperbolehkan**

Di kolom **"Redirect URIs yang Diperbolehkan"**, tambahkan:

```
https://seu-servidor.com/callback
```

> Ganti `seu-servidor.com` dengan nama domain atau alamat IP server Anda
> (termasuk metode port jika diperlukan, contoh:
> `http://45.33.32.156:20128/callback`).

**4. Simpan dan Salin kreditensi**

Setelah membuat, Google akan menampilkan **Klient ID** dan **Rahasia Klient**.

**5. Konfigurasi Variabel Lingkungan**

Pada `your.env` (atau variabel lingkungan Docker):

```bash
# Untuk Antigravity:
ANTIGRAVITY_OAUTH_CLIENT_ID=seu-client-id.apps.googleusercontent.com
ANTIGRAVITY_OAUTH_CLIENT_SECRET=GOCSPX-seu-secret

# Untuk Gemini CLI:
GEMINI_OAUTH_CLIENT_ID=seu-client-id.apps.googleusercontent.com
GEMINI_OAUTH_CLIENT_SECRET=GOCSPX-seu-secret
GEMINI_CLI_OAUTH_CLIENT_SECRET=GOCSPX-seu-secret
```

**6. Mulai ulang OmniRoute**

```bash
# Jika menggunakan npm:
npm run dev

# Jika menggunakan Docker:
docker restart omniroute
```

**7. Coba hubungi lagi**

Dashboard → Provider → Antigravity (atau Gemini CLI) → OAuth

Sekarang Google akan mengarah pada `https://server-mu.com/callback` dengan benar
dan autentikasi akan berfungsi.

---

#### Kerja sementara (tidak mengkonfigurasi kredit sendiri)

Jika Anda tidak ingin membuat kredit sendiri sekarang, masih memungkinkan
menggunakan aliran **manual URL**:

1. OmniRoute akan membuka URL otorisasi Google
2. Setelah Anda mengotorisasi, Google akan mencoba mengarah pada
   `localhost[/X66X] (yang gagal pada server jauh)
3. **Salin URL lengkap** dari alamat URL browser (baik URL berhasil di buka atau
   tidak)
4. Tulis URL tersebut ke dalam bidang yang muncul di modal koneksi OmniRoute
5. Klik **"Connect"[/X21X]

> Bantuan kerja ini efektif karena kode otorisasi di dalam URL masih valid
> meskipun pengalihan gagal di tangani.

</details>

---

</details>

## 🛠️ Pustaka

<details>
<summary><b>Click to expand tech stack details</b></summary>

- **Runtime**: Node.js 18-22 LTS (⚠️ Node.js 24+ tidak **tidak didukung** — kode
  Native Binaries dari sqlite3 bukan kompatibel)
- **Bahasa**: TypeScript 5.9 — **100% TypeScript** di atas `src/` dan `open-ss/`
  (Zero `any` core modules sejak v 2.0)
- **Fasililtas**: Next.js 16 + React 19 + Tailwind CSS 4
- **Database**: LowDB (JSON) + SQLite (domain state + prosesi log + audit audit
  MCP + keputusan routing)
- **Schemas**: Zod (MCP Alat I/O Validasi, Kontrak API)
- **Protokol**: MCP (stdio / HTTP) + A2A v0.3 (JSON-RPC 2.0 + SSE)
- **Streaming**: Streaming Servis (SSE)
- **Auth**: Oauth 2.0 (PKCE) + JWT + Kunci API + Otorisasi Scoped MCP
- **Testing**: Pengujian Node.js + Vitest (900+ pengujian termasuk unit,
  integrasi, E2E)
- **CI/CD**: Aksi GitHub (otentikasi otomatis npm publish + Docker Hub pada
  rilis)
- **Website**: [omniroute.online](https://omniroute.online)
- **Package**:
  [npmjs.com/package/omniroute](https://www.npmjs.com/package/omniroute)
- **Docker**:
  [hub.docker.com/r/diegosouzapw/omniroute](https://hub.docker.com/r/diegosouzapw/omniroute)
- **Resilience**: Pembatas lingkaran, backoff eksponensial, anti-gangguan lalu,
  palsu TLS, auto-combo peawasan diri

</details>

---

## Dokumentasi

| Dokumentasi                                            | Pengenalan                                                        |
| ------------------------------------------------------ | ----------------------------------------------------------------- |
| [Panduan Pengguna](docs/USER_GUIDE.md)                 | Ekstensi penyedia, kombasi, integrasi CLI, implementasi           |
| [Referensi API](docs/API_REFERENCE.md)                 | Semua endpoint dengan contoh                                      |
| [Pengaturan Server MCP](open-sse/mcp-server/README.md) | 16 alat MCP, pengaturan IDE, klien Python/TS/Go                   |
| [Pengaturan Server A2A](src/lib/a2a/README.md)         | Protokol JSON-RPC 2.0, keterampilan, streaming, pengelolaan tugas |
| [Evaluasi Oto-Akombasi](docs/auto-combo.md)            | 6-Faktor Skoring, paket mode, self-healing                        |
| [Troubleshooting](docs/TROUBLESHOOTING.md)             | Masalah umum dan solusi                                           |
| [Arsitektur](docs/ARCHITECTURE.md)                     | Arsitektur sistem dan bagian dalam                                |
| [Contributing](CONTRIBUTING.md)                        | Pengaturan pengembangan dan pedoman                               |
| [OpenAPI Spec](docs/openapi.yaml)                      | Spesifikasi OpenAPI 3.0                                           |
| [Security Policy](SECURITY.md)                         | Laporan keamanan dan praktik keamanan                             |
| [VM Deployment](docs/VM_DEPLOYMENT_GUIDE.md)           | Petunjuk lengkap: setting VM + nginx + Cloudflare                 |
| [Galeri Fitur](docs/FEATURES.md)                       | Tur dashboard visual dengan screenshot                            |
| [Tangga Rilis](docs/RELEASE_CHECKLIST.md)              | Langkah-langkah validasi pra-rilis                                |

---

## 🗺️ Rencana Strategis

OmniRoute memiliki **210+ fitur yang direncanakan** di berbagai fase
pengembangan. Berikut adalah area utama:

| Kategori                     | Fitur yang Sudah Dibuat | Kemunculan Utama                                                                                                                |
| ---------------------------- | ----------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| 🧠 **Rute & Intelektualitas** | 25+                     | Routing Rute dengan Latensi Terendah, Penyortiran Berdasarkan Label, Persunting Kuantitas Sebelum Pengujian, Pemilihan Akun P2C |
| 🔒 **Keamanan & Keselarasan** | 20+                     | Pengaktifan Hardening SSRF, Penggabungan Kredensial Penuh, Pengendalian Laju per Endpoint, Pengurutan Kunci Manajemen           |
| 📊 **Tampak Kegiatan**        | 15+                     | Pengintegrasian OpenTelemetry, Pengawasan Kuantitas Sempurna dalam Waktu Nyata, Pengukuran Biaya per Model                      |
| 🔄 **Integrasi Pemasok**      | 20+                     | Registry Model Dinamis, Pengendalian Pemasok, Codex Akun Multi, Pengolahan Kuantitas Copilot                                    |
| ⚡ **Performa**               | 15+                     | Lapisan Cache Ganda, Pengolahan Cache Prompt, Pengolahan Cache Respons, Streaming Sambungan Aktif, API Bersama                  |
| 🌐 **Komunitas**              | 10+                     | API WebSocket, Pengeload Konfigurasi Skenario, Penyimpanan Konfigurasi Terdistribusi, Mode Komersial                            |

### 🔜 Segera Hadir

- 🔗 **Integrasi OpenCode** — Penyokong Pemasok Asli untuk IDE Coding AI OpenCode
- 🔗 **INTEGRASI TRAE** — Pendukung lengkap untuk kerangka pengembangan AI TRAE
- 📦 **API BATCH** — Proses batch asyncronus untuk permintaan bulk
- 🎯 **Rute Berdasarkan Tag** — Jalankan permintaan berdasarkan tag dan metadata
  kustom
- 💰 **Strategi Biaya Terendah** — Pilih otomatis penyedia tersedia yang termurah

> 📝 Spesifikasi fitur lengkap tersedia di
> [`docs/baru-fitur/`](docs/new-features/) (217 spesifikasi terperinci)

---

## 👥 Kontributor

[![Kontributor](https://contrib.rocks/image?repo=diegosouzapw/OmniRoute&max=100&columns=20&anon=1)](https://github.com/diegosouzapw/OmniRoute/graphs/contributors)

### Bagaimana Berkontribusi

1. Fork repositori
2. Buat cabang fitur (`git checkout -b feature/amazing-feature`)
3. Komit perubahanmu (`git commit -m 'Tambah fitur luar biasa'`)
4. Tampilkan ke cabang (`git push origin feature/amazing-feature`)
5. Buat Permintaan Gabung

Lihat [[CONTRIBUTING.md](CONTRIBUTING.md)] untuk pedoman terperinci

### Menerbitkan Versi Baru

```bash
# Buat menerbitkan — terbit otomatis dengan npm
gh rilis buat v2.0.0 --judul "v2.0.0" --generate-notes
```

---

## 📊 Sejarah Bintang

## Bintang perlahan

## [![Bintang perlahan](https://starchart.cc/diegosouzapw/OmniRoute.svg?variant=adaptive)](https://starchart.cc/diegosouzapw/OmniRoute)

## 🙏 Penghargaan

Terima kasih kepada **[CLIProxyAPI](https://github.com/decolua/9router)[X36X] —
implementasi asli Go yang menginspirasi port JavaScript ini.

Special thanks to
**[9router](https://github.com/router-for-me/CLIProxyAPI)[X32X] by
[X38X][decolua]{2}[X52X] — proyek asli yang menginspirasi perambahan ini.
OmniRoute membangun pada foundation luar biasa ini dengan fitur tambahan, API
multy-modal, dan tama-rewrite dalam TypeScript.

---

## 📄 Lisensi

Lisensi MIT — lihat [LICENSE](LICENSE) untuk detail.

---

<div align="center">
  <sub>Built with ❤️ for developers who code 24/7</sub>
  <br/>
  <sub><a href="https://omniroute.online">omniroute.online</a></sub>
</div>
<!-- GitHub Discussions enabled for community Q&A -->
