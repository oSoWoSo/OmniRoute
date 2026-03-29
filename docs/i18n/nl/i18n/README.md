# 🚀 OmniRoute — De Vrije AI Gateway

### Stop nooit met coderen. Slimme routering naar **VRIJE EN LAGE-KOSTENDE AI-modellen**-met automatische fallback.

_Uw universele API-proxy — één eindpunt, 67+ providers, geen downtime. Nu met
**MCP & A2A** agent-orchestration._

**Chat Completions • Embeddings • Afbeeldinggeneratie • Video • Muziek • Audio •
Reranking • **Web Zoeken** • MCP Server • A2A Protocol • 100% TypeScript**

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
[![Licentie](https://img.shields.io/github/license/diegosouzapw/OmniRoute)](https://github.com/diegosouzapw/OmniRoute/blob/main/LICENSE)
[![Website](https://img.shields.io/badge/Website-omniroute.online-blue?logo=google-chrome&logoColor=white)](https://omniroute.online)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-Community-25D366?logo=whatsapp&logoColor=white)](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

[🌐 Website](https://omniroute.online) • [🚀 Quick Start](#-quick-start) • [💡
Features](#-key-features) • [📖 Documentatie](#-documentation) • [💰
Prijzen](#-pricing-at-a-glance) • [💬
WhatsApp](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

</div>

🌐 **Beschikbaar in:** 🇺🇸 [Engels](README.md) | 🇧🇷 [Portugees
(Brasil)](docs/i18n/pt-BR/README.md) | 🇪🇸 [Spaans](docs/i18n/es/README.md) | 🇫🇷
[Frans](docs/i18n/fr/README.md) | 🇮🇹 [Italiaans](docs/i18n/it/README.md) | 🇷🇺
[Russisch](docs/i18n/ru/README.md) | 🇨🇳 [Hanzi
(vereenvoudigd)](docs/i18n/zh-CN/README.md) | 🇩🇪 [Duits](docs/i18n/de/README.md)
| 🇮🇳 [Hindi](docs/i18n/in/README.md) | 🇹🇭 [Thai](docs/i18n/th/README.md) | 🇺🇦
[Oekraïens](docs/i18n/uk-UA/README.md) | 🇸🇦 [Arabisch](docs/i18n/ar/README.md) |
🇯🇵 [Japannees](docs/i18n/ja/README.md) | 🇻🇳 [Vietnamees](docs/i18n/vi/README.md)
| 🇧🇬 [Bulgaars](docs/i18n/bg/README.md) | 🇩🇰 [Deens](docs/i18n/da/README.md) |
🇫🇮 [Fins](docs/i18n/fi/README.md) | 🇮🇱 [Hebreeuws](docs/i18n/he/README.md) | 🇭🇺
[Hongaars](docs/i18n/hu/README.md) | 🇮🇩 [Indonesisch](docs/i18n/id/README.md) |
🇰🇷 [Koreaans](docs/i18n/ko/README.md) | 🇲🇾 [Maleis](docs/i18n/ms/README.md) | 🇳🇱
[Nederlands](docs/i18n/nl/README.md) | 🇳🇴 [Noors](docs/i18n/no/README.md) | 🇵🇹
[Portugees (Portugal)](docs/i18n/pt/README.md) | 🇷🇴
[Roemeens](docs/i18n/ro/README.md) | 🇵🇱 [Pools](docs/i18n/pl/README.md) | 🇸🇰
[Sloveens](docs/i18n/sk/README.md) | 🇸🇪 [Zweeds](docs/i18n/sv/README.md) | 🇵🇭
[Filipino](docs/i18n/phi/README.md) | 🇨🇿 [Tsjechisch](docs/i18n/cs/README.md)

---

## 🆕 Wat is nieuw in v3.0.0

> **Upgraden vanuit v2.9.5?** — Zie de [volledige
> CHANGELOG](CHANGELOG.md#300--2026-03-22-release-candidate--not-yet-merged-to-main)
> voor alle wijzigingen.

| Area                              | Verandering                                                                                                                                                                               |
| --------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🔒 **CodeQL Beveiliging**          | 10+ CodeQL waarschuwingen aangepast: polynomial-redos, onveilige randomiteit, schelp-injectie remediatie                                                                                  |
| ✅ **Route Validatie**             | Alle 176 API-routes nu gevalideerd met Zod-schemas + `validateBody()`-— CI `check:route-validation:t06` slaagt                                                                            |
| 🐛 **omniModel Etiket Leak**       | Interne `<omnimodel>`-etiketten komen niet meer naar buiten in SSE-streaming-antwoorden (#585)</omnimodel>                                                                                |
| 🔑 **Geregistreerde SLEUTELS API** | Automatische registratie van API-sleutels via `POST /api/v1/registered-keys`-met per-provider/account quota-handhaving, idempotentie, SHA-256-opslag en optionele GitHub-issue-rapportage |
| 🎨 **Provider Iconen**             | 130+ provider logo's via `@lobehub/icons` (SVG) met PNG → algemene fallback keten                                                                                                         |
| 🔄 **Model Auto-Sync**             | 24uurs planner en handmatige UI-togge om modellijsten synchroon te maken voor ingebouwde en aangepaste OpenAI-gecompatibele leveranciers                                                  |
| 🌐 **OpenCode Zen/Go**             | Twee nieuwe leveranciers van @kang-heewon via pull-request #530: GRATIS laag + abonnementslaag via `OpencodeExecutor`                                                                     |
| 🐛 **Gemini CLI OAuth**            | Handgreep op fout bij `GEMINI_OAUTH_CLIENT_SECRET` is ontbreekt in Docker (was cryptische Google fout)                                                                                    |
| 🐛 **OpenCode configuratie**       | `saveOpenCodeConfig()` schrijft nu correct TOML in `XDG_CONFIG_HOME`                                                                                                                      |
| 🐛 **Pinned model override**       | `body.model` wordt nu correct ingesteld op `pinnedModel` bij context-cache bescherming                                                                                                    |
| 🐛 **Codex/Claude loop**           | `tool_result` blokken worden nu omgezet naar tekst om oneindige lussen te voorkomen                                                                                                       |
| 🐛 **Login redirect**              | Login wordt niet meer vastgeklemd nadat het wachtwoord instellen is oversprongen                                                                                                          |
| 🐛 **Windows paden**               | MSYS2/Git-Bash paden (`/c/...`) worden geautomatiseerd omgezette naar `C:\...`                                                                                                            |

---

## 🖼️ HoofdDashboard

<div align="center">
  <img src="./docs/screenshots/MainOmniRoute.png" alt="OmniRoute Dashboard" width="800"/>
</div>

---

## 📸 Dashboard Preview

<details>
<summary><b>Click to see dashboard screenshots</b></summary>

| Pagina            | Scherm afbeelding                                 |
| ----------------- | ------------------------------------------------- |
| **Provideren**    | ![Provideren](docs/screenshots/01-providers.png)  |
| **Combos**        | ![Combos](docs/screenshots/02-combos.png)         |
| **Analytics**     | ![Analytics](docs/screenshots/03-analytics.png)   |
| **Gezondheid**    | ![Gezondheid](docs/screenshots/04-health.png)     |
| **Vertaler**      | ![Vertaler](docs/screenshots/05-translator.png)   |
| **Instellingen**  | ![Instellingen](docs/screenshots/06-settings.png) |
| **CLI-tools**     | ![CLI-tools](docs/screenshots/07-cli-tools.png)   |
| **Gebruiks logs** | ![Gebruik](docs/screenshots/08-usage.png)         |
| **Eindpunten**    | ![Eindpunten](docs/screenshots/09-endpoint.png)   |

</details>

---

### 🤖 Gratis AI-provider voor je favoriete coderingsagenten.

_Verbind elke AI-bevoegde IDE of CLI-tool met OmniRoute — gratis API-gateway
voor onbeperkt coden._

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

<sub>📡 Alle agents connecteren via <code>http://localhost:20128/v1</code> of
<code>http://cloud.omniroute.online/v1</code> — één configuratie, onbeperkte
model en quota</sub>

---

## 🤔 Waarom OmniRoute?

** Stop geld verspillen en limieten raken:**

- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Abonnementsquota loopt iedere maand niet af
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Limieten stoppen je in het midden terwijl je aan het coderen bent
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Duurdere APIs ($20-50 per maand per provider)
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Manuele schakeling tussen providers

**OmniRoute lost dit op:**

- ✅ **Maximaliseer abonnementen** - volg quota, gebruik elke bit vóór reset
- ✅ **Auto-fallback** - Abonnement → API-sleutel → Duurzaam → Gratis, zero
  downtime
- ✅ **Meerdere account** - Rondrobin tussen accounts per provider
- ✅ **Universaal** - Werkt met Claude Code, Codex, Gemini CLI, Cursor, Cline,
  OpenClaw, elke CLI-tool

---

## 📧 Ondersteuning

> 💬 **Sluit je aan bij onze gemeenschap!** [WhatsApp
> Group](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t) — Krijg
> hulp, deel tips, en blijf op de hoogte.

- **Website**: [omniroute.online](https://omniroute.online)
- **GitHub**:
  [github.com/diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute)
- **Issues**:
  [github.com/diegosouzapw/OmniRoute/issues](https://github.com/diegosouzapw/OmniRoute/issues)
- **WhatsApp**: [Community
  Group](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)
- **Contribueren**: Kijk naar [CONTRIBUTING.md](CONTRIBUTING.md), open een PR,
  of kies een `goede eerste issue`
- **Oorspronkelijke Project**: [9router by
  decolua](https://github.com/decolua/9router)

### 🐛  Een foutmelding melden?

Wanneer u een issue aanmaakt, voert u het commando system-info uit en plakt u de
gegenereerde bestand bij:

```bash
npm run system-info
```

Dit gegenereert een `system-info.txt` met uw Node.js-versie, OmniRoute-versie,
OS-details, geïnstalleerde CLI-tool (iflow, gemini, claude, codex, antigravity,
droid, etc.), status Docker/PM2, en systeempakketten — alles wat we nodig hebben
om uw issue snel te reproduceren. Plak het bestand rechtstreeks bij uw
GitHub-issue.

---

## Hoe het werkt

```
┌─────────────┐
│  Uw CLI-    │  (Claude Code, Codex, Gemini CLI, OpenClaw, Cursor, Cline...)
│   hulpprogramma│
└──────┬──────┘
       │ http://localhost:20128/v1
       ↓
┌─────────────────────────────────────────┐
│           OmniRoute (Slimme Router)        │
│  • Vertaling van formaten (OpenAI ↔ Claude) │
│  • Quotatracking + Embeddings + Beelden │
│  • Automatische tokenvernieuwing         │
└──────┬──────────────────────────────────┘
       │
       ├─→ [Tier 1: ABONNEMENT] Claude Code, Codex, Gemini CLI
       │   ↓ quota verbruikt
       ├─→ [Tier 2: API-TOETSEN] DeepSeek, Groq, xAI, Mistral, NVIDIA NIM, etc.
       │   ↓ budget limiet
       ├─→ [Tier 3: CHEAP] GLM ($0.6/1M), MiniMax ($0.2/1M)
       │   ↓ budget limiet
       └─→ [Tier 4: GRATIS] iFlow, Qwen, Kiro (oneindig)

Resultaat: Nooit meer coderen, minimal kosten
```

---

## 🎯 Wat OmniRoute oplost — 30 Reële Pijnpunten & Toepassingsgevallen

> **Iedere ontwikkelaar die AI-hulpmiddelen gebruikt, stoot iedere dag op deze
> problemen.** OmniRoute is ontwikkeld om ze allemaal op te lossen — van
> kostenoverschotten tot regionale blokkades, van gebroken OAuth-stromen tot
> protocoloperaties en bedrijfsobservatie.

<details>
<summary><b>💸 1. "I pay for an expensive subscription but still get interrupted by limits"</b></summary>

Ontwikkelaars betalen $20–200 per maand voor Claude Pro, Codex Pro of GitHub
Copilot. Zelfs als ze betalen, heeft quota een plafond — 5 uur gebruik,
wekelijkse limieten of per-minuut limieten. Midden in een coderingsessie stopt
de provider reacties op te geven en verliest de ontwikkelaar vloei en
productiviteit.

**Hoe OmniRoute het oplost:**

- **Slimme 4-Tier Fallback** — Als abonnementsquota op is, wordt automatisch
  omgezet naar API-Toets → Cheap → Free zonder tussenkomst
- **Real-Time Quota Tracking** — Toont tokenverbruik in real-time met
  reset-uurlijk (5 uur, dagelijks, wekelijks)
- **Multi-Account Ondersteuning** — Meerdere accounts per provider met
  automatische rond-robin — wanneer één op is, wordt omgeschakeld naar de
  volgende
- **Custom Combos** — Aanpassbare fallbackketens met 6 evenwichtsx strategieën
  (vul-eerst, rond-robin, P2C, willekeurig, minst-gebruikt,
  kost-geoptimaliseerd)
- **Codex Business Quotas** — Business/Team-arbeidsomgevingsquota op basis van
  bedrijf/-team in de dashboard

</details>

<details>
<summary><b>🔌 2. "I need to use multiple providers but each has a different API"</b></summary>

OpenAI gebruikt één formaat, Claude (Anthropic) een ander, Gemini weer een
ander. Als een dev-modellen van verschillende providers of fallbacks tussen hen
wil testen, moeten ze SDK's aanpassen, endpoints veranderen, rekening houden met
onverenigbare formats. Eigen providers (FriendLI, NIM) hebben geen standaard
modelpointers.

**Hoe OmniRoute het oplost:**

- **Unified Endpoint** — Een enkel `http://localhost:20128/v1` serveert als
  proxy voor alle +67 providers
- **Format Vertaling** — Automatisch en opmerkelijk: OpenAI ↔ Claude ↔ Gemini ↔
  Respons-API
- **Reageerbasischering** — Strips non-standaards velden (`x_groq`,
  `usage_breakdown`, `service_tier`) die niet OpenAI SDK v1.83+ respecteren
- **Rol Normalisatie** — Verander[d]`ontwikkelaar` → `systeem` voor
  niet-OpenAI-pakketten; `systeem` → `gebruiker` voor GLM/ERNIE
- **Think-blokken Uitpluizen** — Uitpluist `<think>`-blokken van modellen zoals
  DeepSeek R1 in gestandaardiseerde `redeneringsinhoud`</think>
- **Gestructureerde Uitvoer voor Gemini** — `json_schema` →
  `responseMimeType`/`responseSchema` automatisch converteren
- **`stream` staat standaard op `false`** — Aanstip in OpenAI-schethtels, wat
  onverwachte SSE in Python/Rust/Go SDK's voorkomt

</details>

<details>
<summary><b>🌐 3. "My AI provider blocks my region/country"</b></summary>

OpenAI/Codex heeft toegang tot bepaalde landen/nationale gebieden geblokkeerd.
Gebruikers krijgen foutenmeldingen zoals `unsupported_country_region_territory`
tijdens OAuth-verificatie en API-verbindingen. Dit is vooral frustrerend voor
ontwikkelaars uit ontwikkelende landen

**Hoe OmniRoute het oplost:**

- **3-Level Proxy Config** — Confiabele proxy op 3 niveaus: globaal (alle
  verkeer), per-provider (één provider alleen) en per-verbinding/sleutel
- **Kleurcoderde Proxy Badges** — Visuele indicatoren: 🟢 globaal proxy, 🟡
  provider proxy, 🔵 verbinding proxy; IP-adres altijd weergeven
- **OAuth Toestemming Uitwisseling Via Proxy** — OAuth-procedure gaat ook via de
  proxy doorheen, oplossing voor `unsupported_country_region_territory`
- **Verbindingstests Via Proxy** — Verbindingstests maken gebruik van de
  geconfigureerde proxy (geen directe omleiding meer)
- **SOCKS5- Ondersteuning** — Volledige SOCKS5-proxy ondersteuning voor uitgaand
  verkeer
- **TLS-Vingerafdruk Spoelen** — Browser-achtige TLS-vingerafdruk via `wreq-js`
  om botsdetectie te omzeilen
- **CLI Vingerafdruk Matchen** — Ordenen van headers en lichaamsvelden om native
  CLI-bestandsignatuur te matchen, waardoor het risico van accountindicatie
  aanzienlijk vermindert

</details>

<details>
<summary><b>🆓 4. "I want to use AI for coding but I have no money"</b></summary>

Niet iedereen kan $20–200 per maand betalen voor AI-abonnementen. Studenten,
ontwikkelaars uit opkomende landen, hobbyisten en freelancers hebben toegang tot
kwalitatieve modellen nodig zonder kosten

**Hoe OmniRoute het oplost:**

- **Gebouwde-In Providers voor Free- Tier** — Natieve ondersteuning voor 100%
  gratis providers: iFlow (5 oneindige modellen via OAuth: kimi-k2-thinking,
  qwen3-coder-plus, deepseek-r1, minimax-m2, kimi-k2), Qwen (4 oneindige
  modellen: qwen3-coder-plus, qwen3-coder-flash, qwen3-coder-nach, visie-model),
  Kiro (Claude + AWS Bouwblokkenspecificatie voor gratis), Gemini CLI (180K
  token per maand gratis)
- **Ollama Cloud** — Ollama-modellen gehostd op `api.ollama.com` vrij "Light
  Usage"-schetsel; gebruik `ollamacloud/<model>` voorsyteem</model>
- **Combinaties voor Free- Tier** — Chain `gc/gemini-3-flash →
  if/kimi-k2-thinking → qw/qwen3-coder-plus` = $0 per maand met geen
  onderbrekingen
- **NVIDIA NIM Vrij Toegangen** — ~40 RPM dev-forever gratis toegang tot 70+
  modellen op build.nvidia.com (overgang van creditlimieten naar pure
  waarderingssluitingen)
- **Geoptimaliseerde Strategie** — Routering strategy die automatisch de
  goedkoopste beschikbare provider kiest

</details>

<details>
<summary><b>🔒 5. "I need to protect my AI gateway from unauthorized access"</b></summary>

Wanneer een AI-gateway wordt uitgezet op het netwerk (LAN, VPS, Docker), kan
iedereen met de adres toegang krijgen tot de tokens/de quota van de
ontwikkelaar. Zonder bescherming zijn APIs kwetsbaar voor misbruik,
prompt-injectie en misbruik.

**Hoe OmniRoute het oplost:**

- **API Sleutelbeheer** — Generatie, rotatie en scope per provider met een
  aparte `/dashboard/api-manager` pagina
- **Modelniveau-toestemmingen** — API-sleutels beperken tot specifieke modellen
  (`openai/*`, wildcards), met toets "toestaan alles/uitsluiten"
- **Bescherming van API-eindpunten** — Vereist een sleutel voor `/v1/models` en
  block specifieke providers van de lijst
- **Auth Guard + CSRF Bescherming** — Alle dashboard routes beschermd met
  `withAuth` middleware + CSRF-tokens
- **Snelheidsbeperking** — Per-IP snelheidsbeperking met configurabele vensters
- **IP-filtering** — Allowlist/blocklist voor toegangscontrole
- **Prompt-injectieguard** — Reinhouding tegen kwetsbare prompt-patterns
- **AES-256-GCM-Encryptie** — Gegevens versleuteld op de schijf

</details>

<details>
<summary><b>🛑 6. "My provider went down and I lost my coding flow"</b></summary>

AI-providers kunnen instabiel zijn, 5xxfouten retourneren, of tijdelijke
snelheidsbeperkingen hebben. Als een ontwikkelaar afhankelijk is van één
provider, worden ze onderbroken. Zonder circuitbreakers worden herhalingse
pogingen de applicatie tot een instortingen kunnen brengen.

**Hoe OmniRoute het oplost:**

- **Circuit Breaker per-model** — Auto-open/close met configurabele drempels en
  cooldown (Geclosed/Geopend/Half-gesloten), gestroomlijnd per-model om
  blokkeringen te voorkomen
- **Exponentiele Backoff** — Progressieve vertraging van herhalingen
- **Anti-Thundering Herd** — Mutex + semafoorbescherming tegen concurrerende
  herhalingsspecials
- **Combinatie Failoverketen** — Als de primaire provider faalt, valt af
  automatisch met de keten zonder tussenkomst
- **Combinatie Circuit Breaker** — Autodisables falende providers binnen een
  combinatieketen
- **Verbindingsstatusscherm** — Uptime-metrieken, circuitbreaker-status,
  uitschakelingen, cachestatistieken, p50/p95/p99 latentietijden

</details>

<details>
<summary><b>🔧 7. "Configuring each AI tool is tedious and repetitive"</b></summary>

Ontwikkelaars gebruiken Cursor, Claude Code, Codex CLI, OpenClaw, Gemini CLI,
Kilo Code... Elke tool heeft een andere configuratie (API-einde punt, sleutel,
model). Het opnieuw configureren als tussen aanbieders of modellen wordt
verdaagd is een verspilling van tijd.

**Hoe OmniRoute het oplost:**

- ** CLI-Tools Dashboard ** - Gedeschilderde pagina met één-klik setup voor
  Claude Code, Codex CLI, OpenClaw, Kilo Code, Antigravity, Cline
- ** GitHub Copilot Config Generator ** - Maakt ` chatLanguageModels.json ` aan
  voor VS Code met bulk model selectie
- ** Onboarding Wizard ** - Gidsde 4-stappen inrichting voor nieuwe gebruikers
- ** Eén endpoint, al model ** - Configureer ` http://localhost:20128/v1 ` een
  keer, en toegang tot 67+ providers

</details>

<details>
<summary><b>🔑 8. "Managing OAuth tokens from multiple providers is hell"</b></summary>

Claude Code, Codex, Gemini CLI, Copilot — allemaal gebruiken OAuth 2.0 met
verlopende tokens. Ontwikkelaars moeten zich constant opnieuw aanmelden, hebben
last van ` client_secret is missing `, ` redirect_uri_mismatch ` en failures op
afstandse servers. OAuth op LAN/VPS is zeer problematic.

**Hoe OmniRoute het oplost:**

- ** Auto-token Refresh ** - OAuth tokens vernieuwen in de achtergrond voordat
  deze verlopen
- ** OAuth 2.0 (PKCE) Built-in ** - Automatische flow voor Claude Code, Codex,
  Gemini CLI, Copilot, Kiro, Qwen, iFlow
- ** Multi-Account OAuth ** - Meerdere accounts per provider via JWT/ID token
  extractie
- ** OAuth LAN/Remote Fix ** - Privé IP detectie voor ` redirect_uri ` +
  handmatige URL modus voor afstandse servers
- ** OAuth Behind Nginx ** - Gebruikt ` window.location.origin ` voor reverse
  proxy compatibiliteit
- ** Remote OAuth Guide ** - stap-voor-stap gids voor Google Cloud credentials
  op VPS/Docker

</details>

<details>
<summary><b>📊 9. "I don't know how much I'm spending or where"</b></summary>

Ontwikkelaars gebruiken meerdere betaalde providers maar hebben geen
geïntegreerde weergave van uitgaven. Elke provider heeft zijn eigen factuur
dashboard, maar er is geen geconsolideerde weergave. Onverwachte kosten kunnen
opstapelen.

**Hoe OmniRoute het oplost:**

- ** Cost Analytics Dashboard ** - Kostenanalyse per token en budgetbeheer per
  provider
- ** Budget Limiet per Trimester ** - Uitgavengrens per trimester die
  automatisch valt achterwege
- ** Per-Model Pricing Configuratie ** - Configureerbare prijzen per model
- ** Gebruikersstatistieken per API Sleutel ** - Aantal aanvragen en datum van
  laatste gebruik per sleutel
- ** Analytics Dashboard ** - Statische kaarten, modelgebruik chart,
  providerlijst met succespercentages en latentie

</details>

<details>
<summary><b>🐛 10. "I can't diagnose errors and problems in AI calls"</b></summary>

Ongelukkige aanroepen laten de ontwikkelaar niet weten of het door
rate-limiting, een verlopen token, een verkeerde indeling of een
leveranciersfout kwam. Geschakeerde logboeken over verschillende terminals.
Zonder observabiliteit is debuggen een trial-and-error proces.

**Hoe OmniRoute het oplost:**

- **Integrated Logs Dashboard** — 4 tabs: Verzoek Logboeken, Proxy Logboeken,
  Audit Logboeken, Console
- **Console Log Viewer** — Real-time terminal-stijl weergave met
  kleurengecodeerde niveaus, automatisch scrollen, zoeken, filteren
- **SQLite Proxy Logboeken** — Persistente logboeken die server-restarten
  overleven
- **Translator Playground** — 4 debbugingsmodi: Playground (formaatvertaling),
  Chat Tester (ronde-weg), Test Bench (groeps), Live Monitor (real-time)
- **Verzoek Telemetrie** — p50/p95/p99 vertraging + X-Verzoek-Id traceren
- **Bestands gebaseerde Loggen met Rotatie** — Console-interceptorcaptureert
  alles naar JSON log met op maat gemaakte rotatie
- **Systeeminformatie Rapport** — `npm run system-info` genereert
  `system-info.txt` met uw volledige omgeving (Node-versie, OmniRoute-versie,
  OS, CLI- tools, Docker /PM2-status). Plaats het bij het melden van problemen
  voor instant triage.

</details>

<details>
<summary><b>🏗️ 11. "Deploying and maintaining the gateway is complex"</b></summary>

Het installeren, configureren en onderhouden van een AI-proxy over verschillende
omgevingen (lokaal, VPS, Docker, cloud) is arbeidsintensief. Problemen zoals
vastgelegde paden, `EACCES` in mappen, poortconflicten en cross-platform
bouwsommen frictie toevoegen.

**Hoe OmniRoute het oplost:**

- **npm globale installeren** — `npm install -g omniroute &amp;&amp; omniroute`
  — klaar
- **Docker Multi-Platform** — AMD64 + ARM64 native (Apple Silicon, AWS Graviton,
  Raspberry Pi)
- **Docker Compose Profielen** — `basis` (geen CLI-hulpmiddelen) en `CLI` (met
  Claude Code, Codex, OpenClaw)
- **Electron Desktop App** — Natieve app voor Windows /macOS /Linux met
  systeemschijf, automatische start, offline-modus
- **Gesplitste-Port Modus** — API en Dashboard op aparte poorten voor
  geavanceerde scenario's (omgekeerde proxy, container-netwerken)
- **Cloud Sync** — Confiuguratie syncronisatie over apparaten via Cloudflare
  Workers
- **Database Backups** — Automatisch backup, herstellen, exporteren en
  importeren van alle instellingen

</details>

<details>
<summary><b>🌍 12. "The interface is English-only and my team doesn't speak English"</b></summary>

Teams in niet-Angelsprekende landen, vooral in Latijns-Amerika, Azië en Europa,
worstelen met Engelstalige interfaces. Taalbarrières verlagen de adoptie en
verhogen de configuratiefouten.

**Hoe OmniRoute het oplost:**

- **Dashboard i18n — 30 talen** — Alle 500+ sleutels getranslateerd, inclusief
  Arabisch, Bulgaars, Deens, Duits, Spaans, Fins, Frans, Hebreeuws, Hindi,
  Hongaars, Indonesisch, Italiaans, Japans, Koreaans, Maleis, Nederlands, Noors,
  Pools, Portugees (PT/BR), Roemeens, Russisch, Slovaaks, Zweeds, Thais,
  Oekraïens, Vietnamees, Chinees, Filipijns, Engels
- **RTL-ondersteuning** — Rechts-naar-links-ondersteuning voor Arabisch en
  Hebreeuws
- **Meertalig READMEs** — 30 complete documentatievertalingen
- **Taalselectie** — Wereldmapicoon in header voor real-time doorwijk

</details>

<details>
<summary><b>🔄 13. "I need more than chat — I need embeddings, images, audio"</b></summary>

AI is niet enkel chatcompletering. Devs moeten afbeeldingen genereren,
geluidsopnames transcriberen, embeddings maken voor RAG, documenten doorhalen,
en inhoud modereren. Elke API heeft een verschillend eindpunt en format.

**Hoe OmniRoute het oplost:**

- **Embeddings** — `/v1/embeddings` met 6 providers en 9+ modellen
- **Afbeelding** — `/v1/images/generations` met 10 providers en 20+ modellen
  (OpenAI, xAI, Together, Fireworks, Nebius, Hyperbolic, NanoBanana,
  Antigravity, SD WebUI, ComfyUI)
- **Tekst-naar-Video** — `/v1/videos/generations` — ComfyUI (AnimateDiff, SVD)
  en SD WebUI
- **Tekst-naar-Muziek** — `/v1/music/generations` — ComfyUI (Stable Audio Open,
  MusicGen)
- **Audio-Transcriptie** — `/v1/audio/transcriptions` — Whisper + Nvidia NIM,
  HuggingFace, Qwen3
- **Tekst-naar-Spraak** — `/v1/audio/speech` — ElevenLabs, Nvidia NIM,
  HuggingFace, Coqui, Tortoise, Qwen3, **Inworld**, **Cartesia**, **PlayHT**, +
  bestaande providers
- **Moderaties** — `/v1/moderations` — Inhoudsveiligheidscontrole
- **Opnieuw Rangschikken** — `/v1/rerank` — Documenten relevante opnieuw
  rangschikken
- **Antwoorden API** — Volledige `/v1/responses`-ondersteuning voor Codex

</details>

<details>
<summary><b>🧪 14. "I have no way to test and compare quality across models"</b></summary>

Ontwikkelaars willen weten welk model het best geschikt is voor hun gebruikgeval
— code, vertaling, redenering — maar vergelijken is manueel langzaam en geen
geïntegreerde evaltools bestaan.

**Hoe OmniRoute het oplost:**

- **LLM-Evaluaties** — Goudensettesten met 10 vooraf geladen gevalsen omvattende
  groet, wiskunde, geografie, code generatie, JSON-compliance, vertaling,
  markdown, veiligheidseisen
- **4 Strategieën voor Match** — `exact`, `bevat`, `regex`, `kunstmatig`
  (JS-functie)
- **Vertaler Playground Test Bench** — Massatesten met meerdere invoerders en
  verwachte uitvoerders, overstreeptjegevende vergelijking
- **Chat Tester** — Volledige rondbuffer met visuele respons rendering
- **Live Monitor** — Echte-tijdstroom van alle verzoeken die via de proxy
  stromen

</details>

<details>
<summary><b>📈 15. "I need to scale without losing performance"</b></summary>

Als de verzoekvolume groeit, genereren dezelfde vragen zonder caching dezelfde
kosten. Zonder idempotentie verbruiken dubbele verzoeken processing.
Per-providers limieten moeten worden gerespecteerd

**Hoe OmniRoute het oplost:**

- **Semantic Cache** — Twee-laagige cache (tekenreekssignatuur + semantisch)
  vermindert kosten en latentie
- **Request Idempotency** — 5 secunden deduplicatievenster voor identieke
  verzoeken
- **Rate Limit Detection** — Per-providers RPM, min verschil, en max
  gelijktijdige tracking
- **Editable Rate Limits** — Configuurbaar standaard in Settings → Resilience
  met persistie
- **API Key Validation Cache** — 3-laagige cache voor productie prestaties
- **Health Dashboard met Telemetry** — p50/p95/p99 latentie, cache stat, uptime

</details>

<details>
<summary><b>🤖 16. "I want to control model behavior globally"</b></summary>

Ontwikkelaars die willen dat alle antwoorden in een specifieke taal zijn, met
een specifieke toon, of willen dat de redeneringstokens worden beperkt.
Configureren van deze in elke tool/vraag is onpraktisch

**Hoe OmniRoute het oplost:**

- **System Prompt Injection** — Globaal prompt aan alle verzoeken toegepast
- **Thinking Budget Validation** — Redenering token allocatie controle per
  verzoek (pasdoor, automatisch, aanpasbaar, geadapt)
- **6 Routing Strategies** — Globale strategieën die bepalen hoe verzoeken
  worden gedistribueerd
- **Wildcard Router** — `provider/*` patronen routeen dynamisch naar elk
  provider
- **Combo Enable/Disable Toggle** — Klikcombinatiesdirect op de dashboard
  activeren
- **Provider Toggle** — Alles aan of uitzichelen voor een provider met één klik
- **Blocked Providers** — Exclude specifieke providers van `/v1/models` listing

</details>

<details>
<summary><b>🧰 17. "I need MCP tools as first-class product capabilities"</b></summary>

Veel AI-gatewayen openbaren MCP alleen als verborgen implementatiedetail. Teams
moeten een zichtbare en beheerbare operatieschicht hebben.

**Hoe OmniRoute het oplost:**

- NCP verschijnt in navigatie over het dashboard en tabblad protocol-eindpunt
- Aanrechtte gepersonaliseerde NCP-beheerpagina met processen, gereedschap,
  bereik en audit
- Geïntegreerde quick-start-omgeving voor `omniroute --ncp` en client
  registratie

</details>

<details>
<summary><b>🧠 18. "I need A2A orchestration with sync + stream task paths"</b></summary>

Agent-werkstromen hebben zowel directe antwoorden als langlopende gestreamde
uitvoering met levenscycluscontrole.

**Hoe OmniRoute het oplost:**

- A2A JSON-RPC-eindpunt (`POST /a2a`) met `bericht/sturen` en `bericht/stroom`
- SSE-streaming met terminale staatverdeling
- API's voor levenscyclus van taken voor `taken/ophalen` en `taken/annuleren`

</details>

<details>
<summary><b>🛰️ 19. "I need real MCP process health, not guessed status"</b></summary>

Teamleiders moeten weten of NCP daadwerkelijk aanwezig is, niet alleen of een
API bereikbaar is.

**Hoe OmniRoute het oplost:**

- Runtime hartslagbestand met PID, tijdstempels, transport, gereedschaps telling
  en scope-modus
- NCP-status-API die combinatie maakt van hartslag + recente activiteit
- UI-statuskaarten voor processen/uptime/hartslagverscherpte

</details>

<details>
<summary><b>📋 20. "I need auditable MCP tool execution"</b></summary>

Als gereedschappen de configureren of optreden als onderdelen voor acties,
hebben teams noodzakelijkerwijs gerechtvaardigde afkomst.

**Hoe OmniRoute het oplost:**

- SQLite-gebackte audit-registratie voor NCP-gereedschapaanroepen
- Filtreer per gereedschap, succes/fout, API-sleutel en paginatie
- Audit-tabblad + statistieken eindpunten voor automatisering

</details>

<details>
<summary><b>🔐 21. "I need scoped MCP permissions per integration"</b></summary>

Verschillende clients hebben het minimaal-privileges toegang recht tot
categorieën van gereedschappen.

**Hoe OmniRoute het oplost:**

- 9 precisie MCP-scopes voor gecontroleerd toegang tot tools
- Toepsleeping van toepassing en zichtbaarheid in MCP-beheerdersinterface
- Veilige standaardhouding voor operationele tooling

</details>

<details>
<summary><b>⚙️ 22. "I need operational controls without redeploying"</b></summary>

Teams hebben snelle runtime-wijzigingen nodig tijdens incidenten of cost-events.

**Hoe OmniRoute het oplost:**

- Directe activering van switches vanuit MCP-dashboard
- Toepassen van profielen voor resilience vanuit voorgedefinieerde beleidssets
- Herstellen van een circuitbreaker-state vanuit hetzelfde werkingspaneel

</details>

<details>
<summary><b>🔄 23. "I need live A2A task lifecycle visibility and cancellation"</b></summary>

Zonder levenscyclusvisibiliteit worden incidenten van taken moeilijk triage.

**Hoe OmniRoute het oplost:**

- Verwerving, filtrering van taken op basis van staat/skil met paginatie
- Doordraaien op task-metadata, evenementen en artifacts
- Einde-task- endpoint en UI-actie met bevestiging

</details>

<details>
<summary><b>🌊 24. "I need active stream metrics for A2A load"</b></summary>

Streaming workflows vereisen operationele inzicht in concurrentie en live
verbindingen

**Hoe OmniRoute het oplost:**

- Actieve stroomgetallets geïntegreerd in A2A-status
- Laatstekentijd en per-toestands getelde
- A2A-dashboardkaarten voor live-ops-monitoren

</details>

<details>
<summary><b>🪪 25. "I need standard agent discovery for clients"</b></summary>

Externe klanten en orchestrators hebben machinelezbare metadata voor onboarding
nodig.

**Hoe OmniRoute het oplost:**

- Agent kaart wordt blootgesteld aan `/.well-known/agent.json`
- Vaardigheden en competenties worden getoond in het management UI
- De A2A status API bevat ontdekking gegevens voor automatisering

</details>

<details>
<summary><b>🧭 26. "I need protocol discoverability in the product UX"</b></summary>

Als gebruikers geen protocollen op een oppervlak kunnen ontdekken, neemt de
kwaliteit van adoptie en ondersteuning af.

**Hoe OmniRoute het oplost:**

- Geconsolideerde **Afmetingen** pagina met tabs voor Proxy-server, MCP, A2A, en
  API -afmetingen
- Inline-opstartstatusknoppen (Online/Offline) voor MCP en A2A
- Koppelingen vanwege overzicht naar dediceerde tabs voor beheer

</details>

<details>
<summary><b>🧪 27. "I need end-to-end protocol validation with real clients"</b></summary>

Mock-tests zijn niet genoeg om de compatibiliteit van protocollen te valideren
voordat hij wordt gelanceerd.

**Hoe OmniRoute het oplost:**

- E2E suite die de applicatie aanzwengt en een echte MCP SDK client transport
  gebruikt
- A2A-clienttests voor ontdekken, sturen, streamen, halen, en annuleren stromen
- Overeenkomstige claims richten op MCP-audit en A2A-taken APIs

</details>

<details>
<summary><b>📡 28. "I need unified observability across all interfaces"</b></summary>

Het splitsen van observabiliteit door protocollen creëert blinde vlekken en
langere MTTR.

**Hoe OmniRoute het oplost:**

- Geïntegreerde dashboards/registers/analytische gegevens in één product
- Gezondheid + audit + aanvraag telemetriek over OpenAI, MCP, en A2Alagen
- Operationele APIs voor status en automatisering

</details>

<details>
<summary><b>💼 29. "I need one runtime for proxy + tools + agent orchestration"</b></summary>

De werking van vele aparte services verhoogt de operationele kosten en failure
modes.

**Hoe OmniRoute het oplost:**

- Een OpenAI-compatibele proxy, MCP-server en A2A-server in één stack
- Gedeeld authenticatie, resilience, gegevensarchief en inzichtelijkheid
- Konsistente beleidmodel over alle interactie-oppervlakken

</details>

<details>
<summary><b>🚀 30. "I need to ship agentic workflows without glue-code sprawl"</b></summary>

Teams verliezen snelheid wanneer zij meerdere ad-hoc diensten en scripts
uitvoeren.

**Hoe OmniRoute het oplost:**

- Geünificeerd eindpuntstrategie voor clients en agents
- Ingebouwde protocolbeheer UI's en rookvalidatieroutes
- Producie-klaar fundamenten (beveiliging, loggen, resilience, backup)

</details>

### Forbeeldspelkaarten (Integreerde Gebruiksscenario's)

**Spelkaart A: Geavanceerd betalen en voordelige backup**

```txt
Combinatie: "maximize-claude"
  1. cc/claude-opus-4-6
  2. glm/glm-4.7
  3. if/kimi-k2-denken

Maandelijkse kosten: $20 + kleine back-upsommen
Uitkomst: hogere kwaliteit, bijna-nul-interruptie
```

**Spelkaart B: Kostenloze coderingsstack**

```txt
Combinatie: "vrij-vrij"
  1. gc/gemini-3-flits
  2. if/kimi-k2-denken
  3. qw/qwen3-coder-plus

Maandelijkse kosten: $0 
Uitkomst: stabiele gratis coderingsstroom
```

**Spelkaart C: 24/7 altijd-actief fallback keten**

```txt
Combinatie: "altijd-actief"
  1. cc/claude-opus-4-6
  2. cx/gpt-5.2-codex
  3. glm/glm-4.7
  4. minimax/MiniMax-M2.1
  5. if/kimi-k2-denken

Uitkomst: diepe fallbackdiepte voor deadline-kritische belastbaarheden
```

**Spelkaart D: Agentsbeheer met MCP + A2A**

```txt
1) Start MCP-transport (`omniroute --mcp`) voor tool-gestuurde operationen
2) Verzend A2A-taken via `bericht/sturen` en `bericht/stroom`
3) Bekijk via /dashboard/endpoint (MCP en A2A-tabbladen)
4) Zoep services via inline status controle-elementen
```

---

## 🆓 Start Vrij — Zero Configuratie Kosten

> Setup AI coderen in minuten tegen een maandelijkse bijdrage van **$0**.
> Connecteer deze gratis accounts en gebruik de ingebouwde **Vrije Stack**
> Koppelcombinatie.

| Stap | Actie                                                | Toegangshebbers Ontgrendeld                                      |
| ---- | ---------------------------------------------------- | ---------------------------------------------------------------- |
| 1    | Verbind **Kiro** (AWS Builder ID OAuth)              | Claude Sonnet 4.5, Haiku 4.5 — **onbeperkt**                     |
| 2    | Verbind **iFlow** (Google OAuth)                     | kimi-k2-denken, qwen3-coder-plus, deepseek-r1... — **onbeperkt** |
| 3    | Verbind **Qwen** (Device Code)                       | qwen3-coder-plus, qwen3-coder-flash... — **onbeperkt**           |
| 4    | Verbind **Cassiopee CLI** (Google OAuth)             | cassiopee-3-flash, cassiopee-2.5-pro — **180K/mo gratis**        |
| 5    | `/dashboard/combos` → **Gratis Staal (€0)** sjabloon | Allesmaal automatisch wisselen tussen alle gratis providers.     |

**Wijst enige IDE/CLI naar:** `http://localhost:20128/v1` · API-Sleutel:
`enige-tekst` · Klaar.

> **Optionele extra dekking (ook gratis):** Groq API sleutel (30 RPM gratis),
> NVIDIA NIM (40 RPM gratis, 70+ modellen), Cerebras (1M tok/day), LongCat API
> sleutel (50M tokens/day!), Cloudflare Workers AI (10K Neuronen/day, 50+
> modellen).

## Snel beginnen

### 1. Installeren en uitvoeren

```bash
npm install -g omniroute
omniroute
```

> **pnpm gebruikers:** Voer `pnpm approve-builds -g` uit nadat geïnstalleerd is,
> om native build scripts te activeren die vereist zijn voor `better-sqlite3` en
> `@swc/core`:
> 
> ```bash
> pnpm install -g omniroute
> pnpm approve-builds -g   # Selecteer alle pakketten → benadrukken
> omniroute
> ```

Het dashboard wordt geopend op `http://localhost:20128` en de API basis-URL is
`http://localhost:20128/v1`.

| Cmd                     | Beschrijving                                                        |
| ----------------------- | ------------------------------------------------------------------- |
| `omniroute`             | Server opstarten (`PORT=20128`, API en dashboard op dezelfde poort) |
| `omniroute --port 3000` | Stel het kanonische/API-poortnummer vast op 3000                    |
| `omniroute --mcp`       | MCP-server opstarten (stdio-transport)                              |
| `omniroute --no-open`   | Het browservenster niet automatisch openen                          |
| `omniroute --help`      | Help weergeven                                                      |

Optionele splitspoortmode:

```bash
PORT=20128 DASHBOARD_PORT=20129 omniroute
# API:       http://localhost:20128/v1
# Dashboard: http://localhost:20129
```

### 1) Verbind providers en maak je API sleutel aan

1. Open Dashboard → `Providers` en verbind minstens één provider (OAuth of API
   sleutel).
2. Open Dashboard → `Punten` en maak een API sleutel.
3. (Optielijk) Open Dashboard → `Combinaties` en instelling van je fallback
   keten.

### 2) Punt je coderingstool naar OmniRoute

```txt
Base URL: http://localhost:20128/v1
API Sleutel:  [kopiëren van Punt pagina]
Model:    als/kimi-k2-denken (of welke provider/model voorvoegsel dan ook)
```

Werkt samen met Claude Code, Codex CLI, Gemini CLI, Cursor, Cline, OpenClaw,
OpenCode en OpenAI-gecompatibele SDK's.

### 3) Activeer en valideer protocollen (v2.0)

**MCP (voor tool-aangedreven operaties):**

```bash
omniroute --mcp
```

Daarna verbinding maak je MCP-client over `stdio` en test tools zoals:

- `omniroute_get_health`
- `omniroute_list_combos`

**A2A (voor agent-to-agent workflows):**

```bash
curl http://localhost:20128/.well-known/agent.json
```

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"quickstart","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"Geef me een korte quota samenvatting."}]}}'
```

### 4) Valideer alles eind-to-eind (aanbevolen)

```bash
npm run test:protocols:e2e
```

Dit set validerend reële MCP en A2A clientstromen tegen een lopende app.

### Alternatief: draai vanuit broncode.

```bash
cp .env.example .env
npm install
PORT=20128 DASHBOARD_PORT=20129 NEXT_PUBLIC_BASE_URL=http://localhost:20129 npm run dev
```

---

## 🐳 Docker

OmniRoute is available as a public Docker image on [Docker
Hub](https://hub.docker.com/r/diegosouzapw/omniroute).

**Quick run:**

```bash
docker run -d \
  --name omniroute \
  --restart unless-stopped \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:latest
```

**With environment file:**

```bash
# Copy and edit .env first
cp .env.example .env

docker run -d \
  --name omniroute \
  --restart unless-stopped \
  --env-file .env \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:latest
```

**Using Docker Compose:**

```bash
# Base profile (no CLI tools)
docker compose --profile base up -d

# CLI profile (Claude Code, Codex, OpenClaw built-in)
docker compose --profile cli up -d
```

| Afbeelding               | Tag      | Grootte | Beschrijving          |
| ------------------------ | -------- | ------- | --------------------- |
| `diegosouzapw/omniroute` | `latest` | ~250MB  | Latest stable release |
| `diegosouzapw/omniroute` | `1.0.3`  | ~250MB  | Current version       |

---

## 🖥️ Desktop App — Offline & Always-On

> 🆕 **Nieuw!** OmniRoute is nu beschikbaar als een **native
> bureaubus-toepassing** voor Windows, macOS en Linux.

Draai OmniRoute als een standalone bureaubus-app — geen terminal, geen browser,
geen internet vereist voor lokale modellen. De Electron-basisapplicatie bevat:

- 🖥️ **Native Windows** – Geïntegreerde appvenster met systeembronzen integratie
- 🔄 **Auto-Start** – Start OmniRoute bij systeemlogin
- 🔔 **Native Notificaties** – Krijg berichten voor quota's die zijn uitgeput of
  providerissues
- ⚡ **Eén-punt Install** – NSIS (Windows), DMG (macOS), AppImage (Linux)
- 🌐 **Offline Modus** – Kan volledig offline werken met ingebouwde server

### Snel beginnen

```bash
# Ontwikkelingsmodus
npm run electron:dev

# Bouw voor je platform
npm run electron:build       # Huidig platform
npm run electron:build:win   # Windows (.exe)
npm run electron:build:mac   # macOS (.dmg) – x64 &amp; arm64
npm run electron:build:linux # Linux (.AppImage)
```

### Systeembronze

Als je het venster minimaliseert, leeft OmniRoute in je systeembronz met snelle
acties:

- Dashboard openen
- Verander serverpoort
- Verlaat toepassing

📖 Volledige documentatie: [`electron/README.md`](electron/README.md)

---

## 💰 Prijzen op een Klik

| Tarief             | Aanbieder                  | Kosten                          | Quota Reset            | Best For                                  |
| ------------------ | -------------------------- | ------------------------------- | ---------------------- | ----------------------------------------- |
| **💳 SUBSCRIPTION** | Claude Code (Pro)          | $20/mo                          | 5h + weekly            | Already subscribed                        |
|                    | Codex (Plus/Pro)           | $20-200/mo                      | 5h + weekly            | OpenAI users                              |
|                    | Gemini CLI                 | **FREE**                        | 180K/mo + 1K/day       | Everyone!                                 |
|                    | GitHub-copiloot            | $10-19/mo                       | Monthly                | GitHub users                              |
| **🔑 API KEY**      | NVIDIA NIM                 | **FREE** (dev forever)          | ~40 RPM                | 70+ open modellen                         |
|                    | Cerebras                   | **Gratis** (1M token/dag)       | 60K TPM / 30 RPM       | Snelste ter wereld                        |
|                    | Groq                       | ** Gratis** (30 RPM)            | 14,4K RPD              | Ultrazwarte Llama/Gemma                   |
|                    | DeepSeek V3.2              | $0,27/$1,10 per 1 miljoen       | Geen                   | Bij beste prijs/kwaliteit reden           |
|                    | xAI Grok-4 Fast            | **$0,20/$0,50 per 1 miljoen** 🆕 | Geen                   | Snelste + hulpmiddeloproepen, ultrazwarte |
|                    | xAI Grok-4 (standaard)     | $0,20/$1,50 per 1 miljoen 🆕     | Geen                   | Vlaggenschipaanvaarding van xAI           |
|                    | Mistral                    | Vrije proef + betaalde          | Tarief beperkt         | Europees kunstmatig intelligentie         |
|                    | OpenRouter                 | Aanpak-op-maat                  | Geen                   | Meerdere modellen beschikbaar: 100+       |
| **💰 KIEKMETAAL **  | GLM-5 (via Z.AI) 🆕         | $0,50/1 miljoen                 | Alledag 10 AM          | 128K uitvoer, nieuwste vlaggenschip       |
|                    | GLM-4.7                    | $0,60/1 miljoen                 | Alledag 10 AM          | Budgetterings backup                      |
|                    | MiniMax M2,5 🆕             | $0,30/1 miljoen invoer          | Rolling: 5 uur         | Redeneren + taken voor agentie            |
|                    | MiniMax M2,1               | 0,20/1 miljoen                  | Rolling: 5 uur         | Cheapest optie                            |
|                    | Kimi K2.5 (Moonshot API) 🆕 | Aanpak-op-maat                  | Geen                   | Direct toegang tot de Moonshot API        |
|                    | Kimi K2                    | 9,00 p/m. rechtstreeks          | 10 miljoen tokens/p.m. | Voorspelbare kosten                       |
| **🆓 GRATIS**       | iFlow                      | **$0**                          | Oneindig               | 5 modelen oneindig                        |
|                    | Qwen                       | **$0**                          | Oneindig               | 4 modelen oneindig                        |
|                    | Kiro                       | **$0**                          | Oneindig               | Claude Sonnet/Haiku (AWS Builder)         |
|                    | LongCat Flash-Lite 🆕       | **$0** (50 miljoen tok/p.d. 🔥)  | 1 vraag per seconde    | Largest free quota op aarde               |
|                    | Pollinations AI 🆕          | **$0** (geen sleutel vereist)   | 1 req/15s              | GPT-5, Claude, DeepSeek, Llama 4          |
|                    | Cloudflare Workers AI 🆕    | **$0** (10K Neuronen/dag)       | ~150 resp/day          | 50+ modellen, wereldwijde randapplicatie  |
|                    | Scaleway AI 🆕              | **$0** (1M tokens totaal)       | Tarief beperkt         | EU/GDPR, Qwen3 235B, Llama 70B            |

> 🆕 **Nieuwe modellen toegevoegd (mrt 2026): ** Grok-4 Fast Familie bij
> $0,20/$0,50/M (geteste op 1143ms — 30% sneller dan Gemini 2.5 Flash) , GLM-5
> via Z.AI met 128K uitvoer, MiniMax M2.5 redenering, DeepSeek V3.2 geüpdatete
> prijzen, Kimi K2.5 via Moonshot direct API

**💡 $0 Combo Stappenplank — De Compleet Gratis Instelling:**

```
# 🆓 Ultimate Free Stappenplank 2026 — 11 aanbieders, $0 Forever
Kiro (kr/)             → Claude Sonnet/Haiku ONBEPERKT
iFlow (if/)            → kimi-k2-denken, qwen3-coder-plus, deepseek-r1 ONBEPERKT
LongCat Lite (lc/)     → LongCat-Flash-Lite — 50M tokens/dag 🔥
Pollinations (pol/)    → GPT-5, Claude, DeepSeek, Llama 4 — geen sleutel vereist
Qwen (qw/)             → qwen3-coder-plus, qwen3-coder-flash, qwen3-coder-next ONBEPERKT
Gemini (gemini/)       → Gemini 2.5 Flash — 1,500 req/dag gratis API-sleutel
Cloudflare AI (cf/)    → Llama 70B, Gemma 3, Mistral — 10K Neuronen/dag
Scaleway (scw/)        → Qwen3 235B, Llama 70B — 1M gratis tokens (EU)
Groq (groq/)           → Llama/Gemma ultraprofessioneel — 14.4K req/dag
NVIDIA NIM (nvidia/)   → 70+ openbare modellen — 40 RPM eeuwigdurend
Cerebras (cerebras/)   → Llama/Qwen snelste ter wereld — 1M tok/dag
```

**Nul kosten. Nooit stopt met coderen.** Configureer dit als één alomvattend
combo en alle achterhaalde situaties gebeuren automatisch — geen handmatige
overschakeling ooit.

---

---

## 🆓 Gratis Modellen — Wat je Actueel Krijgt

> Alle modellen hieronder zijn **100% gratis met geen creditcard vereist**.
> OmniRoute routet automatisch tussen hen wanneer de één quotabeperking op is —
> combineer hen allemaal voor een onaantastbaar $0 combo.

### 🔵 CLAUDE MODELLEN (via Kiro — AWS Bouwer ID)

| Model               | Voorvoegsel | Limiet        | Tarieflimiet           |
| ------------------- | ----------- | ------------- | ---------------------- |
| `claude-sonnet-4.5` | `kr/`       | **Onbeperkt** | Geen gemeld daglimiet  |
| `claude-haiku-4.5`  | `kr/`       | **Onbeperkt** | Geen gemeld daglimiet  |
| `claude-opus-4.6`   | `kr/`       | **Onbeperkt** | Nieuwste Opus via Kiro |

### 🟢 IFLOW MODELS (Gratis OAuth — geen Credit Card nodig)

| Model                       | Voorvoegsel | Limiet        | Tarieflimiet       |
| --------------------------- | ----------- | ------------- | ------------------ |
| `kimi-k2-denken`            | `if/`       | **Onbeperkt** | Geen gemeld limiet |
| `qwen3-programmeerder-plus` | `if/`       | **Onbeperkt** | Geen gemeld limiet |
| diepseek-r1`                | `if/`       | **Onbeperkt** | Geen gemeld limiet |
| minimax-m2.1`               | `if/`       | **Onbeperkt** | Geen gemeld limiet |
| kimi-k2`                    | `if/`       | **Onbeperkt** | Geen gemeld limiet |

### 🟡 QR MODELS (Apparaatcode Auth)

| Model                       | Voorvoegsel | Limiet        | Tarieflimiet              |
| --------------------------- | ----------- | ------------- | ------------------------- |
| `qwen3-programmeerder-plus` | `qw/`       | **Onbeperkt** | Geen gemeld limiet        |
| `qwen3-coder-flash`         | `qw/`       | **Onbeperkt** | Geen gemeld limiet        |
| `qwen3-coder-next`          | `qw/`       | **Onbeperkt** | Geen gemeld limiet        |
| `visie-model`               | `qw/`       | **Onbeperkt** | Multimodal (afbeeldingen) |

### 🟣 GEMINI CLI (Google OAuth)

| Model                        | Voorvoegsel | Limiet                                  | Tarieflimiet       |
| ---------------------------- | ----------- | --------------------------------------- | ------------------ |
| `Gemini-3 Flash vooruitblik` | `gc/`       | **180K tokenen per maand** + 1K per dag | Maandelijkse reset |
| `Gemini-2.5 Pro`             | `gc/`       | 180K per maand (gezamelijk pool)        | Zeer kwalitatief   |

### ⚫ NVIDIA NIM (Gratis API-sleutel — build.nvidia.com)

| Tarief                | Dagelijkse limiet | Tarieflimiet | Opmerkingen                                                     |
| --------------------- | ----------------- | ------------ | --------------------------------------------------------------- |
| Gratis (ontwikkelaar) | Geen tokenlimiet  | **~40 RPM**  | 70+ modellen; overstappen naar puur limieten per dag begin 2025 |

Populaire free modellen: `Moonshot ai/kimik 2.5 ` (Kimi K2.5), `Z-ai/glm 4.7 `
(GLM 4.7), `Deepseek-ai/deepseek v3.2 ` (DeepSeek V3.2), `Nvidia/llama
3.3-70b-instruct `, `Deepseek/deepseek r1 `

### ⚪ CEREBRAS (Gratis API-sleutel — inference.cerebras.ai)

| Tarief | Dagelijkse limiet | Tarieflimiet     | Opmerkingen                                     |
| ------ | ----------------- | ---------------- | ----------------------------------------------- |
| Gratis | **1M tokens/dag** | 60K TPM / 30 RPM | Worlds snelste LLM-inferentie; Resets dagelijks |

Beschikbaar gratis: `llama-3.3-70b`, `llama-3.1-8b`,
`deepseek-r1-distill-llama-70b`

### 🔴 GROQ (Gratis API-sleutel — console.groq.com)

| Tarief | Dagelijkse limiet | Tarieflimiet               | Opmerkingen                                                                 |
| ------ | ----------------- | -------------------------- | --------------------------------------------------------------------------- |
| Gratis | **14.4K RPD**     | 30 inhoudsopgave per model | Geen creditcard; 429 wanneer grens bereikt, wordt niet in rekening gebracht |

Beschikbaar gratis: `llama-3.3-70b-versatile`, `gemma2-9b-it`, `mixtral-8x7b`,
`whisper-large-v3`

### 🔴 LONGCAT AI (Gratis API-sleutel — longcat.chat) 🆕

| Model                         | Voorvoegsel | Dagelijkse gratis quota | Opmerkingen                |
| ----------------------------- | ----------- | ----------------------- | -------------------------- |
| `LongCat-Flash-Lite`          | `lc/`       | **50M tokens** 💥        | Grootste gratis quota ooit |
| `LongCat-Flash-Chat`          | `lc/`       | 500K tokens             | Meerturige dialoog         |
| `LongCat-Flash-Thinking`      | `lc/`       | 500K tokens             | Redeneren / CoT            |
| `LongCat-Flash-Thinking-2601` | `lc/`       | 500K tokens             | Januari 2026-edities       |
| `LongCat-Flash-Omni-2603`     | `lc/`       | 500K tokens             | Multimodaal                |

> 100% gratis tijdens het openbare betaalde testen. Meld je aan bij
> [longcat.chat](https://longcat.chat) met email of telefoon. Reset elke dag om
> 00:00 UTC.

### 🟢 POLLINATIONS AI (Geen API Key vereist) 🆕

| Model      | Voorvoegsel | Tarieflimiet | Provider Behind    |
| ---------- | ----------- | ------------ | ------------------ |
| `openai`   | `pol/`      | 1 req/15s    | GPT-5              |
| `claude`   | `pol/`      | 1 req/15s    | Anthropic Claude   |
| `gemini`   | `pol/`      | 1 req/15s    | Google Gemini      |
| `deepseek` | `pol/`      | 1 req/15s    | DeepSeek V3        |
| `llama`    | `pol/`      | 1 req/15s    | Meta Llama 4 Scout |
| `mistral`  | `pol/`      | 1 req/15s    | Mistral AI         |

> ✨ **Zero friction:** No signup, no API key. Add the Pollinations provider with
> an empty key field and it works immediately.

### 🟠 CLOUDFLARE WORKERS AI (Free API Key — cloudflare.com) 🆕

| Tarief | Daily Neurons | Gelijke Gebruiksaanwijzing                         | Opmerkingen                |
| ------ | ------------- | -------------------------------------------------- | -------------------------- |
| Gratis | [10,000][8]   | ~150 LLM resp / 500s geluidsbestanden / 15K embeds | Globale rand, 50+ modellen |

Populaire gratismodellen:[21]@cf/meta/llama-3.3-70b-instruct[53],
[56]@cf/google/gemma-3-12b-it[82], [85]@cf/openai/whisper-large-v3-turbo[119]
(gratis audio!), [136]@cf/qwen/qwen2.5-coder-15b-instruct[172]

> Vereist API-sleutel + Account ID van
> [dash.cloudflare.com](https://dash.cloudflare.com). Bewaar Account ID in
> aanbiederinstellingen.

### 🟣 SCALEWAY AI (1M gratis tokens — scaleway.com) 🆕

| Tarief | Vrije Quota     | Locatie       | Opmerkingen                          |
| ------ | --------------- | ------------- | ------------------------------------ |
| Gratis | [1M tokens][11] | 🇫🇷 Parijs, EU | Geen creditcard nodig binnen grenzen |

Verkrijgbaar gratis:[16]qwen3-235b-a22b-instruct-2507[46] (Qwen3 235B!),
[63]llama-3.1-70b-instruct[86], [89]mistral-small-3.2-24b-instruct-2506[125],
[128]deepseek-v3-0324[145]

> EU/GDPR-compatibel. Haal API-toets op bij
> [console.scaleway.com](https://console.scaleway.com).

> [💡 De Ultieme Vrije Stapel (11 aanbieders, $0 voor altijd):][55]
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

| Aanbieder        | Free Credits           | Best Model                                   | Tarieflimiet                 |
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

Then in `/dashboard/media` → **Transcription** tab: upload any audio or video
file → select your combo endpoint → get transcription in supported formats.

## 💡 Key Features

OmniRoute v2.0 is built as an operational platform, not just a relay proxy.

### 🆕 New — ClawRouter-Inspired Improvements (Mar 2026)

| Feature                             | What It Does                                                                                |
| ----------------------------------- | ------------------------------------------------------------------------------------------- |
| ⚡ **Grok-4 Fast Family**            | xAI models at $0.20/$0.50/M — benchmarked 1143ms (30% faster than Gemini 2.5 Flash)         |
| 🧠 **GLM-5 via Z.AI**                | 128K output context, $0.5/1M — newest flagship from the GLM family                          |
| 🔮 **MiniMax M2.5**                  | Reasoning + agentic tasks at $0.30/1M — significant upgrade from M2.1                       |
| 🎯 **toolCalling Flag per Model**    | Per-model `toolCalling: true/false` in registry — AutoCombo skips non-tool-capable models   |
| 🌍 **Multilingual Intent Detection** | PT/ZH/ES/AR keywords in AutoCombo scoring — better model selection for non-English content  |
| 📊 **Benchmark-Driven Fallbacks**    | Real p95 latency from live requests feeds combo scoring — AutoCombo learns from actual data |
| 🔁 **Request Deduplication**         | Content-hash based dedup window — multi-agent safe, prevents duplicate charges              |
| 🔌 **Plug inbare RouterStrategy**    | Erganigeerbaar `RouterStrategy` interface — voeg uw eigen routinglogica toe als plugins     |

### 🚀 Vorige versie 2.0.9+ — Playground, CLI Fingerprints & ACP

| Feature                                    | What It Does                                                                                                                                                                                                                                                       |
| ------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 🎮 **Model Playground**                     | Hoofdpagina om elke model rechtstreeks te testen — aanbieder/model/eindpuntselecteurs, Monaco Editor, streamen, annuleren, tijden                                                                                                                                  |
| 🔏 **CLI Vingerafdruk matching**            | Per-aanbieder header/body volgorde om aan te sluiten op native CLI signatures — schakel per aanbieder in instellingen > beveiliging aan. **Uw proxy IP wordt bewaard**                                                                                             |
| 🤝 **ACP-steun (Agente Client Protocol)**   | CLI-agentontdekking (Codex, Claude, Goose, Gemiini CLI, OpenClaw + 9 meer), processtarter, `/api/acp/agents` eindpunt                                                                                                                                              |
| 🤖 **ACP-agenten Dashboard**                | Debug › Agents pagina — grid van 14 agents met installatio status, versie, custom agent vorm voor elke CLI-tool. **OpenCode**gebruikers krijgen een "Download opencode.json"-knop die een klaar voor gebruikig config met alle beschikbare modellen automatiseert. |
| 🔧 **Aangepaste Model `apiFormat` Routing** | Aangepaste modellen met `apiFormat: "responses"` routen nu correct naar de Responses API vertaler                                                                                                                                                                  |
| 🏢 **Codex-ruimteafscherming**              | Meerdere Codex-workspaces per e-mail — OAuth is correct onderscheiden door werkruimte ID                                                                                                                                                                           |
| 🔄 **Automaat update Electon**              | Desktop app controleert updates + automatische installatie bij restart                                                                                                                                                                                             |

### 🤖 Agent & Protocol operaties (versie 2.0)

| Feature                               | What It Does                                                                                                           |
| ------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- |
| 🔧 **MCP Server (16 gereedsen)**       | IDE/agen gereedschappen via 3 vervoerbare transports: stdio, SSE (`/api/mcp/sse`), Streamable HTTP (`/api/mcp/stream`) |
| 🤝 **A2A Server (JSON-RPC + SSE)**     | Aanvraag tussen agenten met synchroon en stromend workflow                                                             |
| 🧭 **Consolidated Endpoints Page**     | Tabbemed besturingsscherm met Endpoint Proxy, MCP, A2A, en API Endpoints tabs                                          |
| 🎚️ **Service Enable/Disable Toggles** | AAN/UIT knoppen voor MCP en A2A met instellingsbehoud (standen: UIT)                                                   |
| 🛰️ **MCP Runtime Heartbeat**          | Echte processstatus (PID, uptime, heartbeat-leeftijd, transport, scope-mode)                                           |
| 📋 **MCP Audit Trail**                 | Jitspreuken met succes/fouten en sleutelattributie                                                                     |
| 🔐 **MCP Scope Enforcement**           | 9 granulaire scope-permissies voor gereguleerde toegang tot gereedschaften                                             |
| 📡 **A2A Task Lifecycle Management**   | Lijstenfilter taken, inspecteer evenementen/artefacten, annuleren rennende taken                                       |
| 📋 **Agent Card Discovery**            | `/.well-known/agent.json` voor clientautozocht                                                                         |
| 🧪 **Protocol E2E Test Harness**       | Einde-to-einde protocol testomgeving` test:protocols:e2e`                                                              |
| ⚙️ **Operational Controls**           | Kiesmenu, toepassingsvelden voor eenheden, resetbrekers vanaf één regelingsoppervlak                                   |

### 🧠 Routerings- & Intelligentie

| Feature                               | What It Does                                                                        |
| ------------------------------------- | ----------------------------------------------------------------------------------- |
| 🎯 **Smijt 4-Tier Fallback**           | Automatische route: Abonnement → API-toets → Goedkoop → Gratis                      |
| 📊 **Real-Time Quota Tracking**        | Live token teller + herinnering teller voor provider per minuut                     |
| 🔄 **Format Vertaling**                | OpenAI ↔ Claude ↔ Gemini ↔ Reacties met schema-touwveilig omzettingen               |
| 👥 **Meervoudig accountondersteuning** | Meerdere accounts per provider met intelligente selectie                            |
| 🔄 **Automaat token refresh**          | OAuth tokens refreshen automatisch met herhaalpogingen                              |
| 🎨 **Aangepaste sets**                 | 6 balanceringsstrategieën + fallback ketencontrole                                  |
| 🌐 **Wilkaart routering**              | `leverancier/*` dynamische routers                                                  |
| 🧠 **Denkbeheersel Budgetcontroles**   | Tunneling, auto, aangepast en adaptief rednerig begrenzingen                        |
| 🔀 **Model aliassen**                  | Ingebouwd + aangepaste model-aliasing en migratieveiligheid                         |
| ⚡ **Somsachtergrond verval**          | Rute laagprioritaire achtergrond taken naar goedkope modellen                       |
| 🧪 **Taalbewust smaakrijden**          | Selecteer model automatisch op inhoudstype (coderen/vision/analyse/ samenvatting)   |
| 💬 **Systeem prompt injectie**         | Globale gedragscontroles worden consequent toegepast                                |
| 📄 **Antwoord API compatibiliteit**    | Volledige `/v1/antwoorden`-ondersteuning voor Codex en geavanceerde agent-pipelines |

### 🎵 Multi-Modale APIs

| Feature                        | What It Does                                                                                                                                                                                |
| ------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🖼️ **Afbeelding generatie**    | `/v1/beelden/generaties` met cloud en lokale back-ups                                                                                                                                       |
| 📐 **Embedding**                | `/v1/embeddingen` voor zoekopdrachten en RAG- pipelines                                                                                                                                     |
| 🎤 **Auditie Transscriptie**    | `/v1/audio/transcripties` — 7 aanbieders (Deepgram Nova 3, AssemblyAI, Groq Whisper, HuggingFace, ElevenLabs, OpenAI, Azure), automatische taalbeschrijving, ondersteuning voor MP4/MP3/WAV |
| 🔊 **Tekst-na-Stem**            | `/v1/audio/stem` — 10 aanbieders (ElevenLabs, OpenAI, Deepgram, Cartesia, PlayHT, HuggingFace, Nvidia NIM, Inworld, Coqui, Tortoise) met correcte foutmeldingen                             |
| 🎬 **Video-Generatie**          | `/v1/videos/generaties` (ComfyUI + SD WebUI workflows)                                                                                                                                      |
| 🎵 **Muziek-Generatie**         | `/v1/muziek/generaties` (ComfyUI workflows)                                                                                                                                                 |
| 🛡️ **Beveiliging**             | `/v1/beveiliging` veiligheidschecks                                                                                                                                                         |
| 🔀 **Uitvoeringsrangschikking** | `/v1/uithoofdrangschikking` voor relevantie scorings                                                                                                                                        |
| 🔍 **Web Zoeken** 🆕             | `/v1/zoeken` — 5 aanbieders (Serper, Brave, Perplexity, Exa, Tavily), 6,500+ gratis/maand, automatische failover, cache                                                                     |

### 🛡️ Resistenteiteit, Veiligheid & Beheer

| Feature                            | What It Does                                                                           |
| ---------------------------------- | -------------------------------------------------------------------------------------- |
| 🔌 **Circuitbrekers**               | Per-model reist/word herstel met sleutelcontroles                                      |
| 🎯 **Eindpunt-Aware Modellen**      | Custom models declare supported endpoints + API format                                 |
| 🛡️ **Anti-Thundering Herd**        | Mutex + semaphore protections on retry/rate events                                     |
| 🧠 **Semantic + Signature Cache**   | Cost/latency reduction with two cache layers                                           |
| ⚡ **Request Idempotency**          | Duplicate protection window                                                            |
| 🔒 **TLS Fingerprint Spoofing**     | Browser-like TLS fingerprint — **reduces bot detection and account flagging**          |
| 🔏 **CLI Vingerafdruk matching**    | Matches native CLI request signatures — **reduces ban risk while preserving proxy IP** |
| 🌐 **IP Filtering**                 | Allowlist/blocklist control for exposed deployments                                    |
| 📊 **Editable Rate Limits**         | Configurable global/provider-level limits with persistence                             |
| 🔑 **API Key Management + Scoping** | Secure key issuance/rotation and model/provider controls                               |
| 🛡️ **Protected `/models`**         | Optional auth gating and provider hiding for model catalog                             |

### 📊 Observability & Analytics

| Feature                                  | What It Does                                               |
| ---------------------------------------- | ---------------------------------------------------------- |
| 📝 **Verzoek + Proxy Logregistratie**     | Volledige aanvraag/antwoord en proxy logregistratie        |
| 📋 **Geïntegreerde Logbestandsinterface** | Aanvraag, proxy, audit- en consoleweergaven op één pagina  |
| 🔍 **Verzoeksensors**                     | latenze (p50/p95/p99) en aanvraagnabijhouding              |
| 🏥 **Gezondheidsdashboard**               | Uptime, breaker-toestand, lockouts en cache statistieken   |
| 💰 **Kostenbeheersing**                   | budgetcontroles en per-model prijzigezag                   |
| 📈 **Analysevisualisaties**               | gebruiksonderzoek met trendweergaven                       |
| 🧪 **Beoordelingsframework**              | goudensets testen met configuurbare strategieën voor match |

### ☁️ Implementatie & Platform

| Feature                       | What It Does                                                           |
| ----------------------------- | ---------------------------------------------------------------------- |
| 🌐 **Overal Implementeren**    | Lokale host, VPS, Docker, Cloud omgevingen                             |
| 💾 **Cloud Synchronisatie**    | Configuratie synchronisatie via cloud worker                           |
| 🔄 **Backup/Restore**          | Export/import-en reddingsacties                                        |
| 🧙 **Onboarding Wizard**       | Eerste-run geleide instellingen                                        |
| 🔧 **CLI Tools Dashboard**     | Eenknop- instellingen voor populaire programmeringstools               |
| 🎮 **Model Playground**        | Testen van elke provider/model/endpoint vanuit de dashboard            |
| 🔏 **CLI Vingerafdruk Toggle** | Per-provider vingerafdruk matching in Instellingen > Beveiliging       |
| 🌐 **i18n (30 talen)**         | Volledige dashboard + documentatie taal ondersteuning met RTL-coverage |
| 🧹 **Clear Alle Modellen**     | Eenknop- actie voor het wissen van de modelijst in provider details    |
| 📋 **Issue-sjablonen**         | Gebruikelijke GitHub-sjablonen voor bug's en features                  |
| 📂 **Aangepaste Gegevensmap**  | `DATARICHTE_DIR`  overschrijving voor opslaglocatie                    |

### Deep Dive in functie

#### Verbeterde fallback met praktische kostbeheersing

```txt
Combo: "mijn-dev-omgeving"
  1. cc/claude-opus-4-6
  2. nvidia/llama-3.3-70b
  3. glm/glm-4.7
  4. if/kimi-k2-denken
```

Bij quota, rate of gezondheid falen, slaat OmniRoute automatisch over naar de
volgende kandidaat zonder handmatige schakeling.

#### Protocolbeheer voorzien van inzicht en inbedrijfstelling

- MCP + A2A zijn in de interface en documentatie ontdekt en beschikbaar (niet
  verborgen)
- Protocolstatus-API's exposeren live operationele gegevens (`/api/mcp/*`,
  `/api/a2a/*`)
- Overzichten omvatten acties voor dag-2-operaties (combinatietoegankelijkheid,
  breaker resetten, taakannuleringen)

#### Vertaler + validatieworkflow

De Vertaler-omgeving omvat:

- **Speeltuin**: eenmalige transformatiecontroles
- **Chattester**: volledige vraag-antwoordronde met reële response
- **Testbaan**: meerdere gevallen in één uitvoering
- **Live Observer**: real-time verkeersbeeld

Daarnaast protocolvalidatie met reële clients via `npm run test:protocols:e2e`.

> 📖 **[MCP Server Handleiding](open-sse/mcp-server/README.md)** — Toolvoeringen,
> ontwikkelomgevingenconfiguraties, en clientvoorbeelden
> 
> 📖 **[A2A Server Handleiding](src/lib/a2a/README.md)** — Vaardigheden,
> JSON-RPC-methoden, streaming, en takenleven

## 🧪 Evaluaties (Evals)

OmniRoute bevat een ingebouwde evaluatieframework om de kwaliteit van de
LLM-antwoorden te testen tegen een gouden instelling. Gebruik hiervoor
**Analyseken → Evals** in het overzicht.\
==WEBLATE_PART==

### Ingebouwd Gouden Set

De ingebouwde "OmniRoute Golden Set" bevat testcases voor:

- Hallos, wiskunde, geografie, codegeneratie
- JSON-formaat-compatibiliteit, vertaling, markdown-generatie
- Veiligheidsweigering (schadelijk content), tellen, booleaanse logic

### Evaluatiestrategieën

| Strategie | Beschrijving                                                             | Voorbeeld                              |
| --------- | ------------------------------------------------------------------------ | -------------------------------------- |
| `exact`   | De uitvoer moet exact overeenkomen                                       | `"4"`                                  |
| `bevat`   | De uitvoer moet een onderdeel van een string bevatten (geval ongevoelig) | `"Paris"`                              |
| `regex`   | De output moet overeenkomen met een regex-patroon                        | `"1.*2.*3"`                            |
| `custom`  | Een aanpasbaar JavaScript-gedeelte geeft True/False terug                | `(output) =&gt; output.length &gt; 10` |

---

## 📚 Begin-Handleiding

### ProTOCOL-opstelling (MCP + A2A)

<details>
<summary><b>🧩 MCP Setup (Model Context Protocol)</b></summary>

Start MCP-transport in stdio-modus:

```bash
omniroute --mcp
```

Aanbevolen validatiestroom:

1. Verbinding maken met uw MCP-client via stdio.
2. Draai `omniroute_get_health`.
3. Draai `omniroute_list_combos`.
4. Open `/dashboard/mcp` om hartslag, activiteit en audit te bevestigen.

Handige APIs voor automatisering:

- `HTTP GET /api/mcp/status`
- `HTTP GET /api/mcp/tools`
- `HTTP GET /api/mcp/audit`
- `HTTP GET /api/mcp/audit/stats`

</details>

<details>
<summary><b>🤝 A2A Setup (Agent2Agent)</b></summary>

Het agent ontdekken:

```bash
curl http://localhost:20128/.well-known/agent.json
```

Een taak versturen:

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'inhoud-type: toepassing/json' \
  -d '{"jsonrpc":"2.0","id":"setup-a2a","method":"bericht/versturen","params":{"vaardigheid":"quotagebeheer","berichten":[{"rol":"gebruiker","inhoud":"Samenvatting van quotage_status."}]}}'
```

Levenscyclus beheren:

- `GET /api/a2a/status`
- `GET /api/a2a/taken`
- `GET /api/a2a/taken/:id`
- `POST /api/a2a/taken/:id/annuleren`

Uitvoeringsinterface:

- `/dashboard/a2a` voor taken/staat/s stream volgen en rookacties

</details>

<details>
<summary><b>🧪 End-to-end protocol validation</b></summary>

Controleer beide protocollen met echte clients:

```bash
npm run test:protocols:e2e
```

Dit controleert:

- MCP SDK client connectie/lstellen/overtrek
- A2A ontdekken/sturen/streamen/annuleren
- Voer cross-overigegevens aan in MCP-audit en A2A-taakbeheer-APIs

</details>

<details>
<summary><b>💳 Subscription Providers</b></summary>

### Claude Code (Pro/Max)

```bash
Dashboard → Leveranciers → Connect Claude Code
→ OAuth inloggen → Auto token vernieuwen
→ 5-uur + wekelijks quotaverschil

Modellen:
  cc/claude-opus-4-6
  cc/claude-sonnet-4-5-20250929
  cc/claude-haiku-4-5-20251001
```

**Pro Tip:** Gebruik Opus voor complexe taken, Sonnet voor snelheid. OmniRoute
houdt quotaverschillen per model bij!

### OpenAI Codex (Plus/Pro)

```bash
Dashboard → Leveranciers → Connect Codex
→ OAuth inloggen (poort 1455)
→ 5-uur + wekelijkse reset

Modellen:
  cx/gpt-5.2-codex
  cx/gpt-5.1-codex-max
```

#### Codex Account Beperking Beheer (5u + Wekelijk)

Elk Codex-account heeft nu beleidsuitschakelaars in `Dashboard → Leveranciers`:

- `5u` (AAN/UIT): handhaaf de 5-uurbegrensbeleidspolitiek.
- `Wekelijks` (AAN/UIT): de beleidseiwitten voor wekelijkse vensterstellingen
  forced.
- Schaduwbewithouding: wanneer een ingeschakeld venster >=90% gebruik bereikt,
  word dat account oversprongen.
- Rotatiegedrag: OmniRoute gaat automatisch naar de volgende geschikte Codex
  account.
- Resetgedrag: wanneer de provider `resetAt` tijd verstrijkt, word het account
  weer geschikt.

Scenario's:

- `5h AAN` + `Wekelijks AAN`: het account wordt oversprongen zodra elk venster
  de drempel bereikt.
- `5h UIT` + `Wekelijks AAN`: alleen wekelijkse gebruik kan het account
  blokkeren.
- `5h AAN` + `Wekelijks UIT`: alleen 5-uurgebruik kan het account blokkeren.
- `resetAt` is passed: het account herentreedt de rotatie automatisch (geen
  manuele heractivering vereist).

### Gemini CLI (gratis 180K per maand!)

```bash
Dashboard → Providers ↔ Connect Gemini CLI
 ↔ Google OAuth
 ↔ 180K voltooide taken/month + 1K/dag

Models:
  gc/gemini-3-flash-preview
  gc/gemini-2.5-pro
```

**Beste waarde:** Grote gratis laag! Gebruik deze voordat de betaalde niveaus.

### GitHub-copiloot

```bash
Dashboard → Providers → Connect GitHub
 → OAuth via GitHub
 → Maandelijkse reset (1e van maand)

Models:
  gh/gpt-5
  gh/claude-4.5-sonnet
  gh/gemini-3-pro
```

</details>

<details>
<summary><b>🔑 API Key Providers</b></summary>

### NVIDIA NIM (gratis ontwikkelaarstoeegang — 70+ modellen)

1. Aanmelden: [build.nvidia.com](https://build.nvidia.com)
2. Vrij API-sleutel (1000 inferentiecredits inbegrepen)
3. Dashboard → Provider toevoegen → NVIDIA NIM:
   - API-Sleutel: `nvapi-uw-sleutel`

**Modellen:** `nvidia/llama-3.3-70b-instruct`, `nvidia/mistral-7b-instruct` en
50+ meer

**Pro Tip:** OpenAI-gecompatible API — werkt zonder problemen met de
indelingsvormaat van OmniRoute!

### DeepSeek

1. Inschrijven: [platform.deepseek.com](https://platform.deepseek.com)
2. API-sleutel ophalen
3. Dashboard → Leverancier toevoegen → DeepSeek

**Modellen:** `deepseek/deepseek-chat`, `deepseek/deepseek-coder`

### Groq (Helemaal gratis beschikbaar!)

1. Inschrijven: [console.groq.com](https://console.groq.com)
2. API-sleutel ophalen (gratis niveau inbegrepen)
3. Dashboard → Leverancier toevoegen → Groq

**Modellen:** `groq/llama-3.3-70b`, `groq/mixtral-8x7b`

**Pro Tip:** Ultra-snel beredene meting — beste voor real-time coderen!

### OpenRouter (100+ Modellen)

1. Inschrijven: [openrouter.ai](https://openrouter.ai)
2. API-sleutel ophalen
3. Dashboard → Leverancier toevoegen → OpenRouter

**Modellen:** Toegang tot 100+ modellen van alle belangrijke leveranciers via
een enkel API-sleutel.

</details>

<details>
<summary><b>💰 Cheap Providers (Backup)</b></summary>

### GLM-4.7 (Dagelijkse reset, $0,6/1M)

1. Inschrijven: [Zhipu AI](https://open.bigmodel.cn/)
2. API-sleutel ophalen van Coding-Abonnement
3. Dashboard → API-sleutel toevoegen:
   - leverancier: `glm`
   - API-sleutel: `jouw-sleutel`

**Gebruik:** `glm/glm-4.7`

**Pro Tip:** Coding Plan biedt 3× quota van 1/7 kost! Reset dagelijks om 10:00
AM.

### MiniMax M2.1 (herstel na 5u, $0,20/1 miljoen)

1. Registreer: [MiniMax](https://www.minimax.io/)
2. API-sleutel ophalen
3. Dashboard → API-sleutel toevoegen

**Gebruik:** `minimax/MiniMax-M2.1`

**Pro Tip:** De goedkoopste optie voor lange context (1 miljoen tokens)!

### Kimi K2 ($9 per maand vast)

1. Abonneren: [Astronoom AI](https://platform.moonshot.ai/)
2. API-sleutel ophalen
3. Dashboard → API-sleutel toevoegen

**Gebruik:** `kimi/kimi-laatste`

**Pro Tip:** Vast $9 per maand voor 10 miljoen tokens = $0,90/1 miljoen
effectieve kosten!

</details>

<details>
<summary><b>🆓 FREE Providers (Emergency Backup)</b></summary>

### iFlow (5 gratis modellen via OAuth)

```bash
Dashboard → iFlow aansluiten
→ iFlow OAuth inloggen
→ Onbeperkt gebruik

Modellen:
  if/kimi-k2-denken
  if/qwen3-coder-plus
  if/glm-4.7
  if/minimax-m2
  if/deepseek-r1
```

### Qwen (4 gratis modellen via Apparaatcode)

```bash
DASHBOARD • Connect Qwen
• Toestemming voor apparaatcode
• Onbeperkt gebruik

Modellen:
  qw/qwen3-coder-plus
  qw/qwen3-coder-flash
```

### Kiro (Claude GRATIS)

```bash
DASHBOARD • Connect Kiro
• AWS Builder ID of Google/GitHub
• Onbeperkt gebruik

Modellen:
  kr/klasie-sonnet-4.5
  kr/klasie-haiku-4.5
```

</details>

<details>
<summary><b>🎨 Create Combos</b></summary>

### Voorbeeld 1: Maximize Subscription → Budget Back-up

```
DASHBOARD • Combos • Nieuw aanmaken

Naam: premium-code
Modellen:
  1. cc/klasie-opus-4.6 (Abonnement primer)
  2. glm/glm-4.7 (Betaalde backup, $0,6/1M)
  3. minimax/MiniMax-M2.1 (Goedkoopste valtijd, $0,20/1M)

Gebruiken in CLI: premium-code
```

### Voorbeeld 2: Free-Only (Zeer Goedkoop)

```
Naam: free-combo
Modellen:
  1. gc/gemini-3-flash-preview (180K gratis per maand)
  2. if/kimi-k2-denken (onbeperkt)
  3. qw/qwen3-coder-plus (onbeperkt)

Prijs: $0! Dat staat altijd zo!
```

</details>

<details>
<summary><b>🔧 CLI Integration</b></summary>

### Cursor-IDE

```
Instellingen • Modellen • Geavanceerd:
  OpenAI API Base URL: http://localhost:20128/v1
  OpenAI API-Sleutel: [uit de OmniRoute-dashboard]
  Model: cc/klasie-opus-4.6
```

### Claude Code

Gebruik de **CLI Tools** pagina in de dashboard voor één-klikconfiguratie, of
`~/.claude/gewijzigdeinstellingen.json` handmatig wijzig.

### Codex CLI

```bash
export OPENAI_BASE_URL="http://localhost:20128"
export OPENAI_API_KEY="uw-omniroute-Api-gesluipt"

codex "uw prompt"
```

### OpenClaw

**Optie 1 — Dashboard (aangewezen):**

```
DASHBOARD • CLI Tools • OpenClaw • Selecteer Model • Toepassen
```

**Optie 2 — Handmatig:** Wijzig `~/.openclaw/openclaw.json`:

```json
{
  "modellen": {
    "leveranciers": {
      "omniroute": {
        "baseUrl": "http://127.0.0.1:20128/v1",
        "apiKey": "sk_omniroute",
        "api": "openai-completions"
      }
    }
  }
}
```

> **Opmerking:** OpenClaw werkt alleen lokaal met OmniRoute. Gebruik `127.0.0.1`
> in plaats van `localhost` om IPv6 resolutieproblemen te voorkomen.

### Cline / Verdergaan / RooCode

```
Instellingen → API Configuratie:
  Levert die: OpenAI Compatible
  Basis-URL: http://localhost:20128/v1
  API-sleutel: [afspreken op OmniRoute-dashboard]
  Model: if/kimi-k2-thinking
```

### OpenCode

**Stap 1:** Voeg OmniRoute toe als een aangepast leverancier:

```bash
opencode
/connect
# Selecteer "Andere" → Voer ID in: "omniroute" → Voer jouw OmniRoute API-sleutel in
```

**Stap 2:** Maak/wijzig `opencode.json` in de root van jouw project:

```json
{
  "$schema": "https://opencode.ai/config.json",
  "leverancier": {
    "omniroute": {
      "npm": "@ai-sdk/openai-compatible",
      "naam": "OmniRoute",
      "opties": {
        "basisURL": "http://localhost:20128/v1"
      },
      "modellen": {
        "cc/claude-sonnet-4-20250514": { "naam": "Claude Sonnet 4" },
        "gg/gemini-2.5-pro": { "naam": "Gemini 2.5 Pro" },
        "if/kimi-k2-thinking": { "naam": "Kimi K2 (Gratis)" }
      }
    }
  }
}
```

**Stap 3:** Selecteer het model in OpenCode:

```bash
/models
# Selecteer een OmniRoute-model uit de lijst
```

> **Tip:** Voeg elk beschikbaar model toe in je OmniRoute-`/v1/models` eindpunt
> aan de `modellen`-sectie. Gebruik de indeling `leverancier/model-id` van jouw
> OmniRoute-dashboard.

</details>

---

## Problemen oplossen

<details>
<summary><b>Click to expand troubleshooting guide</b></summary>

**"Gedragemodelleerde taal voorzag geen berichten"**

- Provider-quotum is verbruikt → Controleer de quota tracker van de dashboard
- Oplossing: Gebruik fallback combi of overstap naar goedkopere laag

**Limiet stellen**

- Abonnement-quotum is uitgelopen → Fallback naar GLM/MiniMax
- Voeg combi toe: `cc/claude-opus-4-6 → glm/glm-4.7 → if/kimi-k2-thinking`

**OAuth-token is verlopen**

- Wordt automatisch vernieuwd door OmniRoute
- Als problemen blijven voorkomen: Dashboard → Leverancier → Herconnecteren

**Hoge kosten**

- Controleer gebruikersstatistieken in Ondermeld in Kosten
- Swijp primaire model naar GLM/MiniMax
- Gebruik gratis niveau (Gemini CLI, iFlow) voor niet-kritieke taken

**Dashboard/API poorten zijn onjuist**

- `POORT` is de standaard poort (en API-poort per standaard)
- `API_PORT` overschrijft alleen OpenAI-gecompatibile API-lijstluisteraar
- `DASHBOARD_PORT` overschrijft alleen dashboard/Next.js-lijstluisteraar
- Zet `NEXT_PUBLIC_BASE_URL` in op de URL van je dashboard/public (voor
  OAuth-teruggave)

**Cloud synchronisatie fouten**

- Controleer of `BASE_URL` naar je draaiende instantie wijst
- Controleer of `CLOUD_URL` naar je verwachte cloud-eindpunt wijst
- Houd `NEXT_PUBLIC_*` -waarden in overeenstemming met de waarden van de server

**Eerste inlog niet werkt**

- Controleer `INITIAL_PASSWORD` in `.env`
- Indien onbezet, valt terug op `123456`

**Geen aanvraaglogboeken**

- Zet `ENABLE_REQUEST_LOGS=true` in `.env`

**Verbindings test toont "onjuist" voor OpenAI-gecompatibele providers**

- Veel providers onthullen geen `/models` -eindpunt
- OmniRoute v1.0.6+ bevat back-up validatie via chat-annullingen.
- Zorg er ook voor dat de basis-URL de `/v1`-suffix bevat

### 🔒 OAuth op een Afstandige Server

<a name="oauth-on-a-remote-server"></a> <a name="oauth-em-servidor-remoto"></a>

> **⚠️ Belangrijk voor gebruikers die OmniRoute op een VPS, Docker of enige
> afstandige server** uitvoeren

#### Waarom faalt de Antigravity / Gemini CLI OAuth op afstandige servers?

De **Antigravity**- en **Gemini CLI**-aanbieders maken gebruik van **Google
OAuth 2.0**. Google vereist dat de `redirect_uri` in de OAuth-stroom exact
overeenkomt met een van de vooraf geregistreerde URI's in het apparaat van de
Google Cloud Console.

De OAuth-gegevens die zijn ingebouwd in OmniRoute zijn geregistreerd **voor
`localhost` alleen**. Wanneer u OmniRoute op een afstandige server (bijv.
`https://omniroute.myserver.com`) toegang geeft, weigert Google de authenticatie
met:

```
Fout 400: redirect_uri_mismatch
```

#### Oplossing: Configurer uw eigen OAuth-gegevens

U moet een **OAuth 2.0 Client ID** aanmaken in Google Cloud Console met de URI
van uw server.

#### Stap-voor-stap

**1. Open Google Cloud Console**

Ga naar:
[https://console.cloud.google.com/apis/credentials](https://console.cloud.google.com/apis/credentials)

**2. Maak een nieuwe OAuth 2.0 Client ID**

- Klik **"+ Nieuw credentieel aanmaken"** → **"OAuth client ID"**
- Toepassingstype: **"Webtoepassing"**
- Naam: iets wat u leuk vindt (bijv. `OmniRoute Afstand`)

**3. Voeg Geautoriseerde Redirect URI's toe**

In het **"Geautoriseerde redirect URI's"**-veld voegt u toe:

```
https://uwenigebol.com/callback
```

> Vervang `uwenigebol.com` met de domeinnaam of IP van uw server (inclusief de
> poort als nodig, bijv. `http://45.33.32.156:20128/callback`).

**4. Opslaan en kopiëren van de referenties**

Na het creëren, zal Google **Client ID** en **Client Secret** tonen.

**5. Vaststellen van omgevingsvariabelen**

In uw `.env` (of Docker-omgevingsvariabelen):

```bash
# Voor Antigravity:
ANTIGRAVITY_OAUTH_CLIENT_ID=your-client-id.apps.googleusercontent.com
ANTIGRAVITY_OAUTH_CLIENT_SECRET=GOCSPX-your-secret

# Voor Gemini CLI:
GEMINI_OAUTH_CLIENT_ID=your-client-id.apps.googleusercontent.com
GEMINI_OAUTH_CLIENT_SECRET=GOCSPX-your-secret
GEMINI_CLI_OAUTH_CLIENT_SECRET=GOCSPX-your-secret
```

**6. Herstarten van OmniRoute**

```bash
# npm:
npm run dev

# Docker:
docker restart omniroute
```

**7. Probeer opnieuw te verbinden**

Dashboard → Providers → Antigravity (of Gemini CLI) → OAuth

Google zal nu correct omleiden naar `https://your-server.com/callback`.

---

#### Tijdelijke oplossing (zonder eigen referenties)

Als u nu niet uw eigen referenties wilt configureren, kunt u nog steeds de
**manuele URL-flow** gebruiken:

1. OmniRoute opent de Google-autorisatie-URL
2. Na autorisatie probeert de Google omleiding naar `localhost` (wat in de
   remote server faalt)
3. **Kopieer de hele URL** uit uw browserversnelle (zelfs als de pagina niet
   wordt geladen)
4. Plak die URL in het veld dat wordt getoond in de modem van de verbinding in
   OmniRoute
5. Klik op **"Verbinden"**

> Dit werkt omdat de code in de URL autorisatie geldig is, ongeacht het feit of
> het omleidingspagina werd geladen.

---

<details>
<summary><b>🇧🇷 Versão em Português</b></summary>

#### Waarom faalt OAuth van Antigravity/Gemini CLI op remote servers?

De leveranciers **Antigravity** en **Gemini CLI** maken **Google OAuth 2.0**
gebruik voor authenticatie. Google vereist dat de `redirect_uri` gebruikt in de
OAuth-flux wordt **exact** een van de vooraf ingestelde URI's in het Google
Cloud Console van het toepassingsapplicatie.

Credenciales OAuth ingén dentro de OmniRoute están inscritas **sómente en
`localhost`**. Cuando accedas a OmniRoute en un servidor remoto (ex:
`https://omniroute.meuservidor.com`), Google rechaza la autenticación con:

```
Fout 400: redirect_uri_mismatch
```

#### Solución: Configura tus propias credenciales OAuth

Necesitas crear un **Cliente ID OAuth 2.0** en Google Cloud Console con la URI
de tu servidor.

#### Instrucciones paso a paso

**1. Accede a Google Cloud Console**

Abre:
[https://console.cloud.google.com/apis/credentials](https://console.cloud.google.com/apis/credentials)

**2. Crea un nuevo Cliente ID OAuth 2.0**

- Haz clic en **+ Crear credenciales"** → **"Cliente ID OAuth"**
- Tipo de aplicación: **"Aplicación web"**
- Nombre: elige cualquier nombre (ex: `OmniRoute Remoto`)

**3. Agrega las URIs de redireccionamiento autorizadas**

En el campo **"URIs de redireccionamiento autorizadas"**, agrega:

```
https://tu-servidor.com/callback
```

> Sustituye `tu-servidor.com` por el dominio o IP de tu servidor (incluye la
> puerta si es necesario, ex: `http://45.33.32.156:20128/callback`).

**4. Guarda y copia las credenciales**

Después de crear, Google mostrará el **ID del cliente** y el **Secret del
cliente**.

**5. Configura variables de entorno**

En tu `.env` (o en las variables de entorno de Docker):

```bash
# Para Antigravity:
ANTIGRAVITY_OAUTH_CLIENT_ID=tu-client-id.apps.googleusercontent.com
ANTIGRAVITY_OAUTH_CLIENT_SECRET=GOCSPX-tu-secret

# Para Gemini CLI:
GEMINI_OAUTH_CLIENT_ID=tu-client-id.apps.googleusercontent.com
GEMINI_OAUTH_CLIENT_SECRET=GOCSPX-tu-secret
GEMINI_CLI_OAUTH_CLIENT_SECRET=GOCSPX-tu-secret
```

**6. Herstart de OmniRoute**

```bash
# Als je npm gebruikt:
npm run dev

# Als je Docker gebruikt:
docker restart omniroute
```

**7. Pog Legal opnieuw verbinding**

Dashboard → Providers → Antigravity (of Gemini CLI) → OAuth

De Google zal nu correct naar `https://jouw-servicer.com/callback` worden
omgeleid en de verificatie zal werken.

---

#### Tijdelijke oplossing (zonder eigen inloggegevens configureren)

Als je nog niet je eigen inloggegevens wilt configureren, kun je nog steeds de
manuele **URL-flux** gebruiken:

1. De OmniRoute zal de autorisatie-URL van de Google openen
2. Als je hebt aangeklikt om aan te mogen, zal de Google proberen om naar
   `localhost` (die op de server-fout wordt aangeduid)
3. **Kopieer de volledige URL** uit je browser-adresstrook (zelfs als de pagina
   niet wordt geladen)
4. Plak deze URL in het veld dat in het connectiemodal verschijnt
5. Klik op **"Connect"**

> Deze oplossing werkt omdat het autorisatiecode in de URL onafhankelijk van het
> correct laden of niet van de redirect geldig is.

</details>

---

</details>

## 🛠️ Tech Stack

<details>
<summary><b>Click to expand tech stack details</b></summary>

- **Runtime**: Node.js 18–22 LTS (⚠️ Node.js 24+ is **niet ondersteund** —
  `better-sqlite3` native binaries zijn incompatibel)
- **Taal**: TypeScript 5.9 — **100% TypeScript** over `src/` en `open-sse/`
  (geen `any` in kernmodules sinds v2.0)
- **Framework**: Next.js 16 + React 19 + Tailwind CSS 4
- **Database**: LowDB (JSON) + SQLite (domeinstaten + proxy logs + MCP-audit +
  routingbeslissingen)
- **Schema's**: Zod (MCP-toolkontraktvalidatie, API-contracten)
- **Protocollen**: MCP (stdio/HTTP) + A2A v0.3 (JSON-RPC 2.0 + SSE)
- **Streamen**: Server-Sent Events (SSE)
- **Authenticatie**: OAuth 2.0 (PKCE) + JWT + API Keys + MCP Gescorde
  Autorisatie
- **Testen**: Node.js test runner + Vitest (900+ tests including unit,
  integratie, E2E)
- **CI/CD**: Octopus stapels (auto npm publiceren + Docker Hub bij release)
- **Website**: [omniroute.online](https://omniroute.online)
- **Pakket**:
  [npmjs.com/package/omniroute](https://www.npmjs.com/package/omniroute)
- **Docker**:
  [hub.docker.com/r/diegosouzapw/omniroute](https://hub.docker.com/r/diegosouzapw/omniroute)
- **Resilience**: Totaalherstel circuit breaker, exponentieel backoff,
  anti-thundering herd, TLS spoofing, auto-combo zelfherstel

</details>

---

## Documentatie

| Documenteren                                   | Beschrijving                                              |
| ---------------------------------------------- | --------------------------------------------------------- |
| [Gebruikersgids](docs/USER_GUIDE.md)           | Provider, combinaties, CLI-integratie, implementatie      |
| [API Reference](docs/API_REFERENCE.md)         | Alle eindpunten met voorbeelden                           |
| [MCP Server](open-sse/mcp-server/README.md)    | 16 MCP tools, ID-configs, Python/TS/Go clients            |
| [A2A Server](src/lib/a2a/README.md)            | JSON-RPC 2.0 protocol, vaardigheden, streamen, taakbeheer |
| [Auto-Combo Engine](docs/auto-combo.md)        | 6-factor scoringsysteem, mode packs, zelfherstel          |
| [Troubleshooptips](docs/TROUBLESHOOTING.md)    | Algemene problemen en oplossingen                         |
| [Architectuur](docs/ARCHITECTURE.md)           | Systeemarchitectuur en interna                            |
| [Contribueren](CONTRIBUTING.md)                | Ontwikkelingsomgeving en richtlijnen                      |
| [OpenAPI Spec](docs/openapi.yaml)              | OpenAPI 3.0-specificatie                                  |
| [Beveiligingsbeleid](SECURITY.md)              | Beroepsgeheimhouding en beveiligingspraktijken            |
| [VM Deployeren](docs/VM_DEPLOYMENT_GUIDE.md)   | Volledige handleiding: VM + nginx + Cloudflare setup      |
| [Features Gallery](docs/FEATURES.md)           | Visuele dashboardonderneming met afbeeldingen             |
| [Release Checklist](docs/RELEASE_CHECKLIST.md) | Stappen voor validatie vóór release                       |

---

## 🗺️ Roadmap

OmniRoute heeft **210+ aanwezig functies geplande** over verschillende
ontwikkelingsfases. Hier zijn de sleutelgebieden:

| Categorie                           | Geplande Eigenschappen | Highlighten                                                                                      |
| ----------------------------------- | ---------------------- | ------------------------------------------------------------------------------------------------ |
| 🧠 **Routering & Intelligentie**     | 25+                    | Laagdrempelige routering, taggebaseerde routering, quota voorbereiding, selectie van P2C-account |
| 🔒 **Beveiliging & Overeenstemming** | 20+                    | SSRF-verharding, geheimzinnige vermomming, beperkte rate per eindpunt, beheerderssleutel-scoping |
| 📊 **Observatie**                    | 15+                    | Integratie met OpenTelemetry, echte-time quota monitoring, kostenbewaking per model              |
| 🔄 **Provider Integraties**          | 20+                    | Dynamisch modelregister, provider cooldowns, meervoudige-account Codex, Copilot quotum parsing   |
| ⚡ **Prestaties**                    | 15+                    | Dubbele cache-laag, prompt cache, responsen cache, streaming-alive-houding, batch-API            |
| 🌐 **Ecosysteem**                    | 10+                    | WebSocket-API, configuratie-hot-reload, verspreide configuratie-opslag, commerciële modus        |

### 🔜 Komende Keren

- 🔗 **OpenCode Integratie** — Natieve provider ondersteuning voor het OpenCode
  AI-programmeer idee
- 🔗 **INTEGRATIE TRAE** — Volledige ondersteuning voor het TRAE
  AI-ontwikkelingsframework
- 📦 **Batch API** — Asynchrone batchverwerking voor bulkaanvragen
- 🎯 **Tag-Based Routing** — Verwerk aanvragen op basis van specifieke labels en
  metadata
- 💰 **Laagste-kost-strategie** — Selecteer automatisch de goedkoopste
  beschikbare provider

> 📝 Volledige functionaliteitspecificaties beschikbaar in
> [`docs/nieuwe-features/`](docs/new-features/) (217 gedetailleerde
> specificaties)

---

## 👥 Medewerkers

[![Medewerkers](https://contrib.rocks/image?repo=diegosouzapw/OmniRoute&max=100&columns=20&anon=1)](https://github.com/diegosouzapw/OmniRoute/graphs/contributors)

### Hoe kunt u bijdragen

1. Fork de repository
2. Maak uw feature-branch (`git checkout -b feature/amazing-feature`)
3. Committen uw veranderingen (`git commit -m 'Voeg verbazingwekkende feature
   toe'`)
4. Plakken naar de branch (`git push origin feature/amazing-feature`)
5. Open een_pull-verzoek

Zie [CONTRIBUTING.md](CONTRIBUTING.md) voor gedetailleerde handleidingen.

### Een Nieuwe Versie Uitbrengen

```bash
# Bepaal een release— npm publish gebeurt automatisch
gh release create v2.0.0 — title "v2.0.0" — generate-notes
```

---

## 📊 Stergeschiedenis

## Sterken over tijd

## [![Stergen over tijd](https://starchart.cc/diegosouzapw/OmniRoute.svg?variant=adaptive)](https://starchart.cc/diegosouzapw/OmniRoute)

## 🙏 Acknowledgments (Dankwoord)

Speciaal dank aan **[CLIProxyAPI](https://github.com/decolua/9router)[X36X] — de
oorspronkelijke Go-implemementatie die deze JavaScript-vertaling heeft
geïnspireerd.

Speciaal dank aan
**[9router](https://github.com/router-for-me/CLIProxyAPI)[X32X] door
[X38X][decolua]{2}[X52X] — het originele project dat deze fork heeft
geïnspireerd. OmniRoute bouwt voort op dat geweldige fundament met extra
functionaliteit, multifunctionele APIs en een volledige
TypeScript-reimplementatie.

---

## 📄 Licentie

Licentie MIT - zie [LICENSE](LICENSE) voor details.

---

<div align="center">
  <sub>Built with ❤️ for developers who code 24/7</sub>
  <br/>
  <sub><a href="https://omniroute.online">omniroute.online</a></sub>
</div>
<!-- GitHub Discussions enabled for community Q&A -->
