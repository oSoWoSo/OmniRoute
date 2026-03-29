# 🚀 OmniRoute — Den Frie AI Gateway

### Fortset altid kodning. Smarte ruter til **gratis & lavomkostning AI-modeller** med automatisk fald tilbage.

_Din enhedsværktøj til API - en enkelt slutpunkt, 67+ leverandører, ingen
nedetid. Nu med **MCP & A2A** agentkoordinering._

**Chat Kompletering • Embedding • Billede Generering • Video • Musik • Lyd •
Reranking • **Web Søgning** • MCP Server • A2A Protokol • 100% TypeScript**

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
[![Licens](https://img.shields.io/github/license/diegosouzapw/OmniRoute)](https://github.com/diegosouzapw/OmniRoute/blob/main/LICENSE)
[![Website](https://img.shields.io/badge/Website-omniroute.online-blue?logo=google-chrome&logoColor=white)](https://omniroute.online)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-Community-25D366?logo=whatsapp&logoColor=white)](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

[🌐 Website](https://omniroute.online) • [🚀 Hurtig Start](#-quick-start) • [💡
Færdighed](#-key-features) • [📖 Dokumentation](#-documentation) • [💰
Priser](#-pricing-at-a-glance) • [💬
WhatsApp](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

</div>

🌐 **Tilgængelig i:** 🇺🇸 [Engelsk](README.md) | 🇧🇷 [Portugisisk
(Brasil)](docs/i18n/pt-BR/README.md) | 🇪🇸 [Spansk](docs/i18n/es/README.md) | 🇫🇷
[Fransk](docs/i18n/fr/README.md) | 🇮🇹 [Italiensk](docs/i18n/it/README.md) | 🇷🇺
[Russisk](docs/i18n/ru/README.md) | 🇨🇳 [Kinesisk
(forenklet)](docs/i18n/zh-CN/README.md) | 🇩🇪 [Tysk](docs/i18n/de/README.md) | 🇮🇳
[Hindi](docs/i18n/in/README.md) | 🇹🇭 [Thailandsk](docs/i18n/th/README.md) | 🇺🇦
[Ukrainsk](docs/i18n/uk-UA/README.md) | 🇸🇦 [Arabisk](docs/i18n/ar/README.md) |
🇯🇵 [Japansk](docs/i18n/ja/README.md) | 🇻🇳 [
Vietnamesisk](docs/i18n/vi/README.md) | 🇧🇬 [Bulgarsk](docs/i18n/bg/README.md) |
🇩🇰 [Dansk](docs/i18n/da/README.md) | 🇫🇮 [Finsk](docs/i18n/fi/README.md) | 🇮🇱
[Hebraisk](docs/i18n/he/README.md) | 🇭🇺 [Ungarsk](docs/i18n/hu/README.md) | 🇮🇩
[Indonesisk](docs/i18n/id/README.md) | 🇰🇷 [Koreansk](docs/i18n/ko/README.md) |
🇲🇾 [Malaysisk](docs/i18n/ms/README.md) | 🇳🇱 [Hollandsk](docs/i18n/nl/README.md)
| 🇳🇴 [Norsk](docs/i18n/no/README.md) | 🇵🇹 [Portugisisk
(Portugal)](docs/i18n/pt/README.md) | 🇷🇴 [Rumænsk](docs/i18n/ro/README.md) | 🇵🇱
[Polsk](docs/i18n/pl/README.md) | 🇸🇰 [Slovakisk](docs/i18n/sk/README.md) | 🇸🇪
[Svensk](docs/i18n/sv/README.md) | 🇵🇭 [Filippinsk](docs/i18n/phi/README.md) | 🇨🇿
[Tjekkisk](docs/i18n/cs/README.md)

---

## 🆕 Hva er der nytt i v3.0.0

> **Opgrebet fra v2.9.5?** — Se [fuld
> CHANGELOG](CHANGELOG.md#300--2026-03-22-release-candidate--not-yet-merged-to-main)
> for alle ændringer.

| Omraade                        | Förändring                                                                                                                                        |
| ------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🔒 **CodeQL Sikkerhed**         | Fikset 10+ CodeQL-advarsel: polynomial-redos, usikker tilfældighed, skabelon-injektion reparation                                                 |
| ✅ **Vejr Vejledning**          | Alle 176 API-rute nu valideret med Zod-schemas + `validateBody()` — CI ` check:route-validation:t06` passerer                                     |
| 🐛 **omniModel Tag Udsnit**     | Intern `<omnimodel>` tags ikke længere udstødt til kunder i SSE-strømmede svar (#585)</omnimodel>                                                 |
| 🔑 **Tilmeldt Nyttigave API**   | Auto-provision API-keys via `POST /api/v1/registered-keys` med per-leverandør/konto kvoter, idempotens, SHA-256-lagring og valgfri GitHub-ændring |
| 🎨 **Leverandør Icons**         | 130+ leverandør logoer via `@lobehub/icons` (SVG) med PNG → generel fallback-kæde                                                                 |
| 🔄 **Model Auto-Sync**          | 24 timerscheduler og manuel UI tast for at synkronisere model liste for bygningsofagt og brugerdefinerede OpenAI-kompatible leverandører          |
| 🌐 **OpenCode Zen/Go**          | To nye leverandører fra @kang-heewon via PR #530: gratis niveau + abonnements niveau via `OpencodeExecutor`                                       |
| 🐛 **Gemini CLI OAuth**         | Handlingeligt fejlmeddelelse når `GEMINI_OAUTH_CLIENT_SECRET` mangler i Docker (var tvetydig Google fejl)                                         |
| 🐛 **OpenCode konfiguration**   | `saveOpenCodeConfig()` skriver korrekt TOML til `XDG_CONFIG_HOME`                                                                                 |
| 🐛 **Fastsatte model overstyr** | `body.model` sættes korekt til `pinnedModel` på kontekst-cache beskyttelse                                                                        |
| 🐛 **Codex/Claude loop**        | `tool_result` blokke nu konverteres til tekst for at stoppe uendelige løb                                                                         |
| 🐛 **Login omdirigering**       | Login bevæger sig ikke længere i stå efter at have springt over passwordopsætning                                                                 |
| 🐛 **Windows-stier**            | MSYS2/Git-Bash-stier (`/c/...`) normaliseres til `C:\...` automatisk                                                                              |

---

## 🖼️ Hoveddashboard

<div align="center">
  <img src="./docs/screenshots/MainOmniRoute.png" alt="OmniRoute Dashboard" width="800"/>
</div>

---

## 📸 Omsider for hoveddashboard

<details>
<summary><b>Click to see dashboard screenshots</b></summary>

| Side                    | Skærmbillede                                             |
| ----------------------- | -------------------------------------------------------- |
| **Leverandører**        | ![Leverandører](docs/screenshots/01-providers.png)       |
| **Kombinationer**       | ![Kombinationer](docs/screenshots/02-combos.png)         |
| **Analyser**            | ![Analyser](docs/screenshots/03-analytics.png)           |
| **Sundhed**             | ![Sundhed](docs/screenshots/04-health.png)               |
| **Oversætter**          | ![Oversætter](docs/screenshots/05-translator.png)        |
| **Indstillinger**       | ![Ind Stillinger](docs/screenshots/06-settings.png)      |
| **CLI-Tool**            | ![CLI-Tool](docs/screenshots/07-cli-tools.png)           |
| **Brug Logs**           | ![Brug](docs/screenshots/08-usage.png)                   |
| **Afsluttende punkter** | ![Afsluttende punkter](docs/screenshots/09-endpoint.png) |

</details>

---

### 🤖 Frit AI-leverandør for din favorit coding agent

_Tilslut enhver AI-mydelt integreret IDÉ eller CLI-tool gennem OmniRoute —
gratis API-gateway for uendelig kodeing.

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

<sub>📡 Alle agenter forbinder via <code>http://localhost:20128/v1</code> eller
<code>http://cloud.omniroute.online/v1</code> — én konfiguration, uendeligt
model og kvote</sub>

---

## 🤔 Hvorfor OmniRoute?

** Stop at at sprede pengene og ramme begrænsninger:**

- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Abonnementskvoten udbetales uanvendt hver måned
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Hastighedsgrenser får dig ved at kode
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Dyrte API ($20-50/måned pr. leverandør)
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Manuel switiching mellem leverandører

**OmniRoute løser dette:**

- ✅ **Maximér abonnementer** - Følg kvote, brug hver del før dette udbetales
- ✅ **Auto fallback** - Abonnement → API-kode → Billig → Gratis, ingen down-time
- ✅ **Multi-konto** - Rund-robin-mekanisme mellem konti pr. leverandør
- ✅ **Universel** - Fungerer med Claude Code, Codex, Gemini CLI, Cursor, Cline,
  OpenClaw, hvilken som helst CLI-tool

---

## 📧 Support

> 💬 **Del med os på communityen!** [WhatsApp
> Group](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t) – Få hjælp,
> dele tips og bliv opdateret

- **Hjemmeside**: [omniroute.online](https://omniroute.online)
- **GitHub**:
  [github.com/diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute)
- **Issue**:
  [github.com/diegosouzapw/OmniRoute/issues](https://github.com/diegosouzapw/OmniRoute/issues)
- **WhatsApp**:
  [Fællestillads](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)
- **Bidrag**: Se [CONTRIBUTING.md](CONTRIBUTING.md), åbn en pull request og find
  eller vælg en `god first issue`
- **Original Afhandling**: [9router by
  decolua](https://github.com/decolua/9router)

### 🐛 Rapportér Fejl?

Når du åbner en issue, bedes du køre kommandoen system-info og tilføje den
genererede file:

```bash
npm run system-info
```

Det genererer en `system-info.txt` med din Node.js-version, OmniRoute-version,
OS-oplysninger, installeret CLI-tilgængelighed (iflow, gemini, claude, codex,
antigravitets, droid o. s. v.), Docker/PM2-status og system-pakker - alt hvad vi
behøver for at reproducere dit problem hurtigt. Tilføj filen direkte til din
GitHub-issue.

---

## Hvordan det virker

```
┌─────────────┐
│  Din CLI-tilgængelighed   │  (Claude Code, Codex, Gemini CLI, OpenClaw, Cursor, Cline...)
│   Tool      │
└──────┬──────┘
       │ http://localhost:20128/v1
       ↓
┌─────────────────────────────────────────┐
│           OmniRoute (Smart Router)        │
│  • Formatoversættelse (OpenAI ↔ Claude) │
│  • Quotastyring + Embeddings + Billeder │
│  • Automatisk token gensyn                   │
└──────┬──────────────────────────────────┘
       │
       ├─→ [Niveau 1: Abo] Claude Code, Codex, Gemini CLI
       │   ↓ quota forbrugt
       ├─→ [Niveau 2: API-KEY] DeepSeek, Groq, xAI, Mistral, NVIDIA NIM, osv.
       │   ↓ budgetgrænse
       ├─→ [Niveau 3: BILLIGT] GLM ($0,6/1M), MiniMax ($0,2/1M)
       │   ↓ budgetgrænse
       └─→ [Niveau 4: GRATIS] iFlow, Qwen, Kiro (usideskæbningsgrænse)

Resultat: Aldrig stop med at kode, minimal omkostninger
```

---

## 🎯 Hvad OmniRoute Løser - 30 Reelle Smertepunkter og Brugscasus

> **Hver enkelt udvikler, der bruger AI-tilgængelighed, støder på disse
> problemer dagligt.** OmniRoute er bygget til at løse dem alle - fra
> forbrugsoverdrivelse til regionale blokeringer, fra brudte OAuth-fluer til
> protokoltilgængelighed og enterprise observabilitet.

<details>
<summary><b>💸 1. "I pay for an expensive subscription but still get interrupted by limits"</b></summary>

Udviklere betaler 20-200 kr. om måneden for Claude Pro, Codex Pro eller GitHub
Copilot. Selv når man betaler, er der et tak for quota - 5 timer af brug,
ugentlige begrænsninger eller minutlige rate begrænsninger. Midt om
kodingssessionen går udbyderen i svar, og udvikleren taber flow og
produktivitet.

**Hvordan OmniRoute løser det:**

- **Intelligens 4-Tier Fallback** - Hvis abo-quota er udtømt, automatisk
  omdirigerer til API-KEY → Cheap → Free med ingen manuel indsigt
- **Real-Time Quotastyring** - Viser token forbrug i realtid med rest tid regnes
  (5 h, daglig, ugentlig)
- **Multi-Account Support** - Flere kontoer pr. udbyder med auto rund-robin —
  når en bruges op, skifter til næste
- **Custom Combos** - Anpasselige fallback-kæder med 6 balanceregningsstrategier
  (fill-first, round-robin, P2C, tilfældig, mindst brugt, kost-optimiseret)
- **Codex Business Quotas** - Business/Team workspace-hold quo monitoring
  direkte i dashboardet

</details>

<details>
<summary><b>🔌 2. "I need to use multiple providers but each has a different API"</b></summary>

OpenAI bruger en format, Claude (Anthropic) bruger en anden, Gemini endnu en
anden. Hvis en udvikler vil teste modeller fra forskellige udbydere eller
fallback mellem dem, skal de genconfigurere SDK'er, ændre endpoint, hånde med
uforenelige formattegn. Annoncerede udbydere (FriendLI, NIM) har ikke-standard
model-endpoint.

**Hvordan OmniRoute løser det:**

- **Forenklet Endpoint** — En enkelt `http://localhost:20128/v1` tjener som
  proxy for alle 67+ udbydere
- **Format Oversættelse** — Automatisk og transparent: OpenAI ↔ Claude ↔ Gemini
  ↔ Responses API
- **Svarssanering** — Fjerner ikke-standard felter (`x_groq`, `usage_breakdown`,
  `service_tier`) som kan brædde OpenAI-SDK v1.83+
- **Rollefordeling** — Omformer `udvikler` → `system` for ikke-OpenAI-levere;
  `system` → `bruger` for GLM/ERNIE
- **Tænk-mærkeaftryk extraction** — Fjerner `<think>`-blokke fra modeller som
  DeepSeek R1 til standardiserede `reasoning_content`</think>
- **Struktureret udgave for Gemini** — `json_schema` →
  `responseMimeType`/`responseSchema` automatisk konvertering
- **`stream` er standardmæssigt `false`** — Sammenligner sig med
  OpenAI-specifikationen, hvilket undgår uvante SSE i Python/Rust/Go-SDK'erne

</details>

<details>
<summary><b>🌐 3. "My AI provider blocks my region/country"</b></summary>

Tilbydere som OpenAI/Codex afviser adgang fra vist af bestemte geografiske
regioner. Brugere få mislykkede forsøg som
`unsupported_country_region_territory` under OAuth- og API-forbindelser. Dette
kan være spændende for udviklere fra udviklingslande.

**Hvordan OmniRoute løser det:**

- **3-Niveau Proxykonfiguration** — Konfigurere proxy på 3 niveauer: global
  (alle trafik), per-tilbyder (en tilbyder kun) og per-connection/key
- **Forkoblede proxy-badger** — Visuelle indikatorer: 🟢 global proxy, 🟡 provider
  proxy, 🔵 connection proxy, altid vist IP-adressen
- **OAuth-token udveksling gennem proxy** — OAuth-flådens også går gennem
  proxyen, løsninger for `unsupported_country_region_territory`
- **Forbindelsesprøver gennem proxy** — Forbindelsesprøver bruger konfigureret
  proxy (ingen længere direkte omgåelse)
- **SOCKS5-understøttelse** — Fuld SOCKS5-proxy-understøttelse for udgående
  routing
- **TLS-fingeraftving** — Browser-aktuel TLS-finger aftving ved hjælp af
  `wreq-js` til at undgå bot-detection
- **🔏 CLI-finger-matchning** — Omdaner headers og body-felter til at matche det
  oprindelige CLI-binær-signatur, dramatisk reducerer risiko for
  regneark-flagning. Proxy-IP'en bevarer sig - du får både stealth **og**
  IP-maskering samtidigt

</details>

<details>
<summary><b>🆓 4. "I want to use AI for coding but I have no money"</b></summary>

Ikke alle kan betale 20–200$/måned for AI-tilkøb. Studerende, udviklere fra
fremvoksende lande, hobbiemere og freelancerer har brug for adgang til
kvalifikationsmodeller uden omkostninger.

**Hvordan OmniRoute løser det:**

- **Indbygget tilbydere på fri grund** — Nativ understøttelse af 100% fri
  tilbydere: iFlow (5 ubegrænsede modeller via OAuth: kimi-k2-tenkning,
  qwen3-koder-plus, deepseek-r1, minimax-m2, kimi-k2), Qwen (4 ubegrænsede
  modeller: qwen3-koder-plus, qwen3-koder-flash, qwen3-koder-næste,
  vison-model), Kiro (Claude + AWS Byggeid for frie)
- **Ollama Cloud** — Cloud-fører Ollama-modeller på `api.ollama.com` med fri
  "Lys bæsikt" niveau; brug `ollamacloud/<model>` prefx</model>
- **Fri-only kombineringer** — Kæde `gc/gemini-3-flash → if/kimi-k2-tenkning →
  qw/qwen3-koder-plus` = $0/måned uden nedetid
- **NVIDIA NIM fri adgang** — ~40 RPM-dev forever fri adgang til 70+ modeller på
  build.nvidia.com (overgang fra kreditter til renere rate begrensninger)
- **Strategi for Økonomisk Optimering** — Routing strategi, der automatisk
  vælger den billigste tilgængelige leverandør

</details>

<details>
<summary><b>🔒 5. "I need to protect my AI gateway from unauthorized access"</b></summary>

Når man udsætter en AI Gateway for nettet (LAN, VPS, Docker), kan enhver med
adressen forbruge udviklerens tokens/quotum. Without beskyttelse er APIs
følsomme over for misbrug, prompt-injektion og misbrug.

**Hvordan OmniRoute løser det:**

- **API-nyttekortshåndtering** — Generering, rotation og oprettelse af
  begrænsninger per leverandør på en dedikeret `/dashboard/api-manager` side
- [X2X]Model-niveau tilgange** — Restriks programmer for at begrænse
  nøgleindtastning til bestemte modeller (`openai/*`, wildcard-mønstre), med
  Tillad Alle/Afvis-svitch
- [X3X]Beskyttelse af API-slutpunkter** — Kræver en nøgle for `/v1/models` og
  blokerer specifikke leverandører fra listen
- [X4X]Autograf + CSRF-beskyttelse** — Alle dashboard-ruter beskyttet med
  `withAuth`-middleware + CSRF-token
- [X5X]Taksgrænse for IP-adresser** — Per-IP taksgrænse med konfigurerbare
  vinduer
- [X6X]Filtrering af IP-adresser** — Bemyndigende eller blokliste for
  tilgangskontrol
- [X7X]Våbenhvile før prompt-injektion** — Sanering mod forurenende
  prompt-mønstre
- [X8X]AES-256-GCM-kryptering** — Kreditorer krypteret på hvile

</details>

<details>
<summary><b>🛑 6. "My provider went down and I lost my coding flow"</b></summary>

AI-leverandører kan blive ustabile, vende med 5xx-fejl eller ramme i
midlertidige hastighedsgrænser. Hvis udvikler afhænger af en enlig leverandør,
bliver de afbrudt. Without kredsløbsbrydere kan gentage forsøg ødelægge
aplikationen.

**Hvordan OmniRoute løser det:**

- [X9X]Kredsløbsbrydere per-model** — Auto-åbn/slut med konfigurerbare trin og
  cooldown (Closed/Open/Half-Open), afskåret per-model til at undgå fjernagtige
  blokkeringer
- [X10X]Exponential Backoff** — Fremadgående gentage-forsøg med forsinkelser
- [X11X]Anti-Thundering Herd** — Mutual-exklusivt adgangsskift &
  semafor-protektion mod samtidige genbesøg
- [X12X]Kombinerede faldgrundkæder** — Hvis den primære leverandør mislykkes,
  falder automatisk igennem kæden uden intervenção
- [X13X]Kombineret kredsløbsbrydere** — Auto-ophæver fejlende leverandører inden
  for en kombineret kæde
- [X14X]Helse Dashboard** — Uptime-overvågning, kredsløbsbrydere tilstande,
  bloceringer, cache-statistik, p50/p95/p99 latence

</details>

<details>
<summary><b>🔧 7. "Configuring each AI tool is tedious and repetitive"</b></summary>

Udviklere bruger Cursor, Claude Code, Codex CLI, OpenClaw, Gemini CLI, Kilo
Code... Hver enkelt værktøj har et forskelligt konfiguration (API-slutpunkt,
nøgle, model). Rekondering, når man skifter leverandør eller model, er
tidsslös.\
==WEBLATE_PART==

**Hvordan OmniRoute løser det:**

- **CLI-Toolers Bord** — Dedicated side med én-klikke-konfiguration af Claude
  Code, Codex CLI, OpenClaw, Kilo Code, Antigravity, Cline
- **GitHub Copilot Konfigurationgenerator** — Genererer
  `chatLanguageModels.json` untuk VS Code med bulk-tilgods model valg
- **Onboarding Wizard** — Vejledende 4-stegs oprettelse for første-gangs brugere
- **Een endpoint, alle modeller** — Konfigurer `http://localhost:20128/v1` kun
  én gang, og få adgang til mere end 67 leverandører

</details>

<details>
<summary><b>🔑 8. "Managing OAuth tokens from multiple providers is hell"</b></summary>

Claude Code, Codex, Gemini CLI, Copilot — alle bruger OAuth 2.0 med udløbende
tokens. Udviklere skal genautorisere konstant, håndtere `client_secret er
manglende`, `redirect_uri_mismatch`, og fejl på fjernservere. OAuth på LAN/VPS
er især problematisk.

**Hvordan OmniRoute løser det:**

- **Auto Token Refresh** — OAuth-tokens refreshed i bagskærm før udløb
- **OAuth 2.0 (PKCE) Bygget-in** — Automatisk strøm for Claude Code, Codex,
  Gemini CLI, Copilot, Kiro, Qwen, iFlow
- **Multi-Akkuet OAuth** — Flere konti pr leverandør via JWT/ID token udtrækning
- **OAuth LAN/Remote Fix** — Private IP-detection for `redirect_uri` + manuel
  URL-mode for fjernservere
- **OAuth Bag Nginx** — Bruger `window.location.origin` for
  tilbagefåndighedskompatibilitet med reverse proxy
- **Remote OAuth Guide** — Trin-trin guide for Google Cloud-krediter på
  VPS/Docker

</details>

<details>
<summary><b>📊 9. "I don't know how much I'm spending or where"</b></summary>

Udviklere bruger flere betalende leverandører, men har ikke en Forenede visning
af udgifter. Hvert leverandør har sit eget regningabord, men der er ingen
konsolideret visning. Uventede udgifter kan bygge op.

**Hvordan OmniRoute løser det:**

- **Kostanalysebord** — Per-token udgiftsafstemning og budgetstyring pr
  leverandør
- **Budgetgrænser pr trin** — Omkostningsgulv pr trin, der trigger automatisk
  fald
- **Per-Model Prisconfiguration** — Konfigurerbare priser pr model
- **Brug-tilstuder Statistik pr API-tast** — Opløb og størst-tilsyndt timestamp
  pr tast
- **Analysebord** — Stat kort, model-anvendelsesgrafik, leverandør tabel med
  succeshastigheter og latency

</details>

<details>
<summary><b>🐛 10. "I can't diagnose errors and problems in AI calls"</b></summary>

==WEBLATE_PART==\
[Hver gang et opkald fejler, ved ikke udvikleren om det var på grund af rate
limit, udløbet token, forkert format eller provider-fejl. Fragmenterede logfiler
over forskellige terminaler. uden Observability, debugging er trial-and-fejl.

**Hvordan OmniRoute løser det:**

- ** Forenede Logs Dashboard ** – 4 tabs: Anmodninger Logs, Proxy Logs, Audit
  Logs, Konsoles
- ** Konsole Log Viewer ** — Real-time terminal-stilvis forudfølgende med
  farve-koderede niveauer, auto-skroll, søgning, filter
- ** SQLite Proxy Logs ** — Fastholdte logfiler, der overlever server-restarter
- ** Oversætter Playground ** — 4 udviklingsmodusser: Playground
  (formatoversættelse), Chat Test (round-trip), Test Bench (batch), Live Monitor
  (real-tid)
- ** Anmodning Telemetri ** — p50/p95/p99 latenstid + X- Anmodning-Id - trasing
- ** Filbaseret Logning med Rotation ** — Konsole-inspektoren capturerer alt til
  JSON-log, der roterer ved størrelse-baseret rotation
- ** Systeminfo Rapport ** — `npm run system-info` genererer `system-info.txt`
  med din fulde miljø (Node-version, OmniRoute-version, OS, CLI- værktøjer,
  Docker/PM2-status). Tilføj det ved at rapportere problemer for hurtig triage.

</details>

<details>
<summary><b>🏗️ 11. "Deploying and maintaining the gateway is complex"</b></summary>

Installering, konfiguration og vedligeholdelse af en AI-proxy over forskellige
miljøer (lokal, VPS, Docker, cloud) er arbeidskrævende. Problemer som
hardcoderede sti, ` EACCES ` på mapper, port-konflikter og tværforskningsbygning
tilføjer modstand.

**Hvordan OmniRoute løser det:**

- ** npm global install ** — ` npm install -g omniroute &amp;&amp; omniroute ` —
  gennemført
- ** Docker Multi-Platform ** — AMD64 + ARM64 nativ (Apple Silicon, AWS
  Graviton, Raspberry Pi)
- ** Docker Compose Profiles ** — ` base ` (ingen CLI-værktøjer) og ` cli ` (med
  Claude Code, Codex, OpenClaw)
- ** Electron Desktop App ** — Nativ app til Windows/macOS/Linux med systemtray,
  auto-start, offline-lager
- ** Split-Port Mode ** — API og Dashboard på separate porte for avancerede
  scenarier (omvendt proxy, containernetworking)
- ** Cloud Sync ** — Konfigurationssynchronisering over device via Cloudflare
  Arbejdere
- ** DB Backups ** — Automatisk backup, restore, eksport og import af alle
  indstillinger

</details>

<details>
<summary><b>🌍 12. "The interface is English-only and my team doesn't speak English"</b></summary>

Holdninger til ikke-Engelsktalende lande, i ørlighed Latin Amerika, Asien og
Europa, kæmper med Engelsk-only-grænsser. Sprogskegenskaber reducerer optagelse
og øger konfigurationsfejl.

**Hvordan OmniRoute løser det:**

- **Skærmbord i18n — 30 sprog** — Alle 500+ nøgler oversat, herunder Arabisk,
  Bulgarsk, Dansk, Tysk, Spansk, Finsk, Fransk, Hebraisk, Hind, Ungarsk,
  Indonesisk, Italiensk, Japansk, Koreansk, Malaj, Nederlandsk, Norsk, Polsk,
  Portugisisk (PT/BR), Rumænsk, Russisk, Slovansk, Svensk, Thai, Ukrainsk,
  Vietnamesisk, Kinesisk, Filippinsk, Engelsk
- **RTL-støtte** — Venstre-til-højre-støtte for Arabisk og Hebraisk
- **Multi-sprog READMEs** — 30 fuldstændige dokumentationsoversættelser
- **Sprogvalg** — Globe ikon i hovedet for real-time-skifting

</details>

<details>
<summary><b>🔄 13. "I need more than chat — I need embeddings, images, audio"</b></summary>

AI er ikke kun chatfærdighed. Devs har også brug for at generere billeder,
transskribere lydfiler, oprette embeddings for RAG, reranke dokumenter og
moderere indhold. Hvert API har sine forskellige endpoint og format.

**Hvordan OmniRoute løser det:**

- **Embeddings** — `/v1/embeddings` med 6 leverandører og 9+ model
- **Billedegenerering** — `/v1/images/generations` med 10 leverandører og 20+
  model (OpenAI, xAI, Together, Fireworks, Nebius, Hyperbolic, NanoBanana,
  Antigravity, SD WebUI, ComfyUI)
- **Tekst-til-Videofilm** — `/v1/videos/generations` — ComfyUI (AnimateDiff,
  SVD) og SD WebUI
- **Tekst-til-Musik** — `/v1/music/generations` — ComfyUI (Stable Audio Open,
  MusicGen)
- **Lydvolumetranskription** — `/v1/audio/transcriptions` — Whisper + Nvidia
  NIM, HuggingFace, Qwen3
- **Tekst-til-Tale** — `/v1/audio/speech` — ElevenLabs, Nvidia NIM, HuggingFace,
  Coqui, Tortoise, Qwen3, **Inworld**, **Cartesia**, **PlayHT**, + eksisterende
  leverandører
- **Moderation** — `/v1/moderations` — Indholds sikkerheds kontroller
- **Reranking** — `/v1/rerank` — Dokument relevans reranking
- **Svar API** — Fuldstændig `/v1/responses` understøttelse for Codex

</details>

<details>
<summary><b>🧪 14. "I have no way to test and compare quality across models"</b></summary>

Udviklere vil gerne vide, hvilken model, der er bedst til at føje til deres
brugsscenarie — kode, oversættelse, forklaring — men manuell sammenligne er
langsomt. Der findes heller ikke nogen integreret eval værktøj.

**Hvordan OmniRoute løser det:**

- **LLM-evalueringer** — Guld sætte testing med 10 forudbyggede tilfælde, der
  dækker hej, matematik, geografi, kodegenerering, JSON-kompliance,
  oversættelse, markdown, sikkerhedsafvisning
- **4 Match Strategier** — `eksakt`, ` indeholder`, ` regex`, `
  brugertdefineret` (JS-funktion)
- **Oversætter Prøvebænk** — Gruppe testing med flere input og forventede
  output, tværligende leverandør sammenligning
- **Samtale Prøve** — Fuldrundfærdig med visuel respons rendering
- **Live Monitor** — Enerret strib of all anmodninger der skal gennem proxy

</details>

<details>
<summary><b>📈 15. "I need to scale without losing performance"</b></summary>

Som anmodningsvolumes vokser, uden denne kaching af de samme spørgsmål genererer
duplikerede omkostninger. Uden idempotenti, duplikerede anmodninger vædder
fremgang i procesering. Per-leveranten hæfter rate hensyn skal være respekteret.

**Hvordan OmniRoute løser det:**

- **Semantisk Cache** — To-lags cache (signature + semantisk) reducere
  omkostninger og latency
- **Anmodningens Idempotenti** — 5s deduplication vindue for identiske
  anmodninger
- **Rate Limit Dtection** — Per-leveranten RPM, min og maks gaps tracking
- **Redigerbare Rate Limiter** — Konfigurerbare standarder i Settinge →
  Resilience med persistens
- **API Key Validation Cache** — 3-lags cache for produktionsperformance
- **Helse Dashboard med Telemetry** — p50/p95/p99 latency, cache stats, uptime

</details>

<details>
<summary><b>🤖 16. "I want to control model behavior globally"</b></summary>

Udviklerer som vil have alle responsers i en specifik sprog, med en specifik
tone, eller vil begrænse reasiningstoken skal ikke nødvendigvis konfigurre det i
hver eneste værktøj/ anmodning.

**Hvordan OmniRoute løser det:**

- **System Prompt Injection** — Globalt prompt tilføjet til alle anmodninger
- **Tænkningskasse Vedvalg** — Reasining token alloktion kontrol pr. anmodning
  (passthrough, auto, custom, adaptive)
- **6 Routing Strategier** — Globale strategier der bestemmer hvordan
  anmodninger kommer til at være distribueret
- **Wildcard Router** — `leveranten/*`mønster routeer dynamisk til enhver
  leverantør
- **Kombi Enable/Disable Toggle** — Toggle kombiner fra dashboardet med en
  enkelt klik
- **Leverantør Toggle** — Slut hele forbindelser for en leverantør med ét klik
- **Blokerede Leveranter** — Udeluk lavnevisse leveranter fra
  /v1/models/X67X]-listing

</details>

<details>
<summary><b>🧰 17. "I need MCP tools as first-class product capabilities"</b></summary>

Mange AI-gateways offentliggor MCP som skjult implementerings detalje. Hold
gerne en tydelig, gengældeligt operationslag.\
==WEBLATE_PART==

**Hvordan OmniRoute løser det:**

- MCP viser op i dashboard navigationsmenyen og endpoint-protokollside
- Dedikeret side til MCP-Administration, som indeholder processer, værktøjer,
  scoper og regneark
- Bænket quick-start for oprettelse af omniroute --mcp og klient tilmelding

</details>

<details>
<summary><b>🧠 18. "I need A2A orchestration with sync + stream task paths"</b></summary>

Agent-workflows skal have både direkte besvarelser og lange-running streamede
eksekution med livscykluskontrol.

**Hvordan OmniRoute løser det:**

- A2A JSON-RPC endpoint ( `POST /a2a` ) med `besked/send` og `besked/strøm`
- SSE-Streamning med terminaltilstaaende tilstand propagering
- Opgavs livscyklus APIs for `opgaver/hent` og `opgaver/afmelde`

</details>

<details>
<summary><b>🛰️ 19. "I need real MCP process health, not guessed status"</b></summary>

Rutinehold og udviklingshold skal vide, om MCP stadig er aktiv, ikke bare, om en
API er tilgængelig

**Hvordan OmniRoute løser det:**

- Runtime pulsarkiv med PID, tidsstempel, transport, værktøjsantal og scope-mode
- MCP-status API kombinerer pulsen + nylig aktivitet
- UI-statuskort for proces/holdbarhed/puls-ferskshed

</details>

<details>
<summary><b>📋 20. "I need auditable MCP tool execution"</b></summary>

Når værktøjer ændrer konfiguration eller udløser operations-aftaler skal teammet
have kriminelt tilgængelig skriftgreb.

**Hvordan OmniRoute løser det:**

- SQLite-baglagt regneark-logning for MCP-tools-forbindelser
- Filtrering ved hjælp af værktøj, success/failure, API nøgle og sideloose
  paginering
- Dashboard-regneark tabel + stats endpoints for selvforenende processer

</details>

<details>
<summary><b>🔐 21. "I need scoped MCP permissions per integration"</b></summary>

Klienter skal have mindst adgang til værktøj-kategorier.

**Hvordan OmniRoute løser det:**

- 9 detaljerede MCP-scopes for styring af kontrolleret værktøjsselvagt
- Udøvelse og synlighed af MCP-administrationssystemet
- Sikker standsning tilstandsstillæg for driftsarbejds-værktøj

</details>

<details>
<summary><b>⚙️ 22. "I need operational controls without redeploying"</b></summary>

Hold gerne hurtige justeringer omkring indgående eksempler eller udgifter

**Hvordan OmniRoute løser det:**

- Aktivering af swicth-kombination direkte fra MCP-brugerflade
- Gyldne resilience profiler fra uddragne pakker
- Nul-stemning af kredsløb-åbner fra samme operationspanel

</details>

<details>
<summary><b>🔄 23. "I need live A2A task lifecycle visibility and cancellation"</b></summary>

Uden livscyklus-synlighed bliver årsag til hård triage.

**Hvordan OmniRoute løser det:**

- Opgavesortering og filtrering efter tilstand/skylighed med flere sider
- Dykk ned i opgavelog, begivenheder og artefakter.
- Udsendelse af opgavestygning og UI-handle ved godkendelse

</details>

<details>
<summary><b>🌊 24. "I need active stream metrics for A2A load"</b></summary>

Strømmende værktøjer kræver drifts-synlighed i samtidighed og live-forbindelse.

**Hvordan OmniRoute løser det:**

- Aktive strøm-kunstnere integreret til A2A-status
- Sidste-opgavelog-stempel og tilstand-kunstnere
- A2A-overstyringskort til eksakt ops-montering

</details>

<details>
<summary><b>🪪 25. "I need standard agent discovery for clients"</b></summary>

Eksterne klienter og styrende styrtrenger har maskin-sammenlæsbart metadata i
registrerings-processen.

**Hvordan OmniRoute løser det:**

- Agent kort eksponeret på `/.well-known/agent.json`
- Færdigheder og tilgængelighed vist i driftsinterface
- A2A-status-API indeholder opdagelsesmetadata for automatisering

</details>

<details>
<summary><b>🧭 26. "I need protocol discoverability in the product UX"</b></summary>

Hvis brugere ikke kan opdage protokoloverflader, faldt adoptering og
støttekvalitet.

**Hvordan OmniRoute løser det:**

- Konsolideret **Slutpunkter** siden med faneblade til Proxy, MCP, A2A og
  API-slutpunkter
- Togglader til inline servicestatus (Online/Offline) for MCP og A2A
- Linker fra overview til dedikerede driftsbane

</details>

<details>
<summary><b>🧪 27. "I need end-to-end protocol validation with real clients"</b></summary>

Mock-tests er ikke nok til at validere protokollighed før udgivelse.

**Hvordan OmniRoute løser det:**

- E2E-testsamling der starter appen og bruger virkelig MCP SDK klient transport
- A2A klienttests for opdagelse, sende, strømme, få og aflyse fluxer
- Overstyres påskudd mod MCP Audit og A2A tasks APIs

</details>

<details>
<summary><b>📡 28. "I need unified observability across all interfaces"</b></summary>

Hvis du deler observabilitet efter protokoll, skaber det blinde punkter og
længere DRMT.

**Hvordan OmniRoute løser det:**

- Forenede dashboard/loganalyzer i én produkt
- Helse + audit + anfordring telemetri gennem OpenAI, MCP og A2A lag
- DRIFTSAPI'er for status og automatisering

</details>

<details>
<summary><b>💼 29. "I need one runtime for proxy + tools + agent orchestration"</b></summary>

Hvis mange separate tjenester køres, øger det operationel udgift og fejlmoder.

**Hvordan OmniRoute løser det:**

- Fornybar proxy, MCP-server og A2A-server på en stak
- Delte authentificering, tilgængelighed, opbevaring og overvågning
- Konsekvent politikmodel på alle interaktionsoverflader

</details>

<details>
<summary><b>🚀 30. "I need to ship agentic workflows without glue-code sprawl"</b></summary>

Hold dine holdbarehed da de svigter ved at samle forskellige ad-hoc-tjenester
og-scripts sammen

**Hvordan OmniRoute løser det:**

- Forenlig endpoint-strategi for klienter og agenter
- Bygget-in protokolledelse UI'er og røgfyldningsveje
- Produktionsklare grundlag (sikkerhed, logging, tilgængelighed, backup)

</details>

### Eksempler på Playbooks (Integreede brugscaser)

**Playbook A: Maximerer betalt abonnement + billig backup**

```txt
Combo: "maximere-claude"
  1. cc/claude-opus-4-6
  2. glm/glm-4.7
  3. if/kimi-k2-tank
  (Oversættelse af "thinking" var forkert - konsolideret med den sandsynlige tekst)

Månedlig omkostning: $20 + lille backup udgift
Udbytte: Højere kvalitet, næsten ingen afbrydelser
```

**Playbook B: Nålnegativ programmerings-pæl**

```txt
Combo: "gratis-altid"
  1. gc/gemini-3-flash
  2. if/kimi-k2-tank
  3. qw/qwen3-coder-plus

Månedlig omkostning: $0
Udbytte: Stabil gratis programmerings flow
```

**Playbook C: 24/7 altid-til-bords-fall-selv-fangst kæde**

```txt
Combo: "altid-til-bords"
  1. cc/claude-opus-4-6
  2. cx/gpt-5.2-codex
  3. glm/glm-4.7
  4. minimax/MiniMax-M2.1
  5. if/kimi-k2-tank

Udbytte: Dybbel afgrænsning af afgrænsning af grænsen af deadline-kritiske belastninger
```

**Playbook D: Agent-kontroller med MCP + A2A**

```txt
1) Start MCP-transport (`omniroute --mcp`) for tool-driven operations
2) Kør A2A-opgaver via `besked/send` og `besked/stream`
3) Overvåg via /dashboard/endpoint (MCP- og A2A-skærme)
4) Vippe services via inline-status-kontroller
```

---

## 🆓 Start gratis — Nul-konfiguration-omkostning

> Opsæt AI-programmering på få minutter på **$0/død**. Forbind disse
> gratis-kontoer og brug den indbyggede **gratis-pæl**-combo.

| Trin | Handling                                                    | Tilgængelige Leverandører                                         |
| ---- | ----------------------------------------------------------- | ----------------------------------------------------------------- |
| 1    | HDMI til **Kiro** (AWS Builder ID OAuth)                    | Claude Sonnet 4.5, Haiku 4.5 — **uendeligt**                      |
| 2    | HDMI til **iFlow** (Google OAuth)                           | kimi-k2-tænking, qwen3-coder-plus, deepseek-r1... — **uendeligt** |
| 3    | HDMI til **Qwen** (Device Code)                             | qwen3-coder-plus, qwen3-coder-flash... — **uendeligt**            |
| 4    | HDMI til **Gemini CLI** (Google OAuth)                      | gemini-3-flash, gemini-2.5-pro — **180K/mo gratis**               |
| 5    | `/dashboard/ kombinationer` → ** Gratistak ( $0)** skabelon | Automatisk rundgående mod alle gratis leverandører                |

**Hurtigvis en hvilken som helst IDE/ CLI på:** `http://localhost:20128/v1` ·
API-nøgle: `hvilken som helst streng` · Færdigt.

> **Oplyst ekstra dækning (og gratis):** Groq API-nøgle (30 RPM gratis), NVIDIA
> NIM (40 RPM gratis, 70+ modeller), Cerebras (1M tok/dag), LongCat API-nøgle
> (50M tokens/dag!), Cloudflare Workers AI (10K neuroner/dag, 50+ modeller).

## Hurtig start

### 1. Installer og kør

```bash
npm install -g omniroute
omniroute
```

> **pnpm users:** Ændre `pnpm approve-builds -g` efter installation til at
> aktivere nativ build-scripts, der er nødvendige for `better-sqlite3` og
> `@swc/core`:
> 
> ```bash
> pnpm install -g omniroute
> pnpm approve-builds -g   # Vedhæng alle pakkehierarkier → godkend
> omniroute
> ```

Dashboard åbnes på `http://localhost:20128` og API-basis-URL er
`http://localhost:20128/v1`.

| Kommando                | Beskrivelse                                                     |
| ----------------------- | --------------------------------------------------------------- |
| `omniroute`             | Start server (med `PORT=20128`, API og dashboard på samme port) |
| `omniroute --port 3000` | Sæt kanoniske/API-port til 3000                                 |
| `omniroute --mcp`       | Start MCP-server (stdio-transport)                              |
| `omniroute --no-open`   | Opret browser ikke automatisk                                   |
| `omniroute --help`      | Vis hjælp                                                       |

Tilvalgvis split-port-modus:

```bash
PORT=20128 DASHBOARD_PORT=20129 omniroute
# API:       http://localhost:20128/v1
# Dashboard: http://localhost:20129
```

### 2) Forbind providers og oprett din API-nøgle

1. Åbn Dashboard → `Providers` og forbind mindst én provider (OAuth eller
   API-nøgle).
2. Åbn Dashboard → `Endpoints` og oprett en API-nøgle.
3. (Vælgst) Åbn Dashboard → `Combos` og angiv din faldgruppe.

### 3) Tilføj din koding værktøj til OmniRoute

```txt
Base URL: http://localhost:20128/v1
API-nøgle:  [kopier fra Endpoints-side]
Model:    if/kimi-k2-thinking (eller hvilken som helst provider/model prefix)
```

Funktioner sammen med Claude Code, Codex CLI, Gemini CLI, Cursor, Cline,
OpenClaw, OpenCode, og OpenAI-kompatible SDK'er.

### 4) Aktivér og valider protokoller (v2.0)

**MCP (til værktøj-styret operationer):**

```bash
omniroute --mcp
```

Derefter tilslut din MCP-client over `stdio` og test værktøjer som:

- `omniroute_get_health`
- `omniroute_list_combos`

**A2A (til agent-til-agent-workflows):**

```bash
curl http://localhost:20128/.well-known/agent.json
```

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"quickstart","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"Give me a short quota summary."}]}}'
```

### 5) Valider alt i en ende-til-ende (anbefalet)

```bash
npm run test:protocols:e2e
```

Dette suite validerer ægte MCP og A2A client-strømmer mod en kørende app.

### Alternativ: kørs fra kilde

```bash
cp .env.example .env
npm install
PORT=20128 DASHBOARD_PORT=20129 NEXT_PUBLIC_BASE_URL=http://localhost:20129 npm run dev
```

---

## 🐳 Docker

OmniRoute er tilgængelig som offentligt Docker-billede på [Docker
Hub](https://hub.docker.com/r/diegosouzapw/omniroute).

** hurtig start:**

```bash
docker run -d \
  --name omniroute \
  --restart unless-stopped \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:latest
```

**Med omgivelsesfil:**

```bash
# Kopier og rediger .env først
cp .env.example .env

docker run -d \
  --name omniroute \
  --restart unless-stopped \
  --env-file .env \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:latest
```

**Brug af Docker Compose:**

```bash
# Basis-profil (ingen kommando linje-tilgængelighed)
docker compose --profile base up -d

# CLI-profil (Claude Code, Codex, OpenClaw bygget ind)
docker compose --profile cli up -d
```

| Billede                  | Tegn      | Størrelse | Beskrivelse               |
| ------------------------ | --------- | --------- | ------------------------- |
| `diegosouzapw/omniroute` | `seneste` | ~250MB    | Seneste stabile udgivelse |
| `diegosouzapw/omniroute` | `1.0.3`   | ~250MB    | Aktuel version            |

---

## 🖥️ Desktop App — Offline & Always-On

> 🆕 **NYT!** OmniRoute er nu tilgængelig som en **nativ desktopapplikation** på
> Windows, macOS og Linux.

Kør OmniRoute som en selvstændig desktop-applikation — intet terminal, intet
browser, intet internet kræves for lokale modeller. Den Electron-baserede app
omfatter:

- 🖥️ **Nativt vindue** — Tilpasset applikationssprog med
  systemskufferintegration
- 🔄 **Auto-Start** — Start Omnidirection på system-login
- 🔔 **Nativer tilkald/X24X] — Få varsel for kvotafornydelser eller
  leverandørproblem
- ⚡ **Enkeltklikke-installering** — NSIS (Windows), DMG (macOS), AppImage
  (Linux)
- 🌐 **Afholdningsmodus** — Funktionerer helt afholden af bundlet server

### Hurtig start

```bash
# Udvikling tilstand
npm run electron:dev

# Byg til din platform
npm run electron:byg        # Nuværende platform
npm run electron:byg:win     # Windows (.exe)
npm run electron:byg:mac     # macOS (.dmg) — x64 &amp; arm64
npm run electron:byg:linux   # Linux (.AppImage)
```

### Systemskuffer

Når man minimerer OmniRoute, bor den i din systemskuffer med hurtige handlinger:

- Åbn Dashboard
- Skift serverport
- Quit application

📖 Fuldstændig dokumentation: [`electron/README.md`](electron/README.md)

---

## 💰 Priser på et kast

| Niveau              | Udbyder                    | Kost                          | Quotafornydelse           | Bedst for                          |
| ------------------- | -------------------------- | ----------------------------- | ------------------------- | ---------------------------------- |
| **💳 ABONNEMENT**    | Claude Kode (Pro)          | $20/mo                        | 5h + ugentlig             | Allerede abonnéret                 |
|                     | Codex (Plus/Pro)           | $20-200/mo                    | 5h + ugentlig             | Brukere af OpenAI                  |
|                     | Gemini CLI                 | **TIL FRI**                   | 180K/mo + 1K/dag          | Hver gang!                         |
|                     | GitHub Copilot             | $10-19/mo                     | Månedlig                  | GitHub-brugere                     |
| **🔑 API NÅGRESKEL** | NVIDIA NIM                 | **TIL FRI** (dev forever)     | Ca. 40 RPM                | Lige 70 åbne modeller              |
|                     | Cerebras                   | **gratis** (1M token/dag)     | 60.000 TPM / 30 RPM       | Verdens hurtigste                  |
|                     | Groq                       | **gratis** (30 RPM)           | 14.400 RPD                | Ultra-fremmed Llama/Gemma          |
|                     | DeepSeek V3.2              | 0,27$/1,10 pr. 1M             | Ingen                     | Bedst pris/kvalitetsrationel       |
|                     | xAI Grok-4 Hurtig          | **$0,20/$0,50 pr. 1M** 🆕      | Ingen                     | Hurtigst + værktøjskald, ultralavt |
|                     | xAI Grok-4 (standard)      | $0,20/$1,50 pr. 1M 🆕          | Ingen                     | Reasoning-flagchip fra xAI         |
|                     | Mistral                    | Fristrium + betaling          | Sats begrænset            | Europæisk AI                       |
|                     | OpenRouter                 | Tidsbaseret betaling          | Ingen                     | 100+ modelkombinationer            |
| ** 💰 CHEAP**        | GLM-5 (via Z.AI) 🆕         | 0,50 $/1 mio.                 | Kl. 10 Daily              | 128 KB output, nye flagship        |
|                     | GLM-4.7                    | 0,60 $/1 mio.                 | Kl. 10 Daily              | BUDGETsikkerhed                    |
|                     | MiniMax M2.5 🆕             | 0,30 $/1 mio. indlæg          | 5-timers rullende         | Forskning + agensitæftlige opgaver |
|                     | MiniMax M2.1               | 0,20 $/1M                     | 5-timers rullende         | Cheapest mulighed                  |
|                     | Kimi K2.5 (Moonshot API) 🆕 | Tidsbaseret betaling          | Ingen                     | Direkte adgang til Moonshot API    |
|                     | Kimi K2                    | 9,00 $/måned slet             | 10M brugertoken/måned     | Forudsigelig omkostning            |
| **🆓 GRATIS**        | iFlow                      | **$0**                        | Ubegrænset                | 5 modeller uden begrænsninger      |
|                     | Qwen                       | **$0**                        | Ubegrænset                | 4 modeller uden begrænsninger      |
|                     | Kiro                       | **$0**                        | Ubegrænset                | Claude Sonnet/Haiku (AWS Builder)  |
|                     | LangCat Flash-Lite 🆕       | **$0** (50M tok/day 🔥)        | 1 forespørgsel pr. sekund | Verdens største gratis quota       |
|                     | Bemaling AI 🆕              | **$0** (ingenting nødvendigt) | 1 anmodning/15s           | GPT-5, Claude, DeepSeek, Llama 4   |
|                     | Cloudflare Workers AI 🆕    | **$0** (10K neuroner/dag)     | ~150 svar/dag             | 50+ modeller, global edge          |
|                     | Scaleway AI 🆕              | **$0** (1M tokens som helhed) | Sats begrænset            | EU/GDPR, Qwen3 235B, Llama 70B     |

> 🆕 **Nye modeller tilføjet (marts 2026):** Grok-4 Fast-familie til
> $0,20/$0,50/M (testet til 1143ms — 30% hurtigere end Gemini 2,5 Flash), GLM-5
> via Z.AI med 128K output, MiniMax M2,5 reasoning, DeepSeek V3,2 opdateret
> prissættning, Kimi K2,5 via Moonshot direkte API.

**💡 $0 Combo Stak — Den Fuldstændige Gratis Opstilling:**

```
# 🆓 Sidste Free Stak 2026 — 11 Leverandører, $0 Forever
Kiro (kr/)             → Claude Sonnet/Haiku UBEGRENSET
iFlow (if/)            → kimi-k2-hæfte, qwen3-kodermester-plus, deepseek-r1 UBEGRENSET
LongCat Lite (lc/)     → LongCat-Flash-Lite — 50M tokens/dag 🔥
Pollinations (pol/)    → GPT-5, Claude, DeepSeek, Llama 4 — ingen adgangskode nødvendig
Qwen (qw/)             → qwen3-kodermester-plus, qwen3-kodermester-flash, qwen3-kodermester-igen UBEGRENSET
Gemini (gemini/)       → Gemini 2,5 Flash — 1.500 anmodninger/dag gratis API-nyckel
Cloudflare AI (cf/)    → Llama 70B, Gemma 3, Mistral — 10K neuroner/dag
Scaleway (scw/)        → Qwen3 235B, Llama 70B — 1M gratis tokens (EU)
Groq (groq/)           → Llama/Gemma ultra hurtig — 14,4K anmodninger/dag
NVIDIA NIM (nvidia/)   → 70+ åbne modeller — 40 RPM hele tiden
Cerebras (cerebras/)   → Llama/Qwen verdens hurtigste — 1M tok/dag
```

**Nulomre. Aldrig stopper med at koden.** Konfigurér dette som en enkelt
OmniRoute combo og alle fald tilbage sker automatisk — ingen manuel overgang
nødvendig.

---

---

## 🆓 Frie Modeller — Det Du Rent faktisk Får

> Alle modeller nedenfor er **100% gratis uden nogen kreditkort nødvendigt**.
> OmniRoute auto-rotor mellem dem, når en quota udløber — kombinér dem alle til
> en ubrudelig $0 combo.

### 🔵 CLAUDE MODELLER (via Kiro — AWS-bygge-id)

| Model               | Præfiks | Begrænsning  | Satsgrænse                       |
| ------------------- | ------- | ------------ | -------------------------------- |
| `claude-sonnet-4.5` | `kr/`   | **Uendelig** | Ingen rapporterede daglige begær |
| `claude-haiku-4.5`  | `kr/`   | **Uendelig** | Ingen rapporterede daglige begær |
| `claude-opus-4.6`   | `kr/`   | **Uendelig** | Seneste opus via Kiro            |

### 🟢 IFLØB MODELER (Frit OAuth — Ingen Kreditkort)

| Model              | Præfiks | Begrænsning  | Satsgrænse             |
| ------------------ | ------- | ------------ | ---------------------- |
| `kimi-k2-thinking` | `if/`   | **Uendelig** | Ingen rapporterede kap |
| `qwen3-coder-plus` | `if/`   | **Uendelig** | Ingen rapporterede kap |
| `dybdeg-søg-r1`    | `if/`   | **Uendelig** | Ingen rapporterede kap |
| `minimax-m2.1`     | `if/`   | **Uendelig** | Ingen rapporterede kap |
| `kimi-k2`          | `if/`   | **Uendelig** | Ingen rapporterede kap |

### 🟡 QWEN MODULER (Udstyrskode Auth)

| Model               | Præfiks | Begrænsning  | Satsgrænse                   |
| ------------------- | ------- | ------------ | ---------------------------- |
| `qwen3-coder-plus`  | `qw/`   | **Uendelig** | Ingen rapporterede kap       |
| `qwen3-coder-flash` | `qw/`   | **Uendelig** | Ingen rapporterede kap       |
| `qwen3-coder-næste` | `qw/`   | **Uendelig** | Ingen rapporterede kap       |
| `vision-model`      | `qw/`   | **Uendelig** | Kombinationsmodus (billeder) |

### 🟣 GEMINI CLI (Google OAuth)

| Model                          | Præfiks | Begrænsning                     | Satsgrænse            |
| ------------------------------ | ------- | ------------------------------- | --------------------- |
| `Gemini-3-Flash-Visualisering` | `gc/`   | **180 K/token/måned** + 1 K/dag | Månedlig genopbygning |
| `Gemini-2,5-pro`               | `gc/`   | 180 K/token/måned (delt pool)   | Høj kvalitet          |

### ⚫ NVIDIA NIM (Gratis API-nyckel — build.nvidia.com)

| Niveau       | Daglig grænse           | Satsgrænse  | Noter                                                           |
| ------------ | ----------------------- | ----------- | --------------------------------------------------------------- |
| Gratis (Dev) | Ingen token-begrænsning | **~40 RPM** | 70+ modeller; overgang til renhedstalsbegrænsninger midt i 2025 |

Populær gratis modeller: `moonshotai/kimi-k2.5` (Kimi K2.5), `z-ai/glm4.7` (GLM
4.7), `deepseek-ai/deepseek-v3.2` (DeepSeek V3.2),
`nvidia/llama-3.3-70b-instruct`, `deepseek/deepseek-r1`

### ⚪ CEREBRAS (Gratis API-nyckel — inference.cerebras.ai)

| Niveau | Daglig grænse     | Satsgrænse          | Noter                                            |
| ------ | ----------------- | ------------------- | ------------------------------------------------ |
| Gratis | **1M tokens/dag** | 60.000 TPM / 30 RPM | Verdens hurtigste LLM-inferens; resettes dagligt |

Tilgængelig gratis: `llama-3.3-70b`, `llama-3.1-8b`,
`deepseek-r1-distill-llama-70b`

### 🔴 GROQ (Gratis API-nyckel — console.groq.com)

| Niveau | Daglig grænse | Satsgrænse       | Noter                                            |
| ------ | ------------- | ---------------- | ------------------------------------------------ |
| Gratis | **14.4K RPD** | 30 RPD pr. model | Ingen kreditkort; 429 på grænse, ikke faktureret |

Tilgængelig gratis: `llama-3.3-70b-versatile`, `gemma2-9b-it`, `mixtral-8x7b`,
`whisper-large-v3`

### 🔴 LONGCAT AI (Gratis API-nyckel — longcat.chat) 🆕

| Model                            | Præfiks | Daglig fri kvote | Noter                         |
| -------------------------------- | ------- | ---------------- | ----------------------------- |
| `LangtKatte-Flash-Lite`          | `lc/`   | **50M tokens** 💥 | Højeste frie kvote nogensinde |
| `LangtKatte-Flash-Chat`          | `lc/`   | 500K tokens      | Multi-værdschat               |
| `LangtKatte-Flash-Tenkning`      | `lc/`   | 500K tokens      | Betrækningsfacilitet / CoT    |
| `LangtKatte-Flash-Tenkning-2601` | `lc/`   | 500K tokens      | Januar 2026 version           |
| `LangtKatte-Flash-Omni-2603`     | `lc/`   | 500K tokens      | Multimedie                    |

> 100% fri mens man er inden for offentlig beta-version. Tilmeld dig på
> [longcat.chat](https://longcat.chat) med e-mail eller telefon. Resettes
> dagligt kl. 00:00 UTC.

### 🟢 POLLINATIONS AI (Ingen API-nøgle påkrævet) 🆕

| Model      | Præfiks | Satsgrænse      | Leverandør Baggrund |
| ---------- | ------- | --------------- | ------------------- |
| `openai`   | `pol/`  | 1 anmodning/15s | GPT-5               |
| `claude`   | `pol/`  | 1 anmodning/15s | Anthropic Claude    |
| `gemini`   | `pol/`  | 1 anmodning/15s | Google Gemini       |
| `deepseek` | `pol/`  | 1 anmodning/15s | DeepSeek V3         |
| `llama`    | `pol/`  | 1 anmodning/15s | Meta Llama 4 Scout  |
| `mistral`  | `pol/`  | 1 anmodning/15s | Mistral AI          |

> ✨ **Ingen friction:** Ingen tilmelding, ingen API-nøgle. Tilføj
> Pollinations-leverandøren med et tomt nøglefelt, og det fungerer
> øjeblikkeligt.

### 🟠 CLOUDFLARE WORKERS AI (Gratis API-nøgle — cloudflare.com) 🆕

| Niveau | Daglige Neuroner | Lignende Brug                                    | Noter                  |
| ------ | ---------------- | ------------------------------------------------ | ---------------------- |
| Gratis | [10,000]**       | ~150 LLM tilbud / 500s lyd / 15.000 indsættelser | Global edge, 50+ model |

Populære free modeller: `@cf/meta/llama-3.3-70b-instruct`,
`@cf/google/gemma-3-12b-it`, `@cf/openai/whisper-large-v3-turbo` (Free lyd!),
`@cf/qwen/qwen2.5-coder-15b-instruct`

> Kræver API Token + Konto ID fra
> [Dash.cloudflare.com](https://dash.cloudflare.com). Gem Konto ID i
> leverandørinstillingen.

### 🟣 SCALEWAY AI (1M frie token – scaleway.com) ⚙

| Niveau | Frie Quota    | Lokation     | Noter                                   |
| ------ | ------------- | ------------ | --------------------------------------- |
| Gratis | [1M tokens]** | 🇫🇷 Paris, EU | Ingen kreditkort til frie begrænsninger |

Tilgængelige gratis: `qwen3-235b-a22b-instruct-2507` (Qwen3 235B!),
`llama-3.1-70b-instruct`, `mistral-small-3.2-24b-instruct-2506`,
`deepseek-v3-0324`

> EU/GDPR-overensstemmende. Få API-key på
> [Console.scaleway.com](https://console.scaleway.com).

> ** 💡 Den ultimative frie stack (11 levere, 0 kr. for evigt):**
> 
> ```
> Kiro (kr/)             → Claude Sonnet/Haiku UENDELIG
> iFlow (if/)            → kimi-k2-tank, qwen3-koder-plus, deepseek-r1 UENDELIG
> LongCat Lite (lc/)     → LongCat-Flash-Lite — 50M tokens/dag 🔥
> Pollinations (pol/)    → GPT-5, Claude, DeepSeek, Llama 4 — ingen nøgle nødvendig
> Qwen (qw/)             → qwen3-koder-modeller UENDELIG
> Gemini (gemini/)       → Gemini 2.5 Flash — 1.500 req/dag gratis
> Cloudflare AI (cf/)    → 50+ modeller — 10K Neuroner/dag
> Scaleway (scw/)        → Qwen3 235B, Llama 70B — 1M gratis tokens (EU)
> Groq (groq/)           → Llama/Gemma — 14.4K req/dag ultra-rask
> NVIDIA NIM (nvidia/)   → 70+ åbenne modeller — 40 RPM evigt
> Cerebras (cerebras/)   → Llama/Qwen verdens hurtigste — 1M tok/dag
> ```

## 🎙️ Gratis Transkriberingskombination

> Transskribér hvad som helst til **$0** — Deepgram leder med $200 gratis,
> AssemblyAI $50 fallback, Groq Whisper som uendeligt nødnummer.

| Udbyder          | Gratis kredit                | Bedste Model                              | Satsgrænse                             |
| ---------------- | ---------------------------- | ----------------------------------------- | -------------------------------------- |
| 🟢 **Deepgram**   | **$200 gratis** (tilmelding) | `nova-3` — bedste nøjagtighed, 30+ sprog  | Ingen RPM-begrænsning på gratis kredit |
| 🔵 **AssemblyAI** | **$50 gratis** (tilmelding)  | `universal-3-pro` — kapitler, mening, PII | Ingen RPM-begrænsning på gratis kredit |
| 🔴 **Groq**       | **Gratis for evigt**         | `whisper-large-v3` — OpenAI Whisper       | 30 RPM (takstrøm begrænset)            |

**Anbefalet kombination i `/dashboard/combos`:**

```
Navn: free-transcription
Strategi: Prioritet
Noder:
  [1] deepgram/nova-3          → bruger $200 gratis først
  [2] assemblyai/universal-3-pro → fallback når Deepgram-kreditter løber tør
  [3] groq/whisper-large-v3    → gratis for evigt, nødnummer
```

Så her er den oversatte tekst:\
\
Sådan åbner du transkriptionstabellen i `/dashboard/media` → **Transcription**:
Upload din audio eller video fil → vælg din combo-endpunkt → få transskription i
understøttede formater.

## 💡 Vigtigste funktioner

OmniRoute v2.0 er bygget som et operationsplatform, ikke bare som et relay
proxy.

### 🆕 Nyhed — ClawRouter-enspirerede forbedringer (mar. 2026)

| Funktion                          | Hva det gør                                                                                      |
| --------------------------------- | ------------------------------------------------------------------------------------------------ |
| ⚡ **Grok-4 Fast Family**          | xAI-modeller til $0,20/$0,50/M — benchmarked 1143ms (30% hurtigere end Gemini 2,5 Flash)         |
| 🧠 **GLM-5 via Z.AI**              | 128K outputkontekst, $0,5/1M — nyt flageskib fra GLM-familien                                    |
| 🔮 **MiniMax M2,5**                | Ræsonnement + agenteopgaver til $0,30/1M — væsentlig opgradering fra M2,1                        |
| 🎯 **toolCalling Flåde per Model** | Per-model `toolCalling: sand/sand ` i registry — AutoCombo ignorerer ikke-tool- kapable modeller |
| 🌍 **Multilingv Intentsensitet**   | PT/ZH/ES/AR-ord i AutoCombo-scoring — bedre modelvalg til ikke-engelsk indhold                   |
| 📊 **Benchmark-rettet Fallbacks**  | San p95-latence fra levende anmodninger til combo-scoring — AutoCombo lærer fra egentlig data    |
| 🔁 **Anmodning Duplications**      | Content-hashes på duplication-vindue — multi-agentsikre, forhindrer duplikeret besvær            |
| 🔌 **RouterStrategy**              | Ekstendet `RouterStrategy`-grænseflade — tilføj personlige routinger på samme måde som plugins   |

### 🚀 Førige v2.0.9+ — Playground, CLI Fingerprints & ACP

| Funktion                                  | Hva det gør                                                                                                                                                                                                                                                                   |
| ----------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🎮 **Model Playground**                    | Dashboard siden for at teste hvilket som helst model direkte — tilbyder providers/model/endpointvalg, Monaco-Editor, streaming, stop, tid                                                                                                                                     |
| 🔏 **CLI Fingerprint-Matching**            | Per-provider hoved- og body-ordination til at matche native CLI-signaturer — sluk det per-lejer i Indstillinger > Sikkerhed. **Dit proxy IP bliver bibeholdt**                                                                                                                |
| 🤝 **ACP-støtte (Agent-Client-Protokohl)** | CLI-agent opdagelse (Codex, Claude, Goose, Gemini CLI, OpenClaw + 9 flere), process-spawner, `/api/acp/agen`endpoint                                                                                                                                                          |
| 🤖 **ACP-Agendas Dashboard**               | Debbuger› Agenter siden — grid af 14 agenter med opdateringsstatus, version, individuel agent-form til hvilken som helst CLI-verktøy. **OpenCode**brugere får en "Downloade opencode.json"-knap, der genererer en klar til brug konfiguration med alle tilgængelige modeller. |
| 🔧 **Custom Model `apiFormat`-Routing**    | Efterkommende modeller med `apiFormat: "responses"` rutes korrekt med Responds API-oversætter                                                                                                                                                                                 |
| 🏢 **Codex-værksted Isolation**            | Flere Codex-værksteder per email — OAuth-isolerer forbindelser efter arbejdssted-id                                                                                                                                                                                           |
| 🔄 **Electron Auto-Update**                | Dessktop-app tjekker efter opdateringer + automatisk installer på genopstart                                                                                                                                                                                                  |

### 🤖 Agent- & Protokol Operationer (v2.0)

| Funktion                               | Hva det gør                                                                                                     |
| -------------------------------------- | --------------------------------------------------------------------------------------------------------------- |
| 🔧 **Server til MCP (16 værktøjer)**    | IDE/agent værktøjer ved hjælp af 3 transports: stdio, SSE (`/api/mcp/sse`), Streamable HTTP (`/api/mcp/stream`) |
| 🤝 **A2A Server (JSON-RPC + SSE)**      | Agent til agent-opgaver med synkron og strømme-flods eksekution                                                 |
| 🧭 **Opsamlingspunkt for end-pointe**   | Fordelingsmenu med EndPoint Proxy, MCP, A2A og API EndPoint tabs                                                |
| 🎚️ **Taster for servicetilslutning/X** | ON/OFF sluk til MCP og A2A med indstillinger, der følges (standard: OFF)                                        |
| 🛰️ **MCP Runtime Heartbeat**           | Egentlig process status (pid, uptime, heartbeat alder, transport, scope mode)                                   |
| 📋 **MCP Audit Trail**                  | Filterbare audit-log med success/fiasco og nøgletilskrivning                                                    |
| 🔐 **MCP Scope Enforcement**            | 9 nøgle scope tilladelser for styret værktøj adgang                                                             |
| 📡 **A2A Task Lifecycle Management**    | Liste/gennemsyg overgange, inspektér begivenheder/artefakter, afbryd kørende opgaver                            |
| 📋 **MCP-Agent korts opdagelse**        | `/.well-known/agent.json` for klient selvmulig opdagelse                                                        |
| 🧪 **Protokoll E2E Test Harness**       | Echtzeit MCP SDK + A2A client-strømme i `test:protokoll:e2e`                                                    |
| ⚙️ **Operative Kontrols**              | Skift kombinatør, tilpasse redundansprofiler, nulstil samkvæmpe fra én kontrollpanel                            |

### 🧠 Routing & Intelligent

| Funktion                                  | Hva det gør                                                                               |
| ----------------------------------------- | ----------------------------------------------------------------------------------------- |
| 🎯 **Smart 4-Tier Fald tilbage**           | Auto-ruter: Abonnement → API Key → Billige → Begrænsninger                                |
| 📊 **Nuværende Kvotetracking i Real Time** | Levende token-tæl + nulstil tidsregning per leverandør                                    |
| 🔄 **Formatoversættelse**                  | OpenAI → Claude → Gemini → Svaret med schema-sikre omvendelser                            |
| 👥 **Flere Konti støtte**                  | Flere konti pr. leverandør med intelligent udvælgelse                                     |
| 🔄 **Automatisk Opdater Token**            | OAuth-tokens opsættes automatisk med genskring                                            |
| 🎨 **Personlige Kombinationer**            | 6 vægtstreg-strategier + fald tilbagekæde kontrol                                         |
| 🌐 **Vildkaret Router**                    | `leverandør/*` dynamisk routing                                                           |
| 💭 **Tænkende Budsjett Kontroller**        | Gennemstrømning, auto, anpasning og adaptiv begrænsning af resonans-limte                 |
| 🔀 **Model Aliasser**                      | Integreret + Personlig model aliasing og migreringets sikkerhed                           |
| ⚡ **Baggrund Nedtoning**                  | Rute lav-prioritets baggrund opgaver til billigere modeller                               |
| 🧪 **Opjagsvarende Smart Routing**         | Auto-valgte model af efter indsats type (kode/visning/analyse/summering)                  |
| 💬 **Systemets Stimulering af System**     | Globale adfærdskontroller afgrænset konsekvent                                            |
| 📄 **Svar API Kompatibilitet**             | Holdt fuld `/v1/responses` understøttelse for Codex og avancerede agente-arbejdsprocesser |

### 🎵 Flertydende APIs

| Funktion                    | Hva det gør                                                                                                                                                                   |
| --------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🖼️ **Billede Generering**   | `/v1/images/generations` med skyen og lokal baggrunds komponenter                                                                                                             |
| 📐 **Indlejring **           | `/v1/embeddings` for søgning og RAG pipelines                                                                                                                                 |
| 🎤 **Audiobeskrivelse**      | `/v1/lydfil-transkription` — 7 udbydere (Deepgram Nova 3, AssemblyAI, Groq Whisper, HuggingFace, ElevenLabs, OpenAI, Azure), automatisk sprogfyldning, støtte for MP4/MP3/WAV |
| 🔊 **Tekst-til-Tale**        | `/v1/lydfils-tale` — 10 udbydere (ElevenLabs, OpenAI, Deepgram, Cartesia, PlayHT, HuggingFace, Nvidia NIM, Inworld, Coqui, Tortoise) med korrekte fejlbeskeder                |
| 🎬 **Videoplukning**         | `/v1/video-tilskuere` (ComfyUI + SD WebUI flows)                                                                                                                              |
| 🎵 **Musikplukning**         | `/v1/musik-tilskuere` (ComfyUI flows)                                                                                                                                         |
| 🛡️ **Sikkerhedskontroller** | `/v1/sikkerhedskontroller`                                                                                                                                                    |
| 🔀 **Oprører relevans**      | `/v1/oprydningsrelevans`                                                                                                                                                      |
| 🔍 **Web-søgning** 🆕         | `/v1/søgning` — 5 udbydere (Serper, Brave, Perplexity, Exa, Tavily), 6.500+ gratis pr. måned, automatisk failover, cache                                                      |

### 🛡️ Selvheling, Sikkerhed & Regering

| Funktion                                      | Hva det gør                                                                            |
| --------------------------------------------- | -------------------------------------------------------------------------------------- |
| 🔌 **Circuit Breaker**                         | Per-model_trip/recover med trin-threshold kontrol                                      |
| 🎯 **Modeller, der vedligeholder slutpunkter** | Custom models declare supported endpoints + API format                                 |
| 🛡️ **Anti-Thundering Herd**                   | Mutex + semaphore protections on retry/rate events                                     |
| 🧠 **Semantic + Signature Cache**              | Cost/latency reduction with two cache layers                                           |
| ⚡ **Request Idempotency**                     | Duplicate protection window                                                            |
| 🔒 **TLS Fingerprint Spoofing**                | Browser-like TLS fingerprint — **reduces bot detection and account flagging**          |
| 🔏 **CLI Fingerprint-Matching**                | Matches native CLI request signatures — **reduces ban risk while preserving proxy IP** |
| 🌐 **IP Filtering**                            | Allowlist/blocklist control for exposed deployments                                    |
| 📊 **Editable Rate Limits**                    | Configurable global/provider-level limits with persistence                             |
| 🔑 **API Key Management + Scoping**            | Secure key issuance/rotation and model/provider controls                               |
| 🛡️ **Protected `/models`**                    | Optional auth gating and provider hiding for model catalog                             |

### 📊 Observability & Analytics

| Funktion                           | Hva det gør                                                       |
| ---------------------------------- | ----------------------------------------------------------------- |
| 📝 **Forspørgsel + Proxy Loggning** | Full forespørgsel/svar og proxy loggning                          |
| 📋 **Forenede Logs Dashboard**      | Forespørgsel, proxy, revisions- og konsoleudsyn i ét vindue       |
| 🔍 **Forspørgsel Telemetri**        | p50/p95/p99 latens og forespørgselssporing                        |
| 🏥 ** sundhedsdashboard**           | Opstart, breaker-stater, låsninger, cache-statiske                |
| 💰 **Kostfolging**                  | Budget kontrol og visning af model-kostpriser                     |
| 📈 **Analyser med Visualiseringer** | Modellen/leverandørens brugervisdom og trendudsyn                 |
| 🧪 **evaluation framework**         | Guldensemble præfiksning med konfigurerbare tilpasningsstrategier |

### ☁️ Deployment & Platform

| Funktion                                  | Hva det gør                                                                            |
| ----------------------------------------- | -------------------------------------------------------------------------------------- |
| 🌐 **Udgiv Overalt**                       | Lokalserver, VPS, Docker, Cloud-miljøer                                                |
| 💾 **Cloud Synchronisering**               | Konfigurations synchronization via cloud-arbejder                                      |
| 🔄 **Backup/Indlæs**                       | Eksport/import og katastropherede genopretningssystemer                                |
| 🧙 **Indledningsguide**                    | Første gang vejledt opstart                                                            |
| 🔧 **CLI-værktøjsbordet**                  | En-klik-opsætning af populære kodningstørr                                             |
| 🎮 **Model Playground**                    | Test af hvilken leverandør/model/endpoint som endnu fra skærmen                        |
| 🔏 **CLI-petiturfingerprint omstillinger** | Gælder i forbindelse med leverandør-fingerprints matchning i Indstillinger > Sikkerhed |
| 🌐 **Internationalisering (30 sprog)**     | Fullstændig dashboard + dokumentation sprogstøtte med RTL-dækning                      |
| 🧹 **Ryd alle modeller**                   | En-klik model liste rydning i leverandør detaljes                                      |
| 📋 **Issue-billede mallen**                | Standardiserede GitHub-mellemlag for fejl og funktioner                                |
| 📂 **Brugernes egne data-fil**             | `Opbevaringssted` kan overraskes                                                       |

### Funktsionsdybde

#### Smart fallback med praksisrettelse af omkostninger

```txt
Kombination: "min-kodingspil"
  1. cc/claude-opus-4-6
  2. nvidia/llama-3.3-70b
  3. glm/glm-4.7
  4. if/kimi-k2-thinking
```

Når kvote, rate eller helbred failer, flytter OmniRoute automatisk til den næste
kandidat uden manuel overgång.

#### Protokolstyring der er synlig og operabel

- MCP + A2A er opdagelige i UI og dokumentation (ikke skjulte)
- Protokollstatus-API'er afslører live operativ data (`/api/mcp/*`,
  `/api/a2a/*`)
- Dashboards indeholder handlinger til dag-2 ops (kombinationssvarigheder,
  breaker-til-randtager, opgave-afbræk)

#### Oversætter + valideringsworkflow

Oversættelsesområdet inkluderer:

- **Lærelejren**: anmod om transformationsoverføringer
- **Chat tester**: fuld anmodning/antwort rundrejse
- **Testbænk**: flere tilfælde på en gang
- **Live monitor**: næsten real-time trafikvisning

Plus protokolvalidering med virkelige client via `npm run test:protokoll:e2e`.

> 📖 **[MCP server-dokumentation](open-sse/mcp-server/README.md)** —
> Virkestilsreference, IDE-konfigurationer og klientskabeloner
> 
> 📖 **[A2A server-dokumentation](src/lib/a2a/README.md)** — Færdigheder,
> JSON-RPC-metoder, streaming og opgavelivscyklus

## 🧪 Evals (Evals)

OmniRoute indeholder en bygget i et integration af evaluation framework, der
tester LLM-svarets kvalitet i forhold til en guldensæt. Tilgå det via **Analyser
→ Evals** i dashboard'en.

### Indbygget Guldset

"OmniRoute Golden Set" -indbygget indeholder testfald for:

- Hilsener, matematik, geografi, kodegenerator
- JSON-format overholdelse, oversættelse, markdown-udvikling
- Sikkerhedsigngång (skadeligt indhold), tal, boolean logik

### Evalueringsstrategier

| Strategi         | Beskrivelse                                         | Eksempel                                     |
| ---------------- | --------------------------------------------------- | -------------------------------------------- |
| `eksemmer`       | Udput skal stemme overens præcis                    | `"4"`                                        |
| `indeholder`     | Udput skal indeholde undersættet (case-insensitive) | `"Paris"`                                    |
| `regulær udtryk` | Udput skal matche regulær udtryksmønster            | `"1.*2.*3"`                                  |
| `personlig`      | Personlig JS-funktion returnerer true/false         | `(udgivelse) =&gt; udgivelse.length &gt; 10` |

---

## 💻 Opsætningsvejledning

### Protokolsætning (MCP + A2A)

<details>
<summary><b>🧩 MCP Setup (Model Context Protocol)</b></summary>

Start MCP transport i stdio-modus:

```bash
omniroute --mcp
```

Anbefalet valideringsflow:

1. Tilslut din MCP-klient over stdio.
2. Kør `omniroute_get_health`.
3. Kør `omniroute_list_combos`.
4. Åbn `/dashboard/mcp` for at bekræfte pulsen, aktivitet og kontrol.

Brugbare APIs for automatisering:

- `GET /api/mcp/status`
- `GET /api/mcp/tools`
- `GET /api/mcp/audit`
- `GET /api/mcp/audit/stats`

</details>

<details>
<summary><b>🤝 A2A Setup (Agent2Agent)</b></summary>

Opdager agenten:

```bash
curl http://localhost:20128/.well-known/agent.json
```

Send en opgave:

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'indhold-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"opsæt-a2a","method":"message/send","params":{"færdighed":"kvotamangement","meddelelser":[{"rol":"bruger","indhold":"Sammenfatt kvotestatus."}]}}'
```

Hantering af livscyklus:

- `GET /api/a2a/status`
- `GET /api/a2a/opgaver`
- `GET /api/a2a/opgaver/:id`
- `POST /api/a2a/opgaver/:id/afbryd`

Operativ UI:

- `/dashboard/a2a` til opgave/tilstand/streem-observabilitet og røgvisktioner

</details>

<details>
<summary><b>🧪 End-to-end protocol validation</b></summary>

Justér både protokoller med virkelige klienter:

```bash
npm run test:protocols:e2e
```

Dette bekræfter:

- MCP SDK klient forbind/ liste/kald
- A2A opdagelse/send/streem/afbryd
- Overflade-kontrol af data i MCP-audit og A2A-opgave-tilsyn-apis

</details>

<details>
<summary><b>💳 Subscription Providers</b></summary>

### Claude Code (Pro/Max)

```bash
Oversigtsdæk == Leverandører == Forbind Claude Code
→  Oath-login→→&gt;&gt; Automatisk authtoken genopretnning
→  Følgende begrænsninger tilgængelig

Modeler:
  cc/claude-opus-4-6
  cc/claude-sonnet-4-5-20250929
  cc/claude-haiku-4-5-20251001
```

**Pro Tip:** Bru g Opu for komplekse opgaver, Sonnet for hast

### Omni Route følger begrænsning per model!\

```bash
Oversigtsdæk == Leverandører == Forbind Codex
→  Oath-login (port 1455)
→  Følgende begrænsning – afbrydning hver 5 timer

Modeler:
  cx/gpt-5.2-codex
  cx/gpt-5.1-codex-max
```

#### Codex Accounbegrænsning management (5h + Året)

Hvert Codex-konto har nu policy-ændringer i `Oversigtsdæk -&gt; Leverandører`:

- `5h` (T/O): anvend 5 timer vindue-spærrende policy.
- `Weekly` (ON/OFF): enforce the weekly window threshold policy.
- Threshold behavior: when an enabled window reaches >=90% usage, that account
  is skipped.
- Rotation behavior: OmniRoute routes to the next eligible Codex account
  automatically.
- Reset behavior: when the provider `resetAt` time passes, the account becomes
  eligible again automatically.

Scenarios:

- `5h ON` + `Weekly ON`: account is skipped when either window reaches
  threshold.
- `5h OFF` + `Weekly ON`: only weekly usage can block the account.
- `5h ON` + `Weekly OFF`: only 5-hour usage can block the account.
- `resetAt` passed: account re-enters rotation automatically (no manual
  re-enable).

### Gemini CLI (FREE 180K/month!)

```bash
Dashboard → Providers → Connect Gemini CLI
→ Google OAuth
→ 180K completions/month + 1K/day

Models:
  gc/gemini-3-flash-preview
  gc/gemini-2.5-pro
```

**Best Value:** Huge free tier! Use this before paid tiers.

### GitHub Copilot

```bash
Dashboard → Providers → Connect GitHub
→ OAuth via GitHub
→ Monthly reset (1st of month)

Models:
  gh/gpt-5
  gh/claude-4.5-sonnet
  gh/gemini-3-pro
```

</details>

<details>
<summary><b>🔑 API Key Providers</b></summary>

### NVIDIA NIM (FREE developer access — 70+ models)

1. Sign up: [build.nvidia.com](https://build.nvidia.com)
2. Get free API key (1000 inference credits included)
3. Dashboard → Add Provider → NVIDIA NIM:
   - API Key: `nvapi-your-key`

**Models:** `nvidia/llama-3.3-70b-instruct`, `nvidia/mistral-7b-instruct`, and
50+ more

**Pro Tipp:** OpenAI-kompatibel API — fungerer skønt sammen med OmniRutes
formatoversættelse!

### DeepSeek

1. Tilmeld dig: [platform.deepseek.com](https://platform.deepseek.com)
2. Få API-nøgle
3. Oversigt → Tilføj Lejer → DeepSeek

**Modelle:** `deepseek/deepseek-chat`, `deepseek/deepseek-coder`

### Groq (Fri Tier Tilgængelig!)

1. Tilmeld dig: [console.groq.com](https://console.groq.com)
2. Få API-nøgle (fri tier medfølger)
3. Oversigt → Tilføj Lejer → Groq

**Modelle:** `groq/llama-3.3-70b`, `groq/mixtral-8x7b`

**Pro Tipp:** Ekstrem hurtig inference - bedst til realtid coding!

### OpenRouter (100+ Model)

1. Tilmeld dig: [openrouter.ai](https://openrouter.ai)
2. Få API-nøgle
3. Oversigt → Tilføj Lejer → OpenRouter

**Modelle:** Adgang til 100+ model fra alle større lejere gennem en enkelt
API-nøgle.

</details>

<details>
<summary><b>💰 Cheap Providers (Backup)</b></summary>

### GLM-4.7 (Dagligt rest, 0,6$/1M)

1. Tilmeld dig: [Zhipu AI](https://open.bigmodel.cn/)
2. Få API-nøgle fra Coding Plan
3. Oversigt → Tilføj API-nøgle:
   - Leverandør: `glm`
   - API-Nøgle: `din-nøgle`

**Brug:** `glm/glm-4.7`

**Pro Tip:** Coding Plan tilbyder 3 gange mere kvote i 1/7 af prisen! Nulstilles
dagligt kl. 10:00.

### MiniMax M2.1 (5-timers reset, $0,20/1M)

1. Tilmeld: [MiniMax](https://www.minimax.io/)
2. Få API-nøgle
3. Oversigt → Tilføj API-Nøgle

**Brug:** `minimax/MiniMax-M2.1`

**Pro Tip:** Den billigste løsning for lange kontekster (1M tokens)!

### Kimi K2 ($9/måneds fast pris)

1. Abonnér: [Moonshot AI](https://platform.moonshot.ai/)
2. Få API-nøgle
3. Oversigt → Tilføj API-Nøgle

**Brug:** `kimi/kimi-latest`

**Pro Tip:** Fast $9/månedspris for 10M tokens = $0,90/1M effektiv tilbud!

</details>

<details>
<summary><b>🆓 FREE Providers (Emergency Backup)</b></summary>

### iFlow (5 FREEMODELER via OAuth)

```bash
Oversigt → Forbind iFlow
→ iFlow OAuth-login
→ Uendeligt brug
Mods:
  if/kimi-k2-thinking
  if/qwen3-coder-plus
  if/glm-4.7
  if/minimax-m2
  if/deepseek-r1
```

### Qwen (4 FREEMODELER via Enhedscode)

```bash
Dashboard → Tilkoble Qwen
→ Enhedsnummer-autorisering
→ Uendelig brug

Modeller:
  qw/qwen3-coder-plus
  qw/qwen3-coder-flash
```

### Kiro (CLAUDIE GRATIS)

```bash
Dashboard → Tilkoble Kiro
→ AWS-Byggested ID eller Google/GitHub
→ Uendelig brug

Modeller:
  kr/claude-sonnet-4.5
  kr/claude-haiku-4.5
```

</details>

<details>
<summary><b>🎨 Create Combos</b></summary>

### Eksempel 1: Maximere Abonnement → Billig Backup

```
Dashboard → Kombiner → Opret Ny

Navn: premium-koding
Modeller:
  1. cc/claude-opus-4-6 (Abonnements primær)
  2. glm/glm-4.7 (Billig backup, 0,6 $/1M)
  3. minimax/MiniMax-M2.1 (Cheapest fallback, 0,20 $/1M)

Brug i CLI: premium-koding
```

### Eksempel 2: Free-Only (Ingen Omkostninger)

```
Navn: fri-kombination
Modeller:
  1. gc/gemini-3-flash-forudsigelser (180K fri/måned)
  2. if/kimi-k2-tænking (uendelig)
  3. qw/qwen3-coder-plus (uendelig)

Kostnad: $0 for evigt!
```

</details>

<details>
<summary><b>🔧 CLI Integration</b></summary>

### Markør IDE

```
Indstillinger → Modeller → Avanceret:
  Åben AI API-base URL: http://localhost:20128/v1
  Åben AI API-nøgle: [fra OmniRoute-dashboard]
  Model: cc/claude-opus-4-6
```

### Claude kode

Brug den **CLI Toolbox**-side i dashboardet for enkeltklikkonfiguration eller
rediger `~/.claude/instillinger.json` manuelt.

### Codex CLI

```bash
eksport OPENAI_BASE_URL="http://localhost:20128"
eksport OPENAI_API_KEY="din-omniroute-api-nøgle"

codex "din prompt"
```

### OpenClaw

**Valg 1 — Dashboard (anbefalet):**

```
Dashboard → CLI Toolbox → OpenClaw → Vælg Model → Nulæg
```

**Valg 2 — Manuel:** Rediger `~/.openclaw/openclaw.json`:

```json
{
  "modeller": {
    "leverandører": {
      "omniroute": {
        "baseUrl": "http://127.0.0.1:20128/v1",
        "apiKey": "sk_omniroute",
        "api": "openai-completions"
      }
    }
  }
}
```

> **Observation:** OpenClaw fungerer kun med lokal OmniRoute. Brug `127.0.0.1` i
> stedet af `localhost` for at undgå IPv6-resolusionsproblemer.

### Linje / Fortsæt / RooCode

```
IndStillinger → API-Konfiguration:
  Leverandør: OpenAI Compatible
  Basis URL: http://localhost:20128/v1
  API-Nøgle: [fra OmniRoute dashboard]
  Model: if/kimi-k2-thinking
```

### OpenCode

**Trin 1:** Tilføj OmniRoute som en brugerdefineret leverandør:

```bash
opencode
/connect
# Vælg "Anden" → Angiv ID: "omniroute" → Angiv din OmniRoute API-nøgle
```

**Trin 2:** Opdater `opencode.json` i din projektrot:

```json
{
  "$schema": "https://opencode.ai/config.json",
  "leverandør": {
    "omniroute": {
      "npm": "@ai-sdk/openai-compatible",
      "navn": "OmniRoute",
      "indstillinger": {
        "baseURL": "http://localhost:20128/v1"
      },
      "modeller": {
        "cc/claude-sonnet-4-20250514": { "navn": "Claude Sonnet 4" },
        "gg/gemini-2.5-pro": { "navn": "Gemini 2.5 Pro" },
        "if/kimi-k2-thinking": { "navn": "Kimi K2 (Free)" }
      }
    }
  }
}
```

**Trin 3:** Vælg modellen i OpenCode:

```bash
/models
# Vælg hvilken som helst OmniRoute-model fra listen
```

> **Tip:** Tilføj hvilken som helst model, der er tilgængelig på din OmniRoute
> `/v1/models` slutpunkt, til `modeller`-sektionen. Brug formatet
> `leverandør/model-id` fra din OmniRoute dashboard.

</details>

---

## Fejlfinding

<details>
<summary><b>Click to expand troubleshooting guide</b></summary>

**"Sprogmodelen leverede ingen beskeder"**

- Provider-quota udsedd → Kontroller dashboard-quota-sporet
- Løsning: Brug combo-fald eller skift til billigere tarp

**Hastighedskontroles**

- Abonnement-quota udsedd → Fald til GLM/MiniMax
- Tilføj combo: `cc/claude-opus-4-6 → glm/glm-4.7 → if/kimi-k2-thinking`

**OAuth-token udløbet**

- Automatisk genopdateret af OmniRoute
- Hvis problem fortsætter: Dashboard → Leverandør → Genopliver forbindelsen

**Høje omkostninger**

- Tjek brugere i Dashboard → Udgifter
- Sæt primær model til GLM/MiniMax
- Brug free tier (Gemini CLI, iFlow) til ikke-kritiske opgaver

**Dashboard/API-porterne er forkerte**

- `PORT` er den kanoniske base-port (og API-port af grund)
- `API_PORT` erstatter kun OpenAI-kompatibelt API-lytter
- `DASHBOARD_PORT` erstatter kun dashboard/Next.js-lytter
- Indstil `NEXT_PUBLIC_BASE_URL` til dit dashboard/public URL (for OAuth-oprogn)

**Cloud synkroniseringsfejl**

- Verificer, at `BASE_URL` peker til din kørte instance
- Verificer, at `CLOUD_URL` peker til dit forventede cloud-endpunkt
- Hold `NEXT_PUBLIC_*`-værdier i tråd med server-side værdier

**Første login ikke fungerer**

- Tjek `INITIAL_PASSWORD` i `.env`
- Hvis ikke sat, fald tilbage til adgangskode `123456`

**Ingen anmodningslog**

- Indstil `ENABLE_REQUEST_LOGS=true` i `.env`

**Afdrægsprøve viser "Ugyldig" for OpenAI-kompatible leverandører**

- Mange leverandører afslører ikke et `/models`-endpunkt
- OmniRoute v1.0.6+ inkluderer faldgruppe forvaltning via chat-fullendelser
- Ikke indsæt URL til en omni-route server, der inkluderer [/25/] til versjon
  [/29/]

### 🔐 Oauth til fjern server

<a name="oauth-on-a-remote-server"></a> <a name="oauth-em-servidor-remoto"></a>

> **⚠️ Vigtigt for brugere, der kører OmniRoute på en VPS, Docker eller en fjern
> server**

#### Hvorfor mislykkes Antigravity / Gemini CLI Oauth på fjern servere?

Omniroutes levereafgivere, **Antigravity** og **Gemini CLI**, bruger **Google
Oauth 2.0**. Google kræver, at `redirect_uri` i OAuth fluen nøjagtigt matcher en
af de registrerede URI'er i appens Google Cloud Console.

Oauth-tilgængeligheder, der er inkluderet i OmniRoute, er registrerede ** kun
til `localhost` **. Når du adgående omniRoute på en fjern server (f.eks.
`https://omniroute.myserver.com`), afviser Google godkendelsen med:

```
Fejl 400: redirect_uri_mismatch
```

#### Løsning: Konfigurér dine egne Oauth-tilgængeligheder

Du skal oprette et **Oauth 2.0 klientidentifikator** i Google Cloud Console med
din servers-URI.

#### Trin for trin

**1. åbn Google Cloud Console**

Gå til:
[https://console.cloud.google.com/apis/credentials](https://console.cloud.google.com/apis/credentials)

**2. Opret en ny Oauth 2.0 klientidentifikator**

- Klik på **"+ Opret Kreditorer"** → **"Oauth klientidentifikator"**
- Til applications type: **"WebApplication"**
- Navn: hvad som helst (f.eks. `Ominroute Fjern`)

**3. Tilføj autoriserede Redirect URI'er**

I **"autoriserede Redirect URI'er"** feltet, tilføj:

```
https://din-server.com/callback
```

> Erstat `din-server.com` med din servers domæne eller IP (inkluder porten hvis
> nødvendigt, f.eks. `http://45.33.32.156:20128/callback`).

**4. Gem på og kopier kredenssier**

Efter oprettelse vil Google vise **KlientID** og **Klient hemmelig**.

**5. Sæt miljøvariabler**

I din `.env` (eller Docker-miljøvariabler):

```bash
# Til Antigravity:
ANTIGRAVITY_OAUTH_KLIENTID=your-client-id.apps.googleusercontent.com
ANTIGRAVITY_OAUTH_KLIENTHEMMELIG=GOCSPX-your-secret

# Til Gemini CLI:
GEMINI_OAUTH_KLIENTID=your-client-id.apps.googleusercontent.com
GEMINI_OAUTH_KLIENTHEMMELIG=GOCSPX-your-secret
GEMINI_CLI_OAUTH_KLIENTHEMMELIG=GOCSPX-your-secret
```

**6. Genstart Omnimarker**

```bash
# npm:
npm run dev

# Docker:
docker genstart omniroute
```

**7. Få forbindelse igen**

Dashboard → Yderforser → Antigravity (eller Gemini CLI) → OAuth

Google vil nu rette korrekt til `https://din-server.com/callback`.

---

#### Midlertidig arbejdsomgang (uden eget klentekredenssier)

Hvis du ikke vil sætte op dine egne kredenssier lige nu, kan du stadig bruge
**manuelt URL-fløget**:

1. Omnimarker åbner Google-authorization URL'en
2. Efter autorisering prøver Google at rette til `localhost` (hvori det fejler
   på fjernserveren)
3. **Kopier alt URL'en** fra din browser-adresselinje (selv hvis siden ikke
   indlæser)
4. Indsæt URL'en i feltet vist i Omnimarkets forbindelsesmodal
5. Klik på **"Forbind"**

> Det Virker arbejdsomgang, fordi autorizations-koden i URL'en er gyldig, uanset
> om retur-indlæsningssiden indlæser eller ej.

---

<details>
<summary><b>🇧🇷 Versão em Português</b></summary>

#### Hvorfor opgraver OAuth hos Antigravity / Gemini CLI på fjernsergere?

Yderforserne **Antigravity** og **Gemini CLI** bruger **Google OAuth 2.0** for
autentifikation. Google kræver, at `redirect_uri` brugt i OAuth-fløget er
**exakt** en af de registrerede URIs i Google Cloud Console til dit applikation.

As credenciais OAuth innervuam i OmniRoute er sted tilmeldt **kun på
'localhost'**. Når du tilgår OmniRoute på en fjern server (fx
`https://omniroute.meuservidor.com`), accepterer Google ikke certificering med:

```
Fejl 400: redirect_uri_mismatch
```

#### Løsning: Indstil dine egne OAuth 1 credenciales

Du skal oprette en **OAuth-2-0 Client ID** i Google Cloud Console med din
servers URI

#### Trin-for-trin

**1. Besøg Google Cloud Console**

Åbn:
[https://console.cloud.google.com/apis/credentials](https://console.cloud.google.com/apis/credentials)

**2. Opret ny OAuth 2.0 Client ID**

- Klik på **+ Create Credentials"** → **"OAuth client ID"**
- Tilbagekaldetype: **"Web application"**
- Navn: Vælg hvilket som helst (fx `OmniRoute Remote`)

**3. Tilføj de auktoriserede TilbagekaldURIs**

I feltet **"Authorized redirect URIs"** tilføj:

```
https://seu-servidor.com/callback
```

> Erstat `seu-servidor.com` med din servers domein eller IP-adresse (inkludering
> af porten, hvis nødvendig, fx `http://45.33.32.156:20128/callback`).

**4. Gem og kopier kredensialerne**

Efter oprettelse viser Google Client ID ' og Client Secret '.

**5. Konfigurér variablen for omgivelserne**

I din `.env` (eller variablerne for omgivelser i Docker):

```bash
# For Antigravity:
ANTIGRAVITY_OAUTH_CLIENT_ID=seu-client-id.apps.googleusercontent.com
ANTIGRAVITY_OAUTH_CLIENT_SECRET=GOCSPX-seu-secret

# For Gemini CLI:
GEMINI_OAUTH_CLIENT_ID=seu-client-id.apps.googleusercontent.com
GEMINI_OAUTH_CLIENT_SECRET=GOCSPX-seu-secret
GEMINI_CLI_OAUTH_CLIENT_SECRET=GOCSPX-seu-secret
```

**6. Start Omnipathen igen**

```bash
# Hvordan bruge npm:
npm run dev

# Hvordan bruge Docker:
docker restart omniroute
```

**7. Føj again til**

Dashboard → Leverandører → Antigravity (eller Gemini CLI) → OAuth

Nu vil Google rette direkte til `https://din-server.com/callback` og
authentication skal fungeren.

---

#### Midlertidig workarund (uden at konfigurere egne kredsløb)

Hvis du ikke ønsker at oprette egne kredsløb nu, kan du stadig bruge URL-flux
**manual handlende URL**:

1. Omniruten skal åbne URL'et for autorisation fra Google
2. Efter du har autoriseret det, skal Google prøve at rette på `localhost` (som
   falder på fjernserveren)
3. ** Kopier URL'en fuldstændigt** fra adressebaren på din browser
4. Indsæt denne URL i feltet på modal connection i Omniruten
5. Klik på **"Connect"**

> Dette middel virker, fordi autorisationskoden i URL'et er gyldig uafhængigt
> af, om redirecten blev lastet eller ej.

</details>

---

</details>

## 🛠️ Tech Stack

<details>
<summary><b>Click to expand tech stack details</b></summary>

- ** Runtime**: Node.js 18-22 LTS (⚠️ Node.js 24+ understøttes ikke** —
  `bedre-sqlite3` native binaries er ikke kompatible)
- ** Sprog**: TypeScript 5.9 — **100% TypeScript** overalt `src/` og `åbne-sse/`
  (ingen `any` i kernemoduler siden v2.0)
- ** Ramme**: Next.js 16 + React 19 + Tailwind CSS 4
- ** Databasen**: LowDB (JSON) + SQLite (domænestatistik + proxy logs + MCP
  audit + routing afgørelser)
- ** Schemas**: Zod (MCP værktøj I/O validering, API kontrakter)
- ** Protokoller**: MCP (stdio/HTTP) + A2A v0.3 (JSON-RPC 2.0 + SSE)
- ** Strømning**: Server-Sent Events (SSE)
- ** Authentificering**: OAuth 2.0 (PKCE) + JWT + API Keys + MCP-scoperet
  Tilladelse
- ** Testering**: Node.js test runner + Vitest (900+ tests herunder enhed,
  integrations, E2E)
- ** CI/CD**: GitHub Actions (auto npm publicere + Docker Hub på release)
- **Hjemmeside**: [omniroute.online](https://omniroute.online)
- ** Pakke**:
  [npmjs.com/package/omniroute](https://www.npmjs.com/package/omniroute)
- ** Docker**:
  [hub.docker.com/r/diegosouzapw/omniroute](https://hub.docker.com/r/diegosouzapw/omniroute)
- ** Resilience**: Krebsom bryder, eksponeret tilbagekobling, anti-kuld,
  TLS-spænding, selv-helbredende kombi

</details>

---

## Dokumentation

| Dokumentere                                     | Beskrivelse                                                  |
| ----------------------------------------------- | ------------------------------------------------------------ |
| [Brugervejledning](docs/USER_GUIDE.md)          | Partnere, kombiner, CLI-integration, deployment              |
| [API Reference](docs/API_REFERENCE.md)          | Alle endpunkter med eksempler                                |
| [MCP Server](open-sse/mcp-server/README.md)     | 16 MCP-værktøjer, IDE-konfigurationer, Python/TS/Go-klienter |
| [A2A Server](src/lib/a2a/README.md)             | JSON-RPC 2.0-proto, færdigheder, streaming, opgave styring   |
| [Kombi-Selv-healing Engine](docs/auto-combo.md) | 6-faktors system, mode pakker selv-hjælpende                 |
| [Troubleshooting](docs/TROUBLESHOOTING.md)      | Felles problemer og løsninger                                |
| [Architecture](docs/ARCHITECTURE.md)            | Systemarkitektur og indre dynamik                            |
| [Contributing](CONTRIBUTING.md)                 | Udviklingssettings og retningslinjer                         |
| [OpenAPI Spec](docs/openapi.yaml)               | OpenAPI 3.0 specification                                    |
| [Security Policy](SECURITY.md)                  | Sårbarhedsrapportering og sikkerhedspraktitker               |
| [VM Deployment](docs/VM_DEPLOYMENT_GUIDE.md)    | Komplet guide: VM + nginx + Cloudflare setup                 |
| [Features Gallery](docs/FEATURES.md)            | Visuel dashboard tur med screenshots                         |
| [Release Checklist](docs/RELEASE_CHECKLIST.md)  | Fremgangsmåde før udgivelse                                  |

---

## 🗺️ Vejledning

OmniRoute har **210+ funktioner planlagt** over flere udviklingsfasener. her er
de vigtige områder:

| Kategori                     | Planlagte Funktioner | Højdepunkter                                                                                     |
| ---------------------------- | -------------------- | ------------------------------------------------------------------------------------------------ |
| 🧠 **Routing & Intellect**    | 25+                  | Lavest-latence-routing, tag-baseret routing, quota præflying, P2C-kontovalg                      |
| 🔒 **Sikkerhed & Compliance** | 20+                  | SSRF-hårdning, legitimationsnogenklost, rate-per endpoint, ledelsessnogenklosting                |
| 📊 **Observabilitet**         | 15+                  | OpenTelemetry-integration, real-time kwota monitorering, omkostningsfølgelig afprøvning af model |
| 🔄 **Provider Integrations**  | 20+                  | Dynamisk modelregister, providerkølighed, multiconto Codex, Copilot-kwotalæsning                 |
| ⚡ **Hastighed**              | 15+                  | Dobbel forlagslage, prompt-forlagslage, svar-forlagslage, streaming-keep-alive, batch API        |
| 🌐 **Miljø**                  | 10+                  | WebSocket-API, config-hot-reload, fordelingskonfigurationsopslag, kommersielt mode               |

### 🔜 Kommer snart

- 🔗 **OpenCode Integration** — Nativt forhandlerstøtte til AI-kodnings-IDE'et
  OpenCode
- 🔗 **TRAE Integration** — Full support for det TRAE AI developpeings framework
- 📦 **Batch API** — Asynkron batch processing for bulk forespørgsler
- 🎯 **Tag-Based Routing** — Rute forespørgsler på baggrund af personlige mærker
  og metadata
- 💰 **Lavest-Kost Strategi** — Automatisk vælg den billigste tilgængelige
  leverandør

> 📝 Full funktionsspecifikationer tilgængelige på
> [`docs/new-features/`](docs/new-features/) (217 detaljerede specifikationer)

---

## 👥 Bidragydere

[![Bidragydere](https://contrib.rocks/image?repo=diegosouzapw/OmniRoute&max=100&columns=20&anon=1)](https://github.com/diegosouzapw/OmniRoute/graphs/contributors)

### Hvordan Bidrage

1. Fork opslaget til vores repository
2. Opret din funktionel gren (`git checkout -b feature/amazing-feature`)
3. Lag din ændring (`git commit -m 'Add amazing feature'`)
4. Push til grenen (`git push origin feature/amazing-feature`)
5. Åben en Pull Request

Se [CONTRIBUTING.md](CONTRIBUTING.md) for detaljerede anvisninger.

### Udsende et Nyt Version

```bash
# Opret en udsendelse — npm publish sker automatisk
gh release create v2.0.0 --title "v2.0.0" --generate-notes
```

---

## 📊 Stjernetilstand

## Stjerner over tid

## [![Stjerner over tid](https://starchart.cc/diegosouzapw/OmniRoute.svg?variant=adaptive)](https://starchart.cc/diegosouzapw/OmniRoute)

## 🙏 Tak til alle bidragydere

Tak til **[router](https://github.com/decolua/9router)** af
**[decolua](https://github.com/decolua)** — den oprindelige projekt, der
inspirerede dette fork. OmniRoute bygger på den fantastiske grundlag med
tilføjelige funktioner, multi-modale APIs og en fuldstændig
TypeScript-overarbejdningsversion.

Tak til **[CLIProxyAPI](https://github.com/router-for-me/CLIProxyAPI)** — den
oprindelige Go-implementering, der inspirerede dette JavaScript-port.

---

## 📄 Licens

MIT-licensen - se [LICENSE](LICENSE) for detaljer.

---

<div align="center">
  <sub>Built with ❤️ for developers who code 24/7</sub>
  <br/>
  <sub><a href="https://omniroute.online">omniroute.online</a></sub>
</div>
<!-- GitHub Discussions enabled for community Q&A -->
