# 🚀 OmniRoute — The Free AI Gateway

### Never stop coding. Smart routing to **FREE & low-cost AI models** with automatic fallback.

_Your universal API proxy — one endpoint, 67+ providers, zero downtime. Now with
**MCP & A2A** agent orchestration._

**Chat Completions • Embeddings • Image Generation • Video • Music • Audio •
Reranking • **Web Search** • MCP Server • A2A Protocol • 100% TypeScript**

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
[![License](https://img.shields.io/github/license/diegosouzapw/OmniRoute)](https://github.com/diegosouzapw/OmniRoute/blob/main/LICENSE)
[![Website](https://img.shields.io/badge/Website-omniroute.online-blue?logo=google-chrome&logoColor=white)](https://omniroute.online)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-Community-25D366?logo=whatsapp&logoColor=white)](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

[🌐 Website](https://omniroute.online) • [🚀 Quick Start](#-quick-start) • [💡
Features](#-key-features) • [📖 Docs](#-documentation) • [💰
Pricing](#-pricing-at-a-glance) • [💬
WhatsApp](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

</div>

🌐 **Available in:** 🇺🇸 [English](README.md) | 🇧🇷 [Português
(Brasil)](docs/i18n/pt-BR/README.md) | 🇪🇸 [Español](docs/i18n/es/README.md) | 🇫🇷
[Français](docs/i18n/fr/README.md) | 🇮🇹 [Italiano](docs/i18n/it/README.md) | 🇷🇺
[Русский](docs/i18n/ru/README.md) | 🇨🇳 [中文 (简体)](docs/i18n/zh-CN/README.md) | 🇩🇪
[Deutsch](docs/i18n/de/README.md) | 🇮🇳 [हिन्दी](docs/i18n/in/README.md) | 🇹🇭
[ไทย](docs/i18n/th/README.md) | 🇺🇦 [Українська](docs/i18n/uk-UA/README.md) | 🇸🇦
[العربية](docs/i18n/ar/README.md) | 🇯🇵 [日本語](docs/i18n/ja/README.md) | 🇻🇳 [Tiếng
Việt](docs/i18n/vi/README.md) | 🇧🇬 [Български](docs/i18n/bg/README.md) | 🇩🇰
[Dansk](docs/i18n/da/README.md) | 🇫🇮 [Suomi](docs/i18n/fi/README.md) | 🇮🇱
[עברית](docs/i18n/he/README.md) | 🇭🇺 [Magyar](docs/i18n/hu/README.md) | 🇮🇩
[Bahasa Indonesia](docs/i18n/id/README.md) | 🇰🇷 [한국어](docs/i18n/ko/README.md) |
🇲🇾 [Bahasa Melayu](docs/i18n/ms/README.md) | 🇳🇱
[Nederlands](docs/i18n/nl/README.md) | 🇳🇴 [Norsk](docs/i18n/no/README.md) | 🇵🇹
[Português (Portugal)](docs/i18n/pt/README.md) | 🇷🇴
[Română](docs/i18n/ro/README.md) | 🇵🇱 [Polski](docs/i18n/pl/README.md) | 🇸🇰
[Slovenčina](docs/i18n/sk/README.md) | 🇸🇪 [Svenska](docs/i18n/sv/README.md) | 🇵🇭
[Filipino](docs/i18n/phi/README.md) | 🇨🇿 [Čeština](docs/i18n/cs/README.md)

---

## 🆕 What's New in v3.0.0

> **Upgrading from v2.9.5?** — See the [full
> CHANGELOG](CHANGELOG.md#300--2026-03-22-release-candidate--not-yet-merged-to-main)
> for all changes.

| Area                               | Change                                                                                                                                                                    |
| ---------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🔒 **CodeQL Security**              | Fixed 10+ CodeQL alerts: polynomial-redos, insecure-randomness, shell-injection remediation                                                                               |
| ✅ **Route Validation**             | All 176 API routes now validated with Zod schemas + `validateBody()` — CI `check:route-validation:t06` passes                                                             |
| 🐛 **omniModel Tag Leak**           | Internal `<omniModel>` tags no longer leak to clients in SSE streaming responses (#585)                                                                                   |
| 🔑 **Registered Keys API**          | Auto-provision API keys via `POST /api/v1/registered-keys` with per-provider/account quota enforcement, idempotency, SHA-256 storage, and optional GitHub issue reporting |
| 🎨 **Provider Icons**               | 130+ leverandørlofter via `@lobehub/icons` (SVG) med PNG-fallbackkjederegle                                                                                               |
| 🔄 Automatiske model-opdateringer** | 24-timers scheduler og manuel UI-tnegling til å oppdatere modell-lister for bygdeinde og egne OpenAI-kompatiblene                                                         |
| 🌐 **OpenCode Zen/Go**              | To nye leverandere fra @kang-heewon via PR #530: gratis nivå + abonnementsnivå via `OpencodeExecutor`                                                                     |
| 🐛 **Gemini CLI OAuth**             | Feilbeskaffenhet når `GEMINI_OAUTH_CLIENT_SECRET` mangler i Docker (var kryptisk Google-fel)                                                                              |
| 🐛 **OpenCode config**              | `saveOpenCodeConfig()` skriver nå riktig TOML til `XDG_CONFIG_HOME`                                                                                                       |
| 🐛 **Pinned model override**        | `body.model` er nå korrekt satt til `pinnedModel` på kontekst-kassebeskyttelse                                                                                            |
| 🐛 **Codex/Claude loop**            | `tool_result` blokker nå konvertert til tekst til å stoppe uendelige løkker                                                                                               |
| 🐛 **Login redirect**               | Innlogging skal ikke lengre fryse etter å ha unngått innloggingsspørreml                                                                                                  |
| 🐛 **Windows vegninger**            | MSYS2/Git-Bash-pad ( `/c/...`) normalisert til `C:\...` automatisk                                                                                                        |

---

## 🖼️ Hovedskjerm

<div align="center">
  <img src="./docs/screenshots/MainOmniRoute.png" alt="OmniRoute Dashboard" width="800"/>
</div>

---

## 📸 Skjermbilde forhåndsvisning

<details>
<summary><b>Click to see dashboard screenshots</b></summary>

| Side               | Skjermbilde                                        |
| ------------------ | -------------------------------------------------- |
| **Tjenere**        | ![Tjenere](docs/screenshots/01-providers.png)      |
| **Kombinasjoner**  | ![Kombinasjoner](docs/screenshots/02-combos.png)   |
| **Analyser**       | ![Analyser](docs/screenshots/03-analytics.png)     |
| **Helse**          | ![Helse](docs/screenshots/04-health.png)           |
| ** Oversetter**    | ![Oversetter](docs/screenshots/05-translator.png)  |
| ** Innstillinger** | ![Innstillinger](docs/screenshots/06-settings.png) |
| ** KLI-verktøy**   | ![KLI-verktøy](docs/screenshots/07-cli-tools.png)  |
| ** Brukslogg**     | ![Brukslogg](docs/screenshots/08-usage.png)        |
| **Endepunkter**    | ![Endepunkter](docs/screenshots/09-endpoint.png)   |

</details>

---

### 🤖 Fria AI-leverandør for dine favoritt kode-agenter

_Samle inn noen av de store AI-prestasjonene eller CLI-verktøyene via OmniRoute
— den gratis API gateway til uendelig kodning._

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

<sub>📡 Alle agenter kobler seg via <code>http://localhost:20128/v1</code> eller
<code>http://cloud.omniroute.online/v1</code> — én konfigurasjon, uendelig
antall modeller og kvoter</sub>

---

## 🤔 Hvorfor OmniRoute?

**Stop med å kaste bort penger og være på grensen for kvoter:**

- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Abonneringskvoten tilbakerolar ubrukt hver måned
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Kvotering kan stoppe deg i middel av koding
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Dyr APIer ($20-50/provisør per måned)
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Manuelt skifting mellom prosjekter

**OmniRoute løser dette:**

- ✅ **Maksimere abonnementer** - Følg kvoter, bruk hver enkel bit før reset
- ✅ **Fall tilbake automatisk** - Abonnement → API nøkkel → Billig → Gratis,
  ingen nedetid
- ✅ **Flere kontoer** - Rundeball mellom konti per prosjektor
- ✅ **Universell** - Fungerer med Claude Code, Codex, Gemini CLI, Cursor, Cline,
  OpenClaw, noen hvilket CLI-verktøy

---

## 📧 Støtte

> 💬 **Slut deg til vårt fellesskap!**
> [WhatsApp-Gruppe](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)
> — Få hjelp, dele tips og holde deg oppdatert.

- **Hjemmeside**: [omniroute.online](https://omniroute.online)
- **GitHub**:
  [github.com/diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute)
- **Spørsmål om integrasjon**:
  [github.com/diegosouzapw/OmniRoute/issues](https://github.com/diegosouzapw/OmniRoute/issues)
- **WhatsApp**: [Sammenhengende
  fellesskap](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)
- **Bidra**: Se [CONTRIBUTING.md](CONTRIBUTING.md), åpne en PR eller finn en
  `god første oppgave`
- **Original Project**: [9router by decolua](https://github.com/decolua/9router)

### 🐛 Reporting a Bug?

When opening an issue, please run the system-info command and attach the
generated file:

```bash
npm run system-info
```

This generates a `system-info.txt` with your Node.js version, OmniRoute version,
OS details, installed CLI tools (iflow, gemini, claude, codex, antigravity,
droid, etc.), Docker/PM2 status, and system packages — everything we need to
reproduce your issue quickly. Attach the file directly to your GitHub issue.

---

## Hvordan det fungerer

```
┌─────────────┐
│  Your CLI   │  (Claude Code, Codex, Gemini CLI, OpenClaw, Cursor, Cline...)
│   Tool      │
└──────┬──────┘
       │ http://localhost:20128/v1
       ↓
┌─────────────────────────────────────────┐
│           OmniRoute (Smart Router)        │
│  • Format translation (OpenAI ↔ Claude) │
│  • Quota tracking + Embeddings + Images │
│  • Auto token refresh                   │
└──────┬──────────────────────────────────┘
       │
       ├─→ [Tier 1: SUBSCRIPTION] Claude Code, Codex, Gemini CLI
       │   ↓ quota exhausted
       ├─→ [Tier 2: API KEY] DeepSeek, Groq, xAI, Mistral, NVIDIA NIM, etc.
       │   ↓ budget limit
       ├─→ [Tier 3: CHEAP] GLM ($0.6/1M), MiniMax ($0.2/1M)
       │   ↓ budget limit
       └─→ [Tier 4: FREE] iFlow, Qwen, Kiro (unlimited)

Result: Never stop coding, minimal cost
```

---

## 🎯 What OmniRoute Solves — 30 Real Pain Points & Use Cases

> **Every developer using AI tools faces these problems daily.** OmniRoute was
> built to solve them all — from cost overruns to regional blocks, from broken
> OAuth flows to protocol operations and enterprise observability.

<details>
<summary><b>💸 1. "I pay for an expensive subscription but still get interrupted by limits"</b></summary>

Developers pay $20–200/month for Claude Pro, Codex Pro, or GitHub Copilot. Even
paying, quota has a ceiling — 5h of usage, weekly limits, or per-minute rate
limits. Mid-coding session, the provider stops responding and the developer
loses flow and productivity.

**How OmniRoute solves it:**

- **Smart 4-Tier Fallback** — If subscription quota runs out, automatically
  redirects to API Key → Cheap → Free with zero manual intervention
- **Real-Time Quota Tracking** — Shows token consumption in real-time with reset
  countdown (5h, daily, weekly)
- **Multi-Account Support** — Multiple accounts per provider with auto
  round-robin — when one runs out, switches to the next
- **Custom Combos** — Customizable fallback chains with 6 balancing strategies
  (fill-first, round-robin, P2C, random, least-used, cost-optimized)
- **Codex Business Quotas** — Business/Team workspace quota monitoring directly
  in the dashboard

</details>

<details>
<summary><b>🔌 2. "I need to use multiple providers but each has a different API"</b></summary>

OpenAI uses one format, Claude (Anthropic) uses another, Gemini yet another. If
a dev wants to test models from different providers or fallback between them,
they need to reconfigure SDKs, change endpoints, deal with incompatible formats.
Custom providers (FriendLI, NIM) have non-standard model endpoints.

**How OmniRoute solves it:**

- **Unified Endpoint** — A single `http://localhost:20128/v1` serves as proxy
  for all 67+ providers
- **Format Translation** — Automatic and transparent: OpenAI ↔ Claude ↔ Gemini ↔
  Responses API
- **Svarssanitizing** — Fjerner ikke-standard felt (`x_groq`,
  `brukeravhengig_opptreden`, `tjenestetilhørighet`) som får årsaker OpenAI SDK
  v1.83+
- **Rolle-normalisering** — Omsetter `utvikler` → `system` for
  ikke-OpenAI-levere; `system` → `bruker` for GLM/ERNIE
- **Tekk-tag utvinning** — Henter ut `` blokker fra modeller som DeepSeek R1
  samlet inn standardiserte `argumentasjonsinnhold`
- **Strukturert utkjøring for Gemini** — `JSON-skjema` →
  `responsType`/`responsSkjema` automatisk omregning
- **`stream` setter standard til `false`** — Samstemmer med
  OpenAI-specifikasjonen, og unngår påtrengende SSE i Python/Rust/Go SDK-er

</details>

<details>
<summary><b>🌐 3. "My AI provider blocks my region/country"</b></summary>

Levere som for eksempel OpenAI/Codex blokkerte tilgang fra visse geografiske
områder. Brukere får feilmeldinger som `ukjent land/region/territorium` under
OAuth og API-tilkoblinger. Dette er særlig frustrerende for utviklere fra u-land

**How OmniRoute solves it:**

- **3-Level Proxy Konfigurering** — Tilpasselig proxy på 3 nivå:
  verdensomspennende (alle trafikk), per-lever (en leverur kun), og
  per-tilkobling/token
- **Fargekodede Proxy Badges** — Visuelle indikatorer: 🟢 global proxy, 🟡
  leveransk proxy, 🔵 tilkobling proxy, viser alltid IP-adressen
- **OAuth-tokenbytte fører proxy** — OAuth-flow går også gjennom proxy, løser
  `ukjent land/region/territorium`
- **Tilkoblingstester via proxy** — Tilkoblingstester benytter den konfigurerte
  proxy (ingenting mer direkte omleidelse)
- **SOCKS5 støtte** — Full støtte for SOCKS5-proxy for utgående routing
- **TLS-fingeravtrykksprenge** — Bruker-liknende TLS-fingeravtrykk via `wreq-js`
  for å gå rundt bot-deteksjon
- **🔏 CLI-fingeravtrykksmatchning** — Sammenfutterer overskrifter og kropsfelt
  på måte å matche native CLI-binary-signaturs, og drastisk reduserer risiko for
  å bli flagget. Proxy-IP bleieres bevart — du får både stealth **og **
  IP-tillatelse samtidig

</details>

<details>
<summary><b>🆓 4. "I want to use AI for coding but I have no money"</b></summary>

Ikke alle kan beta en månedsgebyr på $20-200 for AI-abonnement. Studenter,
utviklere fra u-land, amatører og frilansere trenge tilgang til bedre modeller
uavgiftsfritt

**How OmniRoute solves it:**

- **Bygg Inn Nødvendige Free Tier levere** — Nativ støtte for 100% gratis
  levere: iFlow (5 ubegrensede modeller via OAuth: kimi-k2-thinking,
  qwen3-coder-plus, deepseek-r1, minimax-m2, kimi-k2), Qwen (4 ubegrensede
  modeller: qwen3-coder-plus, qwen3-coder-flash, qwen3-coder-next,
  visjonsmodell), Kiro (Claude + AWS Bygger ID for gratis), Gemini CLI (180K
  tokens/måned gratis)
- **Ollama Cloud** — Ollama-modeller som hostes i skyen på `api.ollama.com` med
  gratis "Light- bruke-til-tilgang"; bruk `ollamacloud/<model>`
  prefikser</model>
- **Kombinasjoner uten avgift** — Ligner `gc/gemini-3-flash →
  if/kimi-k2-thinking → qw/qwen3-coder-plus` = $0/måned med ubegrenset nedetid
- **NVIDIA NIM gratis tilgang** — ~40 RPM utvikler-tirolie-forever avgiftfri
  tilgang til 70+ modeller på build.nvidia.com (transistert fra kreditter til
  enkel rate-limter)
- Tilgangskostnadsstrategi** — Ruteforvaltning som automatisk velger den
  billigste tilgjengelige leverandør

</details>

<details>
<summary><b>🔒 5. "I need to protect my AI gateway from unauthorized access"</b></summary>

Når en AI-port eksponeres for nettverket (LAN, VPS, Docker), kan både hvem som
helst med adressekarakteristisert bruke utviklerens tokens/taksbeløp.
Utstyrsesskjulinger er sårbar for misbruk, prompt injeksjon og abus.

**How OmniRoute solves it:**

- **API-nykselholde** — Generering, rotasjon, og skalarbeiding per leverandør
  med en dedikert `/meldingsflaten/api-meneder` side
- **Modell-nivå tillatelser** — Begrensk API-nykes til spesielle modeller
  (`openai/*`, viltmønster), med Tillat alle/Restriktive knapp
- **API-slutpunktsskjulinger** — Krav om nyke for `/v1/modeller` og blokkere
  spesielle leverandører fra utbedringen
- **Autentiseringsskilt + CSRF beskyttelse** — Alle meldingsflate-ruter
  beskyttet med `med midttallet med midtre middelstørrelse` middelvaren og
  CSRF-tokener
- **Hastighetsgrannelser** — Enkelt-IP hastighets innstrammer med konfigurerbare
  vinduer
- **IP-filtrering** — Allerede/blockliste for tilgjengelighetskontroll
- **Prompt-injsiungsskjulinger** — Urent mot farlige prompt-mønster
- **AES-256-GMC kryptering** — Kredensjaler kryptert på hvilestand

</details>

<details>
<summary><b>🛑 6. "My provider went down and I lost my coding flow"</b></summary>

AI-leverandører kan bli ustabilitet, finne 5xx-feil eller treffer midlertidige
hastighetsgrannelser. Hvis utvikleren avhenger av en enkelt leverandør, er de
avbrutt. Uten sirkelskjalere, kan gjentatte forsøk i stedet krasere
applikasjonen

**How OmniRoute solves it:**

- **Circuit Breaker per-modell** — Autoåpne/slut med konfigurerbare gjeldende
  vektere og nedkjøringsindeks (Stengt/Åpnet/Halv-åpent), tilpasset per modell
  for å unngå kaskadende blokkeringer
- **Exponensiell avbønnelse** — Progressiv vedvarende avsonning
- **Motkraft mot sammenfallende herd** — Mutex + sperrebeskyttelse mot samstemte
  innstrammer
- **Kombinasjonsfall-backkjeder** — Hvis den primære leverandøren tapt, falle
  automatisk gjennom kjeden uten aktivitet
- **Kombinasjonscirkelskjalere** — Omhindre avvirkede leverandører innenfor en
  kombinasjonskjede
- **Tilstandsoversiktsdatabladet** — Tidligere overvåking, cirkelskjalere
  tilstand, avsonning, løpemønster, p50/p95/p99 latens

</details>

<details>
<summary><b>🔧 7. "Configuring each AI tool is tedious and repetitive"</b></summary>

Utviklere bruker Cursor, Claude-kode, Codex CLI, OpenClaw, Gemini CLI,
Kilo-kode... Hvert verktøy trenger en forskjellig konfigurasjon (API-slutpunkt,
nyke, modell). Gjenkonfigurasjon ved å bytte leverandører eller modeller er en
stor skamme

**How OmniRoute solves it:**

- **Kombo Utvikler Dashboard** — Dedikert side med ett-klikk konfigurering for
  Claude Code, Codex CLI, OpenClaw, Kilo Code, Antigravity, Cline
- **GitHub Copilot Config Generator** — Genererer `chatLanguageModels.json` for
  Visual Studio Code med bulkmodellvalg
- **Onboarding Wizard** — Ledet 4-trinn konfigurasjonsflyt for nybrukere
- **En endpoint, alle modeller** — Konfigurer `http://localhost:20128/v1` en
  gang, tilgang til 67+ tilbydere

</details>

<details>
<summary><b>🔑 8. "Managing OAuth tokens from multiple providers is hell"</b></summary>

Claude Code, Codex, Gemini CLI, Copilot — alle bruker Oauth 2.0 med utløpende
tokens. Utviklere må gjenautentiserer konstant, håndtere `client_secret
mangler`, `redirect_uri_mismatch`, og feil på fjerne servere. Oauth på LAN/VPS
er særlig problematk.

**How OmniRoute solves it:**

- **Auto Token Oppdatering** — Oauth tokens oppdateres i bakgrunnen før utløp
- **Oauth 2.0 (PKCE) Bygget Inn** — Automatisk fløyt for Claude Code, Codex,
  Gemini CLI, Copilot, Kiro, Qwen, iFlow
- **Multi-Account Oauth** — Flere konti per tilbyder via JWT/ID token utvinning
- **Oauth LAN/Fjern Fix** — Private IP-diskretion for `redirect_uri` + manuell
  URL-løsning for fjerne servere
- **Oauth Bakom Nginx** — Bruker `window.location.origin` for
  motvirkningskompatibilitet
- **Fjern Oauth-guide** — Trinn-for-trinn guide for Google Cloud-tilgang på
  VPS/Docker

</details>

<details>
<summary><b>📊 9. "I don't know how much I'm spending or where"</b></summary>

Utviklere bruker flere betalingsgivere, men har ingen sammenhengende syn på
utgifterne. Hver giver har sitt eget regneark, men det er ingen konsolideres
syn. Uventede utgifter kan bygge opp seg.

**How OmniRoute solves it:**

- **Kostanalyse Dashboard** — Per-token kostregistrering og budsjettstyring per
  giver
- **Budsjettbegrensninger per Trinn** — Utgiftsgrunnlag per trinn som trigget
  automatisk fallback
- **På modell-basert Pricning-konfigurasjon** — Konfigurerbare priser per modell
- **Bruksstatistikk Per API-ky[F30X] — Anropstall og siste-brukt tidspunkt per
  nyckel
- **Analyse Dashboard** — Stat-kort, modellbrukerstatistikk, leverandørtablå med
  suksesstrater og latentiet

</details>

<details>
<summary><b>🐛 10. "I can't diagnose errors and problems in AI calls"</b></summary>

Hvis en kall feiler, vet utvikler ikke hvilken feil som kan være skyld:
høysnittsgrenser, utgått token, forkert format, eller leverandør-feil.
Fragmenterte loggfiler på ulike terminaler. Med uten observabilitet er
feilsøking en trial og feil.

**How OmniRoute solves it:**

- **Fordoblet Logg-Dashboard** — 4 skjermer: Anrokkende Loggninger, Proxy
  Loggninger, Tilsyn Loggninger, Konsolloggninger
- **Konsolloggviser** — Real-time terminal-stilvisning med fargekoderte nivåer,
  automatisk nedscroll, søking, filtrering
- **SQLite-proxyloggninger** — Permanente loggfiler som overlever server-restart
- **Overfører-Leggstad** — 4 feilsøkningsmoder: Leggstad (formatoversetting),
  Prat-Skjema Sjekketester (rundtur), Testbuk (_batch_), Live Overvåking (i
  realtid)
- **Forskningsanalyserteametri** — p50/p95/p99-forsinkelse + X-Forlangt-Id
  sporingsvurdering
- **Filbasererte Loggninger med Rotasjon** — Konsol-interseptoren fanger opp alt
  til JSON-logg med størrelse-basert rotasjon
- **System-informasjonsrapport** — `npm system-informasjon` generer
  `system-informasjon.txt` med din fullstendige miljø (Node-versjon,
  OmniRoute-versjon, OS, CLI-verktøy, Docker/PM2 status). Fest det når du
  rapporterer feil for å aktivere triage på stedet.

</details>

<details>
<summary><b>🏗️ 11. "Deploying and maintaining the gateway is complex"</b></summary>

Installasjon, konfigurasjon og vedlikehold av en AI-proxy over ulike miljøer
(lokalt, VPS, Docker, skyen) er arbeidsintensivt. Problemer som fastlagte stier,
`EACCES` på mapper, port-konflikter og overføring av krysseplattform kan ha
motstand.

**How OmniRoute solves it:**

- **npm Global Installere** — `npm install -g omniroute &amp;&amp; omniroute` —
  gjort
- **Docker Multi-Plattformer** — AMD64 + ARM64 nativ (Apple Silicon, AWS
  Graviton, Raspberry Pi)
- **Docker Compose Profiler** — `basiskil` (ingen CLI-verktøy) og `cli` (med
  Claude kode, Codex, OpenClaw)
- **Elektron Bajerbare App** — Nativ app for Windows/macOS/Linux med systemtray,
  selv-sjansen, ukonneksjon til nettet
- **Split-Port Modus** — API og dashboard på separate porter for avanserte
  scenarioer (omvendt proxy, kontainer-nettverk)
- **Sky-enhet- Synkroner** — Konfigurasjons-syncronisering over enheter via
  Cloudflare Arbeidere
- **DB Boksingar** — Automatisk boksing, restaurering, eksport og innport av
  alle innstillinger

</details>

<details>
<summary><b>🌍 12. "The interface is English-only and my team doesn't speak English"</b></summary>

Lagene i land hvor ingen engelsk språk brukes, eller i store asiatiske og
europeiske land, har problemer med å forstå engelsk bare-grunnlagte grensesnitt.
Språkbarriere kan hemme adopsjon og øke konfigurasjonsfeil.

**How OmniRoute solves it:**

- **SkjermgrunnDashboard i18n — 30 språk** — Alle 500+ nøkler oversatt,
  inkludert arabisk, bulgarsk, dansk, tysk, spansk, finsk, fransk, hebraisk,
  hindi, ungarsk, indonesisk, italiensk, japansk, koreansk, malaysisk,
  nederlandsk, norsk, polsk, portugisisk (PT/BR), rumensk, russisk, slovakisk,
  svensk, thai, ukrainsk, vietnamesisk, kinesisk, filippinansk, engelsk
- **SVG-Support** — Rihtilsynstopp for arabisk og hebraisk
- **Flerspråkelige READMEs** — 30 complete dokumentasjonsoversettelser
- **Språkvalg** — Globusikoner i headeren for riktig-klassert skifting

</details>

<details>
<summary><b>🔄 13. "I need more than chat — I need embeddings, images, audio"</b></summary>

AI er ikke bare snakkmåling. Utviklere trenger å generere bilder, transkribere
lyd, opprette embedinger for RAG, område dokumenter og modere innhold. Hvert API
har en forskjellende endpunkt og format.

**How OmniRoute solves it:**

- **Embeddings** — `/v1/embeddings` med 6 leter og 9+ modeller
- **Bildegenerering** — `/v1/images/generations` med 10 leter og 20+ modeller
  (OpenAI, xAI, Together, Fireworks, Nebius, Hyperbolic, NanoBanana,
  Antigravity, SD WebUI, ComfyUI)
- **Tekst til Video** — `/v1/videos/generations` — ComfyUI (AnimateDiff, SVD) og
  SD WebUI
- **Tekst til Musik** — `/v1/music/generations` — ComfyUI (Stable Audio Open,
  MusicGen)
- **Lydtranskribering** — `/v1/audio/transcriptions` — Whisper + Nvidia NIM,
  HuggingFace, Qwen3
- **Tekst til tale** — `/v1/audio/speech` — ElevenLabs, Nvidia NIM, HuggingFace,
  Coqui, Tortoise, Qwen3, **Inworld**, **Cartesia**, **PlayHT**, + eksisterte
  leverandører
- **Moderasjoner** — `/v1/moderations` — Innholdsikkevekkskrifter
- **Prioritering** — `/v1/rerank` — Dokumentrelevans prioritering
- **Svar-API** — Full `/v1/responses` støtte for Codex

</details>

<details>
<summary><b>🧪 14. "I have no way to test and compare quality across models"</b></summary>

Utvikler ønsker å vite hvilken modell som er best for deres bruk tilfelle –
kode, oversettelse, og resonering – men sammenligning i hånden er langsom. Ingen
integrerte evalueringstiltakinger eksisterer.

**How OmniRoute solves it:**

- **Læringsmodellene evaluering** — Gullsettest med 10 pre-lagde tilfeller
  dekkende hei, matematikk, geografi, kodegenerering, JSON samholder,
  oversettelse, markdown, trygghensrefusen
- **4 Match Strategier** — `eksakt`, `innefatter`, `regulære uttrykk`,
  `oppbyggd` (JS-funksjon)
- **Translator Playground Test Bench** — Gruppen testing med flere innputer og
  forventede utganger, tvilkorriderende sammenligning
- **Samtale Tester** — Full rundtur med visuell respons rendering
- **Live Overvåker** — Ener real-time strøm av alle forespørsler som flyter
  gjennom proxyen

</details>

<details>
<summary><b>📈 15. "I need to scale without losing performance"</b></summary>

Når forespørselsvolumet vokser, uten å cache samme spørsmål genererer
duplikatere kostnader. Utan idempotens, duplikate forespørsler avlurer
prosesseringen. Måtte respektere per-leverandør takseligner.

**How OmniRoute solves it:**

- **Semantisk Kasse** — To-lags kasse (signatur + semantisk) reduserer kostnad
  og latency
- **Foregående Idempotens** — 5s utvinkelukning for sammenlignbare forespørsler
- **Takseligner Deteksjon** — Per-leverandør RPM, min gap, og maks concurrent
  sporing
- **Redigerebare Takseligner** — Konfigurerebare standarder i Innstillinger →
  Resiliens med persistens
- **API-nykk Verifikasjons Kasse** — 3-lagets kasse for produktions ytelse
- **Helse D dashboard med Telemetri** — p50/p95/p99 latency, kasse statistikker,
  uptime

</details>

<details>
<summary><b>🤖 16. "I want to control model behavior globally"</b></summary>

Utviklere som ønsker alle svar på en bestemt språk, med en bestemt tonen, eller
ønsker å begrense resonere tokens. Konfigurerer dette i hver
hjelpemiddel/forespørsel er praktisk

**How OmniRoute solves it:**

- **System Prompt Injection** — Global prompt tilknyttet til alle forespørsler
- **Tenkende Budgetvalidering** — Resonere tokens allokasjonskontroll per
  forespørsel (pass-through, auto, custom, adaptive)
- **6 Routing Strategier** — Globale strategier som bestemmer hvordan
  forespørsler er distribuert
- **Wildcard Navigator ** — `leverandør/* `mønster ruter dynamisk til noen
  leverandør
- **Kombo Enable/Disable Toggle** — Toggla kombi direkte fra dashboardet
- **Leverandør Toggle** — Aktiver/deaktiver alle koblinger for en leverandør med
  ett trykk
- **Blokkerte Leverandører** — Utslutter specifikke leverandører fra `/v1/models
  ` listevurdering

</details>

<details>
<summary><b>🧰 17. "I need MCP tools as first-class product capabilities"</b></summary>

Mange AI-bruer åpner kun MCP som en skjult utstyres detalje. Holdninger trenger
en synlig, høyste, styremask for operationer.

**How OmniRoute solves it:**

- Navigasjonsknappen til MCP i dashboardsynlisten og endpoint-protokollenappe
- Dedikert siden for MCP-styring med prosess, verktøy, områder og audit
- Innbygd hurtigstart for omniroute --mcp og klientoppbygning

</details>

<details>
<summary><b>🧠 18. "I need A2A orchestration with sync + stream task paths"</b></summary>

Agentflytenes funksjonom trenger både direkte svar og lange, streamet utkjøring
med livssykluskontroll.

**How OmniRoute solves it:**

- A2A JSON-RPC-endpunkt ( [POST /a2a`]) med send-melding og strømmende melding
- SSE-strøming med terminalebetinget tilstandsoverføring
- Tilknyttede API'er for å hente oppgaver [tasks/get`] og avbryte oppgaver
  [tasks/cancel`]

</details>

<details>
<summary><b>🛰️ 19. "I need real MCP process health, not guessed status"</b></summary>

Ansattes hold trenger å vite om MCP faktisk er aktiv, ikke bare om API-en er
tilgjengelig.

**How OmniRoute solves it:**

- Hjertefilstatus med PID, tidsstempel, transport, verktøyrekkefølge og
  områdemodus
- MCP-status- API-en kombinerer hjerte + nylige aktivitet
- Synlighetsskort for prosess/aktivitetstid/livseligenskap

</details>

<details>
<summary><b>📋 20. "I need auditable MCP tool execution"</b></summary>

Når verktøy endrer konfigurasjon eller provoserer automatiseringsaksjoner,
trenger hold forensisk sporbarhet.

**How OmniRoute solves it:**

- SQLite-bakket audit-logg med MCP-verktøykallet
- Filtrering etter verktøy, suksess/filenotat, API-nøkkel og sideinnstilling
- Dashboardsynet for audit + opplysninger om automatisering

</details>

<details>
<summary><b>🔐 21. "I need scoped MCP permissions per integration"</b></summary>

Forskjellige klienter skal ha minst nødvendig tilgang til verktøykategorier.

**How OmniRoute solves it:**

- 9 detaljerte MCP-scoper for kontrollert tilgang til verktøy
- Omfang og synlighet i MCP-dashboard for administrasjon
- Sikker fordeling av standardstand på operasjonsverktøy

</details>

<details>
<summary><b>⚙️ 22. "I need operational controls without redeploying"</b></summary>

Lagene trenger hurtige tilpasninger under hendelser eller kostevent.

**How OmniRoute solves it:**

- Swith-inn-kombinasjon aktivert direkte fra MCP-bilde
- Prosedyrer for åpning av motstandsdemping fra definerte policy-pakker
- Nytt tilstand for å trekke tilbake sirkulær brenner fra samme
  operasjonspanelet

</details>

<details>
<summary><b>🔄 23. "I need live A2A task lifecycle visibility and cancellation"</b></summary>

Uten visning av livssyklus, opptrer hendelser for å bli vanskelige å triaging.

**How OmniRoute solves it:**

- Listevisning og filtrering av oppgaver etter tilstand/talenter med pagninering
- Drill-down på oppgave metadata, hendelser og artefakt
- Konfirmasjonsfunksjonalitet for å kansellere oppgave med UI

</details>

<details>
<summary><b>🌊 24. "I need active stream metrics for A2A load"</b></summary>

Strømende arbeidsflyt krever operasjonsinsight i konkurranse og
live-forbindelser.

**How OmniRoute solves it:**

- Aktive strømrekker integrert i A2A-status
- Siste oppgave-tidsstempel og antall oppgaver pr. tilstand
- Visning av cards for løpelig overvåking på A2A-dashboard

</details>

<details>
<summary><b>🪪 25. "I need standard agent discovery for clients"</b></summary>

Eksterne klienter og orkestratorer trenger maskin-låsbart metadata for å
påmelding.

**How OmniRoute solves it:**

- Agentkort vist ved `/.well-known/agent.json`
- Egenskaper og ferdigheter vist på administrasjons-grunnlaget
- A2A-status-APIne inkluderer oppdagelsesdata for automatisering

</details>

<details>
<summary><b>🧭 26. "I need protocol discoverability in the product UX"</b></summary>

Hvis brukere ikke kan oppdage protokollsflater, følger tilgang og støttekvalitet
ned.

**How OmniRoute solves it:**

- Konsolidert **Sluttpunkter** side med skjemaer for Proksy, MCP, A2A og API
  -slutpunkter
- Innbygde servicestatus-sammenstillinger (Online/Offline) for MCP og A2A
- Lenker fra oversikten til dedikerte administrasjonstabaner

</details>

<details>
<summary><b>🧪 27. "I need end-to-end protocol validation with real clients"</b></summary>

Mogleste tester er ikke nok til å verifisere protokolls-kompatibilitet før
lansering

**How OmniRoute solves it:**

- E2E -sett som trekker opp og bruker virkelige MCP -SDK-klienttransport
- A2A -klient tests for oppdagelse, sende, strøm, get og avbryte strøm
- Tjekke påstanden mot MCP -auditt og A2A -oppdrags-API-eiere

</details>

<details>
<summary><b>📡 28. "I need unified observability across all interfaces"</b></summary>

Delering av oversiktighet etter protokoll skaper blinde flekker og lengre MTTR

**How OmniRoute solves it:**

- Samlet dashboard/logs/analytics i ett produkt
- Helse + logg + forespørsel-telemetri gjennom åpne AI, MCP og A2A -kapper
- Operasjons-APIene for status og automatisering

</details>

<details>
<summary><b>💼 29. "I need one runtime for proxy + tools + agent orchestration"</b></summary>

Å kjøre mange separate tjenester øker operativ kostnad og feilmoduser\
==WEBLATE_PART==

**How OmniRoute solves it:**

- Eksplorer for AI-kompatibilitet, MCP-tjenestebil og A2A-tjenestebil i én stack
- Delad autentisering, motstandsdyktighet, oppbevaring og overvåkning
- Konsistente politimodeller over hele interaksjonsflaten

</details>

<details>
<summary><b>🚀 30. "I need to ship agentic workflows without glue-code sprawl"</b></summary>

Lag leveres ikke noen hastighet når lagene må lime sammen flere ulike
ad-hoc-tjenester og skript.

**How OmniRoute solves it:**

- Samlet slutpunktsstrategi for klienter og agenter
- Bygd-inn i protokollsvedkjørings UI og røykvalideringsbaner
- Produksjonsklare grunner (sikkerhet, logging, motstandsdyktighet, backup)

</details>

### Eksempler på playbook (integrerte bruker cases)

**Playbook A: Fokus på betalte abonnements og billig opplæggsbackup**

```txt
Kombinasjon: "maximize-claude"
  1. cc/claude-opus-4-6
  2. glm/glm-4.7
  3. if/kimi-k2-thinking

Månedlig kostnad: $20 + liten backup-spendering
Utfall: Høyere kvalitet, nær null inngreper
```

**Playbook B: Nøytral kostnad for kodingstack**

```txt
Kombinasjon: "gratis for alltid"
  1. gc/gemini-3-flash
  2. if/kimi-k2-tenkning
  3. qw/qwen3-koder Plus

Månedlig kostnad: $0
Utfall: Stabilt gratis kodingsskift
```

**Playbook C: 24/7 alltid-tilgjengelig fallbackkjede**

```txt
Kombinasjon: "alltid på"
  1. cc/claude-opus-4-6
  2. cx/gpt-5.2-kodeks
  3. glm/glm-4.7
  4. minimax/MiniMax-M2.1
  5. if/kimi-k2-tenkning

Utfall: Dypt fallback for deadline-kritiske lasteposter
```

**Playbook D: Agent-operasjoner med MCP + A2A**

```txt
1) Start MCP transport (`omniroute --mcp`) for instrumenteret driftsoperasjoner
2) Kjør A2A-oppgaver via `melding/send` og `melding/stream`
3) Overvåk via /dashboard/endpoint (MCP og A2A-paneler)
4) Slå opp eller ned services via innbygd statuskontroller
```

---

## 🆓 Start gratis – null konfigurasjonskostnad

> Installasjon av AI-koding i minutter på **$0/month**. Verb integration på
> basis av kombinert inbygd **gratis stack** combo.

| Steg | Handling                                                          | Gjenoppdage Foretak                                             |
| ---- | ----------------------------------------------------------------- | --------------------------------------------------------------- |
| 1    | Ta forbindelse til **Kiro** (AWS-bygger ID OAuth)                 | Claude Sonnet 4.5, Haiku 4.5 — **uendelig**                     |
| 2    | Ta forbindelse til **iFlow** (Google OAuth)                       | kimi-k2-denker, qwen3-koder-plus, deepseek-r1... — **uendelig** |
| 3    | Ta forbindelse til **Qwen** (Utegangsstyringselement)             | qwen3-koder-plus, qwen3-koder-blink — **uendelig**              |
| 4    | Ta forbindelse til **Gemini CLI** (Google OAuth)                  | gemini-3-blink, gemini-2.5-pro — **180K/mo gratis**             |
| 5    | `/dashboards/ kombinasjoner` → **gratis Stapel gratis (0 $)** mal | Rundt danne alle frie anbytere automatisk                       |

**Punkt noen IDE/CLI på: ** `http://localhost:20128/v1` klienttjeneste: `alle
tekster` gjort.

> **Valgfri extra dekke (også gratis): ** Groq API-nøkkel (30 RPM gratis),
> NVIDIA NIM (40 RPM gratis, 70+ modeller), Cerebras (1M tok/døgn), LangKatt
> API-nøkkel (50M tokens/døgn!), Cloudflare Arbeidere AI (10K neuron/døgn, 50+
> modeller).

## Rask start

### 1. Installer og kjør

```bash
npm install -g omniroute
omniroute
```

> **pnpm brukere:** Kjør `pnpm godkjenne-builds -g` etter installasjon for å
> aktivere native build-skripter krevert av `bedre-sqlite3` og `@swc/core`:
> 
> ```bash
> pnpm install -g omniroute
> pnpm godkjenne-builds -g   # Velg alle pakker → godkjenne
> omniroute
> ```

Dashboard åpnes på `http://localhost:20128` og API-bas-URL er
`http://localhost:20128/v1`.

| Kommando               | Beskrivelse                                                 |
| ---------------------- | ----------------------------------------------------------- |
| `omnirute`             | Start server (`PORT=20128`, API og dashboard på samme port) |
| `omnirute --port 3000` | Sette kanoniske/port-API-port til 3000                      |
| `omnirute --mcp`       | Start MCP-server (stdio transport)                          |
| `omnirute --ikke-åpne` | Ikke åpne nettleser automatisk                              |
| `omnirute --hjelp`     | Vis hjelp                                                   |

Valgfri split-port mode:

```bash
PORT=20128 DASHBOARD_PORT=20129 omnirute
# API:       http://localhost:20128/v1
# Dashboard: http://localhost:20129
```

### 1) Løp opp til dashboarden og klikk på [X17X]Tjenere[X27X]

1. Åpne Dashboard → `Tjenere` og kobler opp minst ett tjenere (OAuth eller
   API-nøkkel).
2. Åpne Dashboard → `Punkter` og opprett en API-nøkkel.
3. (Valgfritt) Åpne Dashboard → `Kombinasjoner` og sett din fallback-kjedde.

### 2) Kom i gang med OmniRoute

```txt
Base URL: http://localhost:20128/v1
API-nøkkel:  [ekskjerm fra Punkt-side]
Modell:    if/kimi-k2-thinking (eller noen annen tjenesteanbuddes/modellprefix)
```

Kompater med Claude Code, Codex CLI, Gemini CLI, Cursor, Cline, OpenClaw,
OpenCode, og OpenAI-kompatibelt SDK.

### 3) Aktiver og valider protokoller (2.0)

**MCP (for tool-driven operasjoner):**

```bash
omniroute --mcp
```

Kobler da MCP clientes over `stdio` og tester verktøy slik:

- `omniroute_get_health`
- `omniroute_list_combos`

**A2A (for agent-to-agent workflows):**

```bash
curl http://localhost:20128/.well-known/agent.json
```

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"quickstart","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"Gi meg en kort oversikt over kvoten."}]}}'
```

### 4) Valider alt fra begynnelsen til Ende (anbefalt)

```bash
npm run test:protocols:e2e
```

Dette tilsett validerer gjennomgående MCP og A2A clientfløyer mot en kjører app.

### Alternativ: kobler fra kjelde

```bash
cp .env.example .env
npm install
(PORT=20128 DASHBOARD_PORT=20129 NEXT_PUBLIC_BASE_URL=http://localhost:20129) npm run dev
```

---

## 🐳 Docker

OmniRoute er tilgjengelig som en offentlig Docker-bilde på [Docker
Hub](https://hub.docker.com/r/diegosouzapw/omniroute).

**Rask å kjøre:**

```bash
docker run -d \
  --name omniroute \
  --restart unless-stopped \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:latest
```

**Med miljøfil:**

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

**Bruk Docker Compose:**

```bash
# Basis-profil (ingen CLI-verktøy)
docker compose --profile base up -d

# CLI-profil (Claude Code, Codex, OpenClaw bygget inn)
docker compose --profile cli up -d
```

| Bilde                    | Versjon  | Størrelse | Beskrivelse            |
| ------------------------ | -------- | --------- | ---------------------- |
| `diegosouzapw/omniroute` | `nyeste` | ~250MB    | Seneste stabile utgave |
| `diegosouzapw/omniroute` | `1.0.3`  | ~250MB    | Nåværende versjon      |

---

## 🖥️ Desktop-App — Offline & Alltid-På

> 🆕 **NyTT!** OmniRoute er nå tilgjengelig som et **native desktop applikasjon**
> for Windows, macOS, og Linux.

Kjør OmniRoute som en separat desktop applikasjon — uten terminal, nettleser,
eller Internett kreves for lokale modeller. Electron-baserte applikasjonen
inkluderer:

- 🖥️ **Native Window** — Dedikert applikasjon vindu med systemfaner integrasjon
- 🔄 **Auto-Start** — Start OmniRoute på systemtidsinnlogging
- 🔔 **Native Notifications** — Få varsler for lagringsutslitthet eller tilganger
  på provider
- ⚡ **One-Click Install** — NSIS (Windows), DMG (macOS), AppImage (Linux)
- 🌐 **Offline Mode** — Fonker fullt offline med samlet server

### Rask start

```bash
# Utviklingsmodus
npm run electron:dev

# Bygg for din plattform
npm run electron:bygg        # Nåværende plattform
npm run electron:bygg:win     # Windows (.exe)
npm run electron:bygg:mac     # macOS (.dmg) — x64 &amp; arm64
npm run electron:bygg:linux   # Linux (.AppImage)
```

### Systemfaner

Når miniaturering, OmniRoute bor i din systemfaner med rask handling:

- Åpne Dashboard
- Endre server port
- Avslutt applikasjon

📖 Full dokumentasjon: [`electron/README.md`](electron/README.md)

---

## 💰 Priser på et enkelt blikk

| Nivå                     | Provider                   | Kostnad                               | Lagrings- gjenoppretting                         | Best for deg                       |
| ------------------------ | -------------------------- | ------------------------------------- | ------------------------------------------------ | ---------------------------------- |
| **💳 SUBSKU**             | Claudekode (Pro)           | $20/mo                                | 5t + uke                                         | Allerede abonnent                  |
|                          | Codex (Plus/Pro)           | $20-200/mo                            | 5t + uke                                         | Brukere av OpenAI                  |
|                          | Gemini CLI                 | **gratis**                            | 180K/mo + 1K/dag                                 | Alle!                              |
|                          | GitHub Copilot             | $10-19/mo                             | Månedlig                                         | Brukere på GitHub                  |
| **🔑 API NYTTEKSNAKVARD** | NVIDIA NIM                 | **gratis** (for udviklere for alltid) | ≈40 takt/minutt                                  | 70+ åpne modeller                  |
|                          | Cerebras                   | **Gratis** (1M tok/dag)               | 60 000 transaksjoner pr. minutt / 30 takt/minutt | Verdens raskeste                   |
|                          | Groq                       | **Gratis** (30 takt/minutt)           | 14,4 tusen transaksjoner per sekund              | Ekstrem hastig Llama / Gemma       |
|                          | DeepSeek V3.2              | $0,27 / $1,10 per 1M                  | Ingen                                            | Best praktisk kvalitet             |
|                          | xAI Grok-4 Enkel           | **$0,20 / $0,50 per 1M** 🆕            | Ingen                                            | Rask + verktøykall, ultralow       |
|                          | xAI Grok-4 (standard)      | $0,20 / $1,50 per 1M 🆕                | Ingen                                            | Grunnlag for argumentasjon fra xAI |
|                          | Mistral                    | Free trial + paid                     | Begrenset pris                                   | European AI                        |
|                          | OpenRouter                 | Pay-per-use                           | Ingen                                            | 100+ models aggr.                  |
| **💰 CHEAP**              | GLM-5 (via Z.AI) 🆕         | $0.5/1M                               | Daily 10AM                                       | 128K output, newest flagship       |
|                          | GLM-4.7                    | $0.6/1M                               | Daily 10AM                                       | Budget backup                      |
|                          | MiniMax M2.5 🆕             | $0.3/1M input                         | 5-hour rolling                                   | Reasoning + agentic tasks          |
|                          | MiniMax M2.1               | 0,2/1M                                | 5-hour rolling                                   | Den billigste muligheten           |
|                          | Kimi K2.5 (Moonshot API) 🆕 | Pay-per-use                           | Ingen                                            | Direkte tilgang til Moonshot API   |
|                          | Kimi K2                    | 9/mo flate pris                       | 10M tokener/mo                                   | Forutsigbar kostnad                |
| **🆓 GRATIS**             | iFlow                      | **$0**                                | Uendelig                                         | 5 modeller uten grunn              |
|                          | Qwen                       | **$0**                                | Uendelig                                         | 4 modeller uten grunn              |
|                          | Kiro                       | **$0**                                | Uendelig                                         | Claude Sonnet/Haiku (AWS Builder)  |
|                          | LangKat Flash-Lite 🆕       | **$0** (50M tok/day 🔥)                | 1 RPS                                            | Vert fre porto på jorden           |
|                          | Pollen AI 🆕                | **$0** (ingen nøkkel påkråvet)        | 1 forespørsel/15s                                | GPT-5, Claude, DeepSeek, Llama 4   |
|                          | Cloudflare Workers AI 🆕    | **$0** (10K Neuroner/dag)             | ~150 respons/dag                                 | 50+ modeller, globale kantstrekker |
|                          | Scaleway AI 🆕              | **$0** (1M tokener totalt)            | Begrenset pris                                   | EU/GDPR, Qwen3 235B, Llama 70B     |

> 🆕 **Nye modeller tilføyd (Mar 2026): ** Grok-4 Fast-familie på $0,20/$0,50/M
> (mål for 1143 ms – 30% raskere enn Gemini 2,5 Flash), GLM-5 via Z.AI med 128K
> utgang, MiniMax M2,5 resonanse, DeepSeek V3,2 oppdatert prismatching, Kimi
> K2,5 via Moonshot direkte API

**💡 $0 Combo Stack — Den komplette free-setup: **

```
# 🆓 Ultimate Free Stack 2026 — 11 Providerer, $0 Evighets
Kiro (kr/)             → Sonnet/ Haikur Claudes/ Uendelig
iFlow (if/)            → kimi-tenkning-k2 , qwen3-sykepleier-plus, sykdomsinnsikt-r1 Uendelig
LongCat Lite (lc/)     → LongCat-Flash-Lite – 50M tokener/dag 🔥
Pollinations (pol/)    → GPT-5, Claud, DeepSeek, Llama 4 - Ingen nøkkel påkrav
Qwen (qw/)             → qwen3-sykepleier-plus, qwen3-syke pleier-Flash, qwen3-sykepleier-next Uendelig
Gemini (gemini/)       → Gemini 2,5 Flash - gratis api-nøkkel med 1 500 forespørsler gratis API-nøkkel
Cloudflare AI (cf/)    → Llama 70B, Gemma 3, Mistral - 10K Neuroner/dag
Scaleway (scw/)        → Qwen3 235B, Llama 70B - 1M gratis tokener (EU)
Groq (groq/)           → Llama/Gemma ultra-rask – 14.4K forespørsel/dag
NVIDIA NIM (nvidia/)   → 70+ åpne modeller – 40 RPM for evig tid
Cerebras (cerebras/)   → Llama/Qwen verdens-raskeste - 1M tok/dag
```

**Nul koster. Den stopper aldri med koding.** Konfigur dette som én
OmniRoute-kombinasjon og alle backup-strategiene skjer automatisk - ingen
manuell valg noen gang.

---

---

## 🆓 Gratis modeller – Det du faktisk får

> Alle modellene nedenfor er **100% gratis uten noen kreditkort påkrav**.
> OmniRoute rutestreker mellom dem når et kvot er slutt – kombiner dem alle for
> en ubrakkbar $0 kombinasjon.

### 🔵 CLAUDE MODELLER (via Kiro – AWS byggings ID)

| Model               | Prefiks | Begrensinger | Satsgrense                     |
| ------------------- | ------- | ------------ | ------------------------------ |
| `claude-sonnet-4.5` | `kr/`   | **Uendelig** | Ingen rapportert daglig grense |
| `claude-haiku-4.5`  | `kr/`   | **Uendelig** | Ingen rapportert daglig grense |
| `claude-opus-4.6`   | `kr/`   | **Uendelig** | Siste opus via Kiro            |

### 🟢 IFLOW-MODELLER (Gratis OAuth – Ingen kredittkort)

| Model                  | Prefiks | Begrensinger | Satsgrense              |
| ---------------------- | ------- | ------------ | ----------------------- |
| `kimi-k2-tenkning`     | `if/`   | **Uendelig** | Ingen rapportert grense |
| `qwen3-kodepluks/X17X] | `if/`   | **Uendelig** | Ingen rapportert grense |
| `dyptiske-søk-r1`      | `if/`   | **Uendelig** | Ingen rapportert grense |
| `minimax-m2.1`         | `if/`   | **Uendelig** | Ingen rapportert grense |
| `kimi-k2`              | `if/`   | **Uendelig** | Ingen rapportert grense |

### 🟡 QWEN MODELLER (Uten å kunne QWEN-koder)

| Model                     | Prefiks | Begrensinger | Satsgrense              |
| ------------------------- | ------- | ------------ | ----------------------- |
| `qwen3-kodepluks/X17X]    | `qw/`   | **Uendelig** | Ingen rapportert grense |
| `qwen3-kode-rasker-flash` | `qw/`   | **Uendelig** | Ingen rapportert grense |
| `qwen3-kode-neste`        | `qw/`   | **Uendelig** | Ingen rapportert grense |
| `vision-modell`           | `qw/`   | **Uendelig** | Multimodal (bilder)     |

### 🟣 GEMINI CLI (Google-Authentisering)

| Model                    | Prefiks | Begrensinger                      | Satsgrense             |
| ------------------------ | ------- | --------------------------------- | ---------------------- |
| Gemini-3-flash-preview'` | `gc/`   | **180 000 tok/month** + 1 000/day | Månedlig gjennomføring |
| `Gemini-2,5-pro`         | `gc/`   | 180 000/tok måned (delt pool)     | Høy kvalitet           |

### ⚫ NVIDIA NIM (Gratis API-nyksel — build.nvidia.com)

| Nivå      | Daglig grense | Satsgrense     | Notater                                                       |
| --------- | ------------- | -------------- | ------------------------------------------------------------- |
| Fri (Dev) | Ingen tokkaps | ** ~ 40 RPM ** | 70+ modeller; overgang til rene begrensinger i midten av 2025 |

Populære frie modeller: `moonshotai/kimi-k2,5` (Kimi K2,5), `z-ai/glm4,7` (GLM
4,7), `deepseek-ai/deepseek-v3,2` (DeepSeek V3,2),
`nvidia/llama-3,3-70b-instruct`, `deepseek/deepseek-r1`

### ⚪ CEREBRAS (Gratis API-nyksel — inference.cerebras.ai)

| Nivå   | Daglig grense      | Satsgrense                                       | Notater                                           |
| ------ | ------------------ | ------------------------------------------------ | ------------------------------------------------- |
| Gratis | **1M tekster dag** | 60 000 transaksjoner pr. minutt / 30 takt/minutt | Verdens raskeste LLM-inferens; daglig innsettelse |

Tilgjengelig gratis: `llama-3.3-70b`, `llama-3.1-8b`,
`deepseek-r1-distill-llama-70b`

### 🔴 GROQ (Gratis API-nyksel — console.groq.com)

| Nivå   | Daglig grense | Satsgrense        | Notater                                              |
| ------ | ------------- | ----------------- | ---------------------------------------------------- |
| Gratis | **14.4K RPD** | 30 RPM per modell | Ingen kredittkort; 429 på begrensning, ikke beregnet |

Tilgjengelig gratis: `llama-3.3-70b-versatile`, `gemma2-9b-it`, `mixtral-8x7b`,
`whisper-large-v3`

### 🔴 LONGCAT AI (Gratis API-nyksel — longcat.chat) 🆕

| Model                          | Prefiks | Dagsgratist kvote | Notater                        |
| ------------------------------ | ------- | ----------------- | ------------------------------ |
| `LangtKatt-Flash-Lite`         | `lc/`   | [50M tokens** 💥]  | Største gratis kvote noen gang |
| `LangtKatt-Flash-Chat`         | `lc/`   | 500K tokens       | Mellomturnerende samtale       |
| `LangtKatt-Flash-Tenking`      | `lc/`   | 500K tokens       | Argumentering / CoT            |
| `LangtKatt-Flash-Tenking-2601` | `lc/`   | 500K tokens       | Januar 2026 versjon            |
| `LangtKatt-Flash-Omni-2603`    | `lc/`   | 500K tokens       | Multimodal                     |

> 100% gratis så lenge den er i offentlig beta. Godt seg inn på
> [langtKatt.chat](https://longcat.chat) med e-post eller telefon. Nå på nytt
> hver dag kl 00:00 UTC.

### 🟢 POLLINATIONS AI (Ingen API-gateway nødvendig) 🆕

| Model      | Prefiks | Satsgrense        | Levert Av Produsent |
| ---------- | ------- | ----------------- | ------------------- |
| `openai`   | `Pol/`  | 1 forespørsel/15s | GPT-5               |
| `Claude`   | `Pol/`  | 1 forespørsel/15s | Anthropic Claude    |
| `Gemini`   | `Pol/`  | 1 forespørsel/15s | Google Gemini       |
| `Deepseek` | `Pol/`  | 1 forespørsel/15s | DeepSeek V3         |
| `Llama`    | `Pol/`  | 1 forespørsel/15s | Meta Llama 4 Scout  |
| `Mistral`  | `Pol/`  | 1 forespørsel/15s | Mistral AI          |

> ✨ **Nøytral belastning:** Ingen registrering, ingen API-nyckel. Legg til
> Pollinations-leverandøren med ett tomt felt for API-nyckel slik at det
> fungerer øyeblikkelig.

### 🟠 CLOUDFLARE WORKERS AI (Gratis API-nyckel – cloudflare.com) 🆕

| Nivå   | Daglige Neuroner | Lignende bruk                                                | Notater                      |
| ------ | ---------------- | ------------------------------------------------------------ | ---------------------------- |
| Gratis | **10,000**       | Kring 150 AI-modeller / 500 sekunders lyd / 15 000 innEmbeds | Globale kanten, 50+ modeller |

Populære gratis modeller: `@cf/meta/llama-3.3-70b-instruct`,
`@cf/google/gemma-3-12b-it`, `@cf/openai/whisper-large-v3-turbo` (gratis lyd!),
`@cf/qwen/qwen2.5-coder-15b-instruct`

> Tilpasser API-tokens + konto ID fra
> [dash.cloudflare.com](https://dash.cloudflare.com). Lagre Konto ID i
> provider-innstillinger.

### 🟣 SKALA AI (1M gratis tokens — scaleway.com) 🆕

| Nivå   | Fri Omland    | Lokasjon     | Notater                                             |
| ------ | ------------- | ------------ | --------------------------------------------------- |
| Gratis | **1M tokens** | 🇫🇷 Paris, EU | Ingen kortbehøring nødvendig innenfor grenseverdier |

Tilgjengelige gratis: `qwen3-235b-a22b-instruct-2507` (Qwen3 235B!),
`llama-3.1-70b-instruct`, `mistral-small-3.2-24b-instruct-2506`,
`deepseek-v3-0324`

> EU / GDRP-kompatibel. Få API-nytta på
> [console.scaleway.com](https://console.scaleway.com).

> **💡 Den ultimate gratis stacken (11 tilbydere, $0 For alltid):**
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

| Provider         | Free Credits           | Best Model                                   | Satsgrense                   |
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

Så her er oversettelsen: \
\
Siden `/innstillinger/medier` → **Transkripsjon** -skjerm: last opp noen lyd-
eller videofil → velg kombiende hvorpå slutten skjerm: hent transkripsjon i
støttede former.

## 💡 Viktig funksjoner

OmniRoute v2.0 er bygget som et operasjonelt plattform, og ikke bare en
reléproxy.

### 🆕 Nytt — ClawRouter-Inspirerte Improvisasjoner  (Mar 2026)

| Funksjon                                | Hva Den Gjør                                                                                         |
| --------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| ⚡ **Grok-4 Fast Familie**               | xAI-modeller på $0,20/$0,50/M — benchmarket 1143ms (30% raskere enn Gemini 2,5 Flash)                |
| 🧠 **GLM-5 via Z.AI**                    | 128K utgangs kontekst, $0,5/1M — nyeste følgesvenn fra GLM-familien                                  |
| 🔮 **MiniMax M2,5**                      | Årsaken + agente oppgaver på $0.30/1M — betydelig oppgradering fra M2.1                              |
| 🎯 **modellBruker flagg per modell**     | Per-modell `modellBruker: true/false` i registeret — AutoCombo unngår ikke-verktøy-kapable modeller  |
| 🌍 **Multi -språklig Intents Deteksjon** | PT/ZH/ES/AR nøkkelord i AutoCombo poenggiving — bedre modellvalg for innhold på andre språk          |
| 📊 **Benchmark -drevet fallback**        | Faktisk p95 latens fra levende kjørebøger foder combo poenggiving — AutoCombo lærer fra sjelden dato |
| 🔁 **Forsking Deduplikasjon**            | InnhaldHash-basert dedup-window — flere agent sikre, forhindrer på nytt påføringskostnader           |
| 🔌 **Pluggbart RouterStrategy**          | Tilgjengelig `RouterStrategy`-grunnlag — legg til kustom tilkoblingslogikk som plugins               |

### 🚀 Tidligere v2.0.9+ — Playground, CLI Fingerprints & ACP

| Funksjon                                          | Hva Den Gjør                                                                                                                                                                                                                                                |
| ------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🎮 **Modell Playground**                           | Oversikts-side for å teste hvilket model som helst – provider/model/endpoint-velger, Monaco-redigerer, streaming, avbryte, tid                                                                                                                              |
| 🔏 **CLI Fingerprints Overensstemmelse**           | Hodning-per-provider for header/body ordening til å matche native CLI tegn – skru av per provider i Innstillinger > Sikkerhet. **Ditt proxy-IP forblir bevarert**                                                                                           |
| 🤝 **ACP-tilstedeværelse (Agent client protocol)** | CLI-agentoppdagelse (Codex, Claude, Goose, Gemini CLI, OpenClaw + 9 flere), prosess-spawner, `/api/acp/agents` sluttsted                                                                                                                                    |
| 🤖 **ACP Agenter Oversiktsflate**                  | Feillogg› Agenter-side – grid av 14 agenter med installasjonsstatus, versjon, anleggsform for hva som helst CLI-verktøy. ** OpenCode**-brukere får en "Hent opencode.json" knapp som autogenererer en klar til bruk config med alle tilgjengelige modeller. |
| 🔧 **Anleggsmodell `apiFormat` Tilkobling**        | Anleggsmodeller med `apiFormat: "svar"` ruter nå korrekt til Svar-API-forhandler                                                                                                                                                                            |
| 🏢 **Codex Arbeidsrom Isolering**                  | Flere Codex arbeidsrom per e-post – OAuth samles korrekt opp koblinger etter arbeidsrom ID                                                                                                                                                                  |
| 🔄 **Elektron Automatisk Oppdateringer**           | Dessktop-app sjekker etter oppdateringer + auto-installer på restart                                                                                                                                                                                        |

### 🤖 Operasjoner for agenter & protokoll (v2.0)

| Funksjon                              | Hva Den Gjør                                                                                        |
| ------------------------------------- | --------------------------------------------------------------------------------------------------- |
| 🔧 **MCP Server (16 tools)**           | IDE/agent tools via 3 transports: stdio, SSE (`/api/mcp/sse`), Streamable HTTP (`/api/mcp/stream`)  |
| 🤝 **A2A Server (JSON-RPC + SSE)**     | Agent-to-agent task execution with sync and streaming flows                                         |
| 🧭 **Consolidated Endpoints Page**     | Tabbed management page with Endpoint Proxy, MCP, A2A, and API Endpoints tabs                        |
| 🎚️ **Service Enable/Disable Toggles** | ON/OFF switches for MCP and A2A with settings persistence (default: OFF)                            |
| 🛰️ **MCP Runtime Heartbeat**          | Real process status (pid, uptime, heartbeat age, transport, scope mode)                             |
| 📋 **MCP Audit Trail**                 | Filterable audit logs with success/failure and key attribution                                      |
| 🔐 **MCP Scope Enforcement**           | 9 granular scope permissions for controlled tool access                                             |
| 📡 **A2A Task Lifecycle Management**   | List/filter tasks, inspect events/artifacts, cancel running tasks                                   |
| 📋 **Agent Card Discovery**            | `/.well-known/agent.json` for client auto-discovery                                                 |
| 🧪 **Protokoll E2E Test Harness**      | Sannsynlig MCP SDK + A2A klientstrømme i `test:protocols:e2e`                                       |
| ⚙️ ** Operasjonskontroller**          | Ventilskurv, tilpasning av resistensprofiler, og tidsstyrd avbrytning fra en enkelt kontrollsurface |

### 🧠 Routing & Intelligence

| Funksjon                                 | Hva Den Gjør                                                                          |
| ---------------------------------------- | ------------------------------------------------------------------------------------- |
| 🎯 ** Smart 4-nivå fall tilbake**         | AUTO-rute: Abonnement → API-nøkkel → billig → gratis                                  |
| 📊 ** Real-time kvotetracking**           | Live token telle med avrundningsinformasjon per provider                              |
| 🔄 ** Formatomsetting**                   | OpenAI → Claude → Gemini → Svar med skjemaelement-sikre omsettinger                   |
| 👥 ** Støtte for flere kontoer**          | Flere kontoer per provider med intelligente valg                                      |
| 🔄 ** Automatisk tokenoppdatering**       | OAuth-tokens oppdaterer automatisk med tilbakeforsøk                                  |
| 🎨 ** Personlige kombinasjoner**          | 6 balanserende strategier + kontroll på fall tilbakekjeder                            |
| 🌐 ** Vildkort routrute**                 | `leverandør/*` dynamisk routing                                                       |
| 💭 **Tænkende Budget-Styring**            | Automatisk, selvvalgt, anpasset og adaptive grænseverdier for årsagsrapportering      |
| 🔄 **Modell Aliaser**                     | Innbygd + tilpasset modellaliasing og migrasjonssikkerhet                             |
| ⚡ **Bakgrunn degradering**               | Ruteering for lavprioriterte bakgrunnsoppgaver til billigere modeller                 |
| 💡 **Oppgavebevisst intelligent routing** | Automatisk valg av modell innenfor innholdstype (kode, visjon, analyse, sammenfating) |
| 💬 **System-prompt injeksjon**            | Globale atferdskontroller tilfellet på enhver forespørsel                             |
| 📄 **Svar API-kompatibilitet**            | Full `/v1/svar` støtte til Codex og avansert agential workflows                       |

### 🎵 Multi-Modal APIs

| Funksjon                | Hva Den Gjør                                                                                                                                                          |
| ----------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🖼️ **Bildegenerering**  | `/v1/bilder/ genereringer` med sky og lokal backend                                                                                                                   |
| 📐 **Embedding**         | `/v1/embedding` for søking og RAG-pipeliner                                                                                                                           |
| 🎤 **Tonetranskription** | `/v1/lyd/transkriptioner` — 7 leverandører (Deepgram Nova 3, AssemblyAI, Groq Whisper, HuggingFace, ElevenLabs, OpenAI, Azure), auto-språksneming, MP4/MP3/WAV-støtte |
| 🔊 **Tekst-til-språk**   | `/v1/lyd/tal` — 10 leverendører (ElevenLabs, OpenAI, Deepgram, Cartesia, PlayHT, HuggingFace, Nvidia NIM, Inworld, Coqui, Tortoise) med korrekte feilmeldinger        |
| 🎬 **Videoer Generere**  | `/v1/videofilm/generere` (ComfyUI + SD WebUI-workflows)                                                                                                               |
| 🎵 **Musik Generere**    | `/v1/musik/generere` (ComfyUI-workflows)                                                                                                                              |
| 🛡️ **Moderatorer**      | `/v1/moderatorer` trygghetskontroller                                                                                                                                 |
| 🔄 **Reranking**         | `/v1/gjenranger` for relevansvurdering                                                                                                                                |
| 🔍 **Hjemmeside Søke** 🆕 | `/v1/søk` — 5 leverandører (Serper, Brave, Perplexity, Exa, Tavily), 6 500+ gratis hver måned, auto-failover, cache                                                   |

### 🛡️ Styrke, Sikkerhet og Regulering

| Funksjon                                                          | Hva Den Gjør                                                                                                         |
| ----------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| 🔌 **Ømfunksjonsfelt**                                             | Per-modell turer/håndter med gangbordkontroller                                                                      |
| 🎯 **Modeller med Fokus pÃ Endepunkt**                             | 🛡️ [X3X]Anti-Thundering Herd[X25X]                                                                                   |
| Sekvensemonitoring og låsesemaforsikring på retry-/rate-hendelser | Lite-/vanskelighetsreduksjon ved hjelp av to cash-lagere                                                             |
| 🧠 **Semantic + Signatur Cache**                                   | Kostnad-/trekkferdighetsoptimiert med to cash-lagere                                                                 |
| ⚡ **Request Idempotens**                                          | Duplikatvern frafeldningstid                                                                                         |
| 🔒 **TLS Fingeravtrykk-udåen**                                     | Klientt-typisk TLS-fingeravtrykk — **minimerer robot-dybde og konto-flagging**                                       |
| 🔏 **CLI Fingerprints Overensstemmelse**                           | Samsvarer nativt CLI-oppfordrings-signaturer — **minimerer risiko for å bli blokkert mens man preserverer proxy-IP** |
| 🌐 **IP-Filtering**                                                | Allgjort/tilmegler- og stilisert kontroll for utsatt utgivelse                                                       |
| 📊 **Brukere-tilpasse grense-**                                    | Konfigurerbare global-leverandørs-nivågrenser med beständige verdiene                                                |
| 🔑 **API-nøkkel-administrering + ramme**                           | Sikre nøkkelutstedelses-/omstrenging-og-tilpasse kontroller for levereandør                                          |
| 🛡️ **Beskyttelig `/models`-**                                     | Valgfri auth-gating og levereandør-forskjell-skjul for modellkatalog                                                 |

### Observering og analyser

| Funksjon                                       | Hva Den Gjør                                          |
| ---------------------------------------------- | ----------------------------------------------------- |
| 📝 **Begran reqeust + Proxy Logging**           | Full request/response and proxy logging               |
| 📋 **Samlet logger for åseende Logs Dashboard** | Request, proxy, audit, and console views in one page  |
| 🔍 **Reqeust Telemetry**                        | p50/p95/p99 latency and request tracing               |
| 🏥 **Helsedashboard**                           | Uptime, breaker states, lockouts, cache stats         |
| 💰 **Kostoverførsel og Overholdt budget**       | Budget controls and per-model pricing visibility      |
| 📈 **Analyse og Visuelle **                     | Model/provider usage insights and trend views         |
| 🧪 **Evalueringssystem**                        | Golden set testing with configurable match strategies |

### ☁️ Drift & Plattform

| Funksjon                     | Hva Den Gjør                                                          |
| ---------------------------- | --------------------------------------------------------------------- |
| 🌐 **Deploy Anywhere**        | Hjemme, VPS, Docker, cloudmiljøer                                     |
| 💾 **Cloud Sync**             | Konfigurasjonsinnlasting via moln-arbeider                            |
| 🔄 **Backup/Restore**         | Eksport/import og katastrofehjelpemekanismer                          |
| 🧙 **Onboarding Wizard**      | Førstepassertsledde setup                                             |
| 🔧 **CLI Tools Dashboard**    | Enknapp-opsett for populær kodingstool                                |
| 🎮 **Modell Playground**      | Test noen hvilken som helst leverandør/modell/endpoint fra dashboard  |
| 🔏 **CLI Fingerprint Toggle** | Per-leverandørfingeravtrykkssammenligning i Innstillinger > Sikkerhet |
| 🌐 **i18n (30 språk)**        | Full dashboard + dokumenter språkstøtte med RTL-dekning               |
| 🧹 **Clear All Models**       | Enknapp-modelllistenåpning i leverandørdetaljer                       |
| 📋 **Issue Templates**        | Standardiserte GitHub-mal for feil og funksjoner                      |
| 📂 **Custom Data Directory**  | `opplager_dir` overskrivelse for lagringssted                         |

### Dybdykk i funksjon

#### SMART fallback med praktisk kostkontroll

```txt
Kombo: «min-koding-stakk »
  1. cc/claude-opus-4-6
  2. nvidia/llama-3.3-70b
  3. glm/glm-4.7
  4. if/kimi-k2-væker
```

Når aksesskonto, pris eller helse mislykkes automatisk flyttes OmniRoute til
neste kandidat uten håndheving.

#### Protokollsadministrasjon som er synlig og operabel

- MCP + A2A er oppdagelige i UI og dokumenter (ikke skjulte)
- Protokolls status-API-er åpreger live operasjon data (`/api/mcp/*`,
  `/api/a2a/*`)
- Panesere inneholder handlingsmuligheter for dag-2- drift (kjøringsslutter
  kombi, bryter reset, oppgave avslutning)

#### Oversetter + valideringsflyt

Translator området inkluderer:

- **Spielbar**: forespørsel om overgang for sjekker
- **Chat testasje**: full forespørsel/svar rundtur
- **Test-bank**: flere tilfeller i en løp
- **Livemonitorer**: real-time trafikk visuellisering

Plus protokollvalidering med koblede klienter via `npm kjør:
test:protokoll-e2e`.

> 📖 **[MCP Server README](open-sse/mcp-server/README.md)** — Verktøy referanse,
> IDE konfigurasjoner, og klienteksempler
> 
> 📖 **[A2A Server README](src/lib/a2a/README.md)** — Ferdigheter, JSON-RPC
> metoder, strømming, og oppgavelivssyklus

## 🧪 Evalueringer (Evals)

OmniRoute inkluderer en bygget innevært evaluering ramme til å teste LLM svar
kvalitet mot et gyllen sett. Åpner det opp via **Analitisker → Evals ** i
panelen\
==WEBLATE_PART==

### Bygget-inne Golden Set

Den innbygde "OmniRoute Golden Set"-enheten inneholder tester av typen:

- Heisninger, matematikk, geografi, kodegenerering
- JSON-format-kompliance, oversettelse, markdown-generering
- Ikke-sikkerhetsavvisning (skadelig innhold), tellingsfunksjoner, boolesk
  logikk

### Evalueringsstrategier

| Strategi           | Beskrivelse                                                                                   | Eksempel      |
| ------------------ | --------------------------------------------------------------------------------------------- | ------------- |
| `eksaktt`          | Utstedelsen må være så nær eksakt som muligt                                                  | `"4"`         |
| `inneholder`       | Utstedelsen må inneholde tekststrengen (følsomhet mot stor-bunnpåfallsforsikring ikke-takere) | `"Paris"`     |
| `regulære uttrykk` | Utstedelsen må måtte overensstemme med regulære uttrykk                                       | `"1.*2.*3"`   |
| `personlig`        | Personlig funksjon skriver ut true/false                                                      | `(utgisninng) |

---

## 📚 Innstillasjonsveileder

### Konfigurering av protokoll (MCP + A2A)

<details>
<summary><b>🧩 MCP Setup (Model Context Protocol)</b></summary>

Start MCP-transporten i stdio-lag:

```bash
omniroute --mcp
```

Anbefalte valideringsfløyr:

1. Koble opp MCP-klient over stdio.
2. Utfør `omniroute_get_health`.
3. Utfør `omniroute_list_combos`.
4. Åpne `/dashboard/mcp` for å bekrefte heartbeat, aktivitet og audit.

Bruksomfanger APIs for automatikk:

- `GET /api/mcp/status`
- `GET /api/mcp/tools`
- `GET /api/mcp/audit`
- `GET /api/mcp/audit/stats`

</details>

<details>
<summary><b>🤝 A2A Setup (Agent2Agent)</b></summary>

Oppdag agenten:

```bash
curl http://localhost:20128/.well-known/agent.json
```

Send en oppgave:

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'innholdstyp: applikasjons/json' \
  -d '{"jsonrpc":"2.0","id":"innstallas-a2a","metode":"message/send","parametre":{"ferdighet":"kvotahåndtering","beskjeder":[{"rolle":"bruker","innhold":"Sammenfatting av kvotestatus."}]}}'
```

Forespill livssyklus:

- `GET /api/a2a/status`
- `GET /api/a2a/oppgaver`
- `GET /api/a2a/oppgaver/:id`
- `POST /api/a2a/oppgaver/:id/avbryt`

Operasjons-UI:

- `/kantoor/a2a` for oppgave/tillstand/streameobservasjon og ukefester

</details>

<details>
<summary><b>🧪 End-to-end protocol validation</b></summary>

Verifiser begge protokoller med virkelige klienter:

```bash
npm run test:protocols:e2e
```

Dette verifiser:

- MCP SDK-klient koble/listen/ring
- A2A oppdager/send/streame/get/avbryt
- Kryss-kontroll data i MCP-revisjon og A2A oppgavemanagements API-er

</details>

<details>
<summary><b>💳 Subscription Providers</b></summary>

### Claude Code (Pro/Max)

```bash
Skjermbilde → Leverandører → Koble Claude Code
→ OAuth-innlogging → Auto-tekning avtoken
→ Quota-føring på 5timer + ukedag
Modeller:
  cc/claude-opus-4-6
  cc/claude-sonnet-4-5-20250929
  cc/claude-haiku-4-5-20251001
```

**Pro tips:** Bruk Opus for komplekse oppgaver, Sonnet for raskhet. OmniRoute
sporer quota per modell!

### OpenAI Codex (Plus/Pro)

```bash
Skjermbilde → Leverandører → Koble Codex
→ OAuth-innlogging (port 1455)
→ 5timer + ukedag återstel
Modeller:
  cx/gpt-5.2-codex
  cx/gpt-5.1-codex-max
```

#### Codex konto begrensning Management (5 timer + ukedag)

Hver Codex-konto har nåpolicy-overstykker i `Skjermbilde → Leverandører`:

- `5 timer` (På/Av): tilpasse den 5-timeglassetspolicytregsel.
- [Vekelyse`] (PÅ/SVÅN): tvangsspåring for å gjennomføre veiledende policy for
  vekelysopphem.
- Trekkspalte oppførsel: når en aktiviserer vinduet nådde ≥90% bruk, dette
  kontoen blir overskygget.
- Rotasjon oppførsel: OmniRoute sender til nærmeste kvalifiserte Codex konto
  automatisk.
- Nulstilling oppførsel: når levere `nåddeX42X] tidsfrist går igjen, kontoen
  blir kvalifisert igjen automatisk.

Scenarioer:

- `5h ON` + `Vekeleg ON`: kontoen blir overskygget når en vindu nådde tregå til
  begrænsning.
- `5h OFF` + `Vekeleg ON`: Berøring vekekonskons besåt blokkerer ikke kontoen.
- `5h ON` + `Vekeleg OFF`: bare 5 timme besåten gir kontoen begrænsning.
- `nådde` gått igjen tid og kontoen reentres automatisk (ingen manuell
  påståsende).

### Gemini CLI (gratis, 180K/måndel!)

```bash
Oversikt → Levere → Connect Gemini CLI
→ Google OAuth
→ 180K kompletteringer/måndel + 1K/dag

Modeller:
  gc/gemini-3-flash-forutsigelse
  gc/gemini-2.5-pro
```

**Beste Vurde:** Stort gratis nivå! Bruk dette før betalingsnivå.

### GitHub Copilot

```bash
Oversikt → Levere → Connect GitHub
→ OAuth via GitHub
→ Månedlig nulstilling (1ste i måndel)

Modeller:
  gh/gpt-5
  gh/claude-4.5-sonnet
  gh/gemini-3-pro
```

</details>

<details>
<summary><b>🔑 API Key Providers</b></summary>

### NVIDIA NIM (gratis utvikler tilgang — 70+ modeller)

1. Skriv inn: [build.nvidia.com](https://build.nvidia.com)
2. Få gratis API-nyckel (1000 inferences inkludert)
3. Oversikt → Tilføyer Lever → NVIDIA NIM:
   - API-nyckel: ` nvapi-din-nyckel`

**Modeller:** ` nvidia/llama-3.3-70b-instruct`, `nvidia/mistral-7b-instruct`, og
50+ flere

Pro Tipp: **Pro Tipp:** Compatible med OpenAI-api — fungerer smukt med OmniRutes
formatoversettelse!

### Dyb Søk

1. Tast inn: [platform.deepseek.com](https://platform.deepseek.com)
2. Få API-nøkkel
3. Oversikt → Legg til Leverandør → Dyb Søk

**Modeller:** `dyb-søkj/deepseek-chat`, `dyb-søkj/deepseek-coder`

### Groq (Erhvervspakke tilgjengelig!)

1. Tast inn: [console.groq.com](https://console.groq.com)
2. Få API-nøkkel (erhvervspakken inkludert)
3. Oversikt → Legg til Leverandør → Groq

**Modeller:** `groq/llama-3.3-70b`, `groq/mixtral-8x7b`

**Pro Tipp:** Ultra-rask innførsel — best for i realtid!

### Åpenruter (100+ Modeller)

1. Tast inn: [openrouter.ai](https://openrouter.ai)
2. Få API-nøkkel
3. Oversikt → Legg til Leverandør → Åpenruter

**Modeller:** Tilgang til 100+ modeller fra alle store leverandører ved hjelp av
en enkel API-nøkkel.

</details>

<details>
<summary><b>💰 Cheap Providers (Backup)</b></summary>

### GLM-4.7 (Daglig nulstilling, 0,6 $/1M)

1. Tast inn: [Zhipu AI](https://open.bigmodel.cn/)
2. Få API-nøkkel fra koding-planen
3. Værfratabell → Tilføy API-nøkkel:
   - Leiser: `glm`
   - API-nøkkel: `din-nøkkel`

**Bruk:** `glm/glm-4.7`

**Pro Tip:** Coding-plan tilbyr 3-ganger kvot uten forsinkelse hver 7ende dag!
Reset daglig 10.00.

### MiniMax M2.1 (5 timers reset, $0,20/1M)

1. Tilkoble: [MiniMax](https://www.minimax.io/)
2. Få API-nøkkel
3. Værfratabell → Tilføy API-nøkkel

**Bruk:** `minimax/MiniMax-M2.1`

**Pro Tip:** Det billigste alternativet for lange kontekster (1M tegn)!

### Kimi K2 ($9/måned flat)

1. Abonner: [Moonshot AI](https://platform.moonshot.ai/)
2. Få API-nøkkel
3. Værfratabell → Tilføy API-nøkkel

**Bruk:** `kimi/kimi-siste`

**Pro Tip:** Fast $9 måned for 10M tegn = $0,90/1M effektiv kost!

</details>

<details>
<summary><b>🆓 FREE Providers (Emergency Backup)</b></summary>

### iFlow (5 FRIE modeller via OAuth)

```bash
Værfratabell → Tilføyn iFlow
→ iFlow OAuth-innlogging
→ Upplært bruk

Modeller:
  if/kimi-k2-thinking
  if/qwen3-coder-plus
  if/glm-4.7
  if/minimax-m2
  if/deepseek-r1
```

### Qwen (4 FRIE modeller via Utstyrsbokskode)\

```bash
Verktøyfelt → Forbinde Qwen
→ Enhetskode autorisasjon
→ Uendelig bruk

Modeller:
  qw/qwen3-coder-plus
  qw/qwen3-coder-flash
```

### Kiro (Claude GRATIS)

```bash
Verktøyfelt → Forbinde Kiro
→ AWS-bygger ID eller Google/GitHub
→ Uendelig bruk

Modeller:
  kr/claude-sonnet-4.5
  kr/claude-haiku-4.5
```

</details>

<details>
<summary><b>🎨 Create Combos</b></summary>

### Eksempel 1: Maksimere Abonnement → Billig Reserve

```
Verktøyfelt → Kombinasjoner → Nytt
Navn: premium-tkoding
Modeller:
  1. cc/claude-opus-4-6 (Abonnements primæropdateringer)
  2. glm/glm-4.7 (Billig reserve, $0.6/1M)
  3. minimax/MiniMax-M2.1 (Cheapest fallback, $0.20/1M)

Bruk i CLI: premium-tkoding
```

### Eksempel 2: Innbetaling Fritt (Ingen Kostnad)

```
Navn: gratis-kombo
Modeller:
  1. gc/gemini-3-flash-forslag (180K fritt/måned)
  2. if/kimi-k2-gjennomtenking (uendelig)
  3. qw/qwen3-coder-plus (uendelig)

Kostnad: $0 fore evigt!
```

</details>

<details>
<summary><b>🔧 CLI Integration</b></summary>

### Markør IDE

```
Innstillinger → Modeller → Avansert:
  OpenAI API Base URL: http://localhost:20128/v1
  OpenAI API Key: [fra OmniRoute-dashboard]
  Model: cc/claude-opus-4-6
```

### Claude Code

Bruk **Verktøy CLI**-siden i verktøyfeltet for énklingskonsfigurasjon, eller
rediger `~/.claude/instillinger.json` manuelt.

### Codex CLI

```bash
eksport OPENAI_BASE_URL="http://localhost:20128"
eksport OPENAI_API_KEY="din-omniroute-api-nøkkel"

codex "din prompt"
```

### OpenKlaue

**Valg 1 — Verktøyfelt (anbefalt):**

```
Verktøyfelt → Verktøy CLI → OpenKlaue → Velg Model → Tilført
```

**Valg 2 — Manuelt:** Rediger `~/.openclaw/openclaw.json`:

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

> **Mer:** OpenKlaue fungerer kun lokalt ved OmniRoute. Bruk `127.0.0.1` i
> stedet av `localhost` for å unngå IPv6-resolusjonsproblemer.

### Kline / Fortsett / RooCode

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

## Feilsøking

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

- Sjekk brukerstatistikk i Startside → Utkostninger
- byt primærmodell til GLM/MiniMax
- Bruk gratis niveau (Gemini CLI, iFlow) for ikke-kritiske oppgaver

**Startside/API porter er feil**

- `PORT` er den kanoniske base porten (og API-porten som standard)
- `API_PORT` overstyres kun åbenne AI-kompatibel API-lister
- `DASHBOARD_PORT` overstyres kun dashboard/Next.js listener
- Sett `NEXT_PUBLIC_BASE_URL` til din startside/offentlige URL (for OAuth-oprop)

**Cloud synkronter feil**

- Verifiser `BASE_URL` peker til din kjørende instance
- Verifiser `CLOUD_URL` peker til din forventede sky-endepunkt
- Hold `NEXT_PUBLIC_*`-verdier i line med verdiene på server-siden

**Første innlogging ikke fungerer**

- Sjekk `INITIAL_PASSWORD` i `.env`
- Hvis udefinert, falt tilbake password er `123456`

**Ingen forespørslerlogg**

- Sett `ENABLE_REQUEST_LOGS=true` i `.env`

**Koblingstest viser "Ugyldig" for åpne AI-kompatible oppgaveskabere**

- Mange oppgaveskabere eksponerer ikke en `/modeller`-endepunkt
- OmniRoute v1.0.6+ inkluderer fallback-validering gjennom chattefullendinger
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

**4. Save and copy the credentials**

After creating, Google will show the **Client ID** and **Client Secret**.

**5. Set environment variables**

In your `.env` (or Docker environment variables):

```bash
# For Antigravity:
ANTIGRAVITY_OAUTH_CLIENT_ID=your-client-id.apps.googleusercontent.com
ANTIGRAVITY_OAUTH_CLIENT_SECRET=GOCSPX-your-secret

# For Gemini CLI:
GEMINI_OAUTH_CLIENT_ID=your-client-id.apps.googleusercontent.com
GEMINI_OAUTH_CLIENT_SECRET=GOCSPX-your-secret
GEMINI_CLI_OAUTH_CLIENT_SECRET=GOCSPX-your-secret
```

**6. Restart OmniRoute**

```bash
# npm:
npm run dev

# Docker:
docker restart omniroute
```

**7. Try connecting again**

Dashboard → Providers → Antigravity (or Gemini CLI) → OAuth

Google will now redirect correctly to `https://your-server.com/callback`.

---

#### Temporary workaround (without custom credentials)

If you don't want to set up your own credentials right now, you can still use
the **manual URL flow**:

1. OmniRoute opens the Google authorization URL
2. After authorizing, Google tries to redirect to `localhost` (which fails on
   the remote server)
3. **Copy the full URL** from your browser's address bar (even if the page
   doesn't load)
4. Paste that URL into the field shown in the OmniRoute connection modal
5. Click **"Connect"**

> This works because the authorization code in the URL is valid regardless of
> whether the redirect page loaded.

---

<details>
<summary><b>🇧🇷 Versão em Português</b></summary>

#### Por que o OAuth do Antigravity / Gemini CLI falha em servidores remotos?

Os provedores **Antigravity** e **Gemini CLI** usam **Google OAuth 2.0** para
autenticação. O Google exige que a `redirect_uri` usada no fluxo OAuth seja
**exatamente** uma das URIs pré-cadastradas no Google Cloud Console do
aplicativo.

As kredensialer OAuth integrert i OmniRoute er registrert **bare for
`localhost`**. Når du logger på OmniRoute på en fjernserver (f.eks.
`https://omniroute.mineventer.com`), avviser Google autentisering med:

```
Error 400: redirect_uri_mismatch
```

#### Løsning: Konfigurer egne kredensialer OAuth

Du må opprette et **OAuth 2.0 Client ID** på Google Cloud Console med URI til
din server.

#### Trinn-for-trinn

**1. Logg inn på Google Cloud Console**

Åpne:
[https://console.cloud.google.com/apis/credentials](https://console.cloud.google.com/apis/credentials)

**2. Opprett et nytt OAuth 2.0 Client ID**

- Klikk på **"+" Nye kredensialer"** → **"OAuth 2.0 Client ID**
- Applikasjontype: **"Web-applikasjon"**
- Navn: velg et navn (f.eks. `OmniRoute Remote`)

**3. Legg til Autoriserte Redirect URIs**

I feltet **"Autoriserte Redirect URIs"**, legg til:

```
https://din-server.com/callback
```

> Erstatt `din-server.com` med domenet eller IP-adressen til din server
> (innlemmende port dersom nødvendig, f.eks.
> `http://45.33.32.156:20128/callback`).

**4. Lagre og kopier kredensialene**

Etter å ha opprettet det, lar Google deg se **Client ID** og **Client Secret**.

**5. Konfigurer miljøvariablene**

På din `.env` (eller miljøvariablene til Docker):

```bash
# For Antigravity:
ANTIGRAVITY_OAUTH_CLIENT_ID=din-client-id.apps.googleusercontent.com
ANTIGRAVITY_OAUTH_CLIENT_SECRET=GOCSPX-din-hemmelig

# For Gemini CLI:
GEMINI_OAUTH_CLIENT_ID=din-client-id.apps.googleusercontent.com
GEMINI_OAUTH_CLIENT_SECRET=GOCSPX-din-hemmelighet
GEMINI_CLI_OAUTH_CLIENT_SECRET=GOCSPX-din-hemmelighet
```

**6. Start omnirotten omniRoute omni[]

```bash
# Hvis du bruker npm:
npm run dev

# Hvis du bruker Docker:
docker restart omniroute
```

**7. Få prøvd igjen**

Oversikt → Leverandører → Antigravity (eller Gemini CLI) → OAuth

Nå vil Google korrekt omdirige til `https://din-server.com/callback` og
autentisering vil fungere.

---

#### Midlertidig arbeidskring (uten å bruke egne kredenssial)

Hvis du ikke vil bli skapt egne kredenssial nå, kan du fremdeles bruke
omflytningsveien **håndbok for URL**:

1. OmniRoute åpner URL for autorisasjon fra Google
2. Etter å ha gitt tillatelse, prøver Google å omdirige til `localhost` (som
   mangler på fjernserver)
3. **kopier hele URL'en fra din nettleser adresselinje**
4. Skriv inn denne URLen i feltet i innkoneksjonsmodalen i OmniRoute
5. Klikk på **"Koble til"**

> Dette midlertidige løsningen fungerer fordi kode i autorisasjonsadresse i
> URL'en er gyldig selv om omdirigeringen ikke lastet eller ikke.

</details>

---

</details>

## 🛠️ Teknologi

<details>
<summary><b>Click to expand tech stack details</b></summary>

- **Kjøringstid**: Node.js 18–22 LTS (⚠️ Node.js 24+ er **ikke støttet** — `
  bedre-sqlite3` native binaries er kompatibelt)
- **Språket**: TypeScript 5.9 — **100% TypeScript** i `src/` og ` åpenne sse/`
  (siden v2.0 ingen `tull` i kjerne moduler)
- **Rammeverk**: Next.js 16 + React 19 + Tailwind CSS 4
- **Databasen**: LowDB (JSON) + SQLite (domein-tilstandet+ proxy-logge +
  MCP-audit + rutevalg)
- **Schemas**: Zod (MCP-verktøy for I/verifikasjon, API-kontrakter)
- **Protokollen**: MCP (stdio/HTTP) + A2A v0.3 (JSON-RPC 2.0 + SSE)
- Strømminne**Strømminne**: Server-Sent Events (SSE)
- **Autentisering**: OAuth 2.0 (PKCE) + JWT + API Keys + MCP Tilgangsbegrenser
- **TESTERING**: Node.js test runner + Vitest (900+ tester, inkl. enhetstester,
  integrasjonstester, E2E tester)
- ** CI/CD**: GitHub Actions (auto npm publiser + Docker Hub ved utgivelse)
- **Hjemmeside**: [omniroute.online](https://omniroute.online)
- **Pakke**:
  [npmjs.com/package/omniroute](https://www.npmjs.com/package/omniroute)
- **Docker**:
  [hub.docker.com/r/diegosouzapw/omniroute](https://hub.docker.com/r/diegosouzapw/omniroute)
- **Resilletighet**: Kretskommer, eksponentialt nødling, mot-herde,
  TLS-imitasjon, auto-kombo selv-gjenopprettelse

</details>

---

## Dokumentasjon

| Dokumentere                                    | Beskrivelse                                                       |
| ---------------------------------------------- | ----------------------------------------------------------------- |
| [Brukerguide](docs/USER_GUIDE.md)              | Giver, kombinasjoner, CLI-integrering, deployment                 |
| [API-referanse](docs/API_REFERENCE.md)         | Alle slutener med eksempler                                       |
| [MCP-SERVER](open-sse/mcp-server/README.md)    | 16 MCP-verktøy, IDÉ-konfigurasjoner, Python/TS/Go-klienter        |
| [A2A-SERVER](src/lib/a2a/README.md)            | JSON-RPC 2.0-protokoll, ferdigheter, strømming, oppgavehåndtering |
| [AUTO-KOMBO-MOTOR](docs/auto-combo.md)         | 6-faktorskjønnsmåling, modupakker, selv-fornyende                 |
| [Troubleshutting](docs/TROUBLESHOOTING.md)     | Vanlige problemer og løsninger                                    |
| [Arkitektur](docs/ARCHITECTURE.md)             | Systemarkitektur og interne detaljer                              |
| [Contributing](CONTRIBUTING.md)                | Utviklingssetting og retningslinjer                               |
| [OpenAPI Spec](docs/openapi.yaml)              | OpenAPI 3.0-spesifikasjon                                         |
| [Security Policy](SECURITY.md)                 | Sårbarhetsrapportering og sikkerhetspraksis                       |
| [VM Deployment](docs/VM_DEPLOYMENT_GUIDE.md)   | Fullstendig guide: VM + nginx + Cloudflare-setup                  |
| [Features Gallery](docs/FEATURES.md)           | Visualiserende tur gjennom skjermen med skjermbilder              |
| [Release Checklist](docs/RELEASE_CHECKLIST.md) | Foreløpig valideringsgrenger før utgivelse                        |

---

## 🗺️ Veitabell

OmniRoute har **210+ funksjoner planlagt** over flere utviklingsfaser. Her er de
viktigste områdene:

| Kategori                     | Planned Features | Highlights                                                                             |
| ---------------------------- | ---------------- | -------------------------------------------------------------------------------------- |
| 🧠 **Routing & Intelligence** | 25+              | Lowest-latency routing, tag-based routing, quota preflight, P2C account selection      |
| 🔒 **Security & Compliance**  | 20+              | SSRF hardening, credential cloaking, rate-limit per endpoint, management key scoping   |
| 📊 **Observability**          | 15+              | OpenTelemetry integration, real-time quota monitoring, cost tracking per model         |
| 🔄 **Provider Integrations**  | 20+              | Dynamic model registry, provider cooldowns, multi-account Codex, Copilot quota parsing |
| ⚡ **Performance**            | 15+              | Dual cache layer, prompt cache, response cache, streaming keepalive, batch API         |
| 🌐 **Ecosystem**              | 10+              | WebSocket API, config hot-reload, distributed config store, commercial mode            |

### 🔜 Coming Soon

- 🔗 **OpenCode Integration** — Native provider support for the OpenCode AI
  coding IDE
- 🔗 **INTEGRERING med TRAE** — Fulle støtte for TRAE- AI-utviklingsrammen
- 📦 **MELDINGER-API** — Asynkron måte for å behandle bulk-opplysninger
- 🎯 **MERKE-BASERT RUTERING** — Retningslinjer til å rette forespørsler på basis
  av eget merke og metadata
- 💰 **Laveste-kostnad-STRATEGI** — Automatiske velg den billigste tilgjengelige
  leverandør

> 📝 Fullførte funksjonsbeskrivelser tilgjengelig i [`dok/de nye
> funksjonene/`](docs/new-features/) (217 detaljerte beskrivelser)

---

## 👥 Medvirkende

[![Medvirkende](https://contrib.rocks/image?repo=diegosouzapw/OmniRoute&max=100&columns=20&anon=1)](https://github.com/diegosouzapw/OmniRoute/graphs/contributors)

### Hva er nødvendig for å bidra

1. Kopier prosjektet (Fork)
2. Opprett din egen branch ( `git checkout -b feature/amazing-feature` )
3. Legg til forskjell mot version ( `git commit -m 'Legg til enstemmig funksjon
   `' )
4. Sender branch til opphavskilden ( `git push origin feature/amazing-feature` )
5. Åpne et pull-krav

Se [CONTRIBUTING.md](CONTRIBUTING.md) for detaljerte retningslinjer.

### Publiser en Ny Versionsnummer

```bash
# Opprett en ny versjon - npm publiser skjer automatisk
gh release create v2.0.0 --tile "v2.0.0" --generate-notes
```

---

## 📊 Stjernehistorikk

## Stjernere over tid

## [![Stjernere over tid](https://starchart.cc/diegosouzapw/OmniRoute.svg?variant=adaptive)](https://starchart.cc/diegosouzapw/OmniRoute)

## 🙏 Tilhørigheter

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
