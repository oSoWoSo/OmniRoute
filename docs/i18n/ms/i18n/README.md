# 🚀 OmniRoute — The Free AI Gateway

### Bermula mencodai. Laluan pintas cerdas ke model AI percuma ** dan mesra kos yang automatik dengan pemulihan semula jadi.

_Pintas API universal anda — satu endpoint, 67+ penyedia, tanpa gangguan.
Sekarang dengan **MCP & A2A** pemarkur anjakan agent.

**Penyelesaian Chat • Embeddings • Penerbangan Gambar • Video • Muzik • Audio •
Penambahan Semula • **Pencarian Web** • Pelayan MCP • Protokol A2A • 100%
TypeScript**

---

<div align="center">

[![npm
version](https://img.shields.io/npm/v/omniroute?color=cb3837&logo=npm)](https://www.npmjs.com/package/omniroute)
[![npm
downloads](https://img.shields.io/npm/dm/omniroute?color=cb3837&logo=npm&label=npm%20downloads)](https://www.npmjs.com/package/omniroute)
[![Docker
Hub](https://img.shields.io/docker/v/diegosouzapw/omniroute?label=Docker%20Hub&logo=docker&color=2496ED)](https://hub.docker.com/r/diegosouzapw/omniroute)
[![Docker
Pulls](https://img.shields.io/docker/pulls/diegosouzapw/omniroute?logo=docker&color=2496ED&label=docker%20pulls)](https://hub.docker.com/r/diegosouzapw/omniroute)
[![Lisensi](https://img.shields.io/github/license/diegosouzapw/OmniRoute)](https://github.com/diegosouzapw/OmniRoute/blob/main/LICENSE)
[![Laman
Web](https://img.shields.io/badge/Website-omniroute.online-blue?logo=google-chrome&logoColor=white)](https://omniroute.online)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-Community-25D366?logo=whatsapp&logoColor=white)](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

[🌐 Laman Web](https://omniroute.online) • [🚀 Mulakan Cepat](#-quick-start) • [💡
Ciri-ciri](#-key-features) • [📖 Dokumen](#-documentation) • [💰
Harga](#-pricing-at-a-glance) • [💬
WhatsApp](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

</div>

🌐 **Tersedia dalam:** 🇺🇸 [Inggeris](README.md) | 🇧🇷 [Portugis
(Brazillia)](docs/i18n/pt-BR/README.md) | 🇪🇸 [Sepanyol](docs/i18n/es/README.md)
| 🇫🇷 [Perancis](docs/i18n/fr/README.md) | 🇮🇹 [Itali](docs/i18n/it/README.md) |
🇷🇺 [Rusia](docs/i18n/ru/README.md) | 🇨🇳 [Cina
(Sederhana)](docs/i18n/zh-CN/README.md) | 🇩🇪 [Jerman](docs/i18n/de/README.md) |
🇮🇳 [Hindi](docs/i18n/in/README.md) | 🇹🇭 [Thai](docs/i18n/th/README.md) | 🇺🇦
[Ukraine](docs/i18n/uk-UA/README.md) | 🇸🇦 [Arab](docs/i18n/ar/README.md) | 🇯🇵
[Jepun](docs/i18n/ja/README.md) | 🇻🇳 [Vietnam](docs/i18n/vi/README.md) | 🇧🇬
[Bulgaria](docs/i18n/bg/README.md) | 🇩🇰 [Denmark](docs/i18n/da/README.md) | 🇫🇮
[Finland](docs/i18n/fi/README.md) | 🇮🇱 [Ibrani](docs/i18n/he/README.md) | 🇭🇺
[Hungary](docs/i18n/hu/README.md) | 🇮🇩 [Indonesia](docs/i18n/id/README.md) | 🇰🇷
[Korea](docs/i18n/ko/README.md) | 🇲🇾 [Bahasa Melayu](docs/i18n/ms/README.md) |
🇳🇱 [Belanda](docs/i18n/nl/README.md) | 🇳🇴 [Norway](docs/i18n/no/README.md) | 🇵🇹
[Portugis (Portugal)](docs/i18n/pt/README.md) | 🇷🇴
[Romania](docs/i18n/ro/README.md) | 🇵🇱 [Perancis](docs/i18n/pl/README.md) | 🇸🇰
[Slovak](docs/i18n/sk/README.md) | 🇸🇪 [Sweden](docs/i18n/sv/README.md) | 🇵🇭
[Filipino](docs/i18n/phi/README.md) | 🇨🇿 [Czech](docs/i18n/cs/README.md)

---

## 🆕 Apa Yang Baru Dalam v3.0.0

> **Bagaimana untuk Menaikkan dari v2.9.5?** - Lihat [full
> CHANGELOG](CHANGELOG.md#300--2026-03-22-release-candidate--not-yet-merged-to-main)
> untuk semua perubahan.

| Sektor                      | Perubahan                                                                                                                                                              |
| --------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🔒 **Keselamatan CodeQL**    | Diperbaiki 10+ Notis Keselamatan CodeQL: polinom-redos, ketidakpastian rawak, pemulihan injeksyen tapak                                                                |
| ✅ **Sahkan Laluan**         | Semua 176 laluan API kini sah dengan skema Zod + `validateBody()` — CI `check:route-validation:t06` berjaya                                                            |
| 🐛 **OmniModel Tag Tergiur** | Sulit `<omnimodel>` tag tidak lagi teriakan ke klien dalam respon streaming SSE (#585)</omnimodel>                                                                     |
| 🔑 **API Kunci Terdaftar**   | Auto-provisi API kunci melalui `POST /api/v1/registered-keys` dengan kuota per-penyedia/pengguna, idempotensi, penyimpanan SHA-256, dan melaporkan isu GitHub opsional |
| 🎨 **Ikon Penyedia**         | 130+ provider logos via `@lobehub/icons` (SVG) with PNG → generic fallback chain                                                                                       |
| 🔄 **Model Auto-Sync**       | 24h scheduler and manual UI toggle to sync model lists for built-in and custom OpenAI-compatible providers                                                             |
| 🌐 **OpenCode Zen/Go**       | Two new providers from @kang-heewon via PR #530: free tier + subscription tier via `OpencodeExecutor`                                                                  |
| 🐛 **Gemini CLI OAuth**      | Actionable error when `GEMINI_OAUTH_CLIENT_SECRET` is missing in Docker (was cryptic Google error)                                                                     |
| 🐛 **OpenCode config**       | `saveOpenCodeConfig()` now correctly writes TOML to `XDG_CONFIG_HOME`                                                                                                  |
| 🐛 **Pinned model override** | `body.model` correctly set to `pinnedModel` on context-cache protection                                                                                                |
| 🐛 **Codex/Claude loop**     | `tool_result` blocks now converted to text to stop infinite loops                                                                                                      |
| 🐛 **Login redirect**        | Login no longer freezes after skipping password setup                                                                                                                  |
| 🐛 **Windows paths**         | MSYS2/Git-Bash paths (`/c/...`) normalized to `C:\...` automatically                                                                                                   |

---

## 🖼️ Main Dashboard

<div align="center">
  <img src="./docs/screenshots/MainOmniRoute.png" alt="OmniRoute Dashboard" width="800"/>
</div>

---

## 📸 Dashboard Preview

<details>
<summary><b>Click to see dashboard screenshots</b></summary>

| Page                  | Kecerahan Skrin                                    |
| --------------------- | -------------------------------------------------- |
| [P0X]Pembekal**       | ![Pembekal](docs/screenshots/01-providers.png)     |
| [P0X]Kombo**          | ![Kombo](docs/screenshots/02-combos.png)           |
| [P0X]Analisis**       | ![Analisis](docs/screenshots/03-analytics.png)     |
| [P0X] Kesihatan**     | ![Kesihatan](docs/screenshots/04-health.png)       |
| [P0X]Terjemahan**     | ![Terjemahan](docs/screenshots/05-translator.png)  |
| [P0X]Pengawalan**     | ![Pengawalan](docs/screenshots/06-settings.png)    |
| [P0X]Alat CLI**       | ![Alat CLI](docs/screenshots/07-cli-tools.png)     |
| [P0X]Log Penggunaan** | ![Log Penggunaan](docs/screenshots/08-usage.png)   |
| [P0X]Kad Endpoints**  | ![Kad Endpoints](docs/screenshots/09-endpoint.png) |

</details>

---

### Robot AI Percuma untuk Pembekal yang disukai AgentCoding Anda

_Hubungi mana-mana alat IDE atau CLI berkuasa AI melalui OmniRoute — jambatan
API percuma untuk pemrograman tanpa had._

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

<sub>📡 Semua agen menghubungi melalui <code>http://localhost:20128/v1</code>
atau <code>http://cloud.omniroute.online/v1</code> — satu pengaturan, model
tidak terbatas dan kuota</sub>

---

## 🤔 Mengapa OmniRoute?

**Jangan buang-buang wang dan kehabisan had:**

- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Kuota sambungan mengakhiri setiap bulan tanpa digunakan
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Had sambungan menghentikan di pertengahan kod
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  API mahal ($20-50/bulan per penyedia)
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Pengalihan tangan oleh pengguna

**OmniRoute menyelesaikan masalah ini:**

- ✅ **Maksimalkan sambungan** - Kaji kuota, gunakan setiap kaitan sebelum reset
- ✅ **Pengalihan automatik** - Sambungan → Kunci API → Murah → Percuma, tiada
  gangguan
- ✅ **Sambungan berganda** - Saling-salir antara akaun per penyedia
- ✅ **Universal** - Berfungsi dengan Claude Code, Codex, Gemini CLI, Cursor,
  Cline, OpenClaw, mana-mana alat CLI

---

## 📧 Sokongan

> 💬 **Sertai komuniti kami!** [Kumpulan
> WhatsApp](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t) —
> Dapatkan bantuan, berbagi tips, dan berjalan dengan kini.

- **Tapak web**: [omniroute.online](https://omniroute.online)
- **GitHub**:
  [github.com/diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute)
- **Isu**:
  [github.com/diegosouzapw/OmniRoute/issues](https://github.com/diegosouzapw/OmniRoute/issues)
- **WhatsApp**: [Kumpulan
  Komuniti](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)
- **Berkhidmat**: Lihat [PERANAN MEREKA YANG BERKHIDMAT.md](CONTRIBUTING.md),
  buka PR, atau pilih `isu pertama yang bagus`
- **Projek Asal**: [9rouser oleh decolua](https://github.com/decolua/9router)

### Apakah Pelaporan Bug Wajib?

Apabila membuka isu, sila jalankan arahan system-info dan lampirkan fail yang
dihasilkan:

```bash
npm run system-info
```

Fail semacam `system-info.txt` yang mengandungi versi Node.js, versi OmniRoute,
butiran sistem, alat CLI yang dipasang (iflow, gemini, claude, codex,
antigravity, droid, dsb.), status Docker/PM2, dan paip sistem -- sepertimana
kami perlukan untuk mengulangi isu tersebut dengan cepat. Lampirkan fail secara
langsung ke isu GitHub anda.

---

## Bagaimana Ia Berfungsi

```
┌─────────────┐
│  Alat CLI   │  (Claude Code, Codex, Gemini CLI, OpenClaw, Cursor, Cline...)
│   Tool      │
└──────┬──────┘
       │ http://localhost:20128/v1
       ↓
┌─────────────────────────────────────────┐
│           OmniRoute (Penghantar Cerdik)        │
│  • Pemindahkan format translation (OpenAI ↔ Claude) │
│  • Menjejaki kuota + Embeddings + Images │
│  • Auto pemulihan token                    │
└──────┬──────────────────────────────────┘
       │
       ├─→ [Tier  1: PREMIUM] Claude Code, Codex, Gemini CLI
       │   ↓ kuota habis
       ├─→ [Tier  2: API KEY] DeepSeek, Groq, xAI, Mistral, NVIDIA NIM, dsb.
       │   ↓ hadiah hadiah anggaran
       ├─→ [Tier  3: MAHSUL] GLM ($0.6/1M), MiniMax ($0.2/1M)
       │   ↓ hadiah anggaran
       └─→ [Tier  4: TELUSUR] iFlow, Qwen, Kiro (tidak terhad)

Hasil: Tiada henti coding, kos minimal
```

---

## 🎯 Apa itu Omniroute Selesaikan – 30 Masalah Nyata & Kes Pemakaian

> **Setiap pembangun menggunakan alat AI menghadapi masalah-masalah ini setiap
> hari.** OmniRoute dibina untuk menyelesaikannya – dari perbelanjaan melebihi
> had dan gangguan zon ke aliran OAuth pecah dan operasi pemantauan perniagaan.

<details>
<summary><b>💸 1. "I pay for an expensive subscription but still get interrupted by limits"</b></summary>

Pembangun membayar $20–200/bulan untuk Claude Pro, Codex Pro, atau GitHub
Copilot. Sama pun pembelian, kuota mempunyai had – 5 jam penggunaan, had
mingguan, atau had kadar minit. Hujung sesi kod, pembekal berhenti berfungsi dan
pembangun kehilangan proses dan produktif.

**Bagaimana OmniRoute menyelesaikannya:**

- **Penggantian Kuota Cerdik** — Sekiranya kuota pembelian habis, secara
  automatik redarah ke API Key → Mahsul → Telusur tanpa intervensi tangan
- **Menjejaki Kuota Sepenuh Masa** — Menunjukkan penggunaan token dalam masa
  nyata dengan hitung mundur pemulihan (5 jam, harian, mingguan)
- **Dukung Akun Banyak** — Banyak akun per provider dengan sambungan roti putih
  otomatik – Apabila satu habis, pindah ke yang seterusnya
- **Pilihan Kombinasi** — Pilihan rangkaian sambungan khas dengan 6 strategi
  keseimbangan (penuh terlebih dahulu, sambungan roti putih otomatik, P2C, acak,
  yang paling kurang dilihat, yang paling ekonomi)
- **Akses Kuota Perniagaan** — Pengawasan kuota paksi perniagaan/dewan
  perniagaan langsung di papan pengurus

</details>

<details>
<summary><b>🔌 2. "I need to use multiple providers but each has a different API"</b></summary>

OpenAI menggunakan format yang lain, Claude (Anthropic) menggunakan format yang
berlainan, Gemini pula menggunakan format yang berlainan. Sekiranya sesama
pembangun ingin mengetes model dari provider yang berbeza atau balik hubung
antara mereka, mereka perlu rekonfigurasi SDK, menukar endpoint, menghadapi
format yang tidak bersesuaian. Provider khas (FriendLI, NIM) mempunyai model
endpoint tidak standard.

**Bagaimana OmniRoute menyelesaikannya:**

- **Penghantaran Endpoints** — Pelayan tunggal `http://localhost:20128/v1`
  digunakan sebagai proxy untuk semua 67+ provider
- **Pekerjaan Format** — Otomatik dan transparan: OpenAI ↔ Claude ↔ Gemini ↔
  Pelayan API
- Pembersihan Respons — Menghilangkan bidang yang tidak standard (`x_groq`,
  `usage_breakdown`, `service_tier`) yang mengganggu SDK OpenAI v1.83 +
- Normalisasi Peranan — Mengubah `developer` → `system` untuk penyedia
  non-OpenAI; `system` → `user` untuk GLM/ERNIE
- Pemulangan Tag Berpikir — Mengambil `<think>` blok dari model seperti DeepSeek
  R1 ke `reasoning_content` yang di standardisasi</think>
- Keluaran Terstruktur untuk Gemini — `json_schema` →
  `responseMimeType`/`responseSchema` konversi automatik
- `stream` bawaan adalah `false` — Menekan dengan spesifikasi OpenAI, mengelakan
  SSE yang tidak diharapkan di SDK Python/Rust/Go

</details>

<details>
<summary><b>🌐 3. "My AI provider blocks my region/country"</b></summary>

Penyedia seperti OpenAI/Codex menghalangi akses dari beberapa wilayah geografik.
Pengguna akan mendapatkan kesalahan seperti
`unsupported_country_region_territory` semasa koneksi OAuth dan API. Ini sangat
menjengkelkan bagi pengembang dari negara berkembang.

**Bagaimana OmniRoute menyelesaikannya:**

- Konfigurasi Proksi 3-Tingkat** — Proksi pada 3 tahap: global (seluruh lalu
  lintas), per-penyedia (satu penyedia saja) dan per-koneksi/kunci
- Tanda Proxy yang Berwarna** — Indikator visual: 🟢 proksi global, 🟡 proksi
  penyedia, 🔵 proksi koneksi, menampilkan IP selalu
- Tukar Token Oauth Lewat Proksi** — Aliran oauth juga melewati proksi,
  mengatasi `unsupported_country_region_territory`
- Uji Koneksi Lewat Proksi** — Pengujian koneksi menggunakan proksi yang
  dikonfigurasi (tidak ada lagi lepaskan langsung)
- Dukungan SOCKS5** — Dukungan khusus proksi SOCKS5 untuk pengalihan keluar
- Palsu Print Fingerprint TLS** — Membayangkan prinsipan browser-like TLS
  menggunakan `wreq-js` untuk mengelak deteksi bot
- Mengikuti Jejak Fingerprint CLI** — Mengatur semula kepala dan bidang tubuh
  untuk membentuk tanda tangan alami CLI asli, memperkecil risiko tindakan
  pengakuan\
  Proksi IP dipertahankan. Anda mendapatkan keselamatan ** dan ** bersamaan.

</details>

<details>
<summary><b>🆓 4. "I want to use AI for coding but I have no money"</b></summary>

Siapa yang mampu membayar $20–200/bulan untuk langganan AI? Mahasiswa,
pengembang dari negara berkembang, penggemar, dan freelancer memerlukan akses ke
model berkualitas tanpa biaya.

**Bagaimana OmniRoute menyelesaikannya:**

- Penyedia Tier Bawaan yang Bebas** — Dukungan asli 100% tanpa biaya: iFlow (5
  model tanpa batas melalui OAuth: kimi-k2-thinking, qwen3-coder-plus,
  deepseek-r1, minimax-m2, kimi-k2), Qwen (4 model tanpa batas:
  qwen3-coder-plus, qwen3-coder-flash, qwen3-coder-next, vision-model), Kiro
  (Claude + ID Pembina AWS untuk bebas), Gemini CLI (180K token/bulan bebas)
- Ollama Cloud** — Ollama yang dihoskan di awan di `api.ollama.com` dengan tier
  "Light usage" bebas; gunakan prefix `ollamacloud/<model>`</model>
- Paduan Bebas Hanya** — Cabut `gc/gemini-3-flash → if/kimi-k2-thinking →
  qw/qwen3-coder-plus` = $0/bulan dengan tanpa gangguan
- Akses NIM NVIDIA Bebas** — ~40 RPM akses foren dev-bebas untuk 70+ model di
  build.nvidia.com (mengalihkan dari kredit ke batasan tingkat)
- Pesan Optimitasi Kos Biayadan Strategi — Strategi pelayaran yang secara
  automatik memilih penyedia paling murah yang tersedia

</details>

<details>
<summary><b>🔒 5. "I need to protect my AI gateway from unauthorized access"</b></summary>

Ketika menghadirkan pintu gerbang AI ke jaringan (LAN, VPS, Docker), siapa saja
yang memiliki alamat dapat mengonsumsi token/potongan khas para pengembang,
tanpa perlindungan, APIs rentan terhadap pemakaian yang tidak sah, injeksi
prompt, dan penggunaan.

**Bagaimana OmniRoute menyelesaikannya:**

- Pengurusan Kunci API — Pembuatan, rotasi, dan pembatasan per penyedia dengan
  halaman dashboard/api-manager khusus
- Keselarasan Pada Madunya — Menghalangi kunci API untuk model tertentu
  ([openai/*, pola pola wildcard], pola toggle Buat Semua/Haluskan
- Pelelangan Posisi Endpoint API — Memerlukan kunci untuk /v1/models dan
  melarang penyedia tertentu dari daftar
- Kurap Penggunaan + Perlindungan CSRF — Semua ulasan dashboard dilindungi
  dengan middleware + token CSRF
- Pembatasan Indera — Pembatasan IP per Indera dengan jendela Konfigurasi
- Pemfilter IP — Daftar putih atau hitam untuk kontrol akses
- Kurap Penginjeksian Prompt — Sanitasi terhadap pola penginjeksian prompt yang
  berbahaya
- Enkripsi AES-256-GCM — Kredensial dienkripsi pada medan istirahat

</details>

<details>
<summary><b>🛑 6. "My provider went down and I lost my coding flow"</b></summary>

Penyedia AI dapat mengekspose instabil, meraih 5xx kesalahan, atau mengenai
pembatasan beban sementara. Jika seorang dev mengergantung pada penyedia
tunggal, mereka diinterupsi. Tanpa pembatas penggantung, retakan berulang dapat
menjatuhkan aplikasi.

**Bagaimana OmniRoute menyelesaikannya:**

- Penggantung Pintasan per-model — Membuka/Tutup secara otomatis dengan
  pengaturan ambang batas dan pendingin (Tutup/Tergantung/Tiga-Setengah Tutup)
- Pembalikan Exponensial — Postifensi penundaan reaksi yang berlapis
- Anti-Azakan Keroncong — Pelindungan mutex + kunci semafora terhadap badai
  reaksi berulang
- Pintasan Penggabungan — Jika penyedia utama gagal, secara otomatis gagal
  melalui rantai dengan tidak memerlukan bantuan
- Pintasan Penggantung Berpasangan — Membuka kunci penyedia berjalan gagal dalam
  rantai kombinasi
- Dashboard Kesadaran Kesehatan — Menjaga kesehatan, keadaan pembatas perangkat
  penggantung, pengeblok, statistik cache, latency p50/p95/p99

</details>

<details>
<summary><b>🔧 7. "Configuring each AI tool is tedious and repetitive"</b></summary>

Para pengembang menggunakan Cursor, Claude Code, Kode Codex CLI, OpenClaw,
Gemini CLI, Kilo Code... Setiap alat memerlukan konfigurasi yang berbeda (posisi
endpoint API, kunci, model)\
==WEBLATE_PART==

**Bagaimana OmniRoute menyelesaikannya:**

- **Papan Pelayanan CLI** — Mukaan dedikasi dengan setup satu-tik untuk Claude
  Code, Codex CLI, OpenClaw, Kilo Code, Antigravity, Cline
- **Pengguna Copilot GitHub Config Generator** — Menghasilkan
  `chatLanguageModels.json` untuk VS Code dengan pemilihan model dalam jumlah
  banyak
- **Pengguna Pemandu Pelajar** — Setup 4 langkah yang disarankan untuk pengguna
  baru
- **Satu endpoint, semua model** — Tugas `http://localhost:20128/v1` sekali,
  akses penyedia 67+

</details>

<details>
<summary><b>🔑 8. "Managing OAuth tokens from multiple providers is hell"</b></summary>

Claude Code, Codex, Gemini CLI, Copilot — semua menggunakan OAuth 2.0 dengan
token yang kadaluarsa. Pengembang perlu melakukan semula autentikasi, menghadapi
`client_secret tidak ada`, `redirect_uri mismatch`, dan kegagalan di server
jarak jauh. OAuth di LAN/VPS sangat bermasalah.

**Bagaimana OmniRoute menyelesaikannya:**

- **Penggunaan Otomatis Tokoan Menghidupkan** — Tokoan OAuth dihidupkan kembali
  di latar belakang sebelum kadaluarsa
- **OAuth 2.0 (PKCE) Terpadu** — Aliran yang otomatis untuk Claude Code, Codex,
  Gemini CLI, Copilot, Kiro, Qwen, iFlow
- **OAuth Berbilang Akun** — Banyak akun per penyedia melalui ekstraksi JWT/ID
  token
- **Penggunaan Fix OAuth LAN/Remote** — Mendeteksi IP pribadi untuk
  `redirect_uri` + mode URL manual untuk server jarak jauh
- **Penggunaan OAuth Di Belakang Nginx** — Menggunakan `window.location.origin`
  untuk konsolitas proxy belakang
- **Panduan Jarak OAuth** — Langkah demi langkah untuk kredential Google Cloud
  di VPS/Docker

</details>

<details>
<summary><b>📊 9. "I don't know how much I'm spending or where"</b></summary>

Pengembang menggunakan penyedia dibayar yang banyak tetapi tidak memiliki
pandangan bersatu mengenai pengeluaran. Setiap penyedia memiliki dashboard
pengeluaran sendiri, namun tidak ada pandangan perusahaan. Biaya yang tidak
terduga dapat berkumpul.

**Bagaimana OmniRoute menyelesaikannya:**

- **Papan Analisis Biaya** — Mengikuti biaya per-token dan pengelolaan anggaran
  per penyedia
- **Had Uang Per Kelas** — Had pengeluaran per kelas yang mengaktifkan jatuh
  kembali otomatis
- **Pengaturan Harga Per Model** — Mengatur harga per model
- **Statistik Penggunaan Per API Key** — Hitungan permintaan dan tanda waktunya
  terakhir per kunci
- **Papan Analisis** — Kartu stat, grafik penggunaan model, dan meja penyedia
  dengan kadar keberhasilan dan keterlambatan

</details>

<details>
<summary><b>🐛 10. "I can't diagnose errors and problems in AI calls"</b></summary>

==WEBLATE_PART==\
Dalam kesilapan panggilan, pengembang tidak tahu jika hanya rate limit, token
yang telah kedaluwarsa, format yang salah, atau error penyedia. Log yang
terfragmentasi di hampir semua terminal tanpa pengawasan. Tanpa observability,
debugging hanyalah permainan coba-coba.

**Bagaimana OmniRoute menyelesaikannya:**

- **Periapan Log Dashboard ** — 4 tab: Log Permintaan, Log Proxy, Log Audit,
  Konsol
- **Pemutus Log Pemutus Konsol ** — Pemutus waktu nyata yang menampilkan
  garis-garis warna, scroll otomatis, cari, dan filter
- **Log Proxy SQLite ** — Log-log yang berlangsung meskipun server melakukan
  restart
- **Mainan Playground Bahasa ** — 4 Mode Debug: Mainan (penerjemah format),
  Tester Obrolan (round-trip), Papan Uji (perkumpulan), Monitor Hidup (yang
  nyata)
- **Penyelidikan Permintaan ** — latency 50%/95%/99% + Tracing X-Request-Id
- **Logging dengan Penyimpanan Berkas ** — Pemutus Konsol menangkap segalanya
  menjadi log JSON dengan rotasi berdasarkan ukuran
- **Laporan Info Sistem ** — `npm run system-info` menghasilkan
  `system-info.txt` dengan lingkunganmu penuh (versi Node, OmniRoute, OS, alat
  CLI, Docker/PM2). Pasang saat melaporkan masalah untuk mempercepat pergeseran.

</details>

<details>
<summary><b>🏗️ 11. "Deploying and maintaining the gateway is complex"</b></summary>

Pemasangan, pengaturan, dan pemeliharaan proxy AI di berbagai lingkungan (lokal,
VPS, Docker, awan) sangat merepotkan. Masalah seperti directory yang telah
terhardcode, `EACCES` pada direktori, konflik porta, dan bangun-bangun
lintas-platform menambah gesekan.

**Bagaimana OmniRoute menyelesaikannya:**

- **Instalasi npm Global ** — `npm install -g omniroute &amp;&amp; omniroute` —
  selesai
- **Docker Multi-Platform ** — AMD64 + ARM64 asli (Apple Silicon, AWS Graviton,
  Raspberry Pi)
- **Docker Compose Profil ** — `dasar` (tanpa alat CLI) dan `CLI` (dengan Claude
  Code, Codex, OpenClaw)
- **Aplikasi Desktop Electron ** — Aplikasi asli untuk Windows/macOS/Linux
  dengan tray sistem, mulai otomatis, dan mode offline
- **Modus Port Terpisah ** — API dan Dashboard di porta yang berbeda untuk
  skenario lanjutan (reverse proxy, jaringan kontainer)
- **Sinkronisasi Awan ** — Sinkronisasi konfigurasi di semua perangkat melalui
  Cloudflare Workers
- **Cadangan DB ** — Cadangan otomatis, pulihkan, eksport, dan import semua
  pengaturan

</details>

<details>
<summary><b>🌍 12. "The interface is English-only and my team doesn't speak English"</b></summary>

Tim-tim di negara-negara non-Bahasa Inggris, terutama di Amerika Latin, Asia,
dan Eropa, mengalami kesulitan dengan wawasan Bahasa Inggris. Barisan Bahasa
menurunkan penerimaan dan meningkatkan kesalahan pengaturan.

**Bagaimana OmniRoute menyelesaikannya:**

- **Iklan Pamela — 30 Bahasa - Seperti Arab, Bulgaria, Denmark, Jerman, Spanyol,
  Finland, Perancis, Ibrani, Hindi, Hungary, Indonesia, Italia, Jepun, Korea,
  Melayu, Belanda, Norway, Poland, Portugis (PT/BR), Romania, Rusia, Slovakia,
  Sweden, Thai, Ukraine, Vietnam, Cina, Filipina, Inggeris
- **Dukungan Lekar Besar** — Dukungan Lekar Kanan untuk Arab dan Ibrani
- **Bacan Melayu MANUALS** — 30 pemindahan Dokumentasi Penuh
- **Pelaras Bahasa** — Sumbang Minyak di kepala untuk menukar Melayu secara
  langsung

</details>

<details>
<summary><b>🔄 13. "I need more than chat — I need embeddings, images, audio"</b></summary>

Teknologi AI bukan saja melengkapkan percakapan. Pembangun perlu menghasilkan
imej, mengiktiraf audio, mencipta pautan bagi RAG, mengehadkan dokumen, dan
mengawal kandungan. Setiap Modul API mempunyai titik akhir dan format yang
berbeza.

**Bagaimana OmniRoute menyelesaikannya:**

- **Pautan Embedding** — `/v1/pautan_embedding` dengan 6 pembekal dan 9+ model
- **Penghasilan Imej** — `/v1/imej/penghasilan` dengan 10 pembekal dan 20+ model
  (OpenAI, xAI, Bersama, Fireworks, Nebius, Hyperbolic, NanoBanana, Antigravity,
  SD WebUI, ComfyUI)
- **Text-to-Video** — `/v1/video/penghasilan` — ComfyUI (AnimateDiff, SVD) dan
  SD WebUI
- **Text-to-Muzik** — `/v1/muzik/penghasilan` — ComfyUI (Stable Audio Open,
  MusicGen)
- **Pengiktirafan Audio** — `/v1/audio/pengiktirafan` — Whisper + Nvidia NIM,
  HuggingFace, Qwen3
- **Pamanyaucar Tekks** — `/v1/audio/pamanyaucar` — ElevenLabs, Nvidia NIM,
  HuggingFace, Coqui, Tortoise, Qwen3, **Dalam Dunia**, **Cartesia**,
  **Tertarik**, + pembekal sedia ada
- **Perenggan Moderasi** — `/v1/Perenggan_moderasi` — Pemeriksaan selamat
  kandungan
- **Ranking semula** — `/v1/rank_sembulan` — Reranking keberlakuan dokumen
- **API Respons** — Dukungan sepenuhnya `/v1/apipembalas` untuk Codex

</details>

<details>
<summary><b>🧪 14. "I have no way to test and compare quality across models"</b></summary>

Pembangun mahu tahu model mana yang terbaik untuk kes-kes mereka — kod,
menerjemah, sebab memikir — tetapi menerangkan secara manual perlahan-lahan.
Tiada alat penggunaan dibuka terpadu.

**Bagaimana OmniRoute menyelesaikannya:**

- **Pendedahan Model AI** — Pengujian set emas dengan 10 kes memuat-muat sendiri
  menutup mesyuarat, aritmatik, geografi, pengeluaran kod, jaminan JSON,
  terjemahan, perenggan markah, penggagalan safes
- **Empat Strategi Mencari** — `sekata`, `tercari`, `rreg_XXreg`, `sekonstan`
  (fungsian JS)
- **Bengkel Cetakan Test** — Pengujian set dalam bentuk-bentuk beberapa mulaan
  dan tuntutan keluar, perbandingan antara pembekal
- **Pengujian Chat** — Pemungutan penuh melalui penampilan respons visual
- **Pengawasan Langsung** — Aleran masa nyata semua permintaan mengalir melalui
  perantara

</details>

<details>
<summary><b>📈 15. "I need to scale without losing performance"</b></summary>

Serta dengan volum permintaan meningkat, tanpa caching sama pertanyaan yang sama
yang menghasilkan kosmet yang ganda. Tanpa ketegasan idempotensi, permintaan
ganda menggantung proses. Batasan per-tiap-perusahaan harus dihormati.

**Bagaimana OmniRoute menyelesaikannya:**

- **Perekam Semantic** — Keping dua-lapis ( tandatangan + semantik ) menurunkan
  biaya dan laten
- **Ketegasan Idempotensi** — Jendela deduplikasi 5s untuk permintaan yang sama
- **Pengenalan Batasan Seharusnya** — Aleran per-tiap-perusahaan RPM, jarak
  minimum dan maksimum sekaligus pengawasan
- **Keseimbangan Batasan Seharusnya** — Pengaturan standar pada Settings →
  Ketahanan dengan kemampuan bertahan
- **Perekam API Kunci Validate** — Keping tiga-lapis untuk kinerja produksi
- **Pusat Kerusakan Penyusun dengan Pelacakan** — laten p50/p95/p99, statistik
  perekam, ketersediaan

</details>

<details>
<summary><b>🤖 16. "I want to control model behavior globally"</b></summary>

Pengembang yang ingin semua respons dalam bahasa tertentu, dengan nada tertentu,
atau ingin membatasi tokenn logika. Mengatur hal ini dalam setiap alat/perintah
perintah yang lain adalah tidak prakgs.

**Bagaimana OmniRoute menyelesaikannya:**

- **Pengembalian Prompt Sitema** — Prompt global yang digunakan sebagai semua
  permintaan
- **Pengecekan Anggaran Logika** — Pengaturan alokasi token logika per-perintah
  (penjembatan, auto, khusus, adaptif)
- **6 Strategi Routing** — Strategi global yang menentukan bagaimana permintaan
  diagihkan
- **Perekam Wildcard** — `perusahaan/*` pola menerapkan dinamis ke provider apa
  saja
- **Klik Tombol Nyalakan/Matikan Combos** — Tombol combos dapat dilakukan
  langsung dari pengawasan
- **Tombol Nyalakan/Matikan Provider** — Matikan/aktifkan semua koneksi untuk
  perusahaan dalam satu klik
- **Perusahaan Terblokir** — Perusahaan tertentu ekskluskan dari `/v1/models`
  daftar

</details>

<details>
<summary><b>🧰 17. "I need MCP tools as first-class product capabilities"</b></summary>

Banyak pengawal AI mengorbankan MCP sebagai detail implementasi yang
disembunyikan. Tim yang memerlukan lapisan operasi yang terlihat serta dapat
dielak.

**Bagaimana OmniRoute menyelesaikannya:**

- Navebenu muncul pada navigasi dashboard dan tab protocol sambungan
- Halaman pengurusan Navebenu khusus dengan proses, alat, ruang lingkup, dan
  siasat auditor
- Pelan cepat-masuk yang built-in untuk `omniroute --mcp` dan pendaftaran
  pelanggan

</details>

<details>
<summary><b>🧠 18. "I need A2A orchestration with sync + stream task paths"</b></summary>

Aliran kerja ejen memerlukan jawapan langsung dan eksekusi berjenama (streamed)
yang berlangsung lama dengan kawalan hayat.

**Bagaimana OmniRoute menyelesaikannya:**

- Titik akhir JSON-RPC A2A (`POST /a2a`) dengan `message/send` dan
  `message/stream`
- Penyiaran SSE dengan penerapan keadaan terminal
- API hayat tugas untuk `tasks/get` dan `tasks/cancel`

</details>

<details>
<summary><b>🛰️ 19. "I need real MCP process health, not guessed status"</b></summary>

Pasukan operasional ingin tahu apakah Navebenu hidup, bukannya hanya apakah API
terhubung.

**Bagaimana OmniRoute menyelesaikannya:**

- Fail henti-henti Navebenu yang sedang berjalan dengan PID, tanda kurun waktu,
  kaedah pengangkutan, bilangan perkakasan, dan mod ruang lingkup
- API status Navebenu yang menggabungkan henti-henti + kesarjanaan terbaru
- Kard penjaga status UI untuk hayat proses, kestabilan, dan keheningan
  henti-henti

</details>

<details>
<summary><b>📋 20. "I need auditable MCP tool execution"</b></summary>

Apabila perkakasan berubah konfigurasi atau memperantarai tindakan aksi
pengoperasian, pasukan perlu perekodan siasat.

**Bagaimana OmniRoute menyelesaikannya:**

- Perekodan audit SQLite yang bersekutu dengan panggilan perkakasan Navebenu
- Paparan filer berdasarkan perkakasan, kesuksesan/silang, kunci API, dan
  paginan
- Paparan penukaran audit + titik akhir statistik untuk automatikasi

</details>

<details>
<summary><b>🔐 21. "I need scoped MCP permissions per integration"</b></summary>

Pelanggan berbeza hendaklah mempunyai akses kategori perkakasan dengan tahap
kefahaman yang kurang.

**Bagaimana OmniRoute menyelesaikannya:**

- 9 Ruang MCP yang dapat dikustomkan untuk akses peralatan yang terkontrol
  dengan tahap yang halus
- Pengesahan dan visibiliti skop MCP dalam antarmuka pengurusan
- Posisi lalai yang selamat untuk peralatan operasi

</details>

<details>
<summary><b>⚙️ 22. "I need operational controls without redeploying"</b></summary>

Rancangan tim memerlukan perubahan runtime cepat semasa kejadian insiden atau
ketibaan kos.

**Bagaimana OmniRoute menyelesaikannya:**

- Aktifasi combo beralih secara langsung dari papan dasbor MCP
- Buat profil ketahanan dari paip kebijaksanaan yang dibuat terlebih dahulu
- Reset keadaan pelanggang sirkuit dari panel operasi yang sama

</details>

<details>
<summary><b>🔄 23. "I need live A2A task lifecycle visibility and cancellation"</b></summary>

Tiada kawalan kehidupan akan menyulitkan tugas insiden untuk penjarakan.

**Bagaimana OmniRoute menyelesaikannya:**

- Senarai tugas/pembahagian dari keadaan/pelbagai ciri dengan halaman penukaran
  yang berpagar
- Turun ke metadata, kejadian, dan artifact tugas dengan skrol
- Tangkapan tugas dengan tanda tanya dan konfirmasi UI dengan tindakan

</details>

<details>
<summary><b>🌊 24. "I need active stream metrics for A2A load"</b></summary>

Aliran kerja streaming memerlukan pandangan operasi kepada kekonkurenan dan
koneksi langsung yang berfungsi.

**Bagaimana OmniRoute menyelesaikannya:**

- Penghitungan aliran aktif dipentaskan dalam status A2A
- Masa tugas terakhir dan kiraan untuk setiap keadaan
- Kard A2A papan dasbor untuk pemantauan operasi dalam masa nyata

</details>

<details>
<summary><b>🪪 25. "I need standard agent discovery for clients"</b></summary>

Raden pelanggan luaran dan pengaturcara perlu metadata peralatan yang membaca
oleh maklumat pengenalan.

**Bagaimana OmniRoute menyelesaikannya:**

- Kartu ejen di `/.well-known/agent.json`
- Kemampuan dan kebolehan dipaparkan di antara antaramuka pengurusan
- API A2A status termasuk metadata pembentukan untuk automasi

</details>

<details>
<summary><b>🧭 26. "I need protocol discoverability in the product UX"</b></summary>

Jika pengguna tidak boleh membentuk permukaan protokol, kualiti penggunaan dan
sokongan akan merosot.

**Bagaimana OmniRoute menyelesaikannya:**

- Laman **Penerapan Endpoint** sambungkan berjadual dengan papan pita untuk
  Proxy, MCP, A2A, dan Penerapan API
- Pilihan status perkhidmatan secara garis dalam (Aktif / Tidak Aktif) utk MCP
  dan A2A
- Pautan dari paparan ke pita pengurusan berasingan.

</details>

<details>
<summary><b>🧪 27. "I need end-to-end protocol validation with real clients"</b></summary>

Pemeriksaan mock tidak cukup untuk mengesahkan kemampuan protokol sebelum
pelancaran.

**Bagaimana OmniRoute menyelesaikannya:**

- Sistem kelayakan akhir (E2E) yang melayakkan aplikasi dan menggunakan
  transport klien MCP SDK yang sebenar.
- Pemeriksaan klien A2A bagi pembentukan, hantar, aliran hayat, mengambil, dan
  batalkan aliran
- Penapisan aksi semula terhadap MCP audit dan penerapan A2A API

</details>

<details>
<summary><b>📡 28. "I need unified observability across all interfaces"</b></summary>

Pemisahan sediaan keseluruhan oleh protocol menjadikan cincin kejahatan dan masa
batal pelancongan yang lebih lama (MTTR)

**Bagaimana OmniRoute menyelesaikannya:**

- Papan keputusan tergabung antara satu produk
- Sediaan keseluruhan kesejahteraan + audit + telemetri permintaan secara
  melintang di lapisan OpenAI, MCP, dan A2A
- API operasional bagi status dan automasi

</details>

<details>
<summary><b>💼 29. "I need one runtime for proxy + tools + agent orchestration"</b></summary>

Pengendalian banyak perkhidmatan yang berasingan meningkatkan kos operasional
dan kegagalan.\
==WEBLATE_PART==

**Bagaimana OmniRoute menyelesaikannya:**

- OpenAI-compatible proxy, MCP server, and A2A server in one stack
- Shared auth, resilience, data store, and observability
- Consistent policy model across all interaction surfaces

</details>

<details>
<summary><b>🚀 30. "I need to ship agentic workflows without glue-code sprawl"</b></summary>

Teams lose velocity when stitching multiple ad-hoc services and scripts.

**Bagaimana OmniRoute menyelesaikannya:**

- Unified endpoint strategy for clients and agents
- Built-in protocol management UIs and smoke validation paths
- Production-ready foundations (security, logging, resilience, backup)

</details>

### Example Playbooks (Integrated Use Cases)

**Playbook A: Maximize paid subscription + cheap backup**

```txt
Combo: "maximize-claude"
  1. cc/claude-opus-4-6
  2. glm/glm-4.7
  3. if/kimi-k2-thinking

Monthly cost: $20 + small backup spend
Outcome: higher quality, near-zero interruption
```

**Playbook B: Zero-cost coding stack**

```txt
Combo: "free-forever"
  1. gc/gemini-3-flash
  2. if/kimi-k2-thinking
  3. qw/qwen3-coder-plus

Monthly cost: $0
Outcome: stable free coding workflow
```

**Playbook C: 24/7 always-on fallback chain**

```txt
Combo: "always-on"
  1. cc/claude-opus-4-6
  2. cx/gpt-5.2-codex
  3. glm/glm-4.7
  4. minimax/MiniMax-M2.1
  5. if/kimi-k2-thinking

Outcome: deep fallback depth for deadline-critical workloads
```

**Playbook D: Agent ops with MCP + A2A**

```txt
1) Start MCP transport (`omniroute --mcp`) for tool-driven operations
2) Run A2A tasks via `message/send` and `message/stream`
3) Observe via /dashboard/endpoint (MCP and A2A tabs)
4) Toggle services via inline status controls
```

---

## 🆓 Start Free — Zero Configuration Cost

> Setup AI coding in minutes at **$0/month**. Connect these free accounts and
> use the built-in **Free Stack** combo.

| Langkah | Tindakan                                                             | Pemberi Sumber Unlocked                                           |
| ------- | -------------------------------------------------------------------- | ----------------------------------------------------------------- |
| 1       | Hubungkan **Kiro** (AWS Builder ID OAuth)                            | Claude Sonnet 4.5, Haiku 4.5 — **tanpa had**                      |
| 2       | Hubungkan **iFlow** (Google OAuth)                                   | kimi-k2-pikiran, qwen3-koder-plus, deepseek-r1... — **tanpa had** |
| 3       | Hubungkan **Qwen** (Device Code)                                     | qwen3-koder-plus, qwen3-koder-flow-s... — **tanpa had**           |
| 4       | Hubungkan **Gemini CLI** (Google OAuth)                              | gemini-3-flow, gemini-2.5-pro — **180K/mo percuma**               |
| 5       | /X0X/papan pengawas/combos` → **Stack Penuh Percuma (RM0)** template | Semua pemberi sumber percuma digantung secara automatik           |

/X0X/Hubungkan mana-mana IDE/CLI ke:** `http://localhost:20128/v1` · Kunci API:
`apa-apa-string` · Selesai.

> /X0X/Selain itu adalah kesan tambahan (juga percuma):** Kunci API Groq (30 RPM
> percuma), NVIDIA NIM (40 RPM percuma, 70+ model), Cerebras (1M tok/day), Kunci
> API LongCat (50M token/day!), Pekerja AI Cloudflare (10K Selarah Neu/day, 50+
> model).

## Mula Pantas

### 1. Pasang dan jalankan

```bash
npm install -g omniroute
omniroute
```

> **pnpm pengguna:** Jalankan `pnpm approve-builds -g` setelah pasang untuk
> aktifkan skrip pemasangan yang diperlukan oleh `better-sqlite3` dan
> `@swc/core`:
> 
> ```bash
> pnpm install -g omniroute
> pnpm approve-builds -g   # Pilih semua paket → persetujuan
> omniroute
> ```

Halaman utama dibuka di `http://localhost:20128` dan URL dasar API adalah
`http://localhost:20128/v1`.

| Perintah                | Deskripsi                                                          |
| ----------------------- | ------------------------------------------------------------------ |
| `omniroute`             | Mulai server (`PORT=20128`, API dan dashboard pada port yang sama) |
| `omniroute --port 3000` | Atur port kanonis/API ke 3000                                      |
| `omniroute --mcp`       | Mulai server MCP (transport standar stdio)                         |
| `omniroute --no-open`   | Jangan membuka browser secara otomatis                             |
| `omniroute --help`      | Tunjukkan bantuan                                                  |

Pilihan mode berbagi-port:

```bash
PORT=20128 DASHBOARD_PORT=20129 omniroute
# API:       http://localhost:20128/v1
# Dashboard: http://localhost:20129
```

### 2) Sambungkan penyedia dan buat kunci API

1. Buka Dashboard → `Penyedia` dan sambungkan setidaknya satu penyedia (OAuth
   atau kunci API).
2. Buka Dashboard → `Endpoint` dan buat kunci API.
3. Opsional) Buka Dashboard → `Kombinasi` dan tetapkan rantai fallback.

### 3) Arahkan alat kode Anda ke OmniRoute

```txt
URL dasar: http://localhost:20128/v1
Kunci API:  [kopikan dari halaman Endpoint]
Model:    jika/kimi-k2-pemikiran (atau prefix penyedia/model mana pun)
```

Sangsai dengan Claude Code, Codex CLI, Gemini CLI, Cursor, Cline, OpenClaw,
OpenCode, dan SDK kompatibel OpenAI.

### 4) Aktifkan dan validasi protokol (v2.0)

**MCP (untuk operasi berbasis alat):**

```bash
omniroute --mcp
```

Lalu sambungkan klien MCP Anda melalui `stdio` dan uji alat-alat seperti:

- `omniroute_get_health`
- `omniroute_list_combos`

**A2A (untuk arahan-ke-arahan):**

```bash
curl http://localhost:20128/.well-known/agent.json
```

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"quickstart","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"Berikan saya ringkasan kuota yang singkat."}]}}'
```

### 5) Validasi segalanya end-to-end (disarankan)

```bash
npm run test:protocols:e2e
```

Suite ini mengvalidasi aliran klien MCP dan A2A nyata terhadap aplikasi yang
berjalan.

### Alternatif: jalankan dari sumber.

```bash
cp .env.contoh .env
npm install
PORT=20128 DASHBOARD_PORT=20129 NEXT_PUBLIC_BASE_URL=http://localhost:20129 npm run dev
```

---

## 🐳 Kapsel Containers

OmniRoute adalah Kapsel Kontena Awam yang terdapat pada [Docker
Hub](https://hub.docker.com/r/diegosouzapw/omniroute).

**Kirim cepat:**

```bash
docker run -d \
  --nama omniroute \
  --restart kecuali-mati \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:latest
```

**Dengan fail penting:**

```bash
# Salin dan sunting fail .env terlebih dahulu
cp .env.contoh .env

docker run -d \
  --nama omniroute \
  --restart kecuali-mati \
  --env-file .env \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:latest
```

**Menggunakan Kapsel Kontena:**

```bash
# Fail profil asas (tidak menggunakan alat kawalan CLI)
docker compose --profile base up -d

# Profill CLI (Claude Code, Codex, Terbinafril built-in)
docker compose --profile cli up -d
```

| Imej                     | Tajuk     | Saiz   | Deskripsi               |
| ------------------------ | --------- | ------ | ----------------------- |
| `diegosouzapw/omniroute` | `terbaru` | ~250MB | Keluaran stabil terkini |
| `diegosouzapw/omniroute` | `1.0.3`   | ~250MB | Versi terkini           |

---

## 🖥️ Aplikasi Desktop — Tidak terhubung lori & Sentiasa Aktif

> 🆕 **YANG!** OmniRoute kini sedia sebagai **permohonan desktop asli** untuk
> Windows, macOS, dan Linux.

Ejalankan OmniRoute sebagai satu aplikasi desktop berasingan — tiada terminal,
peramban, dan internet diperlukan untuk model tempatan. Aplikasi Electron ini
termasuk:

- 🖥️ **Tetingkap Asli** — Tetingkap aplikasi yang dilucutkan dengan integrasi
  tray sistem
- 🔄 **Bermulai Automatik** — Jalankan OmniRoute pada log masuk sistem
- 🔔 **Pemberitahuan Asli** — Terima pemberitahuan untuk habis kuota atau
  pengaturcaraan isu
- ⚡ **Pemasangan Sat-Sat** — NSIS (Windows), DMG (macOS), AppImage (Linux)
- 🌐 **Mod Ghoib** — Fungsikan penuh tanpa internet dengan server berpangkalan
  padu

### Mula Pantas

```bash
# Mod pembangunan
npm run electron:dev

# Tutup untuk platform
npm run electron:build         # Platform terkini
npm run electron:build:win     # Windows (.exe)
npm run electron:build:mac     # macOS (.dmg) — x64 &amp; arm64
npm run electron:build:linux   # Linux (.AppImage)
```

### Tray Sistem

Ketika diteliti, OmniRoute tinggal di tray sistem dengan aksi cepat:

- Buka Papan Pemuka
- Tukar port pengaturcaraan
- Keluarkan aplikasi

📖 Dokumentasi penuh: [`electron/README.md`](electron/README.md)

---

## Harga dengan Cenah

| Paket                       | Provider                   | Biaya                                                 | Pulih Kuota              | Terbaik Bagi                                  |
| --------------------------- | -------------------------- | ----------------------------------------------------- | ------------------------ | --------------------------------------------- |
| **💳 PEMBAYARAN SUBSCRIPSI** | Claude Code (Pro)          | $20/bulan                                             | 5j + mingguan            | Sudah tersambung                              |
|                             | Codex (Plus/Pro)           | $20-200/bulan                                         | 5j + mingguan            | Pengguna OpenAI                               |
|                             | Gemini CLI                 | **TUNGGAK LEBIH RENDAH**                              | 180K/bulan + 1K/hari     | Semua orang!                                  |
|                             | GitHub Copilot             | $10-19/bulan                                          | Bulan                    | Pengguna GitHub                               |
| **💼 KUNJUNGI API**          | NVIDIA NIM                 | **TUNGGAK LEBIH RENDAH** (selamanya untuk pengembang) | ~40 RPM                  | 70+ buku model terbuka                        |
|                             | Cerebras                   | **TANPA BIAYA** (1 juta token/hari)                   | 60K TPM / 30 RPM         | Tepat setelah masa                            |
|                             | Groq                       | **TANPA BIAYA** (30 RPM)                              | 14.4K RPD                | Llama/Gemma ultracepat                        |
|                             | DeepSeek V3.2              | $0.27/$1.10 per 1 juta                                | tiada                    | Alasan harga/kualitas terbaik                 |
|                             | xAI Grok-4 Cepat           | **$0.20/$0.50 per 1 juta** 🆕                          | tiada                    | Cepat + panggilan alat, ultratal              |
|                             | xAI Grok-4 (standar)       | $0.20/$1.50 per 1 juta 🆕                              | tiada                    | Panutan alasan dari xAI                       |
|                             | Mistral                    | Bicara percubaan percuma + bayaran                    | Kadar terhad             | AI Eropah                                     |
|                             | OpenRouter                 | Bayar mengikut pengguna                               | tiada                    | 100+ model agregat                            |
| **💰 TIPSAH **               | GLM-5 (melalui Z.AI) 🆕     | $0.5/1M                                               | Setiap 10PG, setiap hari | 128K pembesar, paling baru flagship           |
|                             | GLM-4.7                    | $0.6/1M                                               | Setiap 10PG, setiap hari | Cadangan budasan                              |
|                             | MiniMax M2.5 🆕             | $0.3/1M input                                         | 5 jam peringkat          | Tugas ketinggian pengambilan dan tugas agenif |
|                             | MiniMax M2.1               | 0.2 dolar/1 juta                                      | 5 jam peringkat          | Pilihan tercheapest                           |
|                             | Kimi K2.5 (Moonshot API) 🆕 | Bayar mengikut pengguna                               | tiada                    | Akses Moonshot API secara langsung            |
|                             | Kimi K2                    | Flat $9/bulan                                         | 10 juta token/bulan      | Kos yang dapat diprediksi                     |
| **FREE** 🆓                  | iFlow                      | **$0**                                                | Tidak terhadap batasan   | 5 model tidak ada batasan                     |
|                             | Qwen                       | **$0**                                                | Tidak terhadap batasan   | 4 model tidak ada batasan                     |
|                             | Kiro                       | **$0**                                                | Tidak terhadap batasan   | Claude Sonnet/Haiku (AWS Builder)             |
|                             | LongCat Flash-Lite 🆕       | **$0** (50M tok/hari 🔥)                               | 1 PPS (Per second)       | Besar kuota percuma di Bumi                   |
|                             | Migrasi AI 🆕               | **$0** (tidak memerlukan kunci)                       | 1 permintaan/15s         | GPT-5, Claude, DeepSeek, Llama 4              |
|                             | Workers AI Cloudflare 🆕    | **$0** (10K Seluron sehari)                           | ~150 respons/sehari      | 50+ model, edge global                        |
|                             | AI Scaleway 🆕              | **$0** (1M token total)                               | Kadar terhad             | EU/ GDPR, Qwen3 235B, Llama 70B               |

> 🆕 **Model-model baru ditambah (Mac 2026):** Grok-4 Fast keluarga di
> $0.20/$0.50/M (ditetapkan pada 1143ms — 30% lebih cepat daripada Gemini 2.5
> Flash), GLM-5 melalui Z.AI dengan 128K output, MiniMax M2.5 berpikir, DeepSeek
> V3.2 harga dicetak, Kimi K2.5 melalui API langsung Moonshot.

**💡 Combo Stack — Seluruh Percuma Kompleks: **

```
# 🆓 Kombo Utama Percuma 2026 — 11 penyedia, $0 Selamanya
Kiro (kr/)             → Claude Sonnet/Haiku TANPA BAYAR
iFlow (if/)            → kimi-k2-pikir, qwen3-penulis-plus, deepseek-r1 TANPA BAYAR
LongCat Lite (lc/)     → LongCat-Nefalas-Lite — 50M token/hari 🔥
Migrasi (pol/)         → GPT-5, Claude, DeepSeek, Llama 4 — tidak memerlukan kunci
Qwen (qw/)             → qwen3-penulis-plus, qwen3-penulis-noflash, qwen3-penulis-setelah UNLIMITED
Gemini (gemini/)       → Gemini 2.5 Flash — 1,500 permintaan/hari API kunci gratis
AI Cloudflare (cf/)    → Llama 70B, Gemma 3, Mistral — 10K Seluron sehari
Scaleway (scw/)        → Qwen3 235B, Llama 70B — 1M token percuma (UE)
Groq (groq/)           → Llama/Gemma tercepat — 14.4K permintaan sehari
NVIDIA NIM (nvidia/)   → 70+ model terbuka — 40 RPM selamanya
Cerebras (cerebras/)   → Llama/Qwen tercepat di dunia — 1M tok sehari
```

**Tanpa kos. Tidak berhenti memprogram.** Konfigurasi ini sebagai satu Kombo
OmniRoute dan semua fallback terjadi secara otomatis — tidak ada manual beralih
pernah.

---

---

## 🆓 Model Percuma — Apa Yang Anda Dapatkan Secara Akhirnya

> Semua model di bawah ini adalah **100% percuma dengan nill kad kredit
> diperlukan**. OmniRoute menyalurkan antara mereka ketika satu kuota habis —
> padukan mereka semua untuk paket combo $0 yang tidak dapat patah.

### 🔵 MODEL CLAUDE (via Kiro — ID Pembina AWS)

| Model               | Awalan | Had              | Had Kadar                                |
| ------------------- | ------ | ---------------- | ---------------------------------------- |
| `claude-sonnet-4.5` | `kr/`  | **Tidak Terhad** | Tiada had cip tambahan harian dilaporkan |
| `claude-haiku-4.5`  | `kr/`  | **Tidak Terhad** | Tiada had cip tambahan harian dilaporkan |
| `claude-opus-4.6`   | `kr/`  | **Tidak Terhad** | Versi Opu terbaru melalui Kiro           |

### 🟢 MODELS IFLOW (OAUTH percuma - Tiada Kredit Kad)

| Model                                    | Awalan | Had              | Had Kadar                |
| ---------------------------------------- | ------ | ---------------- | ------------------------ |
| `kimi-k2-thinking`                       | `if/`  | **Tidak Terhad** | Tiada had cap dilaporkan |
| `qwen3-coder-plus`                       | `if/`  | **Tidak Terhad** | Tiada had cap dilaporkan |
| Pencarian dalam depth rujukan-1 `        | `if/`  | **Tidak Terhad** | Tiada had cap dilaporkan |
| [Minimax model 2.1 dengan nilai rujukan` | `if/`  | **Tidak Terhad** | Tiada had cap dilaporkan |
| Kimi dengan model rujukan-2 `            | `if/`  | **Tidak Terhad** | Tiada had cap dilaporkan |

### Mod Aplikasi QWEN (Kod Utama Peranti)

| Model                                                                        | Awalan | Had              | Had Kadar                |
| ---------------------------------------------------------------------------- | ------ | ---------------- | ------------------------ |
| `qwen3-coder-plus`                                                           | `qw/`  | **Tidak Terhad** | Tiada had cap dilaporkan |
| Aplikasi Pencarian QWEN Kod Rujukan Pembangun Peralihan Sinaran Penerangan ` | `qw/`  | **Tidak Terhad** | Tiada had cap dilaporkan |
| Aplikasi Pencarian QWEN Cod Utama Pembangun Selanjutnya Sinaran Penerangan ` | `qw/`  | **Tidak Terhad** | Tiada had cap dilaporkan |
| Model Penuh Sinaran Penerangan `                                             | `qw/`  | **Tidak Terhad** | Multimodal (Gambar)      |

### GEMINI CLI (Kesetiaan Google)

| Model                    | Awalan       | Had                             | Had Kadar         |
| ------------------------ | ------------ | ------------------------------- | ----------------- |
| `Gemini-3 Flash Preview` | `gerakan/c/` | **180K tok/month** + 1K/hari    | Pemulihan Bulanan |
| `Gemini-2.5 Pro`         | `gerakan/c/` | 180K/bulan (kumpulan berkongsi) | Kualiti Tinggi    |

### ⚫ Perkhidmatan NVIDIA NIM (API Kunci Percuma — build.nvidia.com)

| Paket             | Had Harian      | Had Kadar   | Nota                                                                      |
| ----------------- | --------------- | ----------- | ------------------------------------------------------------------------- |
| Free (Pengembang) | Tiada had capor | **~40 RPM** | 70+ model; berpindah ke had limit arah perantaraan pertengahan tahun 2025 |

Model percuma popular: `moonshotai/kimi-k2.5` (Kimi K2.5), `z-ai/glm4.7` (GLM
4.7), `deepseek-ai/deepseek-v3.2` (DeepSeek V3.2),
`nvidia/llama-3.3-70b-instruct`, `deepseek/deepseek-r1`

### ⚪ CEREBRAS (API Kunci Percuma — inference.cerebras.ai)

| Paket   | Had Harian        | Had Kadar        | Nota                                                    |
| ------- | ----------------- | ---------------- | ------------------------------------------------------- |
| Percuma | **1M token/hari** | 60K TPM / 30 RPM | Inferensi LLM tercepat di dunia; me-restart setiap hari |

Tersedia secara percuma: `llama-3.3-70b`, `llama-3.1-8b`,
`deepseek-r1-distill-llama-70b`

### 🔴 GROQ (Kunci API Percuma — console.groq.com)

| Paket   | Had Harian    | Had Kadar        | Nota                                                                          |
| ------- | ------------- | ---------------- | ----------------------------------------------------------------------------- |
| Percuma | **14.4K RPD** | 30 RPS per model | Tidak memerlukan kad kredit; 429 ketika mencapai had, tidak dikenakan bayaran |

Tersedia secara percuma: `llama-3.3-70b-versatile`, `gemma2-9b-it`,
`mixtral-8x7b`, `whisper-large-v3`

### 🔴 LONGCAT AI (Kunci API Percuma — longcat.chat) 🆕

| Model                         | Awalan | Rizab Harian Percuma | Nota                          |
| ----------------------------- | ------ | -------------------- | ----------------------------- |
| `LongCat-Flash-Lite-X`        | `lc/`  | **50M token** 💥      | Kuota percuma terbesar pernah |
| `LongCat-Flash-Chat`          | `lc/`  | 500K token           | Bicara multi-turn             |
| `LongCat-Flash-Thinking`      | `lc/`  | 500K token           | Pemikiran / CoT               |
| `LongCat-Flash-Thinking-2601` | `lc/`  | 500K token           | Versi Jan 2026                |
| `LongCat-Flash-Omni-2603`     | `lc/`  | 500K token           | Multimod                      |

> Sempurna percuma ketika dalam beta awam. Daftar di
> [longcat.chat](https://longcat.chat) dengan emel atau telefon. Dikemaskini
> setiap hari jam 0:00 UTC

### 🟢 PENUBUHAN AI POLLINATIONS (Tiada API Key Diperlukan) 🆕

| Model      | Awalan | Had Kadar        | Provider Behind    |
| ---------- | ------ | ---------------- | ------------------ |
| `openai`   | `pol/` | 1 permintaan/15s | GPT-5              |
| `claude`   | `pol/` | 1 permintaan/15s | Anthropic Claude   |
| `gemini`   | `pol/` | 1 permintaan/15s | Google Gemini      |
| `deepseek` | `pol/` | 1 permintaan/15s | DeepSeek V3        |
| `llama`    | `pol/` | 1 permintaan/15s | Meta Llama 4 Scout |
| `mistral`  | `pol/` | 1 permintaan/15s | Mistral AI         |

> ✨ **Zero friction:** No signup, no API key. Add the Pollinations provider with
> an empty key field and it works immediately.

### 🟠 CLOUDFLARE WORKERS AI (Free API Key — cloudflare.com) 🆕

| Paket   | Daily Neurons | Equivalent Usage                        | Nota                    |
| ------- | ------------- | --------------------------------------- | ----------------------- |
| Percuma | **10,000**    | ~150 LLM resp / 500s audio / 15K embeds | Global edge, 50+ models |

Popular free models: `@cf/meta/llama-3.3-70b-instruct`,
`@cf/google/gemma-3-12b-it`, `@cf/openai/whisper-large-v3-turbo` (free audio!),
`@cf/qwen/qwen2.5-coder-15b-instruct`

> Requires API Token + Account ID from
> [dash.cloudflare.com](https://dash.cloudflare.com). Store Account ID in
> provider settings.

### 🟣 SCALEWAY AI (1M Free Tokens — scaleway.com) 🆕

| Paket   | Free Quota    | Location     | Nota                                |
| ------- | ------------- | ------------ | ----------------------------------- |
| Percuma | **1M tokens** | 🇫🇷 Paris, EU | No credit card needed within limits |

Available free: `qwen3-235b-a22b-instruct-2507` (Qwen3 235B!),
`llama-3.1-70b-instruct`, `mistral-small-3.2-24b-instruct-2506`,
`deepseek-v3-0324`

> EU/GDPR compliant. Get API key at
> [console.scaleway.com](https://console.scaleway.com).

> **💡 The Ultimate Free Stack (11 Providers, $0 Forever):**
> 
> ```
> Kiro (kr/)             → Claude Sonnet/Haiku UNLIMITED
> iFlow (if/)            → kimi-k2-thinking, qwen3-coder-plus, deepseek-r1 UNLIMITED
> LongCat Lite (lc/)     → LongCat-Flash-Lite — 50M tokens/day 🔥
> Pollinations (pol/)    → GPT-5, Claude, DeepSeek, Llama 4 — no key needed
> Qwen (qw/)             → qwen3-coder models UNLIMITED
> Gemini (gemini/)       → Gemini 2.5 Flash — 1,500 req/day free
> Cloudflare AI (cf/)    → 50+ models — 10K Neurons/day
> Scaleway (scw/)        → Qwen3 235B, Llama 70B — 1M free tokens (EU)
> Groq (groq/)           → Llama/Gemma — 14.4K req/day ultra-fast
> NVIDIA NIM (nvidia/)   → 70+ open models — 40 RPM forever
> Cerebras (cerebras/)   → Llama/Qwen world-fastest — 1M tok/day
> ```

## 🎙️ Free Transcription Combo

> Transcribe any audio/video for **$0** — Deepgram leads with $200 free,
> AssemblyAI $50 fallback, Groq Whisper as unlimited emergency backup.

| Provider         | Free Credits           | Best Model                                   | Had Kadar                    |
| ---------------- | ---------------------- | -------------------------------------------- | ---------------------------- |
| 🟢 **Deepgram**   | **$200 free** (signup) | `nova-3` — best accuracy, 30+ languages      | No RPM limit on free credits |
| 🔵 **AssemblyAI** | **$50 free** (signup)  | `universal-3-pro` — chapters, sentiment, PII | No RPM limit on free credits |
| 🔴 **Groq**       | **Free forever**       | `whisper-large-v3` — OpenAI Whisper          | 30 RPM (rate limited)        |

**Suggested combo in `/dashboard/combos`:**

```
Name: free-transcription
Strategy: Priority
Nodes:
  [1] deepgram/nova-3          → uses $200 free first
  [2] assemblyai/universal-3-pro → fallback when Deepgram credits run out
  [3] groq/whisper-large-v3    → free forever, emergency fallback
```

Lalu dalam `/dashboard/media` → **Transkripsi** paparan: muat fail audio atau
video mana saja → pilih endpoint combo tujuan → dapatkan transkripsi dalam
format yang disokong.

## 💡 Ciri-ciri Utama

OmniRoute v2.0 dibina sebagai platform operasi, bukan hanya rewayat proxy.

### 🆕 Baru — Kemas Kini Pembaikan ClawRouter (Mac 2026)

| Ciri                                              | Apa Tujuan Dibuatnya                                                                                                                                      |
| ------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ⚡ **Grok-4 Keluarga Cepat**                       | Model AI bernilai $0.20/$0.50/M — dilakukan ujian prestasi 1143ms (30% lebih pantas daripada Gemini 2.5 Flash)                                            |
| 🧠 **GLM-5 melalui Z.AI**                          | Konteks keluaran 128K, $0.50/1M — model flagship terbaru daripada keluarga GLM                                                                            |
| 🔮 **MiniMax M2.5**                                | Sumber rasa + tugas bertenaga agensi bernilai $0.30/1M — kemas kini signifikan daripada M2.1                                                              |
| 🎯 **Pilih Flag Model Setiap Model**               | Pilih setiap `Pilih Flag: benar/salah` di pendaftaran — Pengguna AutoCombo terlepas model tidak berpemilik                                                |
| 🌍 **Pengesahan Niat Berbilang Bahasa**            | Kata kunci Bahasa Portugal/Zh-Hans/Spanish/Arab di dalam pemarkahan skor AutoCombo — pemilihan model yang lebih baik bagi kandungan bukan bahasa Inggeris |
| 📊 **Kekurangan Perekangan Berdasarkan Benchmark** | Keterlaluan p95 nyata berdasarkan permintaan hidup memberi pemarkahan skor combo — AutoCombo belajar dari data asal sebenar                               |
| 🔁 **Keduplikan Permintaan**                       | Jenama kandungan berdasarkan dedup window — selamat multi-agensi, mencegah kenderaan berlipat ganda                                                       |
| 🔌 **Rout strategi plug-in**                       | Antara muka `Rout strategi` yang boleh diperluas — tambahkan logik pautan khusus sebagai plugin                                                           |

### 🚀 Sebelum v2.0.9+ — PlayGround, CLI Jejak & ACP

| Ciri                                              | Apa Tujuan Dibuatnya                                                                                                                                                                                                                               |
| ------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🎮 **Pelayan Model Playground**                    | Halaman pemain untuk mengujikan model apa saja secara langsung — pilihan penyedia/model/sebalompositor, Editor Monaco, streaming, batal, ketibaan                                                                                                  |
| 🔏 **Keluhan CLI Jejak Sambungan**                 | Susunan kepalan/badan penyedia untuk sambungan native CLI — pilih per penyedia di Pilihan > Keselamatan. **Alamat proxy IP anda tetap tersimpan**                                                                                                  |
| 🤝 **Dukung ACP (Protokol Pelanggan Klien)**       | Tembung agen CLI (Codex, Claude, Goose, Gemini CLI, OpenClaw + 9 lagi), pengguna proses, `/api/acp/agens` hujung puncak                                                                                                                            |
| 🤖 **Penyiapkan ACP Dashboard**                    | Debug › Agents laman — grid 14 agen dengan status pemasangan, versi, formulir agen khusus apa pun alat CLI. **Pengguna OpenCode** menerima butang " Muat opencode.json" yang menghasilkan konfigurasi siap pakai dengan semua model yang tersedia. |
| 🔧 **Mengatur Format `api` untuk model khusus**    | Model khusus dengan `apiFormat: "rencana"` sekarang memadamkan pautan ke penterjemah API Respons corak                                                                                                                                             |
| 🏢 **Pemisahan Lalu lintas Codex Per Ruang kerja** | Banyak ruang kerja Codex per alamat email — OAuth secara korang memisahkan koneksi oleh ID ruang kerja                                                                                                                                             |
| 🔄 **Automuat Pembaruan Elektronik**               | Aplikasi desktop memeriksa pembaruan + menginstal secara otomatis pada restart                                                                                                                                                                     |

### 🤖 Operasi Agen & Protokol (v2.0)

| Ciri                                  | Apa Tujuan Dibuatnya                                                                                    |
| ------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| 🔧 **MCP Server (16 alat))**           | IDE/agens tools secara 3 transportasi: stdio, SSE (`/api/mcp/sse`), HTTP Streamable (`/api/mcp/stream`) |
| 🤝 **A2A Server (JSON-RPC + SSE)**     | Eksekusi tugas antara agen dengan aliran sinkron dan streaming                                          |
| 🧭 **Endpoints Laman Konsolidasi**     | Laman pengurusan tab dengan Endpoint Proxy, MCP, A2A, dan API Endpoints                                 |
| 🎚️ **Perpatoan Pelayanan Buka/Tutup** | Sekop O/N untuk MCP dan A2A dengan kekaliran pengaturan (kebangan: Tutup)                               |
| 🛰️ **MCP Hartanah Proses**            | Status proses nyata (PID, masa uptime, umur deteksi jantung, transportasi, kaedah ruang)                |
| 📋 **MCP Tail Auditi**                 | Catatan auditi boleh difilter dengan kejayaan/fail dan atribusi kunci                                   |
| 🔐 **Pengurusan Kuasa Akses MCP**      | 9 haluan perlu kuasa untuk akses alat terkawal                                                          |
| 📡 **Pengurusan Lifos Tugas A2A**      | Senarai/bilang tugas, memeriksa evento/artisfak, batal tugas berjalan                                   |
| 📋 **Pengenalan Card Agen**            | `/.well-known/agent.json` untuk pemulangan automatik pelanggan                                          |
| 🧪 Protokol E2E Ujian Harness**        | Real SDK sistem MCP + A2A client flows dalam `uji:protokol:e2e`                                         |
| ⚙️ **Kawalan Operasi**                | Combobox, gunakan profil ketahanan, dan reset pemutus bermula dari satu permukaan kawalan               |

### 🧠 & Intelijen Laluan

| Ciri                                    | Apa Tujuan Dibuatnya                                                                  |
| --------------------------------------- | ------------------------------------------------------------------------------------- |
| 🎯 **Gaya Lompatan Bijak 4-Tier**        | Rute secara automatik: Sumber Diperolehi → Kunci API → Murah ← Harga                  |
| 📊 **Pantauan Kuota Saksama Masa Nyata** | Pengiraan token hidup + ketetapan reset per pembekal                                  |
| 🔄 **Percetakan Translation**            | OpenAI ↔ Claude ↔ Gemini ↔ Respons dengan pemindahan skema selamat                    |
| 👥 **Dukungan Pengecaman Semula**        | Pengecaman perisian yang banyak per lembaga pembekal dengan pilihan yang bijak        |
| 🔄 **Penggantian Token Otomatis**        | Token OAuth akan mengekalkan secara automatik dengan cubaan semula                    |
| 🎨 **Kombo Mencetak**                    | 6 strategi seimbang + kawalan rantai gantian                                          |
| 🌐 **Penghantar Wildcard**               | `pembekal/*` penyiaraan dinamik                                                       |
| 🧠 **Buat Perancangan Anggaran**         | Pasar, oto, kustom, dan had perkiraan algoritma                                       |
| 🔀 **Pengenalpastian Model**             | Alasan model binaan dan alihan keselamatan                                            |
| ⚡ **Kerdil Latar Belakang**             | Rute tugas latar belakang yang lebih rendah ke model yang lebih murah                 |
| 🧪 **Rutunag Pintar Tugas-X**            | Pilih model automatik mengikut tipe kandungan (suntingan/bacaan/analisis/summarisasi) |
| 💬 **Masukkan Prompt Sistem**            | Kawalan tingkah laku global diluluskan sebulat bulat                                  |
| 📄 **Selaras Kompatibiliti API Jawapan** | Penyokong sepenuhnya `/v1/responses` untuk Codex dan aliran kerja agenitif maju       |

### 🎵 API-APi Bersepadu

| Ciri                     | Apa Tujuan Dibuatnya                                                                                                                                                                 |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 🖼️ **Penghasilan Imej**  | `/v1/images/generations` dengan latar belakang awan dan tempatan                                                                                                                     |
| 📐 **Kandungan**          | `/v1/embeddings` untuk aliran kumpulan pencarian dan RAG                                                                                                                             |
| 🎤 **Transkripsi Audio**  | `/v1/audio/transcriptions` — 7 penyedia (Deepgram Nova 3, AssemblyAI, Groq Whisper, HuggingFace, ElevenLabs, OpenAI, Azure), pengenalan bahasa secara otomatis, sokongan MP4/MP3/WAV |
| 🔊 **Bacaan Teks**        | `/v1/audio/speech` — 10 penyedia (ElevenLabs, OpenAI, Deepgram, Cartesia, PlayHT, HuggingFace, Nvidia NIM, Inworld, Coqui, Tortoise) dengan kerja sama yang betul                    |
| 🎬 **Penghasil Video**    | `/v1/videos/generations` (Pengaliran ComfyUI + SD WebUI)                                                                                                                             |
| 🎵 **Penghasil Muzik**    | `/v1/music/generations` (Pengaliran ComfyUI)                                                                                                                                         |
| 🛡️ **Moderasi**          | `/v1/moderations` pemeriksaan keselamatan                                                                                                                                            |
| 🔀 **Ukuran Semula**      | `/v1/rerank` untuk mengukur semula ketepatan                                                                                                                                         |
| 🔍 **Carian Laman Web** 🆕 | `/v1/search` — 5 penyedia (Serper, Brave, Perplexity, Exa, Tavily), lebih dari 6,500/minggu secara percuma, bergantian (failover), cache                                             |

### 🛡️ Kebolehpercayaan, Keselamatan & Penguasaan

| Ciri                               | Apa Tujuan Dibuatnya                                                                   |
| ---------------------------------- | -------------------------------------------------------------------------------------- |
| 🔌 **Pengawal Pelayan**             | Pengulangan model/memulihkan dengan perubahan suhu                                     |
| 🎯 **Model-Anda-Tahu[Teknologi]X    | Custom models declare supported endpoints + API format                                 |
| 🛡️ **Anti-Thundering Herd**        | Mutex + semaphore protections on retry/rate events                                     |
| 🧠 **Semantic + Signature Cache**   | Cost/latency reduction with two cache layers                                           |
| ⚡ **Request Idempotency**          | Duplicate protection window                                                            |
| 🔒 **TLS Fingerprint Spoofing**     | Browser-like TLS fingerprint — **reduces bot detection and account flagging**          |
| 🔏 **Keluhan CLI Jejak Sambungan**  | Matches native CLI request signatures — **reduces ban risk while preserving proxy IP** |
| 🌐 **IP Filtering**                 | Allowlist/blocklist control for exposed deployments                                    |
| 📊 **Editable Rate Limits**         | Configurable global/provider-level limits with persistence                             |
| 🔑 **API Key Management + Scoping** | Secure key issuance/rotation and model/provider controls                               |
| 🛡️ **Protected `/models`**         | Optional auth gating and provider hiding for model catalog                             |

### 📊 Observability & Analytics

| Ciri                                    | Apa Tujuan Dibuatnya                                                  |
| --------------------------------------- | --------------------------------------------------------------------- |
| 💻 **Mohon + Log Tangan Proxy**          | Log lengkap permintaan/pertimbangan dan log proxy                     |
| 📋 **Papan Pengawas Log Yang Disatukan** | Lihatan permintaan, proxy, audit, dan terminal di dalam satu muka     |
| 🔍 **Pelacak Teknologi Permintaan**      | Keterlambatan p50/p95/p99 dan menjejaki permintaan                    |
| 🏥 **Papan Petunjuk Kesihatan**          | Masa berfungsi, keadaan pembungkus, keadaan terkunci, statistik cache |
| 💰 **Pengurusan Kos**                    | Kawalan bajet dan keupayaan untuk melihat harga per-muka              |
| 📈 **Visualisasi Analitik**              | Insight penggunaan model/provinsi dan pandangan trend                 |
| 🧪 **Framwork Penilaian**                | Pengujian set emas setelah pilihan strategi sebelah semak             |

### ☁️ Pembinaan & Platform

| Ciri                              | Apa Tujuan Dibuatnya                                          |
| --------------------------------- | ------------------------------------------------------------- |
| 🌐 **Tarikhal Bila-Bila Tempat**   | Lokal, VPS, Docker, Lingkungan awan                           |
| 💾 **Serasi Awan**                 | Serasi konfigurasi melalui pekerja awan                       |
| 🔄 **Cadangan/Tenagawan**          | Pengaliran dan alir balik bencana                             |
| 🧙 **Panduan Pembantu Pemasangan** | Pengaturan sambutan pertama                                   |
| 🔧 **Perintah Baris CLI Pelontar** | Pengaturan satu klik untuk alat menyunting popular            |
| 🎮 **Pelayan Model Playground**    | Ujian pelayan/ model/ penghujung dari panel kendali           |
| 🔏 **Tangkapan Jejak CLI (kotor**  | Pecutan jejak pelayan per-pelayan di Pengaturan > Keselamatan |
| 🌐 **Multibahasa (30 laman)**      | Penyokongan penuh panel kawalan + dokumen dengan Ralat Pintal |
| 🧹 **Buang Semua Model**           | Pembersihan sekali klik senarai model di maklumat pelayan     |
| 📋 **Templat Masalah**             | Templat standar GitHub untuk bug dan ciri                     |
| 📂 **Direktori Data Pilih**        | `Directory Data` penggantian untuk lokasi penyimpanan         |

### Tahap mendalam Pembelajaran Mesin

#### Pengurangan fallback cerdas dengan kawalan kos yang praktikal

```txt
Kombo: "pautan coding saya"
  1. cc/claude-opus-4-6
  2. nvidia/llama-3.3-70b
  3. glm/glm-4.7
  4. if/kimi-k2-pengajar
```

Apabila kuota, kadar atau keadaan kesihatan gagal, OmniRoute secara automatik
berpindah ke calon seterusnya tanpa penukaran manual.

#### Pengurusan protokol yang dapat dilihat dan digunakan

- MCP + A2A dapat ditemui di UI dan dokumen (tidak disembunyikan)
- API status protokol yang mengekspos data operasional langsung (`/api/mcp/*`,
  `/api/a2a/*`)
- Papan pemuka termasuk aksi untuk operasi hari dua (pautan kombinasi, pembaikan
  breaker, pelarangan tugas)

#### Alirannya Translator + validasi

Kawasan Translator menempatkan:

- **Laman Permainan**: kebalikan pengujian kemasukan data
- **Mesin Chat Penguji**: meliputi penukaran permintaan/majikan
- **Tapak Ujian**: beberapa kes dalam satu eksekusi
- **Pemerhati Tegar**: pandangan trafik langsung semasa

Kemudian penukarannya protokol dengan pelanggan sebenar melalui `npm run
test:protocols:e2e`.

> 📖 **[Kandungan Pautan README MCP](open-sse/mcp-server/README.md)** – Sumber
> rujukan, konpigasi IDE, dan contoh klien
> 
> 📖 **[Kandungan Pautan README A2A](src/lib/a2a/README.md)** — Pencapaian,
> kaedah JSON-RPC, penghantaran, dan kehidupan tugas

## 🧪 Evaluasi (Evaluasi)

OmniRoute telah termasuk dalam kerangka kerja ulasan binaan bagi menguji kualiti
jawapan LLM terhadap himpunan emas. Akses ke cawangannya melalui **Analytics →
Evals** di papan pemuka.

### Set Golden Binaan Binaan

Paket "OmniRoute Golden Set" yang dibangunkan secara dalam mengandungi kes-kes
ujian untuk:

- Selawat, matematik, geografi, penghasilan kod
- Kelulusan format JSON, terjemahan, penghasilan markah
- Pengkelasan mengenai kandungan kecederaan, pengiraan, logik boole

### Strategi Penilaian

| Strategi         | Deskripsi                                                                            | Contoh                                 |
| ---------------- | ------------------------------------------------------------------------------------ | -------------------------------------- |
| `tersurat tepat` | Keluaran mestinya sepadan sepenuhnya                                                 | `"4"`                                  |
| `mengandungi`    | Keluaran mestinya mengandungi sub-judul (tanpa mengambil kira huruf besar/mol kecil) | `"Paris"`                              |
| `reguks`         | Keluaran mestinya sepadan dengan rangkaian reguks                                    | `"1.*2.*3"`                            |
| `khusus`         | Kesemuaan fungsi Javascript yang dibangunkan khususnya mengatakan betul/belum        | `(keluar) =&gt; keluar.length &gt; 10` |

---

## Panduan Konfigurasi

### Persetujuan Protokol (MCP + A2A)

<details>
<summary><b>🧩 MCP Setup (Model Context Protocol)</b></summary>

Mulakan pentauliahan MCP dalam mod stdio:

```bash
omniroute --mcp
```

Aliran validasi yang disarankan:

1. Hubungi pelanggan MCP anda melalui stdio.
2. Tatal `omniroute_get_health`.
3. Tatal `omniroute_list_combos`.
4. Buka `/dashboard/mcp` untuk mengesahkan sentuhan jantung, kegiatan, dan
   audit.

APPI yang berguna untuk automatik:

- `GET /api/mcp/status`
- `GET /api/mcp/tools`
- `GET /api/mcp/audit`
- `GET /api/mcp/audit/stats`

</details>

<details>
<summary><b>🤝 A2A Setup (Agent2Agent)</b></summary>

Berkatkan agen:

```bash
curl http://localhost:20128/.well-known/agent.json
```

Hantar tugas:

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"setup-a2a","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"Ringkaskan status kuota."}]}}'
```

Bertadbir kehidupan:

- `AMBIL /api/a2a/status`
- `AMBIL /api/a2a/tasks`
- `AMBIL /api/a2a/tasks/:id`
- `HANTAR /api/a2a/tasks/:id/cancel`

Sistem Operasi:

- `/dashboard/a2a` untuk menyaksikan tugas/negeri/laluan pengenalan api dan
  tindakan asap

</details>

<details>
<summary><b>🧪 End-to-end protocol validation</b></summary>

Periksa kedua protokol dengan klien sebenar:

```bash
npm run test:protocols:e2e
```

Inilah yang membabitkan:

- MCP SDK klien hubungi/daftar/panggil
- Penemuan A2A/menghantar/laluan/carikan/batalkan
- Periksa maklumat di audit MCP dan API pengurusan tugas A2A

</details>

<details>
<summary><b>💳 Subscription Providers</b></summary>

### Claude Kode (Pro/Maksima)

```bash
Peta Carta → Pembekal → Sambung Claude Kode
→ Log masuk OAuth → Merefitkan semula token secara automatik
→ Sambungan 5 jam + rujuk seminggu

Model:
  cc/claude-opus-4-6
  cc/claude-sonnet-4-5-20250929
  cc/claude-haiku-4-5-20251001
```

**Saran Pro:** Gunakan Opus untuk tugas kompleks, Sonnet untuk kesejujuran.
OmniRoute menjejaki kuota per model!

### Codex OpenAI (Plus/Pro)

```bash
Peta Carta → Pembekal → Sambung Codex
→ Log masuk OAuth (port 1455)
→ 5 jam + reset seminggu 

Model:
  cx/gpt-5.2-codex
  cx/gpt-5.1-codex-max
```

#### Pengurusan Had Akun Codex (5 jam + Mingguan)

Kini, setiap akaun Codex telah mempunyai kepingan tetingkap kebijaksanaan di
`Peta Carta → Pembekal`:

- `5 jam` (ON/OFF): Enforce perbatasan ketetapan masa 5 jam.\
  ==WEBLATE_PART##
- `Mingguan` (MULA/MATI): laksanakan dasar kebijakan tingkat jendela mingguan.
- Sifat Pemotong: ketika jendela yang diaktifkan mencapai >=90% penggunaan,
  akaun itu dilupakan.
- Sifat Pemutaran: OmniRoute berlalu ke akaun Codex yang sah secara otomatis.
- Sifat Pembetulan: ketika penyedia `resetAt` waktu melewati, akaun menjadi sah
  lagi secara automatik.

Skenario:

- `5 jam ON` + `Mingguan ON`: akaun dilupakan ketika jendela manapun mencapai
  batas.
- `5 h OFF` + `Mingguan ON`: hanya penggunaan mingguan yang dapat membatu akaun.
- `5 jam ON` + `Mingguan OFF`: hanya penggunaan 5 jam yang dapat membatu akaun.
- `resetAt` telah melewati: akaun kembali ke pembelajaran secara automatik
  (tidak perlu diperbarui manual).

### CLI Gemini (GRATIS 180K/minggu!)

```bash
Dashboard → Penyedia → Hubungi CLI Gemini
→ OAuth Google
→ 180K pengisian lengkap/minggu + 1K/hari

Model:
  gc/gemini-3-preview-gemini
  gc/gemini-2.5-pro
```

**Nilai Terbaik:** Tier gratis yang besar! Pakai ini sebelum tingkat berbayar.

### GitHub Copilot

```bash
Dashboard → Penyedia → Hubungi GitHub
→ OAuth melalui GitHub
→ Reset bulanan (tanggal 1 bulan)

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
2. Dapatkan API Key gratis (1.000 kredit inferensi termasuk)
3. Dashboard → Tambah Penyedia → NVIDIA NIM:
   - API Key: `nvapi-key-anda`

**Model:** `nvidia/llama-3.3-70b-instruct`, `nvidia/mistral-7b-instruct`, dan
50+ model lain

**Cara Bijak:** API yang sesuai dengan OpenAI — bekerja sama lancar dengan
translation format OmniRoute!

### DeepSeek

1. Daftar: [platform.deepseek.com](https://platform.deepseek.com)
2. Akses API
3. Papan Pantau → Tambah Penghantar → DeepSeek

**Model:** `deepseek/deepseek-chat`, `deepseek/deepseek-coder`

### Groq (Tahap Percuma Tersedia!)

1. Daftar: [console.groq.com](https://console.groq.com)
2. Akses API (tahap percuma dihidupkan)
3. Papan Pantau → Tambah Penghantar → Groq

**Model:** `groq/llama-3.3-70b`, `groq/mixtral-8x7b`

**Cara Bijak:** Penjumlahan yang super cepat — terbaik untuk coding
berkelanjutan!

### OpenRouter (100+ Model)

1. Daftar: [openrouter.ai](https://openrouter.ai)
2. Akses API
3. Papan Pantau → Tambah Penghantar → OpenRouter

**Model:** Akses 100+ model dari semua penyedia utama melalui kunci API tunggal.

</details>

<details>
<summary><b>💰 Cheap Providers (Backup)</b></summary>

### GLM-4.7 (Reset harian, $0.6/1M)

1. Daftar: [Zhipu AI](https://open.bigmodel.cn/)
2. Akses API dari Coding Plan
3. Papan Kawalan → Tambah Kunci API:
   - Sumber: `glm`
   - Kunci API: `your-key`

**Gunakan:** `glm/glm-4.7`

**Tip Profesional:** Piawaian Coding menawarkan 3× kuota pada kos 1/7 daripada
biasanya! Semakan harian pada 10:00 pagi.

### MiniMax M2.1 (reset semula 5j, $0.20/1M)

1. Bergabung: [MiniMax](https://www.minimax.io/)
2. Akses API
3. Papan Kawalan → Tambah Kunci API

**Gunakan:** `minimax/MiniMax-M2.1`

**Tip Profesional:** Pilihan termurah untuk konteks panjang (1M token)!

### Kimi K2 ($9/sebulan flat)

1. Daftar: [Moonshot AI](https://platform.moonshot.ai/)
2. Akses API
3. Papan Kawalan → Tambah Kunci API

**Gunakan:** `kimi/kimi-latest`

**Tip Profesional:** Kos efektif $0.90/1M!

</details>

<details>
<summary><b>🆓 FREE Providers (Emergency Backup)</b></summary>

### iFlow (5 model percuma melalui OAuth)

```bash
Papan Kawalan → Hubungkan iFlow
→ Masuk OAuth iFlow
→ Gunakan tanpa had
Model:
  if/kimi-k2-thinking
  if/qwen3-coder-plus
  if/glm-4.7
  if/minimax-m2
  if/deepseek-r1
```

### Qwen (4 model percuma melalui Kod Perkakasan)

```bash
Dashboard → Connais Qwen
→ Kod pengesahan peranti
→ Penggunaan tidak terbatas

Models:
  qw/qwen3-coder-plus
  qw/qwen3-coder-flash
```

### Kiro (Claude percuma)

```bash
Dashboard → Connais Kiro
→ ID Pembina AWS atau Google/GitHub
→ Penggunaan tidak terbatas

Models:
  kr/claude-sonnet-4.5
  kr/claude-haiku-4.5
```

</details>

<details>
<summary><b>🎨 Create Combos</b></summary>

### Contoh 1: Maksimalkan Pelancongan → Bantuan Murah

```
Dashboard → Kombinasi → Buat Baru

Nama: premium-coding
 Models:
  1. cc/claude-opus-4-6 (Pelancongan utama pembayaran)
  2. glm/glm-4.7 (Bantuan murah, $0.6/1M)
  3. minimax/MiniMax-M2.1 (Pengganti paling murah, $0.20/1M)

Gunakan dalam Perintah Antara Muka: premium-coding
```

### Contoh 2: Percuma (Kos sifar)

```
Nama: free-combo
Models:
  1. gc/gemini-3-flash-preview (180K percuma sebulan)
  2. if/kimi-k2-pikiran (tidak terbatas)
  3. qw/qwen3-coder-plus (tidak terbatas)

Kos: $0 selamanya!
```

</details>

<details>
<summary><b>🔧 CLI Integration</b></summary>

### IDE kursor

```
Pengaturan → Model → Maju:
  URL API OpenAI Asas: http://localhost:20128/v1
  API OpenAI: [dari kawasan OmniRoute]
  Model: cc/claude-opus-4-6
```

### Kod Claude

Gunakan halaman **alat-alat CLI** di dashboards untuk pengkonfigurasi tindakan
satu-satu, atau edit `~/.claude/pengaturan.json` secara manual.

### Codex CLI

```bash
eksport OPENAI_BASE_URL="http://localhost:20128"
eksport OPENAI_API_KEY="ID API Anda"

codex "perintah Anda"
```

### OpenClaw

**Pilihan 1 — Dashboard (dipercayai):**

```
Dashboard → Alat-alat Perintah → OpenClaw → Pilih Model → Aplikasikan
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

> **Nota:** OpenClaw hanya berfungsi dengan pelantar OmniRoute tempatan. Gunakan
> `127.0.0.1` daripada `localhost` untuk mengelakan masalah penyelesaian IPv6.

### Cline / Diteruskan / RooCode

```
Settings → API Configuration:
  Provider: OpenAI Compatible
  Base URL: http://localhost:20128/v1
  API Key: [from OmniRoute dashboard]
  Model: if/kimi-k2-thinking
```

### OpenCode

**Step 1:** Add OmniRoute as a custom provider:

```bash
opencode
/connect
# Select "Other" → Enter ID: "omniroute" → Enter your OmniRoute API key
```

**Step 2:** Create/edit `opencode.json` in your project root:

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
        "if/kimi-k2-thinking": { "name": "Kimi K2 (Free)" }
      }
    }
  }
}
```

**Step 3:** Select the model in OpenCode:

```bash
/models
# Select any OmniRoute model from the list
```

> **Tip:** Add any model available in your OmniRoute `/v1/models` endpoint to
> the `models` section. Use the format `provider/model-id` from your OmniRoute
> dashboard.

</details>

---

## Menyelesaikan masalah

<details>
<summary><b>Click to expand troubleshooting guide</b></summary>

**"Language model did not provide messages"**

- Provider quota exhausted → Check dashboard quota tracker
- Solution: Use combo fallback or switch to cheaper tier

**Rate limiting**

- Subscription quota out → Fallback to GLM/MiniMax
- Add combo: `cc/claude-opus-4-6 → glm/glm-4.7 → if/kimi-k2-thinking`

**OAuth token expired**

- Auto-refreshed by OmniRoute
- If issues persist: Dashboard → Provider → Reconnect

**High costs**

- Periksa penggunaan statistik di Dashboard → Kos
- Swtich model utama ke GLM/MiniMax
- Gunakan tahap percuma (Gemini CLI, iFlow) untuk tugas-tugas bukan kritikal

[x0x]Landing Dashboard/API port adalah salah[x31x]

- [x0x]PORT[x5x] ialah sokongan asas canonikal (dan port API keperluan keutamaan
  pula)
- [x0x]API_PORT[x9x] menggantikan hanya pengguna API yang bersesuaian dengan
  OpenAI
- [x0x]DASHBOARD_PORT[x15x] menggantikan hanya pengguna Dashboard/Next.js
- Tetapkan [x4x]NEXT_PUBLIC_BASE_URL[x25x] kepada alamat URL public Anda (untuk
  pemanggilan OAuth)

[x0x]Kemaskini cloud tidak berfungsi[x19x]

- Pastikan [x7x]BASE_URL[x16x] menunjukkan ke alamat kesan Anda sendiri
- Pastikan [x7x]CLOUD_URL[x17x] menunjukkan ke endpoint awam cloud Anda
- Teruskan [x5x]NEXT_PUBLIC_*[x19x] value dengan berafiliasi dengan nilai laman
  server

[x0x]Pertama perlu ke fungsional[tidak berfungsi x25x]

- Periksa [x6x]INITIAL_PASSWORD[x23x] dalam [.env x28x]
- Ditangguhkan bukan, kata laluan yang dapat digunakan boleh [x31x] 123456
  [x38x]

[x0x]Tiada rekod permohonan[x17x]

- Tetapkan [x4x]ENABLE_REQUEST_LOGS=true[x29x] dalam [.env x34x]

[x0x]Ujian kaitan menunjukkan "Invalid" untuk penanfaibar penyedia-penyedia yang
bersesuaian dengan OpenAI[x65x]

- Banyak penyedia tidak mengumumkan endpoint [x30x]/models[x38x]
- OmniRoute 1.0.6+ termasuk perisikan valdasi melalui pilihan jawab chat
- Ensure base URL includes `/v1` suffix

### 🔐 OAuth on a Remote Server

<a name="oauth-on-a-remote-server"></a> <a name="oauth-em-servidor-remoto"></a>

> **⚠️ Important for users running OmniRoute on a VPS, Docker, or any remote
> server**

#### Why does Antigravity / Gemini CLI OAuth fail on remote servers?

The **Antigravity** and **Gemini CLI** providers use **Google OAuth 2.0**.
Google requires the `redirect_uri` in the OAuth flow to exactly match one of the
pre-registered URIs in the app's Google Cloud Console.

The OAuth credentials bundled in OmniRoute are registered **for `localhost`
only**. When you access OmniRoute on a remote server (e.g.
`https://omniroute.myserver.com`), Google rejects the authentication with:

```
Error 400: redirect_uri_mismatch
```

#### Solution: Configure your own OAuth credentials

You need to create an **OAuth 2.0 Client ID** in Google Cloud Console with your
server's URI.

#### Step-by-step

**1. Open Google Cloud Console**

Go to:
[https://console.cloud.google.com/apis/credentials](https://console.cloud.google.com/apis/credentials)

**2. Create a new OAuth 2.0 Client ID**

- Click **"+ Create Credentials"** → **"OAuth client ID"**
- Application type: **"Web application"**
- Name: anything you like (e.g. `OmniRoute Remote`)

**3. Add Authorized Redirect URIs**

In the **"Authorized redirect URIs"** field, add:

```
https://your-server.com/callback
```

> Replace `your-server.com` with your server's domain or IP (include the port if
> needed, e.g. `http://45.33.32.156:20128/callback`).

**4. Simpan dan salin kreditensia**

Selepas mencipta, Google akan menunjukkan **ID Pemohon** dan **Rahsiat
Pemohon**.

**5. Tentukan kawalan persekitaran**

Di dalam `.env` (atau kawalan persekitaran Docker):

```bash
# Untuk Antigravity:
ANTIGRAVITY_OAUTH_CLIENT_ID=your-client-id.apps.googleusercontent.com
ANTIGRAVITY_OAUTH_CLIENT_SECRET=GOCSPX-your-secret

# Untuk Gemini CLI:
GEMINI_OAUTH_CLIENT_ID=your-client-id.apps.googleusercontent.com
GEMINI_OAUTH_CLIENT_SECRET=GOCSPX-your-secret
GEMINI_CLI_OAUTH_CLIENT_SECRET=GOCSPX-your-secret
```

**6. Lakukan semula OmniRoute**

```bash
# npm:
npm run dev

# Docker:
docker restart omniroute
```

**7. Cuba hubungi semula**

Dashboard → Pengedar → Antigravity (atau Gemini CLI) → OAuth

Google kini akan membawa semula dengan betul ke
`https://pelayan-anda.com/callback`.

---

#### Pengecualian sementara (tanpa kreditensia berkaitan)

Jika anda tidak mahu setup kreditensia berbanding sendiri pada masa ini, anda
masih dapat menggunakan **aliran manual URL**:

1. OmniRoute membuka URL untuk pemakrakan Google
2. Selepas pemakrakan, Google cuba membawa semula ke `localhost` (yang gagal
   pada pelayan jauh)
3. **Salin URL penuh** dari tetingkap alamat pelayar anda (kecuali muka hadapan
   tidak dimuatkan)
4. Salin URL berkenaan ke dalam medan ditunjukkan dalam modul penghubung
   OmniRoute
5. Klik **"Hubungi"**

> Jenis kerja ini berjalan kerana kod akses yang disertakan dalam alamat URL
> masih sah walaupun muka hadapan pindahan tidak dimuatkan.

---

<details>
<summary><b>🇧🇷 Versão em Português</b></summary>

#### Mengapa pemakrakan OAuth Antigravity / Gemini CLI gagal di pelayan jauh?

Pengedar-pengedar **Antigravity** dan **Gemini CLI**guna **OAuth 2.0 Google**
bagi pengenalan. Google memerlukan URL `pindahan` digunakan dalam pemakrakan
OAuth ialah **tertentu** diantara URI yang sudah dicadangkan dalam Konsol
Perkhidmatan Google aplikasi.

As credenciais OAuth embutidas no OmniRoute estão cadastradas **apenas para
`localhost`**. Quando você acessa o OmniRoute em um servidor remoto (ex:
`https://omniroute.meuservidor.com`), o Google rejeita a autenticação com:

```
Error 400: redirect_uri_mismatch
```

#### Solução: Configure suas próprias credenciais OAuth

Você precisa criar um **OAuth 2.0 Client ID** no Google Cloud Console com a URI
do seu servidor.

#### Passo a passo

**1. Acesse o Google Cloud Console**

Abra:
[https://console.cloud.google.com/apis/credentials](https://console.cloud.google.com/apis/credentials)

**2. Crie um novo OAuth 2.0 Client ID**

- Clique em **"+ Create Credentials"** → **"OAuth client ID"**
- Tipo de aplicativo: **"Web application"**
- Nome: escolha qualquer nome (ex: `OmniRoute Remote`)

**3. Adicione as Authorized Redirect URIs**

No campo **"Authorized redirect URIs"**, adicione:

```
https://seu-servidor.com/callback
```

> Substitua `seu-servidor.com` pelo domínio ou IP do seu servidor (inclua a
> porta se necessário, ex: `http://45.33.32.156:20128/callback`).

**4. Salve e copie as credenciais**

Após criar, o Google mostrará o **Client ID** e o **Client Secret**.

**5. Configure as variáveis de ambiente**

No seu `.env` (ou nas variáveis de ambiente do Docker):

```bash
# Para Antigravity:
ANTIGRAVITY_OAUTH_CLIENT_ID=seu-client-id.apps.googleusercontent.com
ANTIGRAVITY_OAUTH_CLIENT_SECRET=GOCSPX-seu-secret

# Para Gemini CLI:
GEMINI_OAUTH_CLIENT_ID=seu-client-id.apps.googleusercontent.com
GEMINI_OAUTH_CLIENT_SECRET=GOCSPX-seu-secret
GEMINI_CLI_OAUTH_CLIENT_SECRET=GOCSPX-seu-secret
```

**6. Reinicie OmniRoute**

```bash
# Jika menggunakan npm:
npm run dev

# Jika menggunakan Docker:
docker restart omniroute
```

**7. Mohon mencoba kembali**

Dashboard → Providers → Antigravity (atau Gemini CLI) → OAuth

Sekarang Google akan meredarasi dengan benar ke `https://server-mu.com/callback`
dan autentikasi akan bekerja.

---

#### Pemecahan sementara (tanpa konfigurasi kredensial sendiri)

Jika tidak ingin membuat kredensial sendiri sekarang, masih mungkin menggunakan
aliran **manual URL**:

1. OmniRoute akan membuka URL autorisasi Google
2. Setelah Anda memberi izin, Google akan mencoba merediris ke `localhost`
   (tetapi gagal di server jarak jauh)
3. **Salin URL lengkap** dari alamat URL browser Anda (bahkan jika halaman tidak
   terbuka)
4. Salin URL tersebut ke bidang yang muncul di modal koneksi OmniRoute
5. Klik **"Connect"**

> Pemecahan sementara ini berfungsi karena kode autorisasi dalam URL tetap valid
> meskipun redirect tidak berhasil.

</details>

---

</details>

## 🛠️ Tech Stack

<details>
<summary><b>Click to expand tech stack details</b></summary>

- **Runtime**: Node.js 18–22 LTS (⚠️ Node.js 24+ tidak **didukung** — `binerik
  native-sqlite3` tidak kompatibel)
- **Bahasa**: TypeScript 5.9 — **100% TypeScript** di seluruh `src/` dan
  `open-sse/` (tidak ada `apapun` dalam modul core sejak v2.0)
- **Framework**: Next.js 16 + React 19 + Tailwind CSS 4
- **Database**: LowDB (JSON) + SQLite (domain state + proxy logs + audit MCP +
  keputusan routing)
- **Schemas**: Zod (MCP alat I/O validasi, kontrak API)
- **Protokol**: MCP (stdio/HTTP) + A2A v0.3 (JSON-RPC 2.0 + SSE)
- Stream**Pemancaran**: Server-Sent Events (SSE)
- **Autoriti**: OAuth 2.0 (PKCE) + JWT + Kunci API + Pengawasan Menggunakan MCP
- **Pemantauan**: Pemancar ujian Node.js + Vitest (900+ ujian termasuk unit,
  pengintegrasian, E2E)
- **CI/CD**: GitHub Actions (auto nyalakan semula + Docker Hub pada waktu rilis)
- **Tapak web**: [omniroute.online](https://omniroute.online)
- **Paket**:
  [npmjs.com/package/omniroute](https://www.npmjs.com/package/omniroute)
- **Docker**:
  [hub.docker.com/r/diegosouzapw/omniroute](https://hub.docker.com/r/diegosouzapw/omniroute)
- **Kekuatan Tahan**: Pembatas sirkuit, backoff eksponensial, anti-thundering
  herd, mampasan TLS, auto-combo pemulihan sendiri

</details>

---

## Dokumentasi

| Dokumen                                        | Deskripsi                                                      |
| ---------------------------------------------- | -------------------------------------------------------------- |
| [Panduan Pengguna](docs/USER_GUIDE.md)         | Penyedia, kombinasi, integrasi CLI, pelancaran                 |
| [Panduan Rujukan API](docs/API_REFERENCE.md)   | Semua titik pangkalan data dengan contoh                       |
| [Pelayan MCP](open-sse/mcp-server/README.md)   | 16 alat MCP, konfig IP, klien Python/TS/Go                     |
| [Pelayan A2A](src/lib/a2a/README.md)           | Protokol JSON-RPC 2.0, kemahiran, pemancaran, pengurusan tugas |
| [Ingatan Kombinasi Auto](docs/auto-combo.md)   | Pemantauan 6 faktor, mode paket, penyembuhan diri              |
| [Troubleshutoo](docs/TROUBLESHOOTING.md)       | Masalah-masalah umum dan penyelesaian                          |
| [Arkitektur](docs/ARCHITECTURE.md)             | Arkitektur sistem dan komponennya                              |
| [Kegiatan Kontribusi](CONTRIBUTING.md)         | Pengaturan pengembangan dan pedoman                            |
| [Specifikasi OpenAPI](docs/openapi.yaml)       | Spesifikasi OpenAPI versi 3.0                                  |
| [Kebijakan Keselamatan](SECURITY.md)           | Laporan kelemahan dan amalan keselamatan                       |
| [Pengunduhan VM](docs/VM_DEPLOYMENT_GUIDE.md)  | Pedoman penuh: VM + nginx + Cloudflare                         |
| [Galeri Ciri-ciri](docs/FEATURES.md)           | Tur arahan dashboard visual dengan lukisan skrin               |
| [Senarai Kelulusan](docs/RELEASE_CHECKLIST.md) | Langkah-langkah penambahan pra-kelulusan                       |

---

## Petunjuk Arah

OmniRoute memiliki **210+ kemudahan yang terkelola** dalam beberapa fasa
pengembangan. Berikut adalah kawasan utama:

| Kategori                        | Ciri-ciri yang Dirancang | Peringatan                                                                                                         |
| ------------------------------- | ------------------------ | ------------------------------------------------------------------------------------------------------------------ |
| 💡 **Route & Intelektual**       | 25+                      | Pemantauan Latensi Terendah, Pemantauan Berdasarkan Tag, Pengujian Quota, Pilihan Neraca P2C                       |
| 🔒 **Keselamatan & Kesepahaman** | 20+                      | Peleburan SSRF, Penyamaran Kredit, Had Per Endpoint, Pengkonteksian Kunci Pengurusan                               |
| 📊 **Observabiliti**             | 15+                      | Integrasi OpenTelemetry, Pemantauan Quota Serta Merta, Pemantauan Kos Per Mod                                      |
| 🔄 **Integrasi Pembekal**        | 20+                      | Pendaftaran Model Dinamik, Jeda Pembekal, Pembekal Satu AkaunCodex, Pemerihalan Kuota Codipilot                    |
| ⚡ **Kinerja**                   | 15+                      | Pembinaan Layer Cache Dual, Caching Prompt, Caching Respons, Sambungan Streaming, API yang Dilakukan Sebagai Bilik |
| 🌐 **Ekosistem**                 | 10+                      | API WebSocket, Pemuatan Segera Konfigurasi, Gudang Konfigurasi Berpembagian, Mod Komersial                         |

### 🔜 Akan Datang Lebih Cepat

- 🔗 **Integrasi OpenCode** — Pensokongan Pembekal Asli untuk IDE AI Coding
  OpenCode
- 🔗 **Integrasi TRAE** — Dukungan penuh untuk kerangka kerja perkembangan AI
  TRAE
- 📦 **API Batch** — Proses batch asinkron untuk permintaan dalam jumlah besar
- 🎯 **Rute Berdasarkan Tag** — Jalankan permintaan berdasarkan tag-khusus dan
  metadata
- 💰 **Strategi Biaya Terendah** — Pilih secara otomatis penyedia yang paling
  murah

> 📝 Spesifikasi fitur penuh tersedia di [`docs/baru-fitur/`](docs/new-features/)
> (217 spesifikasi rinci)

---

## 👥 Pengembang

[![Contributors](https://contrib.rocks/image?repo=diegosouzapw/OmniRoute&max=100&columns=20&anon=1)](https://github.com/diegosouzapw/OmniRoute/graphs/contributors)

### Cara Berkontribusi

1. Geser cabang repository
2. Buat cabang fitur baru (`git checkout -b fitur/fitur-amen`)
3. Komit perubahan (`git commit -m 'Tambahkan fitur luar biasa'`)
4. Sampaikan ke cabang (`git push origin fitur/fitur-amen`)
5. Bukalah Pesanan Gabung

Lihat [[CONTRIBUTING.md](CONTRIBUTING.md)] untuk panduan rinci.

### Merekalui Versi Baru

```bash
# Merekalui versi — Terjadilah publishes otomatis dengan npm
gh release create v2.0.0 --title "v2.0.0" --generate-notes
```

---

## 📊 Riwayat Bintang

## Bintang-bintang dalam waktu

## [![Bintang-bintang dalam waktu](https://starchart.cc/diegosouzapw/OmniRoute.svg?variant=adaptive)](https://starchart.cc/diegosouzapw/OmniRoute)

## 🙏 Penghargaan Terima

Special thanks to **[9router](https://github.com/decolua/9router)** by
**[decolua](https://github.com/decolua)** — the original project that inspired
this fork. OmniRoute builds upon that incredible foundation with additional
features, multi-modal APIs, and a full TypeScript rewrite.

Special thanks to
**[CLIProxyAPI](https://github.com/router-for-me/CLIProxyAPI)** — the original
Go implementation that inspired this JavaScript port.

---

## 📄 License

MIT License - see [LICENSE](LICENSE) for details.

---

<div align="center">
  <sub>Built with ❤️ for developers who code 24/7</sub>
  <br/>
  <sub><a href="https://omniroute.online">omniroute.online</a></sub>
</div>
<!-- GitHub Discussions enabled for community Q&A -->
