# 🚀 OmniRoute — Porțiunea Gratuită a Gateway-ului AI

### Niciodată să încetezi să codezi. Rutearea inteligentă către **FREE & AI-modeluri costisite REDUZÂND ** cu declanșare automată.

_Proximitarea tău universală API — un endpoint, 67+ furnizori, zero downtime.
Acum cu agenta de orchestrare a protocolului MCP ȘI A2A._

**Chat Completări • Embedding-uri • Generarea imaginilor • Video • Music • Audio
• Reranking • **Căutare web** • Srv MCP • Protocolul A2A • 100% TypeScript**

---

<div align="center">

[![versiunea
npm](https://img.shields.io/npm/v/omniroute?color=cb3837&logo=npm)](https://www.npmjs.com/package/omniroute)
[![descărcări
npm](https://img.shields.io/npm/dm/omniroute?color=cb3837&logo=npm&label=npm%20downloads)](https://www.npmjs.com/package/omniroute)
[![Docker
Hub](https://img.shields.io/docker/v/diegosouzapw/omniroute?label=Docker%20Hub&logo=docker&color=2496ED)](https://hub.docker.com/r/diegosouzapw/omniroute)
[![Descărări
Docker](https://img.shields.io/docker/pulls/diegosouzapw/omniroute?logo=docker&color=2496ED&label=docker%20pulls)](https://hub.docker.com/r/diegosouzapw/omniroute)
[![Licență](https://img.shields.io/github/license/diegosouzapw/OmniRoute)](https://github.com/diegosouzapw/OmniRoute/blob/main/LICENSE)
[![Website](https://img.shields.io/badge/Website-omniroute.online-blue?logo=google-chrome&logoColor=white)](https://omniroute.online)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-Community-25D366?logo=whatsapp&logoColor=white)](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

[🌐 Website](https://omniroute.online) • [🚀 Start rapid](#-quick-start) • [💡
Caracteristici](#-key-features) • [📖 Documentație](#-documentation) • [💰
Prețuri](#-pricing-at-a-glance) • [💬
WhatsApp](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

</div>

🌐 **Disponibil în:** 🇺🇸 [Engleză](README.md) | 🇧🇷 [Portugheză
(Brazilia)](docs/i18n/pt-BR/README.md) | 🇪🇸 [Spaniolă](docs/i18n/es/README.md) |
🇫🇷 [Franțuză](docs/i18n/fr/README.md) | 🇮🇹 [Italiană](docs/i18n/it/README.md) |
🇷🇺 [Rusă](docs/i18n/ru/README.md) | 🇨🇳 [Chineza
(Simplificată)](docs/i18n/zh-CN/README.md) | 🇩🇪
[Germană](docs/i18n/de/README.md) | 🇮🇳 [Hindi](docs/i18n/in/README.md) | 🇹🇭
[Thai](docs/i18n/th/README.md) | 🇺🇦 [Ucraineană](docs/i18n/uk-UA/README.md) | 🇸🇦
[Arabă](docs/i18n/ar/README.md) | 🇯🇵 [Japoneză](docs/i18n/ja/README.md) | 🇻🇳
[Viets](docs/i18n/vi/README.md) | 🇧🇬 [Bulgară](docs/i18n/bg/README.md) | 🇩🇰
[Daneză](docs/i18n/da/README.md) | 🇫🇮 [Finnese](docs/i18n/fi/README.md) | 🇮🇱
[Ebraică](docs/i18n/he/README.md) | 🇭🇺 [Maghiară](docs/i18n/hu/README.md) | 🇮🇩
[Indoneză](docs/i18n/id/README.md) | 🇰🇷 [Coreeană](docs/i18n/ko/README.md) | 🇲🇾
[Malaeză](docs/i18n/ms/README.md) | 🇳🇱 [Olanda](docs/i18n/nl/README.md) | 🇳🇴
[Norvegiană](docs/i18n/no/README.md) | 🇵🇹 [Portugheză
(Portugalia)](docs/i18n/pt/README.md) | 🇷🇴 [Română](docs/i18n/ro/README.md) | 🇵🇱
[Polonă](docs/i18n/pl/README.md) | 🇸🇰 [Slovacă](docs/i18n/sk/README.md) | 🇸🇪
[Suedeză](docs/i18n/sv/README.md) | 🇵🇭 [Filipineză](docs/i18n/phi/README.md) |
🇨🇿 [Cehă](docs/i18n/cs/README.md)

---

## 🆕 Ce e nou în v3.0.0

> **Actualizarea de la v2.9.5?** — Vezi [logul schimbărilor
> complet](CHANGELOG.md#300--2026-03-22-release-candidate--not-yet-merged-to-main)
> pentru tot ce a fost schimbat.

| Zone                                | Schimbare                                                                                                                                                                                                        |
| ----------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🔒 **Securitate ** CodeQL            | Corectate 10+ avertizări CodeQL: polynomial-redos, inadecvarea randomness, remedierea injecției shell                                                                                                            |
| ✅ **Validerarea rutei**             | Toate 176 de rute API sunt acum validate cu schema Zod + `validateBody()` — CI ` verifică:route-validation:t06` înfăptuește                                                                                      |
| 🐛 **Zăpada de etichete omniModel ** | Etichetele interne `<omnimodel>` nu mai se scurg către clienți în răspunsurile fluxului de streaming SSE (#585)</omnimodel>                                                                                      |
| 🔑 **API Cheia Înregistrată**        | Aprovizionează cheia API automat prin `POST /api/v1/chei înregistrate` cu preluarea cotă obligatorie pentru fiecare furnizor/companie, idempotenie, stocare SHA-256 și raportarea opțională a problemelor GitHub |
| 🎨 **Ierarhia fournizorilor**        | 130+ logouri prin `@lobehub/iconuri` (SVG) cu fallback de tip PNG                                                                                                                                                |
| 🔄 **Model de sincronizare automat** | Un scheduler de 24h̆ și o alternativă manuală pentru a sincroniza lista de modele pentru furnizorii integrati și personalizați                                                                                   |
| 🌐 **OpenCode Zen/Go**               | Două noi furnizori din partea lui @kang-heewon prin PR #530: nivel gratuit și abonament                                                                                                                          |
| 🐛 **Gemini CLI OAuth**              | O eroare și mai clară când `GEMINI_OAUTH_CLIENT_SECRET` nu este disponibil în Docker (eror originală criptică de la Google)                                                                                      |
| 🐛 **Configurația Opencode**         | `salveazăConfigurațiaOpencode()` scrie acum corect Toml în `XDG_CONFIG_HOME`                                                                                                                                     |
| 🐛 **Model pins**                    | `corp.model` este corect setat pe `modelPins` pe protecția context-cache                                                                                                                                         |
| 🐛 **Codex/Claude loop**             | `rezultatulUt ` blocuri acum convertite în text pentru a opri ciclurile infinite                                                                                                                                 |
| 🐛 **Reîndreptarea de acces**        | Login-ul nu se blochează mai mult după ce se sărește setarea parolei                                                                                                                                             |
| 🐛 **Căutări de fise de pe Windows** | Păile MSYS2/Git-Bash (`/c/....`) normalizează automat în `C:\.....`                                                                                                                                              |

---

## 🖼️ Ghid pentru principal

<div align="center">
  <img src="./docs/screenshots/MainOmniRoute.png" alt="OmniRoute Dashboard" width="800"/>
</div>

---

## 📸 Prezentarea imaginilor

<details>
<summary><b>Click to see dashboard screenshots</b></summary>

| Pagină                   | Captură de ecran                                          |
| ------------------------ | --------------------------------------------------------- |
| **Furnizori**            | ![Furnizori](docs/screenshots/01-providers.png)           |
| **Combinări**            | ![Combinări](docs/screenshots/02-combos.png)              |
| **Analize**              | ![Analize](docs/screenshots/03-analytics.png)             |
| **Sănătate**             | ![Sănătate](docs/screenshots/04-health.png)               |
| **Traducător**           | ![Traducător](docs/screenshots/05-translator.png)         |
| **Setări**               | ![Setări](docs/screenshots/06-settings.png)               |
| **Utilitare CLI**        | ![Utilitare CLI](docs/screenshots/07-cli-tools.png)       |
| **Logs de utilizare**    | ![Logs de utilizare](docs/screenshots/08-usage.png)       |
| **Puncte de terminație** | ![Puncte de terminație](docs/screenshots/09-endpoint.png) |

</details>

---

### 🤖 Provedor AI gratuit pentru agenții de cod preferate ale tale.

_Conecta orice instrument IDE sau CLI alimentat de IA prin OmniRoute — API
gateway gratuit pentru codificarea nelimitată._

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

<sub>📡 Toți agenții se conectează prin <code>http://localhost:20128/v1</code>
sau <code>http://cloud.omniroute.online/v1</code> — unul singur, nelimitate
modeling și cote</sub>

---

## 🤔 De ce OmniRoute?

**Opri și risipește bani atârnând de la limitări:**

- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Cota de abonament expire neutilizată la sfârșitul lunii
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Limitările de rata te opresc în timp ce ești în cursul codificării
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  API-uri costisitoare ($20-50/lună pe fiecare furnizor)
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Trecerea manuală între furnizori

**OmniRoute rezolvă asta:**

- ✅ **Maximizează abonamentele** - Urmărește cota, utilizează fiecare mică
  bucățică înainte de a reset.
- ✅ **Fallback autom ** - Abonament → Cheie API → ieftin → Gratuit, fără
  întrerupere a activității
- ✅ **Multi-cont uri** - Rotați între conturi pe fiecare furnizor
- ✅ **Universal** - Funcționează cu Claude Code, Codex, Gemini CLI, Cursor,
  Cline, OpenClaw, orice instrument CLI

---

## 📧 Sprijin

> 💬 **Conectează-te la comunitatea noastră!** [Grup
> WhatsApp](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t) -
> Înscrie-te, împărtășește sfaturi, stai la curent.

- **Site-ul oficial **: [omniroute.online](https://omniroute.online)
- **GitHub**:
  [github.com/diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute)
- **Issue-uri**:
  [github.com/diegosouzapw/OmniRoute/issues](https://github.com/diegosouzapw/OmniRoute/issues)
- **WhatsApp**: [Grupul de
  Comunitate](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)
- **Contribuții**: Vezi [CONTRIBUTING.md](CONTRIBUTING.md), deschide un PR sau
  alege o `treabă bună de început`
- [Proiectul Original **]=Original Project**: [routerul 9] by
  decolua](https://github.com/decolua/9router)

### Ai Vrea să Raportezi o Eroare Bug?

Când deschizi o problemă, te rugăm să rulezi comanda system-info și să ataci
fișierul generat:

```bash
npm run system-info
```

Acest lucru generează un `system-info.txt` cu versiunea Node.js, versiunea
OmniRoute, detaliile sistemului, instrumentele CLI instalate (iflow, gemini,
claude, codex, antigravity, droid, etc.), statutul Docker/PM2, pachetele sistem
și tot ceea ce avem nevoie pentru a reproduce rapid problema ta. Atașează
fișierul direct problema ta GitHub.

---

## Cum funcționează

```
┌─────────────┐
│  CLI-ul tău │  (Claude Code, Codex, Gemini CLI, OpenClaw, Cursor, Cline...)
│   Instrument │
└──────┬──────┘
       │ http://localhost:20128/v1
       ↓
┌─────────────────────────────────────────┐
│           OmniRoute (Routerul Inteligent)  │
│  • Traducere format (OpenAI ↔ Claude) │
│  • Supraveghere a bugetului + Embeddings + Imagini │
│  • Autorefrescare a tokenului                 │
└──────┬──────────────────────────────────┘
       │
       ├─→ [Tier 1: ABONAMENT] Claude Code, Codex, Gemini CLI
       │   ↓ limita bugetului
       ├─→ [Tier 2: CHEIE API] DeepSeek, Groq, xAI, Mistral, NVIDIA NIM, etc.
       │   ↓ buget limitat
       ├─→ [Tier 3: ieftin] GLM ($0.6/1M), MiniMax ($0.2/1M)
       │   ↓ buget limitat
       └─→ [Tier 4: GRATUIT] iFlow, Qwen, Kiro (nespusul limitat)

Rezultat: Niciodata să te oprești de a codifica, cu cost minim
```

---

## 🎯 Ce rezolvă OmniRoute — 30 de puncte de durere reale și utilizare casnică

> **Orice dezvoltator care folosește instrumente AI se confruntă cu aceste
> probleme zilnic.** OmniRoute a fost construit pentru a rezolva toate acestea —
> de la supra Estimates la blocările regionale, de la fluxul OAuth rupt la
> operațiunile de protocol și observabilitatea de tip enterprise.

<details>
<summary><b>💸 1. "I pay for an expensive subscription but still get interrupted by limits"</b></summary>

Dezvoltatorii plătesc 20–200 $/lună pentru Claude Pro, Codex Pro sau GitHub
Copilot. Și plătind, există o limită de buget — 5 ore de utilizare, limite
săptămânale sau rate de limitare pe minut. În timpul unei sesiuni de codare,
furnizorul încetează să răspundă și dezvoltatorul pierde ritmul și
productivitatea.

**Cum rezolvă OmniRoute:**

- **Fallbackului 4-Tier Inteligent** — Dacă quota de abonare se epuizează,
  redirecționează automat la Cheia API → Cheap → Free cu zero intervenție
  manuală
- **Supravegherea în Timp Real a Bugetului** — Arată consumul tokenului în timp
  real cu numărul de reset (5 ore, zilnice, săptămânale)
- **Suportul Multi-Account** — Conturi multiple pe furnizor cu auto-întrecere —
  când una se termină, trece la următoarea
- **Combinațiile Personalizate** — Lanțuri de fallback personalizabile cu 6
  strategii de echilibrare (întâi, în cerc, P2C, la întâmplare, cel mai puțin
  utilizat, optimizat printr-un cost)
- **Quozele de Afaceri Codex** — Monitorizare a Quozelor contului de
  afaceri/spațiu de lucru în dashboard-ul dashboardului

</details>

<details>
<summary><b>🔌 2. "I need to use multiple providers but each has a different API"</b></summary>

OpenAI folosește un format, Claude (Anthropic) altul, Gemini un altul tot. Dacă
va fi un dev care dorește să testeze modele din diferite furnizori sau să se
întrerupă între ei, ei trebuie să redesigure SDK-uri, să schimbe punctele de
acces, să se confrunte cu formate incompatibili. Furnizori personalized
(FriendLI, NIM) au puncte de acces de tip model nu standard.

**Cum rezolvă OmniRoute:**

- **Punctul de Conectare Unificat** — Un singur `http://localhost:20128/v1`
  serveste ca și proxy pentru toate furnizorii
- **Traducerea Formatului** — Automat și transparent: OpenAI ↔ Claude ↔ Gemini ↔
  API de Răspuns
- Răspuns sanitarizare** — Elimină câmpurile ne-standard `, `, ` care încalcă
  API-ul SDK v1.83+ al OpenAI
- Normalizarea rolului** — Convertește ` entitate sistem ` pentru furnizorii
  non-OpenAI; ` utilizator ` pentru GLM/ERNIE
- Extracția tokenului pentru tagul de gândire** — Extrage blocurile <think>` din
  modelele ca DeepSeek R1 în conținutul standardizat de raționament`</think>
- Output structurat pentru Gemini** — Convertire automată a ` schema de
  răspuns`/` schema de răspuns din json`
- `stream` este implicat implicit** — Corespunde specificației OpenAI, evitând
  SSE inesperate în SDK-urile Python/Rust/Go

</details>

<details>
<summary><b>🌐 3. "My AI provider blocks my region/country"</b></summary>

Folositorii blocări de acces din anumite regiuni geografice. Utilizatorii
primesc erori comoară ` în timpul conexiunii OAuth și API.

**Cum rezolvă OmniRoute:**

- Configurarea proxyului cu nivel de protecție 3** — Configurabil în trei
  nivele: global, per-furnizor și per-conexiune/cheg și cheie
- Etichete colorate pentru proxy-uri** — Indici vizuali: 🟢 global proxy, 🟡
  furnizor proxy, 🔵 conexiune proxy, arătând întotdeauna IP-ul
- Intercalare OAuth prin intermediul proxyului** — Fluxul OAuth traversează și
  proxy (șterse problema `)
- Teste de conexiune prin intermediul proxyului** — Testele de conexiune
  folosesc proxy-ul configurat (măcar nu se face înconjurarea directă)
- Sprijin pentru SOCKS5** — Suport SOCKS5 pentru transmiterea în afara rețelei
- Impersonarea semnăturii de certificate TLS** — Semnătură de certificate TLS ca
  la un browser, folosind wreq-js pentru a depăși detectarea bot-urilor
- Conformare a semnăturii CLI** — Redeschidează câmpurile pentru a combina cu
  semnatura natively a binarelor CLI, reducând drastic riscul de sesizare de
  cont.

</details>

<details>
<summary><b>🆓 4. "I want to use AI for coding but I have no money"</b></summary>

Nu oricine poate ajunge [X198X] și [X203X] pentru abonamente către AI.

**Cum rezolvă OmniRoute:**

- Furnizorii de tip free-tier natively integrati** — Suport native pentru
  furnizorii ca iFlow, Qwen și Kiro
- Ollama Cloud** — Ollama cloud-hosted pe ` api.ollama.com` cu un tarif "Light
  usage" gratuit
- Combinații gratuite** — Averșeaza ` combinați iefor `
- Acces liber NIM NVIDIA** — Accesul pentru dev-uri in perpetuar ** la peste
  [X70X]+modele la [X30X] build.nividia.com
- **Cost Optimizat Cu Optimizare Strategii** — Strategia de routing automat care
  alege furnizorul cheapest disponibil

</details>

<details>
<summary><b>🔒 5. "I need to protect my AI gateway from unauthorized access"</b></summary>

Când expuneți un gateway AI spre rețea (LAN, VPS, Docker), oricine dispune de
adresă poate consuma tokenurile/dezvoltatorul cuantum. În absența protecției,
API-urile sunt vulnerabile la uzură, injecția cu prompturi și abuz.

**Cum rezolvă OmniRoute:**

- **Managementul Cheii API** — Génération, rotativă și permisivă la furnizor
  special cu o pagină dedicată `/dashboard/api-manager`
- **Autorizarea La Nivelul Modelului** — Restricționează cheile API la modele
  specifice (`openai/*`, modele cu pâslini), cu un buton Allow All/Restrict
- **Protejarea Punctului de Acces API** — Aici pentru `/v1/models` și blocă
  furnizorii specifice din lista
- **Guardul Aut+CSRF Protecția** — Toate rutele dashboad protejate cu `withAuth`
  middleware + tokenuri CSRF
- **Limitatorul De Rate** — Limitator de rate pentru IP-uri, cu ferestre
  configurabile
- **Filtrația Pachetelor IP** — Permise blocă/blocklist pentru controlarea
  accesului
- **Grinda Razoare de Inject Prompt** — Sanitizarea împotriva tuturor
  pattern-urilor de prompt malici
- **Criptarea AES-256-GCM** — Cheile criptate la stânghit

</details>

<details>
<summary><b>🛑 6. "My provider went down and I lost my coding flow"</b></summary>

Furnizorii AI pot deveni instabili, să returneze eroarea 5xx sau să atingă
limitele de rată temporare. Dacă un dev depinde de furnizorul unic, el este
întrerupt. Fără dispozitiv de stingare, încercările repetate pot face ca
aplicația să se prăbușească.

**Cum rezolvă OmniRoute:**

- **Dispozitivul Stinge Circuit în Model** — Închis/Deschis/Deschis pe jumâtate
  cu praguri configurabile și cooldown, la scară model, pentru a evita blocările
  consecutive
- **Backoff Exponențial** — Încercări retardate progresive
- **Herda Împotriva Thundering** — Protecție mutex + semafor împotriva
  potopurilor de încercări consecutive
- **Combina Fallback Chain** — Dacă furnizorul primar eşuează, se cade în lanț
  cu combina automat
- **Gardianul Circuli din Combo** — împiedică furnizorii eşuați în combina să
  fie închisi automat
- **Bureaurile de Zonă de Sănătate** — monitorizarea uptime, starea
  dispozitivului de stingere, blocări, statistici cache, p50/p95/p99 latență

</details>

<details>
<summary><b>🔧 7. "Configuring each AI tool is tedious and repetitive"</b></summary>

Dvs, dezvoltatorii folosesc Cursor, Claude Code, Codex CLI, OpenClaw, Gemini
CLI, Kilo Code... Fiecare instrument are o config diferențiată (punct de acces
API, cheie, model). Reconfigurarea atunci când se schimbă furnizorii sau
modelurile este un abuz de timp.

**Cum rezolvă OmniRoute:**

- **Interfeța CLI a Dashboard-ului** — Pagină dedicată cu acces direct pentru
  Claude Code, CLI pentru Codex, OpenClaw, Kilo Code, Antigravity, Cline
- **Generatoare de configurări pentru GitHub Copilot** — Generează
  `chatLanguageModels.json` pentru VS Code cu selecție în bloc a modelului
- **Ghid de onboarding** — Setare ghidată de 4 pași pentru utilizatorii noi
- **Un punct de acces, toate modelurile** — Configură
  `http://localhost:20128/v1` doar o dată, accesează 67+ furnizori

</details>

<details>
<summary><b>🔑 8. "Managing OAuth tokens from multiple providers is hell"</b></summary>

Claude Code, Codex, Gemini CLI, Copilot — toate folosesc OAuth 2.0 cu token-uri
expirabile. Dezvolotorilor le este nevoie să se reautentifice permanent, să
gestioneze `client_secret este lipsă`, `redirect_uri_mismatch` și eșecurile pe
serverele remote. OAuth în LAN/VPS este în special problematic.

**Cum rezolvă OmniRoute:**

- **Refrescare automată a tokenurilor** — Tokenurile OAuth se refreshă în fundal
  înainte de expirare
- **OAuth 2.0 (PKCE) Integrat** — Curs automat pentru Claude Code, Codex, Gemini
  CLI, Copilot, Kiro, Qwen, iFlow
- **Multi-Account OAuth** — Conturi multiple pe furnizor prin extracție a
  tokenilor JWT/ID
- **Fixarea OAuth pentru LAN/Remote** — Detectare a adresei private pentru
  `redirect_uri` + mod de manualizare a URLei pentru serverele remote
- **Integrarea OAuth în Nginx** — Utilizează `window.location.origin` pentru
  compatibilitatea cu reverse proxy
- **Ghidul pentru autorizarea OAuth Rețea-X** — Ghid paș cu paș pentru
  credențialele Google Cloud pe VPS/Docker

</details>

<details>
<summary><b>📊 9. "I don't know how much I'm spending or where"</b></summary>

Dezvolotorii folosesc multiple furnizori plătiți dar nu au o vedere unificată a
cheltuielilor. Fiecare furnizor are propria sa panou de administrare a
cheltuielilor dar nu există o vedere consolidată a cheltuielilor. Cheltuielile
neprevăzute pot suma.

**Cum rezolvă OmniRoute:**

- **Dashboard-ul de Analiză a Costurilor** — Urmarirea costurilor pe token și
  gestionarea bugetului pe furnizor
- **Limite de buget pe tier** — Sfat superior de cheltuire pe nivel care
  declanșează automat fallback-ul
- **Configurarea prețurilor modelului** — Prețuri configurabile pe model
- **Statistici de utilizare pe cheie API** — Numărul de răspunsuri și timpii de
  ultimă utilizare per cheie
- **Dashboard-ul de Analiză** — Carte vizuală a statisticii, graficul utilizării
  modelelor, tabel al furnizorilor cu rata de reușită și latență.

</details>

<details>
<summary><b>🐛 10. "I can't diagnose errors and problems in AI calls"</b></summary>

[X0X]Atunci când o apelare eșuează, dezvoltatorul nu știe dacă a fost limitat de
taxa, expirat tokenul, formatul greșit sau erorile fournitorului. Fragmentarea
registrelor în diferite terminale fără vizibilitate îngreunează debugarea.
Debbugingul este o încercare și eroare.

**Cum rezolvă OmniRoute:**

- **Panou integrat pentru Registre Unificate** — 4 submeniuri: Registre
  Solicitanților, Proximători Registre, Registre Audit, Consolă
- **Vizualizator Registrelor Consolă** — privire în timp real a unui viewer cu
  terminal, cu niveluri colorate, auto-scroll, cauterare și filtrare
- **Registre Proximatoare persistente cu SQLite** — registre persistente care
  supraviețuiesc rebooturilor serverului
- **Jardiniere de Traducător** — 4 moduri de debugging: jardiniere (traducere
  format), testator chat (rotund), pavilionul de teste (buletin), monitorul
  real-timp (real-timp)
- **Tehnicul Solicitanților de Cerere** — retard p50/p95/p99 + X-Request-Id cu
  trasee
- **Registrează și închiderea fișierelor cu Rotare** — interceptorul console
  captură toate la un fișier log JSON cu rotire pe baza a mărimii
- **Raportul Informațiilor Sistemului** — `npm run system-info` generează
  `system-info.txt` cu mediul său complet (v. Node, v. OmniRoute, OS,
  instrumente CLI, statut Docker/PM2). Înșurubați-l atunci când raportați
  probleme pentru o clasificare instant.

</details>

<details>
<summary><b>🏗️ 11. "Deploying and maintaining the gateway is complex"</b></summary>

Instalarea, configurarea și întreținerea unui broker artificial în diferite
medii (lokal, VPS, Docker, cloud) este un lucru greu și laborios. Probleme ca
căi hardcodate, `EACCES` pe directorii, conflicturi de ușă și construcții
transplatform îl fac pe cineva să se strecoare.

**Cum rezolvă OmniRoute:**

- **npm instalare global** — `npm instalare -g ierarhie omni și ierarhie omni` —
  făcut
- **Dockerul cu mai multe Platforme** — AMD64 + ARM64 nativă (Apple Silicon, AWS
  Graviton, Raspberry Pi)
- **Profilele Dockerului cu Compoză** — `scurt` (sine instrumente CLI) și `CLI`
  (cu Claude Code, Codex, OpenClaw)
- **Aplicația Desktop Electron** — aplicarea nativă pentru Windows/macOS/Linux
  cu șaua sistemului, auto-start, modul offline
- **Modul Portului Split** — API și Consolă pe porturi separate pentru scenarii
  avansate (reverse proxy, rețea containeră)
- **Sincronizare Cloud** — sincronizarea rețelei configuri pe dispozitive cu
  Workerii Cloudflare
- **Backupuri de Baza de Date** — backup automat, restaurare, export și import a
  tuturor setărilor

</details>

<details>
<summary><b>🌍 12. "The interface is English-only and my team doesn't speak English"</b></summary>

Echipele din țările sălișteşti, mai ales din America Latină, Asia și Europa, au
dificultăți cu interfețele doar în limba engleză. Barierele de limbă scad
adoptarea și măresc erorile de configurare.

**Cum rezolvă OmniRoute:**

- **Interfață dashboard i18n — 30 de limbi** — Toate cheile 500+ traduse,
  inclusiv Arabic, bulgară, daneză, germană, spaniolă, finlandeză, franceză,
  ebraică, hindi, maghiară, indoneziană, italiană, japoneză, coreeană, malaieză,
  olandeză, norvegiană, polonă, portugheză (PT/BR), română, rusă, slovacă,
  suedeză, thailandeză, ucraineană, vietnameză, chineză, filipineză, engleză
- **Spăt de text și citire din dreapta la stânga** — Sprijin pentru limbi scrise
  din dreapta către stânga
- **Manual pentru limbă Multiple** — 30 de traduceri complete ale documentației
- **Selector de limbă** — Icoana glob pentru schimbarea real-time

</details>

<details>
<summary><b>🔄 13. "I need more than chat — I need embeddings, images, audio"</b></summary>

AI nu este doar completarea conversației. Dezvoltatorii au nevoie să genereze
imagini, să transcrie audio, să creeze embeduri pentru RAG, să reordoneze
documentele și să moderere continutul. Fiecare API are un punct de final
terminat diferit și format.

**Cum rezolvă OmniRoute:**

- **Embeduri** — `/v1/embeddings` cu șase furnizori și 9+ modele
- **Generarea de imagini** — `/v1/images/generations` cu 10 furnizori și 20+
  modele (OpenAI, xAI, Together, Fireworks, Nebius, Hyperbolic, NanoBanana,
  Antigravity, SD WebUI, ComfyUI)
- **Text-to-Video** — `/v1/videos/generations` — ComfyUI (AnimateDiff, SVD) și
  SD WebUI
- **Text-to-Music** — `/v1/music/generations` — ComfyUI (Stable Audio Open,
  MusicGen)
- **Transcrierea audio** — `/v1/audio/transcriptions` — Whisper + Nvidia NIM,
  HuggingFace, Qwen3
- **Text-to-Speech** — `/v1/audio/speech` — ElevenLabs, Nvidia NIM, HuggingFace,
  Coqui, Tortoise, Qwen3, **Inworld**, **Cartesia**, **PlayHT**, + furnizori
  existenți
- **Moderare** — `/v1/moderations` — Verificări de siguranță a continutului
- **Reordonează** — `/v1/rerank` — Reordonează relevanța documentelor
- **Răspunsurile API** — Suport complet pentru `/v1/responses` Codex

</details>

<details>
<summary><b>🧪 14. "I have no way to test and compare quality across models"</b></summary>

Dezvoltatorii doresc să știe care sunt cele mai bune modele pentru utilizarea
lor — cod, traducere, raționament — dar comparația manuală este lentă. Nu există
instrumente integrate de evaluare.

**Cum rezolvă OmniRoute:**

- **Evaluare LLM** — Testarea cu setul de aur, cu 10 cazuri pre-testate
  acoperind salutări, matematică, geografie, generarea de cod, respectarea
  formatului JSON, traducere, markdown, respingerea de siguranță
- **4 Strategii Match** — `exact`, `containse`, `regex`, `custom` (funcția JS)
- **Testare de joc de traducere Plaje de testare cu multiple intrări și ieșiri,
  comparare inter-provedor
- Testatorul de **Discuție** — Rutina completă pe drumuri cu reprezentare
  vizuală a răspunsului
- Monitorul în timp real **Live Monitor** — Flux real-time al tuturor cererilor
  care curg prin proxy

</details>

<details>
<summary><b>📈 15. "I need to scale without losing performance"</b></summary>

Când volumul de cereri crește, fără utilizarea unei cache, aceleași întrebări
generează costuri duplicate. Fără idempotență, cererile duplicate devorează
resurse de procesare. Limitele de rata per furnizor trebuie păstrate în vedere.

**Cum rezolvă OmniRoute:**

- [Cachierul semantic]** Semantic Cache** — Cache de două nivele (semnătură +
  semantică) reduce costul și latența
- [idempotența în funcție de cerere]** Request Idempotency** — Fereastra de
  deduplicare de 5 secunde pentru cereri identice
- [Dectare rate limit]** Rate Limit Detection** — Tratarea RPM per furnizor,
  minim gap, și maximul sincronizat în concurentă
- [Limițele rate editabile]** Editable Rate Limits** — Valorile în funcție de
  configurare în Setări → Reziliem cu persistență
- [Cachierul chei API]** API Key Validation Cache** — Cache de trei nivele
  pentru performance în producție
- [Panoul deashboard cu telemetrie]** Health Dashboard with Telemetry** —
  P50/P95/P99 latență, statistici cache, uptime

</details>

<details>
<summary><b>🤖 16. "I want to control model behavior globally"</b></summary>

Dezvoltatorii care doresc ca răspunsurile să fie într-o anumită limbă, cu un
anumit ton, sau să limiteze tokenurile de argumentare. Configurarea acestui în
fiecare instrument/ cerere este impracticabilă.

**Cum rezolvă OmniRoute:**

- [Injecția prompturilor în funcție de sistem]** System Prompt Injection** —
  Prompt global aplicat tuturor cererilor
- [validarea bugetului gândirii]** Thinking Budget Validation** — Controlul
  alocării tokenurilor de argumentare pe cerere (trecere înainte, automat,
  adaptiv, configurabil)
- [Strategiile de rutare]** 6 Routing Strategies** — Strategii globale care
  determină distribuția cererilor
- [Rutera wildcard]** Wildcard Router** — `furnizor/*` modele care rutează
  dinamic la orice furnizor
- [Permiabilitatea combineniilor]** Combo Enable/Disable Toggle** — Butoanele
  directe pentru a permite/disabilita combinații din dashboard
- [Activarea/deactivarea furnizorului]** Provider Toggle** — Disabilizează
  conexiunile pentru un furnizor cu un singur click
- [Procedurile incluse din furnizori blocați]** Blocked Providers** — Exclud
  fără văz, furnizori anumiți din `/v1/models` liste

</details>

<details>
<summary><b>🧰 17. "I need MCP tools as first-class product capabilities"</b></summary>

Multii gateways AI fac publicate MCP doar ca detalii de implementare ascunsă.
Echipele au nevoie de o operatiune vizibilă, manejabilă.

**Cum rezolvă OmniRoute:**

- Navegarea din panoul de control conține MCP și tabul protocol de endpoint
- Pagină personalizată de gestionare a MCP cu proces, instrumente, scopuri și
  audit
- Start rapid integrat pentru `omniroutetot ipul MCP` și client pentru a se
  onboaerd

</details>

<details>
<summary><b>🧠 18. "I need A2A orchestration with sync + stream task paths"</b></summary>

Workflows pentru agenți necesiteând ambele răspunsuri directe și executarea
curentă cu control de lifecycle

**Cum rezolvă OmniRoute:**

- Endpoint JSON-RPC pentru A2A ( `POST /a2a` ) având `mesaj/trimite` și `mesaj/
  flux`
- Streaming SSE cu propagare a stării terminale
- API-uri de life-cycle pentru `taskuri/get` și `taskuri/cancel`

</details>

<details>
<summary><b>🛰️ 19. "I need real MCP process health, not guessed status"</b></summary>

Echipele operative trebuie să știe dacă MCP este în viață, nu numai dacă un API
este accesibil

**Cum rezolvă OmniRoute:**

- Fișier corectură de inimă pentru PID, timpii de timestamp, transmis, numărul
  de instrument și modul de scop
- API de stat al MCP care combină încredințarea + activitatea recentă
- Cărți de stat din UI pentru proces/putureță/ corectură a pulsului

</details>

<details>
<summary><b>📋 20. "I need auditable MCP tool execution"</b></summary>

În momentul în care instrumentele se schimbă configurația sau triggerează
acțiuni de automatizare, echipele au nevoie de un proces de urmărire forensă

**Cum rezolvă OmniRoute:**

- Jurnalarea auditare bazată pe SQLite pentru apelurile de instrumentelor MCP
- Filterează după instrument, succes/fiasco, API key și paginare
- Tabelul de audit și endpointuri statistice pentru automatizare pentru panoul
  de control

</details>

<details>
<summary><b>🔐 21. "I need scoped MCP permissions per integration"</b></summary>

Diferite clienți trebuie să aibă acces cel puțin de privilegiu la categoriile de
instrumente.

**Cum rezolvă OmniRoute:**

- 9 domenii fine detalii de rezolvare a acceselor la instrumente controlate
- Implementarea și vizibilitatea aplicării acestor domenii în interfața de
  administrare MCP
- Poziția de siguranță implicită pentru operațiunile de instrumentare

</details>

<details>
<summary><b>⚙️ 22. "I need operational controls without redeploying"</b></summary>

Echipele necesită schimbări rapide în timpul de execuție la incidente sau la
evenimente cauzate de cost

**Cum rezolvă OmniRoute:**

- Activarea combinației de comenză direct din interfața de instrumentare a MCP
- Aplicarea profilurilor de rezistență din pachetele de politică definite în
  prealabil
- Respingerea stăririi breakerului de circuit din panoul de operații

</details>

<details>
<summary><b>🔄 23. "I need live A2A task lifecycle visibility and cancellation"</b></summary>

Fără vizibilitate a ciclului de viață, incidentele de sarcină devin greu de
triaj

**Cum rezolvă OmniRoute:**

- Listarea și filtrarea sarcinilor după stare/skill cu paginare
- Forțarea-în jos pe metadata, evenimente și artefacte ale sarcinii
- Pentru a renunța la sarcina, se va trimite un endpoint și se va afișa un
  mensaj de confirmare

</details>

<details>
<summary><b>🌊 24. "I need active stream metrics for A2A load"</b></summary>

Fluxurile de lucru care se difuzează necesită perspectivă asupra concurenței și
conexiuni în timp real

**Cum rezolvă OmniRoute:**

- Cifre active de flux integrate în starea A2A
- Ultimultimestamp al sarcinii și numerele de stări per sarcină
- Carduri A2A care urmăresc monitorizarea in timp real a operațiunilor

</details>

<details>
<summary><b>🪪 25. "I need standard agent discovery for clients"</b></summary>

Exterii clienți și orchestratori au nevoie de metadata citirile de mașină pentru
onboardarea clienților

**Cum rezolvă OmniRoute:**

- Cardul Agent expus la `/well-known/agent.json`
- Abilitățile și cunostințele prezentate în panoul de management
- API-ul de stare A2A include metadata de descoperire pentru automatizarea

</details>

<details>
<summary><b>🧭 26. "I need protocol discoverability in the product UX"</b></summary>

Dacă utilizatorii nu pot descoperi suprafețele de protocol, calitatea de adopție
și a implicarea scad.

**Cum rezolvă OmniRoute:**

- Pagină de endpoate consolidate **Endpoate** cu butoane pentru Proxy, MCP, A2A
  și API Endpoate
- Butoane de stare de serviciu rulat (Online/Offline) pentru MCP și A2A
- Legături din rezumat către tabele de management dedicate

</details>

<details>
<summary><b>🧪 27. "I need end-to-end protocol validation with real clients"</b></summary>

Testele de simulare nu sunt suficiente pentru a valida compatibilitatea
protocolului înainte de lansare.

**Cum rezolvă OmniRoute:**

- Suita de teste end-to-end care pornește aplicația și utilizează un transport
  real pentru clientul SDK MCP
- Teste pentru clientul A2A pentru fluzele de descoperire, trimite, stream,
  obține și anulează
- Verificări de aserțiuni împotriva API-urilor de audit MCP și A2A

</details>

<details>
<summary><b>📡 28. "I need unified observability across all interfaces"</b></summary>

Divizarea observabilității în funcție de protocol creează zone călcate și crește
timpul mediu de reparare.

**Cum rezolvă OmniRoute:**

- Tablouri unite de grafice, loguri și statistici într-un singur produs
- Telemetria de stare + audit + cereri pentru straturile OpenAI, MCP și A2A
- API-uri operaționale pentru stare și automatizare

</details>

<details>
<summary><b>💼 29. "I need one runtime for proxy + tools + agent orchestration"</b></summary>

Rularea a multor servicii separate crește costul de operare și numărul de
scenarii de eşec.

**Cum rezolvă OmniRoute:**

- Proximus OpenAI compatibil, server MCP și A2A într-un stack unic
- Autentificare comună, reziliență, stocare de date și observabilitate
- Model de politică consistent pe toate suprafețele de interacțiune

</details>

<details>
<summary><b>🚀 30. "I need to ship agentic workflows without glue-code sprawl"</b></summary>

Echipele pierd ritmul atunci când stichează servicii și scrieri multiple de
ad-hoc.

**Cum rezolvă OmniRoute:**

- Strategie unificată de endpoint pentru clienți și agenți
- Interfețe de gestionare a protocoalelor integrate și căi de validare a fumului
  de siguranță
- Bazele de producție gata (securitate, protocolizare, reziliență, copie de
  rezervă)

</details>

### Exemple de Playbook-uri (utilizări integrate)

**Playbook A: Maximizați abonamentul plătit + backup scump**

```txt
Combo: "maximize-claude"
  1. cc/claude-opus-4-6
  2. glm/glm-4.7
  3. if/kimi-k2-thinking

Cost lunar: $20 + micul spend pentru backup
Rezultat: calitate mai mare, aproape zero întrerupere
```

**Playbook B: Stivă de codare zero-cost**

```txt
Combo: "free-forever"
  1. gc/gemini-3-flash
  2. if/kimi-k2-thinking
  3. qw/qwen3-coder-plus

Cost lunar: $0
Rezultat: flux de codare stabil și gratuit
```

**Playbook C: Lanț de cădere 24/7 întotdeauna**

```txt
Combo: "întotdeauna on"
  1. cc/claude-opus-4-6
  2. cx/gpt-5.2-codex
  3. glm/glm-4.7
  4. minimax/MiniMax-M2.1
  5. if/kimi-k2-thinking

Rezultat: adâncime profundă de cădere pentru sarcini cu termene limită critice
```

**Playbook D: Operațiuni de agent cu MCP + A2A**

```txt
1) Începe transportul MCP (`omniroute --mcp`) pentru operațiuni efectuate prin instrumente
2) Rulați sarcinile A2A prin `message/send` și `message/stream`
3) Observeți prin /dashboard/endpoint (setări de tab-uri MCP și A2A)
4) Schimbați serviciile folosind controale de statut în linie
```

---

## 🆓 Începeți Gratuit — Nici o Costă de Configurare

> Instituiți codarea AI în minute pe **$0/month**. Conectați aceste conturi
> gratuite și utilizați setarul integrat **Free Stack** combo.

| Etapă | Acțiune                                                                           | Părțile furnizorului descoperite                               |
| ----- | --------------------------------------------------------------------------------- | -------------------------------------------------------------- |
| 1     | Conectează **Kiro** (Clitorisul Construcției AWS OAuth)                           | Claude Sonnet 4.5, Haiku 4.5 — **nelimitat**                   |
| 2     | Conectează **iFlow** (OAuth Google)                                               | kimi-k2-gând, qwen3-coder-plus, deepseek-r1... — **nelimitat** |
| 3     | Conectează **Qwen** (Codul dispozitivului)                                        | qwen3-coder-plus, qwen3-coder-flash... — **nelimitat**         |
| 4     | Conectează **Gemini CLI** (Google OAuth)                                          | gemini-3-flash, gemini-2.5-pro — **180K/mo gratuit**           |
| 5     | `/Panoul de monitorizare a combinațiilor` → **Stack gratuit (0$)** fișier de temă | Trezoriți automat toate furnizorii gratuit.                    |

**Puteți să aplicați oriți-vă editor/CLI pe:** `http://localhost:20128/v1` ·
Cheia API: `o oricum-doi` · Terminat.

> **Acoperirea opțională suplimentară (tot gratuită):** cheia API Groq (30 RPM
> gratuit), NVIDIA NIM (40 RPM gratuit, 70+ modele), Cerebra (1M tok/day), Cheia
> API LongCat (50M token/day!).

## Pornire rapidă

### 1. Instalați și rulați

```bash
npm install -g omniroute
omniroute
```

> **pnpm users:** Rulaţi `pnpm approve-builds -g`după instalare pentru a activa
> scripturile de construcţie native necesare de `better-sqlite3` şi `@swc/core`:
> 
> ```bash
> pnpm install -g omniroute
> pnpm approve-builds -g   # Selectaţi toate pachetele → aprobă
> omniroute
> ```

Interfața de comenză deschide la `http://localhost:20128` și adresa de bază a
API-ului este `http://localhost:20128/v1`.

| Comandă                 | Descriere                                                         |
| ----------------------- | ----------------------------------------------------------------- |
| `omniroute`             | Start server (`PORT=20128`, API și interfață în porturi identice) |
| `omniroute --port 3000` | Seta portul canonical/ API la 3000                                |
| `omniroute --mcp`       | Start server MCP (transport stdio)                                |
| `omniroute --no-open`   | Nu deschide automat browsere                                      |
| `omniroute --help`      | Arată ajutorul                                                    |

Modul split-port opţional:

```bash
PORT=20128 DASHBOARD_PORT=20129 omniroute
# API:       http://localhost:20128/v1
# Interfața de dash: http://localhost:20129
```

### 2) Conectați furnizorii și creați cheia dvs. API

1. Deschideți Dashed → `Furnizori` și conectați-vă la cel puțin un furnizor
   (OAuth sau cheie API).
2. Deschideți Dashed → `Puncte de final și creați cheia dvs. API.
3. (Opțional) Deschideți Dashed → `Combinații` și setați lanțul defallback.

### 3) Punctați instrumentul dvs. de programare către OmniRoute

```txt
Adresa de bază: http://localhost:20128/v1
Cheia API: [copiați din pagina Puncte de final)
Model:    if/kimi-k2-pensând (sau orice prefix de furnizor/producător)
```

Funcționează cu Claude Code, Codex CLI, Gemini CLI, Cursor, Cline, OpenClaw,
OpenCode, și SDK-uri compatibile cu OpenAI.

### 4) Activează și validatează protocoalele (v2.0)

**MCP (pentru operațiuni ridicate de instrumente):**

```bash
omniroute --mcp
```

Apoi conectați clientul MCP peste `stdio` și testați instrumente precum:

- `omniroute_get_health`
- `omniroute_list_combos`

**A2A (pentru fluxuri agenților cu agenți):**

```bash
curl http://localhost:20128/.well-known/agent.json
```

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"quickstart","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"Ofereți-mi o rezumat scurt de cotă."}]}}'
```

### 5) Validați totul final la finalizare (recomandat)

```bash
npm run test:protocols:e2e
```

Acest set de teste validează fluxuri MCP și A2A CLI reale împotriva unei
aplicații rulete.

### Alternativ: executați din surse

```bash
cp .env.example .env
npm install
PORT=20128 DASHBOARD_PORT=20129 NEXT_PUBLIC_BASE_URL=http://localhost:20129 npm run dev
```

---

## 🐳 Container Docker

OmniRoute este disponibil ca o imagine publică a Docker-ului pe [Hub do
Docker](https://hub.docker.com/r/diegosouzapw/omniroute).

[R0R]Start rapid:[R12R]

```bash
docker run -d \
  --name omniroute \
  --restart unless-stopped \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:ultimul
```

[R0R]Cu fișierul de mediu:[R24R]

```bash
# Copiați și modificați .env înainte de a face acest lucru
cp .env.example .env

docker run -d \
  --name omniroute \
  --restart unless-stopped \
  --env-file .env \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:ultimul
```

[R0R]Utilizând Docker Compose:[R23R]

```bash
# Profilul de bază (fără instrumente CLI)
docker compose --profile bază up -d

# Profilul CLI (Claude Code, Codex, OpenClaw construit în mod intern)
docker compose --profile cli up -d
```

| Imagine                      | Etichetă        | Dimensiune | Descriere               |
| ---------------------------- | --------------- | ---------- | ----------------------- |
| [diegosouzapw/omnirouteR23R] | [ultimulR7R]    | ~250MB     | Ultima versiune stabilă |
| [diegosouzapw/omnirouteR23R] | [R0R]1.0.3[R6R] | ~250MB     | Versiune curentă        |

---

## 🖥️ Aplicație de birou — Offline & tot timpul-On

> 🆕 **Nou** OmniRoute este acum disponibil ca o aplicație **de birou nativ**
> pentru Windows, macOS și Linux.

Rulează OmniRoute ca o aplicație de birou standalone - nu e necesară nicio
terminală, niciun browser, nici internet pentru modele locale. Aplicația bazată
pe Electron include:

- 🖥️ **Fereastra nativă** — Fereastră dedicată a aplicației cu integrare în
  sistemul de tray
- 🔄 **pornire automat** —pornirea OmniRoute la login-ul sistemului
- 🔔 **Avertizări native** — Avertizări pentru epuizarea cotei sau pentru
  problema furnizorului
- ⚡ **Instalare directă** — NSIS (Windows), DMG (macOS), AppImage (Linux)
- 🌐 **Mod offline** — Functionează complet offline cu serverul integrat

### Pornire rapidă

```bash
# Modul de dezvoltare
npm run electron:dev

# Construiește pentru platforma ta
npm run electron:build         # Platforma curentă
npm run electron:build:win     # Windows (.exe)
npm run electron:build:mac     # macOS (.dmg) — x64 &amp; arm64
npm run electron:build:linux   # Linux (.AppImage)
```

### Tray-ul Sistemului

Când este minimizată, OmniRoute este prezentă în tray-ul sistemului cu acțiuni
rapide:

- Deschideți tabloul de bord
- Schimbă portul serverului
- Inchide aplicația

📖 Documentația completă: [`electron/README.md`](electron/README.md)

---

## Prețuri la o privire

| Borduri [calitative nume] | Provider                   | Costuri                                 | Resetează cota                | Cel Mai bun                                                           |
| ------------------------- | -------------------------- | --------------------------------------- | ----------------------------- | --------------------------------------------------------------------- |
| **💳 ABONAMENT**           | Claude Cod (Pro)           | $20/mo                                  | 5h + săptămânal               | Încă abonat                                                           |
|                           | Codex (Plus/Pro)           | $20-200/mo                              | 5h + săptămânal               | Utilizatori OpenAI                                                    |
|                           | Gemini CLI                 | **GRATUIT**                             | 180K/mo + 1K/zi               | Toată lumea!                                                          |
|                           | Copilotul GitHub           | $10-19/mo                               | Pe parcursul unui lună        | Utilizatori GitHub                                                    |
| **🔑 CHEIE API**           | NVIDIA NIM                 | **GRATUIT** (dev până la sfârșit)       | 40RPM                         | 70+ modele deschise                                                   |
|                           | Cerebras                   | **GRATUIT** (1M tok/day)                | 60.000 de TPM / 40RPM         | Acesta este cel mai rapid din lume                                    |
|                           | Groq                       | **GRATUIT** (40RPM)                     | 14.400 de RPD                 | Llama/Gemma extrem de rapid                                           |
|                           | DeepSeek V3.2              | 0,27$/1,10 per 1M                       | Niciuna                       | Ceai mai bună razoanament calitate/preț                               |
|                           | xAI Grok-4 Rapid           | **$0,20/$0,50 per 1M**  🆕               | Niciuna                       | Cel mai rapid + apelarea instrumentelor, într-un mod extrem de scăzut |
|                           | xAI Grok-4 (standard)      | $0,20/$1,50 per 1M  🆕                   | Niciuna                       | Vânzătorul prețului/calității așteptat din partea xAI                 |
|                           | Mistral                    | Probă gratuită + plătit                 | Tarif limitat                 | Inteligent artificială europeană                                      |
|                           | OpenRouter                 | Plată cu utilizare                      | Niciuna                       | Peste 100 modele agregate                                             |
| ** 💰 ieftin**             | GLM-5 (prin Z.AI) 🆕        | $0,5 la 1 M                             | Orar zilnic, 10 AM            | 128 K de ieșire, nou model                                            |
|                           | GLM-4.7                    | $0.6 la 1 M                             | Orar zilnic, 10 AM            | Sistem de rezervă bugetar                                             |
|                           | MiniMax M2.5  🆕            | $0.3/1M intrare                         | Perioada de expirare de 5 ora | Rezolvarea problemelor + sarcini agentiv                              |
|                           | MiniMax M2.1               | 0,2$/1M                                 | Perioada de expirare de 5 ora | Opțiunea cea mai ieftină                                              |
|                           | Kimi K2.5 (API Moonshot) 🆕 | Plată cu utilizare                      | Niciuna                       | Acces direct API Moonshot                                             |
|                           | Kimi K2                    | flat $9/mo                              | 10M tokeni/mo                 | Cost predictibil                                                      |
| **🆓 GRATUIT**             | iFlow                      | **$0**                                  | Fără limitări                 | 5 modele fără limitări                                                |
|                           | Qwen                       | **$0**                                  | Fără limitări                 | 4 modele fără limitări                                                |
|                           | Kiro                       | **$0**                                  | Fără limitări                 | Claude Sonnet/Haiku (Constructor AWS)                                 |
|                           | LongCat Flash-Lite 🆕       | **$0** (50M tokeni/zi 🔥)                | 1 RPS                         | Cel mai mare aport gratuit de pe Pământ                               |
|                           | Polinării AI               | **$0** (nici o cheie necesară)          | 1 cerere/15s                  | GPT-5, Claude, DeepSeek, Llama 4                                      |
|                           | Cloudflare Workers AI      | **$0** (10.000 Neuroni/zilă)            | ~ 150 răspunsuri/zilă         | 50+ de modele, margine globală                                        |
|                           | Scaleway AI                | **$0** (1.000.000 de tokenuri în total) | Tarif limitat                 | UE/GDPR, Qwen3 235B, Llama 70B                                        |

> [Nouele modele adăugate (martie 2026): ** Grok-4 Fast family la $0,20/$0,50/M
> (benchmarkată la 1143ms — 30% mai rapidă decât Gemini 2.5 Flash), GLM-5 prin
> Z.AI cu 128K de ieșire, MiniMax M2.5 raționament, DeepSeek V3.2 prețuri
> actualizate, Kimi K2.5 prin Moonshot API direct.

** 💡 Combo Stivă gratuită, completă — Setarea Gratisă Totală: **

```
Ultimul Stivă Gratit Fre 2026 — 11 Fournitri, $0 Infinit
Kiro (kr/)             → Claude Sonnet/Haiku fără limită
iFlow (if/)            → kimi-k2-thinking, qwen3-coder-plus, deepseek-r1 fără limită
LongCat Lite (lc/)     → LongCat-Flash-Lite — 50 de milioane de tokenuri pe zi
Pollinations (pol/)    → GPT-5, Claude, DeepSeek, Llama 4 — nici o cheie necesară
Qwen (qw/)             → qwen3-coder-plus, qwen3-coder-flash, qwen3-coder-next fără limită
Gemini (gemini/)       → Gemini 2.5 Flash — 1.500 de cereri pe zi API cheie gratuită
Cloudflare AI (cf/)    → Llama 70B, Gemma 3, Mistral — 10K Neuroni pe zi
Scaleway (scw/)        → Qwen3 235B, Llama 70B — 1.000.000 de tokenuri gratuite (UE)
Groq (groq/)           → Llama/Gemma foarte rapidă — 14.400 de cereri pe zi
NVIDIA NIM (nvidia/)   → 70+ de modele deschise — 40 RPM pentru totdeauna
Cerebras (cerebras/)   → Llama/Qwen cea mai rapidă din lume — 1.000.000 de tok pe zi
```

** Cost zero. Niciodată nu înceta de a codifica.** Configurați această
combinație ca un omnirut de combo și toate repedele căderi are loc automat, fără
nicio schimbare manuală.

---

---

## Modelele gratuite — Ceea ce Prima Vezi Efectul

> Toatemodelele de mai jos sunt ** 100% gratuite, fără o cartă de credit
> necesară**. OmniRoute reorientează automat între ele atunci când un aport se
> termină, combinați-le pe toate pentru un combo ininterrupt din $0.

### CLAUDE MODELE (prin Kiro — AWS Identificatorul Îmbunătățirii)

| Model               | Prefix | Limită                 | Limită de rată                       |
| ------------------- | ------ | ---------------------- | ------------------------------------ |
| `claude-sonnet-4.5` | `kr/`  | **Senegal nemărginit** | Nu s-a raportat o cotă zilnică       |
| `claude-haiku-4.5`  | `kr/`  | **Senegal nemărginit** | Nu s-a raportat o cotă zilnică       |
| `claude-opus-4.6`   | `kr/`  | **Senegal nemărginit** | Proiectul cel mai nou Opus prin Kiro |

### 🟢 SISTEME DE INTEGRARE IFlow (OAuth gratuită — Fără numerarul de credit)

| Model                   | Prefix | Limită                 | Limită de rată        |
| ----------------------- | ------ | ---------------------- | --------------------- |
| `kimi-k2-pensarea`      | `if/`  | **Senegal nemărginit** | Nu s-a raportat capul |
| `qwen3-coder-plus`      | `if/`  | **Senegal nemărginit** | Nu s-a raportat capul |
| searchurmareadepseek-r1 | `if/`  | **Senegal nemărginit** | Nu s-a raportat capul |
| minimaxminisec-m2.1     | `if/`  | **Senegal nemărginit** | Nu s-a raportat capul |
| kimikimimodel-k2        | `if/`  | **Senegal nemărginit** | Nu s-a raportat capul |

### ⁉️ MODELE QWEN (Codul Dispozitivului)

| Model                   | Prefix | Limită                 | Limită de rată        |
| ----------------------- | ------ | ---------------------- | --------------------- |
| `qwen3-coder-plus`      | `q/`   | **Senegal nemărginit** | Nu s-a raportat capul |
| `qwen3-developer-flash` | `q/`   | **Senegal nemărginit** | Nu s-a raportat capul |
| `qwen3-developer-next`  | `q/`   | **Senegal nemărginit** | Nu s-a raportat capul |
| `vision-modul`          | `q/`   | **Senegal nemărginit** | Multimodal (imagini)  |

### 🟣 CLI GEMINI (OAuth Google)

| Model                    | Prefix | Limită                                 | Limită de rată  |
| ------------------------ | ------ | -------------------------------------- | --------------- |
| `gemini-3-flash-preview` | `gc/`  | **180K tok/month** + K pe lawy / ziare | Resetează luna  |
| `gemini-2.5-pro`         | `gc/`  | 180K/tok pe lună (pool partajat)       | Calitate înaltă |

### NVIDIA NIM (Cheie API gratuită — build.nvidia.com)

| Borduri [calitative nume] | Limită zilnică      | Limită de rată | Note                                                                |
| ------------------------- | ------------------- | -------------- | ------------------------------------------------------------------- |
| Libere (Des)              | Nicio cotă de token | **~40 RPM**    | 70+ modele; trecerea la limite pure de rată la mijlocul anului 2025 |

Modele populare gratuite: `moonshotai/kimi-k2.5` (Kimi K2.5), `z-ai/glm4.7` (GLM
4.7), `deepseek-ai/deepseek-v3.2` (DeepSeek V3.2),
`nvidia/llama-3.3-70b-instruct`, `deepseek/deepseek-r1`

### CEREBRAS (Cheie API gratuită — inference.cerebras.ai)

| Borduri [calitative nume] | Limită zilnică                   | Limită de rată        | Note                                            |
| ------------------------- | -------------------------------- | --------------------- | ----------------------------------------------- |
| Gratuit                   | ** 1M unități de mesaj/xomitar** | 60.000 de TPM / 40RPM | Cel mai rapid inferență a LLM; se resete zilnic |

Disponibil gratuit: `llama-3.3-70b`, `llama-3.1-8b`,
`deepseek-r1-distill-llama-70b`

### 🔴 GROQ (Cheie API Gratuită — console.groq.com)

| Borduri [calitative nume] | Limită zilnică | Limită de rată            | Note                                                   |
| ------------------------- | -------------- | ------------------------- | ------------------------------------------------------ |
| Gratuit                   | ** 14,4K RPD** | 30 de cereri RPM pe model | Fără card de credit; 429 pe atingere, nu se facturează |

Disponibil gratuit: `llama-3.3-70b-versatile`, `gemma2-9b-it`, `mixtral-8x7b`,
`whisper-large-v3`

### 🔴 LONGCAT AI (Cheie API Gratuită — longcat.chat) 🆕

| Model                         | Prefix | Cazualități zilnice gratuite | Note                                           |
| ----------------------------- | ------ | ---------------------------- | ---------------------------------------------- |
| `LongCat-Flash-Lite`          | `lc/`  | **50M tokeni**               | Cel mai mare număr de gratuități free vreodată |
| `LongCat-Flash-Chat`          | `lc/`  | 500K tokeni                  | Discuții multi-tur                             |
| `LongCat-Flash-Thinking`      | `lc/`  | 500K tokeni                  | Răspândire/ CoT                                |
| `LongCat-Flash-Thinking-2601` | `lc/`  | 500K tokeni                  | Versiunea din Ianuarie 2026                    |
| `LongCat-Flash-Omni-2603`     | `lc/`  | 500K tokeni                  | Multimodal                                     |

> 100% gratuit în timpul beta-ului public. Înregistrează-te la
> [longcat.chat](https://longcat.chat) cu adresa de email sau număr de telefon.
> Se resetează zilnic ora 0:00 UTC.

### 🟢 POLINATII AI (Fără cheie de API necesară) 🆕

| Model      | Prefix | Limită de rată | Furnizor În Spate  |
| ---------- | ------ | -------------- | ------------------ |
| `openai`   | `pol/` | 1 cerere/15s   | GPT-5              |
| `claude`   | `pol/` | 1 cerere/15s   | Antropic Claude    |
| `gemini`   | `pol/` | 1 cerere/15s   | Google Gemini      |
| `deepseek` | `pol/` | 1 cerere/15s   | DeepSeek V3        |
| `llama`    | `pol/` | 1 cerere/15s   | Meta Llama 4 Scout |
| `mistral`  | `pol/` | 1 cerere/15s   | Mistral AI         |

> ✨ **Fără fricțiuni:** Inregistrați-ul și cheia API nu sunt necesare. Adăugați
> furnizorul Pollinations cu un câmp vid pentru chei și funționează imediat.

### 🟠 ANGĂJAT CLOUDFLARE AI (Cheie API gratuită — cloudflare.com) 🆕

| Borduri [calitative nume] | Neuroni pe zi                | Echivalență de utilizare                             | Note                    |
| ------------------------- | ---------------------------- | ---------------------------------------------------- | ----------------------- |
| Gratuit                   | [10,000[X]10,000[X8]8,000[X] | ~150 LLM înmulțiți / 500 sec și audio / 15K înmulete | Edge globală, 50+ model |

Modele populare gratuite: [X21X}@cf/meta/llama-3.3-70b-instruct`,
`@cf/google/gemma-3-12b-it`, `@cf/openai/whisper-large-v3-turbo` (audio
gratuit!), `@cf/qwen/qwen2.5-coder-15b-instruct`

> Se ceră Token API + ID Account din
> [dash.cloudflare.com](https://dash.cloudflare.com). Să păstrați ID-ul Contului
> în setări furnizor.

### 🟣 AI-ul Scala (1M Tokenuri gratuite — scaleway.com) 🆕

| Borduri [calitative nume] | Păstrarea rateuți                  | Locație      | Note                                          |
| ------------------------- | ---------------------------------- | ------------ | --------------------------------------------- |
| Gratuit                   | [1M token[X]1M token[X11]11M token | 🇫🇷 Paris, UE | Nicio carte de credit necesară până la limită |

Disponibile gratuite: `qwen3-235b-a22b-instruct-2507` (Qwen3 235B!),
`llama-3.1-70b-instruct`, `mistral-small-3.2-24b-instruct-2506`,
`deepseek-v3-0324`

> Conform GDPR/UE. Obțineți cheia API la
> [console.scaleway.com](https://console.scaleway.com).

> [X]Luminița The Ultimate Stivă Gratis (11 Părți, $0 Încă o Dată):**
> 
> ```
> Kiro (kr/)             → Claude Sonnet/Haiku S.fără limită
> iFlow (if/)            → kimi-k2-si-pentru-cod/ qwen3-si-coder-plus, deepseek-r1 S.fără limită
> LongCat Lite (lc/)     → LongCat-Flash-Lite – 50M tokenuri/ziar 
> Pollinations (pol/)    → GPT-5, Claude, DeepSeek, Llama 4 — niciodată cheie nefolosită
> Qwen (qw/)             → qwen3-si-coder modele S.fără limită
> Gemini (gemini/)       → Gemini 2.5 Flash — 1.500 cereri/zi gratis
> Cloudflare AI (cf/)    → 50+ modele — 10K neuroni/zi
> Scaleway (scw/)        → Qwen3 235B, Llama 70B — 1M tokenuri gratuite (UE)
> Groq (groq/)           → Llama/Gemma — 14.4K cereri/zi extrem de rapid
> NVIDIA NIM (nvidia/)   → 70+ modele deschise — 40 RPM în vecinătatea veșnică
> Cerebras (cerebras/)   → Llama/Qwen cea mai rapidă în lume — 1M tok/zi
> ```

## 🎙️ Combinare de Transcriere Gratuită

> Transcrie orice audio/video pentru **$0** — Deepgram conduce cu 200$ gratis,
> AssemblyAI fallback de 50$, Groq Whisper ca următoare copie de stocare.

| Provider         | Credituri Free                        | Cel mai Bun Model                                     | Limită de rată                                 |
| ---------------- | ------------------------------------- | ----------------------------------------------------- | ---------------------------------------------- |
| 🟢 **Deepgram**   | **$200 liber** (singură înregistrare) | `nova-3` — cea mai bună acuratețe, 30+ limbi          | Fără limită de cereeri RPM pe credite gratuite |
| 🔵 **AssemblyAI** | **$50 liber** (singură înregistrare)  | `universal-3-pro` — capitole, sentiment, confidențial | Fără limită de cereeri RPM pe credite gratuite |
| 🔴 **Groq**       | **Gratuit în vecinătate**             | `whisper-large-v3` — OpenAI Whisper                   | 30 RPM (limită de rată)                        |

**Combinație sugerată în `/dashboard/combos`:**

```
Nume: transcriere-gratuită
Estrategie: Prioritate
Node:
  [1] deepgram/nova-3          → folosește primului 200$ liber
  [2] assemblyai/universal-3-pro → înlocuiește când creditele Deepgram se epuizează
  [3] groq/whisper-large-v3    → gratuit, următoarea variantă din stocare
```

Atunci în `/dashboard/media` → **Transcriere** tab: încărcați orice fișier de
audio sau video → selectați endpointul combo → obțineți transcrierea în formatul
sprijinit.

## 💡 Caracteristici cheie

OmniRoute v2.0 este construit ca o platformă de operare, nu numai un proxy de
reîmprospătare.

### 🆕 Nou — Îmbunătățiri inspirate de ClawRouter (Mar 2026)

| Caracteristică                              | Ce face                                                                                                       |
| ------------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| ⚡ **Grok-4 Fast Family**                    | modele AI la 0,20/0,50/M — îmbunătățire de 1143ms (30% mai rapidă decât Gemini 2.5 Flash)                     |
| 🧠 **GLM-5 prin Z.AI**                       | context de 128K de ieșire, 0,5/1M — ceva nou și modern din familia GLM                                        |
| 🔮 **MiniMax M2.5**                          | Raționament și sarcini agente în 0,30/1M — un upgrade semnificativ de la M2.1                                 |
| 🎯 **Flux de apel pentru modele**            | `Flux de apel pentru fiecare model: true/false` în registru — AutoCombo trece cu vederea modelele capabile    |
| 🌍 **Detectare a intenției multilingvă**     | cuvinte cheie PT/ZH/ES/AR în scorarea AutoCombo — selecția mai bună a modelelor pentru conținutul nu-l englez |
| 📊 **fallback-uri pe baza benchmark-urilor** | latență reală de 95% din cererile live care hrănește scorarea combo — AutoCombo învăță de la datele reale     |
| 🔁 **Eliminare de duplicate**                | fereastră de dedup bazată pe hash-ul conținutului — eliminarea sigură, care prevede încărcări duplicate       |
| 🔌 **RouterStrategy Pluggabil**              | Interfața router-ului extensibil[XX] — adăugați logica de ruteare personalizată ca plug-inuri                 |

### 🚀 Anvelopa v2.0.9+ — Joc deashboard, CLI, Parâmeetri și ACP

| Caracteristică                                  | Ce face                                                                                                                                                                                                                                                                                                                      |
| ----------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🎮 ** Testarea Jocului Model**                   | Pagina de dashboard pentru testarea directă a oricărui model — selectoare provider/model/endpoint, Editorul Monaco, streaming, abandon, timp de răspuns                                                                                                                                                                      |
| 🔏 ** Selecția Fingerprint-ului CLI**            | Ordonarea capetelor/corpului furnizată pe baza furnizorului pentru a se potrivi semnăturilor native CLI — activați în Setări > Securitate. **Adresa ta IP proxy este menținută**                                                                                                                                             |
| 🤝 **Suport pentru Protocol ACP (Client-Agent)** | Descoperirea agenților CLI (Codex, Claude, Goose, Gemini CLI, OpenClaw + 9 mai multe), rularea procesului, ` /api /ACP /Agenti` punctul de sfârșit al endpointului                                                                                                                                                           |
| 🤖 **Portofoliul de ACP Agenți**                 | Pagina de Debug› Agenți a portofoliului – grila de 14 agenți cu statut de instalare, versiune, formular de agent personalizat pentru orice instrument CLI. **Utilizatorii OpenCode** primesc un buton „Descărcați opencode.json” care generează automat o configurație gata pentru utilizare cu toate modelurile disponibile |
| 🔧 **Rutearea personalizată Model `apiFormat`**  | Modelurile personalizate cu `apiFormat: „răspunsurile”` se rutează acum corect spre traducătorul API-ului Responsă                                                                                                                                                                                                           |
| 🏢 **Izolare spațiu de lucru Codex**             | Mai multe spații de lucru Codex pe adresa de e-mail — OAuth separă corect conexiunile pe ID-ul spațiului de lucru                                                                                                                                                                                                            |
| 🔄 **Actualizare Electron Automată**             | Aplicația de desktop verifică actualizările + își instalează automat în.restart                                                                                                                                                                                                                                              |

### 🤖 Operație agent & Protocol (v2.0)

| Caracteristică                                                         | Ce face                                                                                                     |
| ---------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| ♛ **Serviciu MCP (16 instrumente)**                                    | Instrumente IDE/agent prin 3 transporturi: stdio, SSE (`/api/mcp/sse`), HTTP fluxabil (`/api/mcp/stream`)   |
| ♟ **Serviciu A2A (JSON-RPC + SSE)**                                    | Execuția sarcinilor binare între agenți cu fluxuri sincron și fluxabile                                     |
| 🗂️ **Pagina de endpoint-uri consolidate**                              | Pagină de management cu perechi de endpoint-uri: Proxy Endpoint, MCP, A2A si API Endpoints                  |
| 🔄 **Comutatoare de service On/Off**                                    | Butoane de ON/OFF pentru MCP și A2A cu persistență a setărilor(implicit: OFF)                               |
| 🛰️ **Inima Serviciului Runtime MCP**                                   | Starea procesului real (id proces, timp de viață, vechimea pulsului, transport, modul de scop)              |
| 📊 **Traseul auditabil MCP**                                            | Loguri de audit cu filtreare și atribuire clare (succes/fală și chei)                                       |
| 🛡️ **Implementarea de scopuri pentru MCP**                             | 9 permisiuni de scop granulare pentru acces controlat la instrumente                                        |
| 🔄 **Managementul ciclului de viață pentru sarcini A2A**                | Listare/ filtrare de sarcini, inspectare de evenimente/articole, anulare de sarcini în curs                 |
| 📋 **Descoperirea cărții de agent**                                     | `/.well-known/agent.json` pentru descoperire auto-client                                                    |
| Fermentatorul protocolului **Testarea finală dincolo de proticol E2E** | MCP SDK real + fluxuri A2A clienți în `test:protocols:e2e`                                                  |
| ⚙️ Controlul operativ **                                               | Butonul de selectare, aplicarea profilului de reziliență, resetarea de la un panou de control a circuitelor |

### Rutează & Intelepciune inteligență

| Caracteristică                                   | Ce face                                                                                             |
| ------------------------------------------------ | --------------------------------------------------------------------------------------------------- |
| Ţinta **Fallback Smart pentru 4 nivele**         | Rutarea automată: Abonament → Cheie API → Barat → Gratuiteminte                                     |
| 📊 **Monitorizarea alocării în timp real**        | Contele de tokeni în timp real + numărul de repornire a contului în timp real pe fiecare furnizor   |
| 🔄 **Traducerea formatului**                      | OpenAI → Claude → Gemini → Conversii cu schema sigură                                               |
| 👥 **Sprijin pentru mai multe conturi**           | Mai multe conturi per furnizor cu selectarea inteligentă                                            |
| 🔄 **Reîmprospătarea automată a tokenului**       | Tokenurile OAuth se reîmprospătează automat cu încercare                                            |
| 🎨 Comboul personalizat **                        | 6 strategii de echilibru + controlul lanțului                                                       |
| 🌐 **Routerul cu marcă sau săgeată**              | `furnizor/*` ruteare dinamic                                                                        |
| 🧠 **Gândire Buget Controale**                    | Transmitere, automat, personalizată, și limite de raționalizare adaptative                          |
| 🔀 **Nume de Model**                              | și migrarea de siguranță a numelor de model integrate și personalizate                              |
| ⚡ **Dezvoltare în Planul Fundal**                | Rutează sarcinile de fundal cu prioritate scăzută către modele mai ieftine                          |
| 🧪 **Routeare Inteligentă Conștientă de Sarcini** | Selectează automat modelul în funcție de tipul conținutului (codare/vizualizare/analiză/sumarizare) |
| 💬 **Injectarea Prompturilor Sistem**             | Conducerea comportamentului global aplicată consistent                                              |
| 📄 **Compatibilitate API-Răspunsuri**             | Suport plin pentru /v1/responses` și codex avansat                                                  |

### 🎵 API-uri Multi-Modal

| Caracteristică              | Ce face                                                                                                                                                                           |
| --------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🖼️ **Generarea de Imagini** | /v1/images/generations` cu surse locale și cloud                                                                                                                                  |
| 📐 **Încorporări**           | /v1/embeddings` pentru pipeline-uri de căutare și RAG                                                                                                                             |
| 🎤 **Transcrierea audio**    | `/v1/audio/transcrieri` — 7 furnizori (Deepgram Nova 3, AssemblyAI, Groq Whisper, HuggingFace, ElevenLabs, OpenAI, Azure), detectare automată a limbii, suport pentru MP4/MP3/WAV |
| 🔊 **Text-to-Speech**        | `/v1/audio/stereovoice` — 10 furnizori (ElevenLabs, OpenAI, Deepgram, Cartesia, PlayHT, HuggingFace, Nvidia NIM, Inworld, Coqui, Tortoise) cu mesajele de eroare corecte          |
| 🎬 **Generare de video**     | `/v1/videos/generari` (fluxurile de lucru ComfyUI + SD WebUI)                                                                                                                     |
| 🎵 **Generare de muzică**    | `/v1/music/generari` (fluxurile de lucru ComfyUI)                                                                                                                                 |
| 🛡️ **Moderări**             | `/v1/moderari` verificări de siguranță                                                                                                                                            |
| 🔀 **Re-rangarea**           | `/v1/rerang` pentru scorarea de relevanță                                                                                                                                         |
| 🔍 **Căutare Web** 🆕         | `/v1/căutare` — 5 furnizori (Serper, Brave, Perplexity, Exa, Tavily), 6.500+ gratuit / lună, failover automat și cache                                                            |

### 🛡️ Reziliencvă, Siguranță și Gestiune

| Caracteristică                              | Ce face                                                                                |
| ------------------------------------------- | -------------------------------------------------------------------------------------- |
| 🔌 **Butoanele de blocare**                  | Per-model cu încărcări și recuperări cu controluri de prag                             |
| 🎯 **Modelul cu conștientizare de endpoint** | Custom models declare supported endpoints + API format                                 |
| 🛡️ **Anti-Thundering Herd**                 | Mutex + semaphore protections on retry/rate events                                     |
| 🧠 **Semantic + Signature Cache**            | Cost/latency reduction with two cache layers                                           |
| ⚡ **Request Idempotency**                   | Duplicate protection window                                                            |
| 🔒 **TLS Fingerprint Spoofing**              | Browser-like TLS fingerprint — **reduces bot detection and account flagging**          |
| 🔏 ** Selecția Fingerprint-ului CLI**        | Matches native CLI request signatures — **reduces ban risk while preserving proxy IP** |
| 🌐 **IP Filtering**                          | Allowlist/blocklist control for exposed deployments                                    |
| 📊 **Editable Rate Limits**                  | Configurable global/provider-level limits with persistence                             |
| 🔑 **API Key Management + Scoping**          | Secure key issuance/rotation and model/provider controls                               |
| 🛡️ **Protected `/models`**                  | Optional auth gating and provider hiding for model catalog                             |

### 📊 Observability & Analytics

| Caracteristică                         | Ce face                                                                           |
| -------------------------------------- | --------------------------------------------------------------------------------- |
| 📝 **Cerere + Ierarhizarea Proxy-ului** | Logarea cererii completă/răspuns și traficului proxy                              |
| 📋 **Dashboard-ul Jurnalului Unificat** | Vizorul cererilor, traficului proxy, auditului și consolei pe o pagină            |
| 🔍 **Instrumentarea Cererilor**         | Latenta de 50%/95%/99% și monitorizarea cererilor                                 |
| 🏥 **DASHBOARD-ul de Sănătate**         | Timpul de disponibilitate, stări de întrerupere, blocările, statisticile de cache |
| 💰 **Tractarea Costurilor**             | Controlul bugetului și vizibilitatea prețului modelului                           |
| 📈 **Vizualizările Analitice**          | Insight-urile privind utilizarea modelului/toleranța și graficurile tendențiale   |
| 🧪 **Folosirea Ramurei de Evaluare**    | Testarea setului de aur cu strategii de acomodare configurabile                   |

### ☁️ Implementarea & Platforma

| Caracteristică                                         | Ce face                                                                                    |
| ------------------------------------------------------ | ------------------------------------------------------------------------------------------ |
| 🌐 **Implantați oriunde**                               | Locghiune locală, VPS, Docker, Medii de încredere în cloud                                 |
| 💾 **Cloud Sync**                                       | Configurarea sincronizării prin intermediul lucrătorului de cloud                          |
| 🔄 **Backup/Restore**                                   | Fluxele de export/import și recuperare în caz de dezastru                                  |
| 🧙 **Asistentul de Onboarding**                         | Setarea îndrumată de pe run-ul prim                                                        |
| 🔧 **Panelul de instrumente CLI**                       | Instalarea simplă pentru instrumentele de codare populare                                  |
| 🎮 ** Testarea Jocului Model**                          | Testați orice furnizor/model/endpoint din panel                                            |
| 🔏 **Funcția de activare/disactivare a imprimatei CLI** | Compatibilitatea de imprimate în funcție de furnizor în Setări > Siguranță                 |
| 🌐 **i18n (30 de limbi)**                               | Suport complet pentru limbajul UI și documentația cu suport pentru formatarea direcțională |
| 🧹 **Șterge Toate Modelurile**                          | Ștergerea rapidă a listei de modeluri din detaliile furnizorului                           |
| 📋 **Șabloanele Issue**                                 | Șablonuri standard pentru GitHub pentru bug-uri și funcționalități                         |
| 📂 **Directory de date personalizată**                  | `DIRECTORIU_DATE` înlocuitor pentru localizarea stocării                                   |

### Folosirea adâncă a componentelor

#### Revenire inteligentă cu control de cost practic

```txt
Combo: "stiva-me-l de codare"
  1. cc/claude-opus-4-6
  2. nvidia/llama-3.3-70b
  3. glm/glm-4.7
  4. if/kimi-k2-gândire
```

Când cotă, rată sau sănătate eşuează, OmniRoute automat trec la candidatul
următor fără schimbări manuale.

#### Administrarea protocolului vizibilă și operațională

- MCP + A2A sunt descoperite în UI și documentație (nu ascunse)
- API-l-e pentru starea protocolului expun date operative în timp real
  (`/api/mcp/*`, `/api/a2a/*`)
- Intrările dashbordului includ acțiuni pentru operarea de zi a doua
  (comutatoare combinate, resetare de reper, anulare de sarcini)

#### Fluxul traducerii + validării

Zona de traducere include:

- **Teatru de joc**: testează transformările
- **Testarea de conversație**: runde de comunicare completă
- **Bancă de teste**: mai multe cazuri într-o rulare
- **Monitor live**: vedere în timp real a traficului

Plus validarea protocolului cu clienții reali prin `npm run test:protocols:e2e`.

> 📖 **Manualul serverului MCP(open-sse/mcp-server/README.md)** — Referință
> pentru instrumente, configurații pentru IDE și exemple de clienți
> 
> 📖 **Manualul serverului A2A(src/lib/a2a/README.md)** — Abilitățile, metodele
> JSON-RPC, fluxul streaming și ciclul de sarcini

## 🧪 Evaluări (Examen)

OmniRoute include un cadru de evaluare intern pentru testarea calității
răspunsurilor LLM în raport cu un set de aur. Accesul se face prin **Analytics →
Evaluări** în parteneriat.\
==WEBLATE_PART==

### Setul Golden Întreg

Setul "OmniRoute Golden Set" preîncărcat conține cazuri de test pentru:

- Salutări, matematică, geografie, generare coduri
- Comformarea formatului JSON, traducere, generare markdonw
- Refuzul de siguranță (conținut rău), numărare, logică booleană

### Strategii de evaluare

| Strategie | Descriere                                                              | Exemplu                                |
| --------- | ---------------------------------------------------------------------- | -------------------------------------- |
| `exact`   | Răspunsul trebuie să se închege exact                                  | `"4"`                                  |
| `conține` | Răspunsul trebuie să conțină subștringul (fără diferență de caz)       | `"Paris"`                              |
| `regex`   | Răspunsul trebuie să se încadreze într-un pattern de expresie regulată | `"1.*2.*3"`                            |
| `custom`  | Functia JS personalizată returnează true/false                         | `(ieşire) =&gt; ieşire.length &gt; 10` |

---

## Ghid de instalare

### Setup-ul protocolului ( MUP + A2A )

<details>
<summary><b>🧩 MCP Setup (Model Context Protocol)</b></summary>

Porniți transportul MUP în modul stdio:

```bash
omniroute --mcp
```

Fluxul de validare recomandat:

1. Conectați clientul MUP în modul stdio.
2. Rulați `omniroute_get_health`.
3. Rulați `omniroute_get_combos`.
4. Deschideți `/dashboard/mcp` pentru a confirma pulsul de inimă, activitatea și
   auditul.

API-uri utile pentru automatizarea:

- `GET /api/mcp/status`
- `GET /api/mcp/tools`
- `GET /api/mcp/audit`
- `GET /api/mcp/audit/stats`

</details>

<details>
<summary><b>🤝 A2A Setup (Agent2Agent)</b></summary>

Descoperiți agentul:

```bash
curl http://localhost:20128/.well-known/agent.json
```

Trimițiți o sarcină:

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"setup-a2a","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"Summarize quota status."}]}}'
```

Gestionați ciclul de viață:

- `GET /api/a2a/status`
- `GET /api/a2a/tasks`
- `GET /api/a2a/tasks/:id`
- `POST /api/a2a/tasks/:id/cancel`

Operational UI:

- `/dashboard/a2a` for task/state/stream observability and smoke actions

</details>

<details>
<summary><b>🧪 End-to-end protocol validation</b></summary>

Validate both protocols with real clients:

```bash
npm run test:protocols:e2e
```

This verifies:

- MCP SDK client connect/list/call
- A2A discovery/send/stream/get/cancel
- Cross-check data in MCP audit and A2A task management APIs

</details>

<details>
<summary><b>💳 Subscription Providers</b></summary>

### Claude Code (Pro/Max)

```bash
Dashboard → Providers → Connect Claude Code
→ OAuth login → Auto token refresh
→ 5-hour + weekly quota tracking

Models:
  cc/claude-opus-4-6
  cc/claude-sonnet-4-5-20250929
  cc/claude-haiku-4-5-20251001
```

**Pro Tip:** Use Opus for complex tasks, Sonnet for speed. OmniRoute tracks
quota per model!

### OpenAI Codex (Plus/Pro)

```bash
Dashboard → Providers → Connect Codex
→ OAuth login (port 1455)
→ 5-hour + weekly reset

Models:
  cx/gpt-5.2-codex
  cx/gpt-5.1-codex-max
```

#### Codex Account Limit Management (5h + Weekly)

Each Codex account now has policy toggles in `Dashboard -> Providers`:

- `5h` (ON/OFF): enforce the 5-hour window threshold policy.
- `Săptămânal` (ACTIVAT/DEACTIVAT): aplică politica pragului de ședere
  săptămânală.
- Comportamentul pragului: când unul dintre ferestre ajunge la >= 90% utilizare,
  contul este ignorat.
- Comportamentul rotirii: OmniRoute redirecționează automat către contul următor
  eligibil Codex.
- Comportamentul resetării: atunci când trecutul `resetAt` timp de resetare,
  contul devine eligibil din nou automat.

Săriuri:

- `5h ACTIVAT` + `Săptămânal ACTIVAT`: contul este ignorat atunci când ajunge
  pragul oricare dintre ferestre.
- `5h DEACTIVAT` + `Săptămânal ACTIVAT`: doar utilizarea săptămânală poate bloca
  contul.
- `5h ACTIVAT` + `Săptămânal DEACTIVAT`: doar utilizarea de 5 ore poate bloca
  contul.
- `resetAt` parcurs: contul reapară în rotirea automată (fără a fi nevoie de
  reabilitare manuală).

### Gemini CLI (GRAȚIAT 180K/lună!)

```bash
Punct de acces → Furnizori → Conectare Gemini CLI
→ Google OAuth
→ 180K de rezultate lunare + 1K zilnic

Model-uri:
  gc/gemini-3-preview-în-școală
  gc/gemini-2.5-pro
```

**Cel mai bun raport:** Cel mai mare nivel de tariful gratuit! Utilizați acesta
înainte de tier-uri plătite.

### Copilotul GitHub

```bash
Punct de acces → Furnizori → Conectare GitHub
→ OAuth prin GitHub
→ Reîmprospătare lunară (prima zi a lunii)

Model-uri:
  gh/gpt-5
  gh/claude-4.5-sonnet
  gh/gemini-3-pro
```

</details>

<details>
<summary><b>🔑 API Key Providers</b></summary>

### NVIDIA NIM (Accesul dezvoltator gratuit — 70+ de modele)

1. Înregistrează-te: [build.nvidia.com](https://build.nvidia.com)
2. Obține claua API gratuită (1000 de credite de inferință incluse)
3. Punct de acces → Adăugare furnizor → NVIDIA NIM:
   - Cheie API: `nvapi-tasta-tastatură-întreabă-cheia`

**Modele:** `nvidia/llama-3.3-70b-instruct`, `nvidia/mistral-7b-instruct`, și
50+ de alte moduri

**Pro Tip:** OpenAI-compatible API — works seamlessly with OmniRoute's format
translation!

### DeepSeek

1. Sign up: [platform.deepseek.com](https://platform.deepseek.com)
2. Get API key
3. Dashboard → Add Provider → DeepSeek

**Models:** `deepseek/deepseek-chat`, `deepseek/deepseek-coder`

### Groq (Free Tier Available!)

1. Sign up: [console.groq.com](https://console.groq.com)
2. Get API key (free tier included)
3. Dashboard → Add Provider → Groq

**Models:** `groq/llama-3.3-70b`, `groq/mixtral-8x7b`

**Pro Tip:** Ultra-fast inference — best for real-time coding!

### OpenRouter (100+ Models)

1. Sign up: [openrouter.ai](https://openrouter.ai)
2. Get API key
3. Dashboard → Add Provider → OpenRouter

**Models:** Access 100+ models from all major providers through a single API
key.

</details>

<details>
<summary><b>💰 Cheap Providers (Backup)</b></summary>

### GLM-4.7 (Daily reset, $0.6/1M)

1. Sign up: [Zhipu AI](https://open.bigmodel.cn/)
2. Get API key from Coding Plan
3. Painel de Control → Adaugă cheia API:
   - Furnizor: `glm`
   - Cheie API: `cheia-ta`

**Sfaturi:** `glm/glm-4.7`

**Sfaturi Pro:** Planul de codare oferă 3 × taxa cu 1/7 din cost! Resetează
zilnic la ora 10:00.

### MiniMax M2.1 (resetează 5 ore, $0.20/1M)

1. Incheagă contul: [MiniMax](https://www.minimax.io/)
2. Get API key
3. Painel de Control → Adaugă cheia API

**Sfaturi:** `minimax/MiniMax-M2.1`

**Sfaturi Pro:** Optiunea ieftină pentru context lung (1M token-uri)!

### Kimi K2 ($9/lună fix)

1. Abonare: [Moonshot AI](https://platform.moonshot.ai/)
2. Get API key
3. Painel de Control → Adaugă cheia API

**Sfaturi:** `kimi/kimi-latest`

**Sfaturi Pro:** $9/lună fix pentru 10M token-uri = $0,90/1M cost efectiv!

</details>

<details>
<summary><b>🆓 FREE Providers (Emergency Backup)</b></summary>

### iFlow (5 modele gratuite prin OAuth)

```bash
Painel de Control → Conectare iFlow
→ Autentificare OAuth iFlow
→ Utilizare nelimitată

Modele:
  if/kimi-k2-thinking
  if/qwen3-coder-plus
  if/glm-4.7
  if/minimax-m2
  if/deepseek-r1
```

### Qwen (4 modele gratuite prin Cod Dispozitiv)\

```bash
Dashboard → Conectează la Qwen
→ Autorizare prin codul dispozitivului
→ Fără limitări de utilizare

Modele:
  qw/qwen3-coder-plus
  qw/qwen3-coder-flash
```

### Kiro (Claude gratuit)

```bash
Dashboard → Conectează la Kiro
→ AWS ID-ul constructorului sau Google/GitHub
→ Fără limitări de utilizare

Modele:
  kr/claude-sonnet-4.5
  kr/claude-haiku-4.5
```

</details>

<details>
<summary><b>🎨 Create Combos</b></summary>

### Exemplu 1: Maximiza Abonamentul → Adăpostire ieftină

```
Dashboard → Combos → Crează Nou

Nume: codificare-premium
Modele:
  1. cc/claude-opus-4-6 (Abonament primar)
  2. glm/glm-4.7 (Adăpostire ieftină, $0.6/1M)
  3. minimax/MiniMax-M2.1 (Falimentul cel mai ieftin, $0.20/1M)

Utilizare în CLI: codificare-premium
```

### Exemplu 2: (Zis costuri - Zero)

```
Nume: combină gratuit
Modele:
  1. gc/gemini-3-flash-preview (180K gratuit/lună)
  2. if/kimi-k2-thinking (fără limitări)
  3. qw/qwen3-coder-plus (fără limitări)

Cost: $0 pentru totdeauna!
```

</details>

<details>
<summary><b>🔧 CLI Integration</b></summary>

### Cursor IDE

```
Setări → Modele → Avansate:
  URL-ul bazei API OpenAI: http://localhost:20128/v1
  Cheie API OpenAI: [împrumutați din dashboard-ul OmniRoute]
  Model: cc/claude-opus-4-6
```

### Claude Cod

Utilizați pagina CLI Tools** în dashboard pentru configurarea cu o singură clic,
sau editați manual `~/.claude/settings.json`.

### Codex CLI

```bash
export OPENAI_BASE_URL="http://localhost:20128"
export OPENAI_API_KEY="cheia-ți-api-omniroute"

codex "prompțul tău"
```

### OpenClaw

**Opțiunea 1 — Dashboard (recomandată):**

```
Dashboard → CLI Tools → OpenClaw → Selectează Model → Aplică
```

**Opțiunea 2 — Manual:** Editați manual `~/.openclaw/openclaw.json`:

```json
{
  "modele": {
    "provideri": {
      "omniroute": {
        "baseUrl": "http://127.0.0.1:20128/v1",
        "apiKey": "sk_omniroute",
        "api": "openai-completions"
      }
    }
  }
}
```

> **Nota:** OpenClaw funcționează doar cu OmniRoute local. Folosiți `127.0.0.1`
> în loc de `localhost` pentru a evita problemele de rezolvare a IPv6.

### Cline / Continuă / RooCode

```
Setări → Configurația API:
  Fornitor: Compatibil cu OpenAI
  Adresă de bază: http://localhost:20128/v1
  Cheie API: [din panoul OmniRoute]
  Model: if/kimi-k2-thinking
```

### Opencode

**Pasi 1:** Adăugați OmniRoute ca furnizor personalizat:

```bash
opencode
 conecta
# Selectează "Altele" → Introduceți ID: "omniroute" → Introduceți cheia dvs. API OmniRoute
```

**Pasi 2:** Creazăți/ediționați `opencode.json` în root-ul proiectului dvs.:

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

**Pasi 3:** Selectați modelul în Opencode:

```bash
/modeluri
# Selectați orice model OmniRoute din listă
```

> **Sfaturi:** Adăugați orice model disponibil în `/v1/modeluri` endpoint-ul
> dvs. OmniRoute în secțiunea `modeluri`. Utilizați formatul `furnizor/model-id`
> din panoul dvs. OmniRoute.

</details>

---

## Depanare

<details>
<summary><b>Click to expand troubleshooting guide</b></summary>

**"Modelul de limbă nu a furnizat mesaje"**

- Exhaustiota limitelor de subcriere → Verificați tracker-ul de subcriere din
  panoul dvs.
- Soluție: Utilizați fallback-ul combo sau schimbați la o căutărie mai ieftină

**Limitări de frecvență**

- Limita subcrierilor depășit → Fallback-ul către GLM/MiniMax
- Adăugați combo: `cc/claude-opus-4-6 → glm/glm-4.7 → if/kimi-k2-thinking`

**Tokenul OAuth expirat**

- Reînnoit automat de către OmniRoute
- Dacă problemele persistă: Panoul > Fornitor > Reconectați-vă

**Costuri ridicate**

- Răsfoiri de utilizare în Panoul de control → Costuri
- Schimbă modelul principal în GLM/MiniMax
- Utilizează nivelul gratuit (Gemini CLI, iFlow) pentru taskuri non-critice

**Panoul de control/Porturile API sunt greșite**

- `PORT` este poarta de bază canonicală (și api portul implicat din definițiie)
- `API_PORT` anulează doar ascultatorul API compatibil cu OpenAI
- `DASHBOARD_PORT` anulează doar ascultatorul Next.js pentru panau
- Setează `NEXT_PUBLIC_BASE_URL` către URL-ul public al panoului/ dashboard
  (pentru apelurile OAuth)

**Erori de sincronizare a cloudului**

- Verificați că `BASE_URL` se referă la instanța dvs. ce rulează
- Verificați că `CLOUD_URL` se referă la punctual expetcat al cloudului
- Păstrați `NEXT_PUBLIC_*` valori aliniate cu valorile de pe server

**Prima autentificare nu este funcțională**

- Verificați `INITIAL_PASSWORD` în [.env`
- Dacă nu este setat, parola de fallback este `123456`

**Nu există registre de cereri**

- Setați `ENABLE_REQUEST_LOGS=true` în [.env`

**Testarea conexiunii arată "Invalid" pentru furnizorii compatibili cu OpenAI**

- Mai toți furnizorii nu expun endpoint-ul `/models`
- OmniRoute v1.0.6+ include verificarea de fallback via completări de
  conversație
- Include `/v1` suffix in the server base URL

### Autentificare OAuth pe un Server Remot

<a name="oauth-on-a-remote-server"></a> <a name="oauth-em-servidor-remoto"></a>

> **⚠️ Importantă pentru utilizatori care rulează OmniRoute pe un server VPS,
> Docker sau orice altă server**

#### De ce autenticarea Antigravity / Gemini CLI OAuth eșuează pe servere remote?

Furnizorii **Antigravity** și **Gemini CLI** utilizează **OAuth 2.0 Google**.
Google cere `redirect_uri` în fluxul OAuth să fie exact identic cu una dintre
URILE pre-registrate în consola Cloud Google a aplicației.

Credentialele OAuth pachetate în OmniRoute sunt înregistrate **numai pentru
`localhost`**. Când accesați OmniRoute pe un server remot (de exemplu
`https://omniroute.myserver.com`), Google respinge autenticarea cu:

```
Eroare 400: redirect_uri_mismatch
```

#### Soluție: Configurează credentialele OAuth proprii

Trebuie să creați un **ID de Client OAuth 2.0** în Consola Google Cloud cu
URI-ul serverului dumneavoastră.

#### Pas cu pas

**1. Deschideți Consola Google Cloud**

Accesați:
[https://console.cloud.google.com/apis/credentials](https://console.cloud.google.com/apis/credentials)

**2. Creați un nou ID de Client OAuth 2.0**

- Dacă **"Cerințe noi Creare"** → **"ID de client OAuth"**
- Tip aplicație: **"Aplicație Web"**
- Nume: orice valori voastre (de exemplu `OmniRoute Remote`)

**3. Adăugați URILE autorizate de returnare**

În câmpul **"URILE autorizate de returnare"**, adăugați:

```
https://your-server.com/callback
```

> Înlocuiți `your-server.com` cu domeniul sau adresa IP a serverului
> dumneavoastră (include portul dacă este necesar, de exemplu
> `http://45.33.32.156:20128/callback`).

** 4. Salvați și copiați creditorii **

După crearea, Google va arăta ID-ul **Client** și secretul **Client**.

** 5. Setează variabilele de mediu **

În fișierul .env ` (sau variabilele de mediu Docker [`):

```bash
# Pentru Antigravity:
ANTIGRAVITY_OAUTH_CLIENT_ID=your-client-id.apps.googleusercontent.com
ANTIGRAVITY_OAUTH_CLIENT_SECRET=GOCSPX-your-secret

# Pentru Gemini CLI:
GEMINI_OAUTH_CLIENT_ID=your-client-id.apps.googleusercontent.com
GEMINI_OAUTH_CLIENT_SECRET=GOCSPX-your-secret
GEMINI_CLI_OAUTH_CLIENT_SECRET=GOCSPX-your-secret
```

** 6. Reîncepe OmniRoute **

```bash
# npm:
npm run dev

# Docker:
docker restart omniroute
```

** 7. Încearcă conectarea din nou **

Panoul controler → Fornitori → Antigravity (sau Gemini CLI) → OAuth

Google va redirecta acum corect în `https://your-server.com/callback`

---

#### Soluție temporară (fără credențiale personalizate)

Dacă nu doriți să configurați credențialele proprii în prezent, puteți totuși
folosi fluxul de URL manual **:

1. OmniRoute deschide URL-ul de autorizare Google
2. După autorizare, Google încearcă să redecoleze în `localhost` (care eşuează
   pe serverul local)
3. ** Copiați URL-ul complet ** din bara de adrese a browserului (înăuntru
   aflate chiar dacă pagina nu s-a încărcat)
4. Înfigeți acel URL în câmpul arătat în modala de conectare OmniRoute
5. Dați clic pe **"Conectare"**

> Acest lucru funcționează fiindcă codul de autorizare din URL este valid
> indiferent de reușita încărcării paginii de redirect.

---

<details>
<summary><b>🇧🇷 Versão em Português</b></summary>

#### De ce OAuth-ul de la Antigravity/Gemini CLI eşuează pe serverele remotoe?

Furnizorii **Antigravity** și **Gemini CLI** folosesc **OAuth 2.0** Google
pentru autentificare. Google cere ca `uricerea de redirect` folosită în fluxul
OAuth să fie **exactă** una dintre URIs-ul pre-defalcate la Google Cloud
Console-ul aplicatieiu.

As credenciais OAuth embutidas no OmniRoute estão cadastradas **apenas para
`localhost`**. Quando você acessa o OmniRoute em um servidor remoto (ex:
`https://omniroute.meuservidor.com`), o Google rejeita a autenticação com:

```
Eroare 400: redirect_uri_mismatch
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

**6. Restartați ruta de Omni**

```bash
# Dacă utilizați npm:
npm run dev

# Dacă utilizați Docker:
docker restart omniroute
```

**7. Încearcă să te conectezi din nou**

Consolă → Furnizori → Antigravitație (sau CLI Gemini) → Autentificare OAuth

Acum, Google-ul va redirecționa corect spre
`https://serviciul-tuw-servidor.com/callback` și autentificarea va funcționa.

---

#### Comportament temporar (fără configurarea propriilor credențiale)

Dacă nu doriți să creați credențiale proprii în prezent, încă puteți folosi
fluxul **manual de URL**:

1. Ruta de Omni își va deschide URL-ul de autorizare al Google-ului
2. După autorizare, Google-ul încearcă să redirecționeze spre `localhost` (care
   eșuează pe serverul de la distanță)
3. **Copiați URL-ul complet** din bara de adrese a browserului dvs. (însă și
   dacă pagina nu se încarcă)
4. Îngropați acea URL în câmpul care apare în modalul de conexiune a Rutei de
   Omni
5. Apăsați pe **"Conectare"**

> Acest lucru funcționează pentru că codul de autorizare din URL este valabil
> indiferent dacă redirectul a încărcat sau nu.

</details>

---

</details>

## 🛠️ Stivă Tehnică

<details>
<summary><b>Click to expand tech stack details</b></summary>

- **Runtime**: Node.js 18–22 LTS (⚠️ Node.js 24+ nu este **suportat** — `bunuri
  native pentru `better-sqlite3[X95X] nu sunt compatibile)
- **Limba**: TypeScript 5.9 - **100% TypeScript** în toate `sursa/` și
  `open-sse/` (nu există `oricine` în modulele de bază din v2.0)
- **Războiul frameworkului**: Next.js 16 + React 19 + Tailwind CSS 4
- **Bază de date**: LowDB (JSON) + SQLite (starea domeniului + jurnale proxy +
  audit MCP + deciziile de rutare)
- **Schemă**: Zod (MCP instrumentelor de validare de I/O, contracte API)
- **Protocol**: MCP (stdio/ HTTP) + A2A v0.3 (JSON-RPC 2.0 + SSE)
- **Transmiterea**: Evenimente Server-Sender (SSE)
- **Autentificare**: OAuth 2.0 (PKCE) + JWT + Chei API + Autorizarea Scoped MCP
- **Testare**: Rulare de test Node.js + Vitest (900+ de teste inclusiv unitare,
  de integrare, E2E)
- **CI/CD**: Acțiuni GitHub (auto publicare npm + Docker Hub la lansare)
- **Site-ul oficial **: [omniroute.online](https://omniroute.online)
- **Pachet**:
  [npmjs.com/package/omniroute](https://www.npmjs.com/package/omniroute)
- **Docker**:
  [hub.docker.com/r/diegosouzapw/omniroute](https://hub.docker.com/r/diegosouzapw/omniroute)
- **Resiliență**: Circuit breaker, backoff exponențial, anti-turbă în hăți,
  spoofing TLS, auto-combo self-healing

</details>

---

## Documentare

| Document                                       | Descriere                                                                       |
| ---------------------------------------------- | ------------------------------------------------------------------------------- |
| [Caietul Utilizator](docs/USER_GUIDE.md)       | Furnizori, combinații, integrare CLI, implementare                              |
| [Răspunsuri API](docs/API_REFERENCE.md)        | Toate endpointurile cu exemple                                                  |
| [Serviciul MCP](open-sse/mcp-server/README.md) | 16 instrumente MCP, configurații IDE, clienți Python/TS/Go                      |
| [Serviciul pentru A2A](src/lib/a2a/README.md)  | Protocolul JSON-RPC 2.0, abilități, transmitere în flux, gestionarea sarcinilor |
| [Motorul Auto-Combo](docs/auto-combo.md)       | 6-factor scoring, mode packs, self-healing                                      |
| [Troubleshooting](docs/TROUBLESHOOTING.md)     | Common problems and solutions                                                   |
| [Architecture](docs/ARCHITECTURE.md)           | System architecture and internals                                               |
| [Contributing](CONTRIBUTING.md)                | Development setup and guidelines                                                |
| [OpenAPI Spec](docs/openapi.yaml)              | OpenAPI 3.0 specification                                                       |
| [Security Policy](SECURITY.md)                 | Vulnerability reporting and security practices                                  |
| [VM Deployment](docs/VM_DEPLOYMENT_GUIDE.md)   | Complete guide: VM + nginx + Cloudflare setup                                   |
| [Features Gallery](docs/FEATURES.md)           | Visual dashboard tour with screenshots                                          |
| [Release Checklist](docs/RELEASE_CHECKLIST.md) | Pre-release validation steps                                                    |

---

## 🗺️ Roadmap

OmniRoute has **210+ features planned** across multiple development phases. Here
are the key areas:

| Category                        | Caracteristici Planificate | In curs de desfăşurare                                                                                        |
| ------------------------------- | -------------------------- | ------------------------------------------------------------------------------------------------------------- |
| 🧠 **Rutare & Intelect**         | 25+                        | Rutare cu latenţă minimă, rutare bazată pe etichete, pre-verificare de cuota, selectare cont P2C              |
| 🔒 **Securitate & Conformitate** | 20+                        | Strecurire anti-SSRF, ascundere a credenţialelor, limitare de rată pe endpoint, scoping cheilor de gestionare |
| 📊 **Observabilitate**           | 15+                        | Integrare OpenTelemetry, monitorizare real-time a cuotelor, urmărire a costurilor pe model                    |
| 🔄 **Integrate Proveidesi**      | 20+                        | dinamic registrare de model, cooldownuri de provider, Codex cu mai multe conturi, paring de cuota Copilot     |
| ⚡ **Performanţă**               | 15+                        | Cache dual, cache de prompturi, cache de răspunsuri, păstrare în urmă de streaming, API în loturi             |
| 🌐 **Eco-sistem**                | 10+                        | API WebSocket, recuperare caldă de configuraţie, stocare distribuită de configuraţie, mod comercial           |

### 🔜 Sfârşit de Zi de Mâine

- 🔗 **Integrare cu OpenCode** — Suport nativ pentru provider-ul IDE-ului de
  codare inteligentă OpenCode
- 🔗 **Integrare TRAE** — Sprijin complet pentru framework-ul de dezvoltare AI
  TRAE
- 📦 **API în Lot** — Prelucrare în paralel în loturi pentru cereri în masă
- 🎯 **Ruteare pe Bază de Etichete** — Rutează cererile pe baze de etichete și
  metadata personalizate
- 💰 **Strategia de Costuri Cele Mai Mici** — Selectează automat furnizorul
  disponibil cel mai ieftin

> 📝 Specificațiile detaliate ale tuturor caracteristicilor disponibile în
> [`docs/nou-acteristici/`](docs/new-features/) (217 speciaifcații detaliate)

---

## 👥 Contribuitori

[![Contribuitori](https://contrib.rocks/image?repo=diegosouzapw/OmniRoute&max=100&columns=20&anon=1)](https://github.com/diegosouzapw/OmniRoute/graphs/contributors)

### Cum să Contribuiți

1. Folosiți fork-ul repozitorului
2. Creați rama cu caracteristicile dumneavoastră (`git checkout -b
   feature/amazing-feature`)
3. Comitereți modificările (`git commit -m 'Adăugați o caracteristică
   amazoană'`)
4. Dați o push pe rama (`git push origin feature/amazing-feature`)
5. Deschideți unul Pull Request

Vedeți pentru ghiduri detaliate [[CONTRIBUTING.md](CONTRIBUTING.md)]

### Publicarea Unei Noi Versiuni

```bash
# Crearea unei noi versiuni – pubicarea cu npm se face automat
gh release create v2.0.0 --title "v2.0.0" --generate-notes
```

---

## 📊 Istoricul Stelelor

## Stelele pe parcursul timpului

## [![Stele pe parcursul timpului](https://starchart.cc/diegosouzapw/OmniRoute.svg?variant=adaptive)](https://starchart.cc/diegosouzapw/OmniRoute)

## 🙏 Mulțumirile noastre

Mulțumiri speciale lui **[9router](https://github.com/decolua/9router)** de
**[decolua](https://github.com/decolua)** — proiectul original care a inspirat
această ramură. OmniRoute construiește asupra acelei fundații incredibile cu
caracteristici suplimentare, API-uri multi-mode și o recompilare completă
TypeScript.

Mulțumiri speciale lui
**[CLIProxyAPI](https://github.com/router-for-me/CLIProxyAPI)** — implementarea
Go originală care a inspirat această portare în JavaScript.

---

## 📄 Licență

Licență MIT - consultați [LICENSE](LICENSE) pentru detalii.

---

<div align="center">
  <sub>Built with ❤️ for developers who code 24/7</sub>
  <br/>
  <sub><a href="https://omniroute.online">omniroute.online</a></sub>
</div>
<!-- GitHub Discussions enabled for community Q&A -->
