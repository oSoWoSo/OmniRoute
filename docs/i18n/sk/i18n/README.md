# 🚀 OmniRoute — Slobodný AI brána

### Ni vždy sa neprestávajte kódovať. Intelektuálna trasa do **zdarmaškých a lacnýchšie modelov AI** s automatickým pádom.

_Vaša všestranná API proxy — jeden koncový bod, 67+ zdrojov, nulový výpadek.
Teraz s **MCP & A2A** zoskupením agentov._

**Rozhovorové ukončenia • Zabudnuté vstupy • Generovanie obrazu • Video • Hudba
• Audio • Reranking • **Web vyhladanie** • MCP Server • A2A Protokoll • 100%
TypeScript**

---

<div align="center">

[![npm
verzia](https://img.shields.io/npm/v/omniroute?color=cb3837&logo=npm)](https://www.npmjs.com/package/omniroute)
[![npm
stiahnutia](https://img.shields.io/npm/dm/omniroute?color=cb3837&logo=npm&label=npm%20downloads)](https://www.npmjs.com/package/omniroute)
[![Docker
Hub](https://img.shields.io/docker/v/diegosouzapw/omniroute?label=Docker%20Hub&logo=docker&color=2496ED)](https://hub.docker.com/r/diegosouzapw/omniroute)
[![Docker
Pulls](https://img.shields.io/docker/pulls/diegosouzapw/omniroute?logo=docker&color=2496ED&label=docker%20pulls)](https://hub.docker.com/r/diegosouzapw/omniroute)
[![Licencia](https://img.shields.io/github/license/diegosouzapw/OmniRoute)](https://github.com/diegosouzapw/OmniRoute/blob/main/LICENSE)
[![Webová
stránka](https://img.shields.io/badge/Website-omniroute.online-blue?logo=google-chrome&logoColor=white)](https://omniroute.online)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-Community-25D366?logo=whatsapp&logoColor=white)](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

[🌐 Webová stránka](https://omniroute.online) • [🚀 Rýchle začatie](#-quick-start)
• [💡 Funkcie](#-key-features) • [📖 Dokumentácia](#-documentation) • [💰
Ceny](#-pricing-at-a-glance) • [💬
WhatsApp](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

</div>

🌐 **Aktívny v:** 🇺🇸 [Anglicky](README.md) | 🇧🇷 [Portugalsky
(Brazília)](docs/i18n/pt-BR/README.md) | 🇪🇸 [Španielsky](docs/i18n/es/README.md)
| 🇫🇷 [Francúzsky](docs/i18n/fr/README.md) | 🇮🇹
[Taliansky](docs/i18n/it/README.md) | 🇷🇺 [Ruština](docs/i18n/ru/README.md) | 🇨🇳
[Čínsky (ostrovní)](docs/i18n/zh-CN/README.md) | 🇩🇪
[Nemecky](docs/i18n/de/README.md) | 🇮🇳 [Hindi](docs/i18n/in/README.md) | 🇹🇭
[Thai](docs/i18n/th/README.md) | 🇺🇦 [Ukrajina](docs/i18n/uk-UA/README.md) | 🇸🇦
[Arabčina](docs/i18n/ar/README.md) | 🇯🇵 [Japončina](docs/i18n/ja/README.md) | 🇻🇳
[Vietnamčina](docs/i18n/vi/README.md) | 🇧🇬 [Bulharčina](docs/i18n/bg/README.md)
| 🇩🇰 [Dánsky](docs/i18n/da/README.md) | 🇫🇮 [Fínsky](docs/i18n/fi/README.md) | 🇮🇱
[Hébridština](docs/i18n/he/README.md) | 🇭🇺 [Maďarčina](docs/i18n/hu/README.md) |
🇮🇩 [Indonézsky](docs/i18n/id/README.md) | 🇰🇷 [Korejčina](docs/i18n/ko/README.md)
| 🇲🇾 [Malajálamsky](docs/i18n/ms/README.md) | 🇳🇱
[Holandčina](docs/i18n/nl/README.md) | 🇳🇴 [Nórsky](docs/i18n/no/README.md) | 🇵🇹
[Portugalsky (Portugalsko)](docs/i18n/pt/README.md) | 🇷🇴
[Rumunčina](docs/i18n/ro/README.md) | 🇵🇱 [Poľština](docs/i18n/pl/README.md) | 🇸🇰
[Slovenčina](docs/i18n/sk/README.md) | 🇸🇪 [Švédsky](docs/i18n/sv/README.md) | 🇵🇭
[Filipínština](docs/i18n/phi/README.md) | 🇨🇿 [Čeština](docs/i18n/cs/README.md)

---

## 🆕 O čom je čerstva v verzi 3.0.0

> **Zlepšujete zo verzie 2.9.5?** — Pozrite sa tiež do [plného
> CHANGELOG](CHANGELOG.md#300--2026-03-22-release-candidate--not-yet-merged-to-main)
> pre všetky zmeny.

| Oblast                                     | Zmena                                                                                                                                           |
| ------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| 🔒 **Kódovy bezpečnostný nástrojom CodeQL** | Vyriešilo 10+ alertov CodeQL: polynomial-redos, nebezpečná náhodnosť, vyberanie shellov  medzi poškodeniami                                     |
| ✅ **Overenie trasy**                       | Všetky 176 API trasy teraz ověřované s pridelenými schémami Zod + `validácia tlačidiel()` — CI `skontrolujte cestu: overenie trasy: t06` uspelo |
| 🐛 **omniModel Značka úniku**               | Interné `tagy <omnimodel>` už netŕžia pre klientov po streamovaní premenených rezonancach (#585)</omnimodel>                                    |
| 🔑 **Registerované Klávesové API**          | Automatické poskytovanie API kláv s per-providerovským údajom quoita, idempotence, úschovávaním SHA-256 a nepovinnou hláškou o GitHub (#585)    |
| 🎨 **Obrazové ikonkyProvider**              | 130+ poskytovateľské logá via `@lobehub/icons` (SVG) so PNG → zjavná fallback chaina                                                            |
| 🔄 **Model Auto-Sync**                      | 24h schéma a ručná UI prevodca na synchrovanie modelových zoznamov pre vstavenejčie a zariadenia OpenAI-kompatibilných poskytovateľov           |
| 🌐 **OpenCode Zen/Go**                      | Dve nové poskytovateľské služby od @kang-heewon cez PR #530: za niektoré úplne zadarmo + predplatené rata pomocou `OpencodeExecutor`            |
| 🐛 **Gemini CLI OAuth**                     | Interaktívny chybový hlásenie, keď `GEMINI_OAUTH_CLIENT_SECRET/X49X] je chýbajúce v Docker (bol kriptický Google chybový hlásenie)              |
| 🐛 **OpenCode konfigurácia**                | `saveOpenCodeConfig()` teraz správne píše TOML do `XDG_CONFIG_HOME`                                                                             |
| 🐛 **Pripínaná modelová aktualizácia**      | `body.model` správne nastavuje `pinnedModel` pri ochrane kontextu-kachy                                                                         |
| 🐛 **Codex/Clad loop**                      | `tool_result` bloky teraz premávajú na text, aby sa zastavili nekonečné smery                                                                   |
| 🐛 **Prihlásenie redirekcia**               | Prihlásenie nezáhadá po tom, ako prekonať skokypasswort                                                                                         |
| 🐛 **Windows cesty**                        | MSYS2/Git-Bash cesty (`/c/...`) sa normalizujú na `C:\...`                                                                                      |

---

## 🖼️ Glavné Dashboard

<div align="center">
  <img src="./docs/screenshots/MainOmniRoute.png" alt="OmniRoute Dashboard" width="800"/>
</div>

---

## 📸 Dashboard Preview

<details>
<summary><b>Click to see dashboard screenshots</b></summary>

| Stránka                   | Zrkad                                                    |
| ------------------------- | -------------------------------------------------------- |
| [D0E1E]Dodávatelia        | ![Dodávatelia](docs/screenshots/01-providers.png)        |
| [D0E8E]Kombinácie         | ![Kombinácie](docs/screenshots/02-combos.png)            |
| [D0E0D]Analýzy            | ![Analýzy](docs/screenshots/03-analytics.png)            |
| [D0E8E]Zdravie            | ![Zdravie](docs/screenshots/04-health.png)               |
| [D0E0F]Prekladateľ        | ![Prekladateľ](docs/screenshots/05-translator.png)       |
| [D0E8E]Nastavenia         | ![Nastavenia](docs/screenshots/06-settings.png)          |
| [D0E9F]Klientské nástroje | ![Klientské nástroje](docs/screenshots/07-cli-tools.png) |
| [D00F1]Nákupné záznamy    | ![Nákupné záznamy](docs/screenshots/08-usage.png)        |
| [D0E4F]Koncové body       | ![Koncové body](docs/screenshots/09-endpoint.png)        |

</details>

---

### Rovník AI Dodávateľ pre vaše obľúbené agentov\

_Pridajte ktorékoľvek AI-poháňané IDE alebo CLI nástrojom cez OmniRoute —
bezplatný API gateway pre neomezené kódovanie._

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

<sub>📡 Všetky agenti sa spájajú cez <code>http://localhost:20128/v1</code> alebo
<code>http://cloud.omniroute.online/v1</code> — jedna konfigurácia, neomezené
modely a kvóty</sub>

---

## 🤔 Prečo OmniRoute?

**Vytiahnite sa z odpadu a necestujte limity:**

- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Kvóta úplaty uplyná nepoužité každý mesiac
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Limity úderníky vás cez kódovanie preruší
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Nepriaznivé APIs ($20-50/ mesiac na poskytovateľa)
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Manuálne přepájanie medzi poskytovateľmi

**OmniRoute rieši to:**

- ✅ **Maximizujte používateľské účty** - Monitor kvóty, použijte všetko pred
  resetom
- ✅ **Automatizované fallback** — Úplaty → API Kľúč → Ľahký → Zdarma, bez
  prestávky
- ✅ **Multi-účel** - Obíhací kruh medzi účtami na poskytovateľa
- ✅ **Universal** - Pracuje so Claude Code, Codex, Gemini CLI, Cursor, Cline,
  OpenClaw, akýkoľvek CLI nástrojom

---

## 📧 Podpora

> 💬 **Príspevkujte k našej komunitnej!** [WhatsApp
> Skupína](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t) —
> Pochopujte sa, zdieľajte tipy a zostupte informovaní

- **Webová stránka**: [omniroute.online](https://omniroute.online)
- **GitHub**:
  [github.com/diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute)
- **Problémy**:
  [github.com/diegosouzapw/OmniRoute/issues](https://github.com/diegosouzapw/OmniRoute/issues)
- **WhatsApp**: [Skupína
  komunity](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)
- **Prispievanie**: Pozrite na [CONTRIBUTING.md](CONTRIBUTING.md), otvorte PR,
  alebo si vyberte `dobre priečinou tému`
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

## Ako to funguje

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
- **Reakcia Sanitizácia** — Odstriese nieštandardné polia (`x_groq`,
  `usage_breakdown`, `service_tier`) ktoré breaking OpenAI SDK v1.83+
- **Rólová normalizácia** — Zmeni `developer` → `system` pre nerodinné
  poskytovateľstvá; `system` → `user` pre GLM/ERNIE
- **Vydanie značk značenia** — Vysledí `<think>` bloky z modelov ako DeepSeek R1
  do stanodnizovanych `reasoning_content`</think>
- **Štruktúrované Vystup pre Gemini** — `json_schema` →
  `responseMimeType`/`responseSchema` automatic conversion
- **Preosvedčení `stream` v podstate `false`** — Zodpovedá OpenAI spec,
  vyhľadávajúc nepredpokladanú SSE v Python/Rust/Go SDK-och

</details>

<details>
<summary><b>🌐 3. "My AI provider blocks my region/country"</b></summary>

Poskytovatelia ako OpenAI/Codex zabraňujú prístupu z určených geografických
oblastiach. Užívateľia sa stretávajú s chybami ako
`unsupported_country_region_territory` počas OAuth a API pripojenia. Táto vec je
čiastočne pre človekov z rozvojových krajín

**How OmniRoute solves it:**

- **Nastavovanie tresťa cez 3 úrovne** — Nastaviteľný tresť na 3 úrovniach:
  globálny (všetky zosielania), na úrovni poskytovateľa (iba jeden poskytovateľ)
  a na úrovni spojenia/clanky
- ** Farbované ozdoby proxy** — Súvislé indikátory: 🟢 Globálne proxy, 🟡
  Rozhranisko proxy, 🔵 spojenie proxy, vždy môžete zobraziť IP
- **Obmen OAuth Token cez tresť** — Fluk Oauth tiež prechádza cez proxy, rieši
  `unsupported_country_region_territory`
- **Testy spojenia cez tresť** — Tests spojenia používajú nastavený tresť
  (ničmenejší bezprostredný bypass)
- **Poddporučiný SOCs5** — Plný podpúchý sokov pre odnosné zosielania
- **Falšovanie otisku TLS** — Browserový otisk TLS cez `wreq-js` prekonať
  detekciu Robot-ov
- ** 🔏 Matching Fingerprint CLI** — Prestavávanie hlavičiek a polí tela aby bolo
  zhodné s pôvodnými binárnymi prvky v klientskej strane. Nastavený IP je
  zachovaný — dostanete simultančné ** a ** IP zakrývanie

</details>

<details>
<summary><b>🆓 4. "I want to use AI for coding but I have no money"</b></summary>

Niektorí nedokážu zaplatiť 20–200/month za AI subskripcie. Studenti, vývojárí z
rozvojových krajín, hobbisté a freelanci potrebujú prístup k kvalitným modelom.

**How OmniRoute solves it:**

- **Zakladné prvky sú zdarma built-in** — Rozhranie pre 100% zdarma poskytuje
  služby: iFlow (5 bezplatné modely pomedzi OAuth: kimi-k2-thinking,
  qwen3-coder-plus, deepseek-r1, minimax-m2, kimi-k2), Qwen(4 neomezené modely:
  qwen3-coder-plus, qwen3-coder-flash, qwen3-coder-next, vision-model), Kiro
  (Claude + AWS Builder ID pre zľavíny), Gemini CLI (180K tokenov / mesiac
  zadarmo)
- **Ollama Cloud súkromná** — Súkromne hoslený model Ollama na `api.ollama.com`
  súkromným „ Light útok“ zľavíny ; použíjte `ollamacloud/<model>`
  Prefix</model>
- **Kombinácie pomocou skratiek** — Reťaz `gc/gemini-3-flash →
  if/kimi-k2-thinking → qw/qwen3-coder-plus` = $0/month s bezposlednou
  zastavením
- **NVIDIA NIM bezplatné prístup** — ~40 RPM Dev-free vek bez konkrétnych
  limitov na 70+ modelov na build.nvidia.com (Prechod z kreditov na skutočné
  omezení)
- Strategies preinicia čnosť: ** CostOptimized Strategy ** — Routing strategy
  that automatically chooses the cheapest available provider

</details>

<details>
<summary><b>🔒 5. "I need to protect my AI gateway from unauthorized access"</b></summary>

Pri vystupovaní AI brány do sieti (LAN, VPS, Docker), každý s adresou má možnosť
spotrebovať vývojársky tokeny/quota. Bez ochrany sa APIs nachádzajú v riziku
zneužívania, vpájania promptov a zneužitia.

**How OmniRoute solves it:**

- **Správa API keyov ** — Generovanie, rotácia a skoping pre poskytovateľa s
  dedikovanou `nástrojom/správou API ` stránkou
- **Oprávnania na úrovni modelu ** — Restrikt API keyov pre konkrétne modely
  (`openai/*`, wildcardové vzory), s možnosťou Povoliť všetko/Zakážiť nastavovať
- **Ochrana URL koncových bodov API ** — Opakujte klúčik pre `/v1/models` a
  zablokujte konkrétne poskytovateľa zo zoznamu
- **Ochrana autentifikácie + prevencia CSRF ** — Všetky dashboard cesty chránené
  s `swithAuth` middleware + CSRF tokenami
- **Limitátor rýchlosti ** — Rýchloosť na úrovni IP s nastaviteľnými oknom
- **Filterovanie IP ** — Povolený/zablokovaný zoznam dôležitých záujmov
- **Stránka proti vpájaniu vstupných podnétokov ** — Sanitácia proti škodlivým
  vzorom vstupných podnietokov
- **Šifrovanie AES-256-GCM ** — Kredenciály šifrované na prirodzenom mieste

</details>

<details>
<summary><b>🛑 6. "My provider went down and I lost my coding flow"</b></summary>

Prodávajcie poskytovateľmi môžu stať nestabilné, vrátiť 5xx chyby alebo narazím
na dočasné limity. Ak sa vývojár závisí na jedinom poskytovateľovi, sú onedlho
prerazený. Bez zástrčiek zostávajú opakovane zmätie zopakovane až prehra
aplikácia

**How OmniRoute solves it:**

- **Zástrčka na úrovni modelu ** — Auto-otvárací/zatknutie s nastaviteľnými
  prahmi a chladením (Zastavené/Príležitostné/Halasné), skutočné na úrovni
  modelu aby sa zabránilo prehráždám odseknutým zostavám
- **Eksponenciálne opakované odôvodnenia ** — Pokračujúce zlačné prepukávanie
- **Anti-horda ** — Mutex + slučky chránenia pred súčasnými pokúskami o
  prehratie súladku
- **Súhra párováním s padnutými ťahmi ** — Ak prvotný poskytovateľ vyhasne,
  automaticky sa presúva súhra bez zásahu
- **Súhra zástrčkami ** — Auto-vynasadenie prechádajúcich poskytovateľov v rámci
  párovanej súhry
- **Panel zdravotného stavu ** — Kontrola dostupnosti, zástrčkové stavy,
  blokovanie, dáta zdieľania a p50/p95/p99 zdieľanie zdržanlivosti

</details>

<details>
<summary><b>🔧 7. "Configuring each AI tool is tedious and repetitive"</b></summary>

Vývojári používajú Cursor, Claude Kód, Codex CLI, OpenClaw, Gemini CLI, Kilo
Kód... Každý nástroj potrebujú iný konfigurovace (adresa konca koncového bodo,
klúče, model). Zobnovovanie čoznivie z mienenia poskytovateľa alebo modely je
odpadom času.

**How OmniRoute solves it:**

- **CLI Tools Dashboard** — Vyhrazená stránka s jednorázovou konfiguráciou pre
  Claude Code, Codex CLI, OpenClaw, Kilo Code, Antigravity, Cline
- **GitHub Copilot Config Generator** — Generuje `chatLanguageModels.json` pre
  VS Code s hromadnou výběrem modelu
- **Onboarding Wizard** — Navedený 4-krokový setup pre prvotní používateľov
- **One endpoint, all models** — Konfigurujte `http://localhost:20128/v1` raz,
  prístup cez 67+ poskytníkov

</details>

<details>
<summary><b>🔑 8. "Managing OAuth tokens from multiple providers is hell"</b></summary>

Claude Code, Codex, Gemini CLI, Copilot — všetky používajú OAuth 2.0 s
prechodnými tokenmi. Vývojári musia neustále re-authentikaovať, zápasia s
`chybným tokenom klienta`, `odkazovaním na nesprávne url` a s problémami na
vzdialených serveroch. OAuth na LAN/VPS je zvlášť problematizované.

**How OmniRoute solves it:**

- **Auto Token Refresh** — Prechodné tokeny sa automaticky obnúbia v pohľade na
  expiráciu
- **OAuth 2.0 (PKCE) Built-in** — Automatický tok pre Claude Code, Codex, Gemini
  CLI, Copilot, Kiro, Qwen, iFlow
- **Multi-Account OAuth** — Viacnásobné účty na poskytníku cez JWT/ID token
- **OAuth LAN/Remote Fix** — Detekcia súkromých IP adres pre `redirect_uri` a
  ručná URL móda pre vzdialené servery
- **OAuth Behind Nginx** — Používa `window.location.origin` pre kompatibilitu s
  reverznym proxy
- **Remote OAuth Guide** — Krátke kroky na vytvorenie Google Cloud credentials v
  VPS/Docker

</details>

<details>
<summary><b>📊 9. "I don't know how much I'm spending or where"</b></summary>

Vývojári používajú viacnásobne preplatné poskytniky, ale nemajú jednotný prehľad
výdavkov. Každý poskytník má vlastnú obrazovku na účtovanie, ale nie je jediná
obecná obnova.

**How OmniRoute solves it:**

- **Cost Analytics Dashboard** — Nákladová analíza a rozpočet v miernom časovom
  odseku pre poskytníka
- **Budget Limits per Tier** — Rozpočetne limity na úrovni viednosti, ktoré
  aktivujú automatický prevrátenie
- **Per-Model Pricing Configuration** — Konfigurovateľné ceny na modelár
- **Usage Statistics Per API Key** — Počtet požadavkov a posledné použitie v
  miernom časovom odseku pre API klíč
- **Analytics Dashboard** — Statové karty, modelový používateľský graf, tabuľka
  poskytníkov s úspešnosťou a časnými zoskokmi

</details>

<details>
<summary><b>🐛 10. "I can't diagnose errors and problems in AI calls"</b></summary>

When a call fails, the dev doesn't know if it was a rate limit, expired token,
wrong format, or provider error. Fragmented logs across different terminals.
Without observability, debugging is trial-and-error.

**How OmniRoute solves it:**

- **Unified Logs Dashboard** — 4 tabs: Request Logs, Proxy Logs, Audit Logs,
  Console
- **Console Log Viewer** — Real-time terminal-style viewer with color-coded
  levels, auto-scroll, search, filter
- **SQLite Proxy Logs** — Persistent logs that survive server restarts
- **Translator Playground** — 4 debugging modes: Playground (format
  translation), Chat Tester (round-trip), Test Bench (batch), Live Monitor
  (real-time)
- **Request Telemetry** — p50/p95/p99 latency + X-Request-Id tracing
- **File-Based Logging with Rotation** — Console interceptor captures everything
  to JSON log with size-based rotation
- **System Info Report** — `npm run system-info` generates `system-info.txt`
  with your full environment (Node version, OmniRoute version, OS, CLI tools,
  Docker/PM2 status). Attach it when reporting issues for instant triage.

</details>

<details>
<summary><b>🏗️ 11. "Deploying and maintaining the gateway is complex"</b></summary>

Installing, configuring, and maintaining an AI proxy across different
environments (local, VPS, Docker, cloud) is labor-intensive. Problems like
hardcoded paths, `EACCES` on directories, port conflicts, and cross-platform
builds add friction.

**How OmniRoute solves it:**

- **npm global install** — `npm install -g omniroute && omniroute` — done
- **Docker Multi-Platform** — AMD64 + ARM64 native (Apple Silicon, AWS Graviton,
  Raspberry Pi)
- **Docker Compose Profiles** — `base` (no CLI tools) and `cli` (with Claude
  Code, Codex, OpenClaw)
- **Electron Desktop App** — Native app for Windows/macOS/Linux with system
  tray, auto-start, offline mode
- **Split-Port Mode** — API and Dashboard on separate ports for advanced
  scenarios (reverse proxy, container networking)
- **Cloud Sync** — Config synchronization across devices via Cloudflare Workers
- **DB Backups** — Automatic backup, restore, export and import of all settings

</details>

<details>
<summary><b>🌍 12. "The interface is English-only and my team doesn't speak English"</b></summary>

Teams in non-English-speaking countries, especially in Latin America, Asia, and
Europe, struggle with English-only interfaces. Language barriers reduce adoption
and increase configuration errors.

**How OmniRoute solves it:**

- X0X]Dáštard ** i18n — 30 jazykov[X32X] — Všechny 500+ klícov preložené,
  vrátane arabského, bulharského, dánština, nemeckého, španielskeho, fínskej,
  francúzštiny, hebrejčiny, hindštiny, maďarčiny, indonézčiny, taliančiny,
  japonského, korejčiny, malajštiny, holandčiny, norštiny, poľštiny,
  portugalčiny (PT/BR), rumunčiny, ruské, slovenčiny, švédčiny, thajčiny,
  ukrajinského, vietnamského a čínskej, filipínskej, angličtiny
- X0X]RTL podporu** — Ľavicovo prúdováť support pre arabský a hebrejčinu
- X0X]Multi-Language READMEs** — 30 úplných preloženého dokumentačných prepisov
- X0X]Jazykovú Selektor** — Globálna ikona v hlavičke pre reálny čas preradienie

</details>

<details>
<summary><b>🔄 13. "I need more than chat — I need embeddings, images, audio"</b></summary>

Ďalej nepreberajú chatové doplnenia len. Aplikácie majú na rozdiel z generovať
obrazy, transkribovať zvuk, vytvárať veľmi podobnosť pre RAG, ponovného vlažení
dokumentov a moderovačný obsah. Každý API má svoju rôznu koncovú či priečinčku a
formát.

**How OmniRoute solves it:**

- X0X]Zálohovanie** — `/v1/embeddings` s 6 poskytovateľmi a 9+ modelami
- X0X]Obrázky Generáciu** — `/v1/images/generations` s 10 poskytovateľmi a 20+
  modelov (OpenAI, xAI, Zajtraj, Kučková, Nebius, Hyperbolická, NanoBanana,
  Antigravitačná, SD WebUI, ComfyUI)
- X0X]Text-to-Video** — `/v1/videos/generations` — ComfyUI (AnimateDiff, SVD) a
  SD WebUI
- X0X]Text-to-Hudba** — `/v1/music/generations` — ComfyUI (Stable Audio Open,
  HudobnáGenerator)
- X0X]Audio Transkripci** — `/v1/audio/transcriptions` — Whisper + Nvidia NIM,
  HuggingFace, Quénsky, Kwenz
- X0X]Text-to-Speech** — `/v1/audio/speech` — ElevenLabs, Nvidia NIM,
  HuggingFace, Stvoření, Totoro, Quénsiky, **Inworld**, **Cartesia**,
  **PlayHT**, + existujúcich poskytovateľov
- X0X]Moderáciu** — `/v1/moderations` — Súkromnosť obsahu
- X0X]Reranking** — `/v1/rerank` — Reranking dokumentu relevancie
- X0X]Odpovede API** — Plná `/v1/responses` support pre Codex

</details>

<details>
<summary><b>🧪 14. "I have no way to test and compare quality across models"</b></summary>

Programátori chcú vedieť, aký model je najvhodnejší pre ich používateľské
priemery — kóda, preklad, rozumie, ale prirovnanie rýchlo manuálna. Keďže nie je
jedného pomocníka.

**How OmniRoute solves it:**

- X0X]Zhodnotenie LLM** — Zlato set tesenie s pomocnými prípadosmi prekrytými:
  pozdrav, matematika, geografia, kód generovať, JSON bezchybný, preklad,
  markdown, odmietnutie vstupného.
- X0X]Štyri strategie Match** — `exakt`, `obsahuje`, `regex`, `článok` (JS
  funkcie)
- X0X]Preklad Playground Test Bench** — Batch tesenie s viacerými vstupnými
  vstupami a očakávaným výsledkom, prevzatím poskytovateľov preporovnanie
- **Konferenčný Tesťovac** — Plná rýchlosporná cesta s vizuálnym zobrazením
  odpovedí
- **Živé Monitorovanie** — Reálne streamy všetkých požiadaviek prechádzajúcich
  cez proxy

</details>

<details>
<summary><b>📈 15. "I need to scale without losing performance"</b></summary>

Pri rastúcom objemu požiadaviek, bez Použitného pamäte ste iste otázky generujú
duplicitné náklady. Bez idempotencie duplicitné požiadavky zatienenia procesov.
Rýchlostné omeškanie, ktoré musia byť dodržované pre každého dodávateľa.

**How OmniRoute solves it:**

- **Semanticná Cache** — Dvojpriečniková cache (signatúra +semantic) znižuje
  náklady a prihladnosť
- **Idempotencia Požiadaviek** — 5s okno deduplikácie pre túžité požiadavky
- **Rozpoznávanie Rýchlosti Omezení** — Per-provider RPM, miním vymedzovacie a
  maximum súčasné sledovanie
- **Upravitelné Rýchlosti Omezení** — Konfigurované výchozije v Nastavenia →
  Odolnosť s ponechávaním
- **Validácia Kľúča k API Cache** — 3-tier cache pre výrobnu výkonnosť
- **Zdravotný Dashboard s Telemetry** — p50/p95/p99 prihladnosť, cache
  informácie, zostaranie

</details>

<details>
<summary><b>🤖 16. "I want to control model behavior globally"</b></summary>

Programátori, ktorí chcú obdržať všetky odpovede v konkrétnej jazyke,
súvisiacich s konkrétne tonale, alebo, ktorí chcú obmedzovať rozumu značky.
Konfiguráciu v každom riadiacom programu/požiadavku je praktickeľne
nepriepravené.

**How OmniRoute solves it:**

- **Systémová Injectia Prompt** — Globálna prompt aplikovaná na všetky
  požiadavky
- **Overovací Budget Rozhodnutie[Test]** — Rozumenie znamienok alokcia kontrola
  pripojenie
- **6 Routing Stratégií** — Globálne stratégie, ktoré určujú, ako sa požiadavky
  rozpočtujú
- **Wildcard Router** — `provider/*` vzory odvádzajú dynamicko na akýkoľvek
  poskytovateľ
- **enable/Disable Toggle Combo** — Vypnenie kombinácií bezpozeravne z dashboard
- **Toggle Dostupnosti** — Aktivovať/deaktivovať všetky spojenia pre
  poskytovateľ pomocou jedného tlačidla
- **Zablokovaní Poskytovateľ** — Nezáležitosť konkrétne poskytovateľa zo
  `/v1/models`

</details>

<details>
<summary><b>🧰 17. "I need MCP tools as first-class product capabilities"</b></summary>

Mnoho Inteligentných brán prenajatý MCP iba ako neviditeľný implementáciu
detailov. Tímu potrebujú viditeľná, spracovateľná operatívna vrstva.

**How OmniRoute solves it:**

- Navigačný panel MCP a endpointový protokoly
- Dedikovaný stránka pre zdlžiteľnosť MCP s procesom, nástromi, rozsahu a
  auditom
- Integrovaný rýchlejší start pre [komniroute --mcp] a zákaznícku prihlášku

</details>

<details>
<summary><b>🧠 18. "I need A2A orchestration with sync + stream task paths"</b></summary>

Pri agentových pracovných postupoch je potrebné používať priamo návzorované a
dlhodobé vykonávanie streamovaných execúcií s kontrolou životného cyklu.

**How OmniRoute solves it:**

- A2A JSON-RPC endpoint (POST /a2a[X]) so zasielkovou [mesáž/send] a
  [mesiég/stream]
- SSE streamovaním s šírením koncového stavu
- API života úloh pre [zadania/get] a [zadania/zakáže]

</details>

<details>
<summary><b>🛰️ 19. "I need real MCP process health, not guessed status"</b></summary>

Operatívnejmu tímu treba vedieť, či je MCP skutočne aktivný, ne len, či je možné
danú API dosiahnuť.

**How OmniRoute solves it:**

- Súbor pre dynamické srdcové tepo s PID, časovými razitkami, prenosnou úložkou,
  počtom nástrojov a režimom rozsahu
- API MCP kombinujúce dynamické srdcové tepo + nedávnu aktivitu
- Informačné stredisko kariet pre proces/dochovanie/čerstvotlivosť srdcového
  tepa

</details>

<details>
<summary><b>📋 20. "I need auditable MCP tool execution"</b></summary>

Keď nástroje zmietajú konfiguráciu alebo aktivujú operačné akcie, tímy potřebujú
forenznú sledovateľnosť.

**How OmniRoute solves it:**

- SQLite zasadený audit logujúca volanie nástrojov MCP
- Cestovanie podľa nástroja, podľa úspechu/neskúsenia, kľúčom API a čiastkovými
  stránkami
- Informačná tábla na dashboard so štatistickými endpointami pre automatáciu

</details>

<details>
<summary><b>🔐 21. "I need scoped MCP permissions per integration"</b></summary>

Mäkkšie práca s minimálnymi oprávneniami pre kategórie nástrojov pre rozdílnych
klientov.

**How OmniRoute solves it:**

- 9 zreteľných rozsahov MCP pre ovládaný prístup k zariadeniam
- Zatváranie a viditeľnosť zhraniať SCP v UI MCP
- Bezpečný defaultný režim pre operátorov kľúčové nástroje

</details>

<details>
<summary><b>⚙️ 22. "I need operational controls without redeploying"</b></summary>

Tím potrebujú rýchle prebudenie výkonu s výnimkami alebo náklady.

**How OmniRoute solves it:**

- Súboru pomocou kombinóra aktivovať priamo od panelu MCP
- Použitie profilov odolnosti z preddefinovaných skupín zásad
- Obnoviť stav prekrycíkov zo tej samej panelu operácií

</details>

<details>
<summary><b>🔄 23. "I need live A2A task lifecycle visibility and cancellation"</b></summary>

Bez viditeľnosti cyklu životnosti úlohy sa stanú ťažké tria úloh

**How OmniRoute solves it:**

- Zobrazenie/zadaniefiltr zo štátu/talentu s pagsaciou
- Vloženie údajov o úlohách, udalosti, a artefaktov
- Pokyn na zrušenie úlohy so zárukou a použitím UI

</details>

<details>
<summary><b>🌊 24. "I need active stream metrics for A2A load"</b></summary>

Témy prebehnutia vyžadujú funkčné vedomosti pre aktívne spojenie konkrétnosti a
prepojenie v reálnom čase.

**How OmniRoute solves it:**

- Aktívne priečiarečky súčasných a účinne súčasných v paneli A2A
- Posledná štartovací čas a počet použitia v každom štáte
- Karty A2A na monitorovanie real-time pracoviska

</details>

<details>
<summary><b>🪪 25. "I need standard agent discovery for clients"</b></summary>

Zameriavení zákazníci a orchestrovari potrebujú strojový rozpoznaveľný datový
metadata pre načítanie.

**How OmniRoute solves it:**

- Agent Card vysiela v `/.well-known/agent.json`
- Možnosti a zručnosti zobrazované v nastavení systému
- API pre A2A status obsahuje metadata pre automatizáciu

</details>

<details>
<summary><b>🧭 26. "I need protocol discoverability in the product UX"</b></summary>

Ak používateľia nedať objaviť povrchy protokolu, poklesá úroveň adoptácie a
podporu kvality.

**How OmniRoute solves it:**

- Zjednocený rozkladník **Koncových bodov** s panelmi pre Proxy, MCP, A2A a API
  Koncové body
- Kariéry stavových nastavení v ploche pre MCP a A2A (Online/Offline)
- Obrázky na prehľad odzách na dedikované taby pre riadenie

</details>

<details>
<summary><b>🧪 27. "I need end-to-end protocol validation with real clients"</b></summary>

Parádné testy nie sú dostačujúce na overenie kompatibility protokolu pred
vydavením.

**How OmniRoute solves it:**

- Kombinovaný nástrojový súbor, ktorý spustí aplikáciu a používa reálny SDK
  klienta pre transport
- Testy klienta A2A pre vyhľadávanie, zoslanie, streamovanie, získanie a
  zrušenie tokov
- Krytykovaním týchto tvrdených protiúdajovými službami MCP a úlohami A2A

</details>

<details>
<summary><b>📡 28. "I need unified observability across all interfaces"</b></summary>

Rozdelovanie observabilitou na protokoly tvorí špecifikácia sťahovacej oblasti a
dlhších časov respodenstia.

**How OmniRoute solves it:**

- Zjednocený rozkladník a dashboardy v jednom produkte
- Zdravie + audit + žiadosťové teleskopy naprieč OpenAI, MCP a A2A vrstvami.
- Operatívne API pre stav a automatizáciu

</details>

<details>
<summary><b>💼 29. "I need one runtime for proxy + tools + agent orchestration"</b></summary>

Běhú veľkého počta separných služieb zvyšuje operatívne náklady a rozšírenie
výroby.

**How OmniRoute solves it:**

- EÚROPSKY PROXY priamie pre OpenAI, server MCP a A2A v jednom zväzku
- Súčasné autentifikácie, odolnosť, úložisko a sledovanie
- Súbor politických modelov súčasne na všetkých interakčných površích

</details>

<details>
<summary><b>🚀 30. "I need to ship agentic workflows without glue-code sprawl"</b></summary>

Tímy zmeniacej rýchlost' keď zdieľajú množstvo nezáväzných služieb a skriptov.

**How OmniRoute solves it:**

- EÚROPSKY stratégia jedného konca na klientov a agentov
- Postavené protokoly riadiace užívateľské rozhrania a dymové cestami overovania
- Produkčne založené základy (bezpečnosť, logovanie, odolnosť, zálohovanie)

</details>

### Príkladové Playbooky (Integrované prípady využitia)

**Playbook A: Maximálne zaplatené predplatné + stredne cenejšia záloha**

```txt
Kombinácia: "maximálne-claude"
  1. cc/claude-opus-4-6
  2. glm/glm-4.7
  3. if/kimi-k2-thinking

Mesačný poplatok: 20 USD + malý zálohový výdaj
Výsledok: vyšší kvalita, bezútešnosť vyše nuly
```

**Playbook B: Zdarmo kódovacími sadami**

```txt
Kombinácia: "zdarmo-forever"
  1. gc/gemini-3-flash
  2. if/kimi-k2-thinking
  3. qw/qwen3-coder-plus

Mesačný poplatok: 0 USD
Výsledok: stabilná zdarmo kódovací kyslina
```

**Playbook C: 24/7 stále fungujúca náhrada postupnosti**

```txt
Kombinácia: "pohotovosť-každý-dňa"
  1. cc/claude-opus-4-6
  2. cx/gpt-5.2-codex
  3. glm/glm-4.7
  4. minimax/MiniMax-M2.1
  5. if/kimi-k2-thinking

Výsledok: vysoká náhrada dĺžky pre deadline-critical zložité prenosy
```

**Playbook D: Agent operačné s MCP + A2A**

```txt
1) Začnite riadiť transport MCP ( `omniroute --mcp`) pre operáciu a podmienky
2) Spustiť A2A úlohy pomocou `pošty/python` a `pošty/stránok`
3) Sledovať pomocou /dashboard/endpoint (MCP a A2A taby)
4) Preložiť služby pomocou Inline riadiacich kontroll
```

---

## 🆓 Zatial zdarma na 0 — 0 výdajov

> Nastavte AI kódovanie do minútek za 30X$$30. Konektujte túto zadarmo úpočet a
> použite postupnosť zdarmo súčasnych služieb.

| Krok | Akcia                                                 | Poskytnutie poskytovateľov                                              |
| ---- | ----------------------------------------------------- | ----------------------------------------------------------------------- |
| 1    | Pripojite **Kiro** ID prehliadača AWS (Builder OAuth) | Claude Sonnet 4.5, Haiku 4.5 - **neokradnutelný**                       |
| 2    | Pripojite **iFlow** (Google OAuth)                    | kimi-k2-thinking, qwen3-coder-plus, deepseek-r1... - **neokradnutelný** |
| 3    | Pripojite **Qwen** (Kód zariadenia)                   | qwen3-coder-plus, qwen3-coder-flash... - **neokradnutelný**             |
| 4    | Pripojite **Gemini CLI** (Google OAuth)               | gemini-3-flash, gemini-2.5-pro - **180K/mo zdarma**                     |
| 5    | `/dashboard/combos` → **Free Stack (0$)** šablóna     | Okruhuj všetky zadarmo dostupné poskytovateľov automaticky              |

**Pojiďte libovolný IDE/CLI:** `http://localhost:20128/v1` • API Key:
`ktokĺvek字符串` • Hotovo.

> **Doplnkový bonus (tiež zdarma):** Groq API key (30 RPM zdarma), NVIDIA NIM
> (40 RPM zdarma, 70+ modelov), Cerebras (1M tok/day), LongCat API key (50M
> značiek/den!), Cloudflare Workers AI (10K neuronov/den, 50+ modelov).

## Rýchly štart

### 1. Nainštalujte a spustite

```bash
npm install -g omniroute
omniroute
```

> **pnpm používateľ:** Spusti `pnpm approve-builds -g` po nainšťatovaní, aby
> boli povolené nákupné skripty vynútené `better-sqlite3` a `@swc/core`:
> 
> ```bash
> pnpm install -g omniroute
> pnpm approve-builds -g   # Vyber všetky balíky → schvaľ
> omniroute
> ```

Rozhranie otvorí na adrese `http://localhost:20128` a API základná URL je
`http://localhost:20128/v1`.

| Prikaz                  | Popis                                                              |
| ----------------------- | ------------------------------------------------------------------ |
| `omniroute`             | Spusti server (port:`20128`, API a rozhranie na štandardnom porte) |
| `omniroute --port 3000` | Stanov pozadanie/API na 3000                                       |
| `omniroute --mcp`       | Spusti server MCP (transport stdio)                                |
| `omniroute --no-open`   | Neotváraj automaticky prehliadač                                   |
| `omniroute --help`      | Zobraz Help                                                        |

Sekčná pomoc:

```bash
PORT=20128 DASHBOARD_PORT=20129 omniroute
# API:       http://localhost:20128/v1
# Rozhranie:  http://localhost:20129
```

### 2) Pripájajteproviderov a vytvorte svoj API kľúč

1. Otvorte dashboard → Povoloční[ovaťX17X]providers` a pripájajte aspoň jeden
   poskytovateľ (OAuth alebo API kľúč).
2. Otvorte dashboard → Povoloční[avaťX17X]endpoints` a vytváte svoj API kľúč.
3. Nástupne: Otvorte dashboard → Povoloční[avaťX28X]combos` a nastavte váš
   spätný rad.

### 3) Orientujte svoj kodovací nástroj na OmniRoute

```txt
Základná URL: http://localhost:20128/v1
API Kľúč:  [skopírujte zo stránky Endpoint]
Model:    ak/kimi-k2-reckoning (alebo akýkoľvek poskytovateľ/model predpony)
```

Pracuje s Claudem Kod, Codex CLI, Gemini CLI, Cursor, Cline, OpenClaw, OpenCode,
a OpenAI-zrozumiteľnými SDKmi.

### 4) Rozšírte a overte protokoly (v2.0)

**MCP (pre tool-driven operácie):**

```bash
omniroute --mcp
```

Potom pripájajte MCP klienta cez `stdio` a overte nástroje ako:

- `omniroute_get_healthy`
- `omniroute_list_combos`

**A2A (pre agent-to-agent práconím):**

```bash
curl http://localhost:20128/.well-known/agent.json
```

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"quickstart","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"Give me a short quota summary."}]}}'
```

### 5) Overte či všetko funguje od začiatku do konca (pou žiadajúce)

```bash
npm run test:protocols:e2e
```

Tato súbor overuje reálne MCP a A2A klientské priloženie proti behu aplikácií.

### Alternatíva: spustiť aj z zdrojového kódu.

```bash
cp .env.example .env
npm install
PORT=20128 DASHBOARD_PORT=20129 NEXT_PUBLIC_BASE_URL=http://localhost:20129 npm run dev
```

---

## 🐳 Kontajner

OmniRoute je k dispozícii ako verejný kontajner v [Docker
Hub](https://hub.docker.com/r/diegosouzapw/omniroute).

**Rýchly spust:**

```bash
kontajner run -d \
  --name omniroute \
  --restart unless-stopped \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:latest
```

**S súborom nastavov:**

```bash
# Kópia a upravenie .env predtým
cp .env.example .env

kontajner run -d \
  --name omniroute \
  --restart unless-stopped \
  --env-file .env \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:latest
```

**Použitím Kontajneru Compose:**

```bash
# Základná profil (bez nástrojov CLI)
kontajner compose --profile base up -d

# Profil CLI (Claude Code, Codex, OpenClaw vkladený)
kontajner compose --profile cli up -d
```

| Obrázok                  | Štárovka   | Veľkosť | Popis                    |
| ------------------------ | ---------- | ------- | ------------------------ |
| `diegosouzapw/omniroute` | `najnovší` | ~250MB  | Najnovší stabilná verzia |
| `diegosouzapw/omniroute` | `1.0.3`    | ~250MB  | Aktuálna verzia          |

---

## 💻 Pultová aplikácia — Offline & Always-On

> 🆕 **NOVO** OmniRoute teraz dostupný ako **domáca aplikácia desktovej úpravy**
> pre Windows, macOS a Linux.

Spustiť OmniRoute ako samostatnú aplikáciu pre desktopej úpravy – žiadne
terminál, žiadne prehliadače, žiadne žiadosť o pripojenie k internetu pre
lokálne modely. Aplikácia založená na Electron obsahuje:

- 🖥️ **Domáci okno** – Náplň aplikáciu s integráciou nástruhe v stredníku
- 🔄 **Automatizovanie spustenia** – Spustiť OmniRoute pri návode systému
- 🔔 **Domáce oznamovanie** – Prísť o varovanie pre ukončenie kreditu alebo
  riešení poskytovateľa
- ⚡ **Jedno-tlačidlo získanie** – NSIS (Windows), DMG (macOS), AppImage (Linux)
- 🌐 **Offline režim** – Pracuje úplne v offline móde s ukladaním serveru

### Rýchly štart

```bash
# Vývojová módo
npm run electron:dev

# Stavba pre váš systém
npm run electron:build         # Aktuálny systém
npm run electron:build:win     # Windows (.exe)
npm run electron:build:mac     # macOS (.dmg) – x64 &amp; arm64
npm run electron:build:linux   # Linux (.AppImage)
```

### Systémová náplň

Kedy sa miniaturizuje, OmniRoute žiada v systémej nástruhov s rýchlymi postupmi:

- Otvorte informačný panel
- Zmeniť serverový port
- Ukončiť aplikáciu

📖 Plná dokumentácia: [`electron/README.md`](electron/README.md)

---

## 💰 Sú hrubinové ceny na prvý pohľad

| Trieda             | Provider                      | Hrubina                                 | Reset_quota                | Best For                                   |
| ------------------ | ----------------------------- | --------------------------------------- | -------------------------- | ------------------------------------------ |
| **💳 SUBSCRIPTION** | Claude Code (Pro)             | $20/mo                                  | 5h + weekly                | Already subscribed                         |
|                    | Codex (Plus/Pro)              | $20-200/mo                              | 5h + weekly                | OpenAI users                               |
|                    | Gemini CLI                    | **FREE**                                | 180K/mo + 1K/day           | Everyone!                                  |
|                    | GitHub Copilot                | $10-19/mo                               | Monthly                    | GitHub users                               |
| **🔑 API KEY**      | NVIDIA NIM                    | **FREE** (dev forever)                  | ~40 revolúcií za minutu    | 70+ otvorených modelov                     |
|                    | Cerebras                      | **zdarmo** (1M tok/day)                 | 60tis. TPM / 30 RPM        | Svetsko najrýchlejšie                      |
|                    | Groq                          | **zdarmo** (30 RPM)                     | 14,4tis. RPD               | Ultra-rýchla Llama/Gemma                   |
|                    | DeepSeek V3.2                 | $0.27/$1.10 za 1M                       | žiadne                     | Priemerná najnižšia cena                   |
|                    | xAI Grok-4 Rýchla             | ** $0,20/$0,50 za 1M ** 🆕               | žiadne                     | Rýchlejšie + nástrojové volanie, najnižšia |
|                    | xAI Grok-4 (štandard)         | $0.20/$1.50 za 1M 🆕                     | žiadne                     | Priemerný flagship xAI                     |
|                    | Mistral                       | Slobodná skúšobná verzia + plná verzia  | Obmedzená sadzba           | Európsky AI                                |
|                    | OpenRouter                    | Podľa použitia                          | žiadne                     | 100+ modelov zosúmovač                     |
| ** 💰 AKECNE**      | GLM-5 (via Z.AI) 🆕            | $0.5 za 1M                              | denné 10AM                 | 128K výstup, najnovší vlajkové lode        |
|                    | GLM-4.7                       | $0.6 za 1M                              | denné 10AM                 | Rozpočet pomocná                           |
|                    | MiniMax M2.5 🆕                | $0.3 za 1M vstup                        | 5-hodinový rolling         | Dôkazné a agentic úlohy                    |
|                    | MiniMax M2.1                  | 0,2 USD/dal 1 miliónu                   | 5-hodinový rolling         | Najlacnejší options                        |
|                    | Kim K 2,5 (Moonshot API) 🆕    | Podľa použitia                          | žiadne                     | Priamo prístup k Moonshot API              |
|                    | Kim K 2                       | flatové 9 USD/mesiac                    | 10 miliónov tokenov/mesiac | Predvídateľná nákladnosť                   |
| **🆓 ZÁKLENIE **    | iFlow                         | **0,00 ** USD                           | Neomezené                  | 5 modelov neomezených                      |
|                    | Qwen                          | **0,00 ** USD                           | Neomezené                  | 4 modely neomezené                         |
|                    | Kiro                          | **0,00 ** USD                           | Neomezené                  | Claude Sonnet / Haiku (AWS Builder)        |
|                    | LongCat Flash-Lite 🆕          | **0,00 ** USD (50 miliónov tok / deň 🔥) | 1 za sekundu               | Najväčší bezplatný rozmer na Zemi          |
|                    | Inovácie A I (Pollinations) 🆕 | **$0** (bez kľúča potrebného)           | 1 žiadosť/15s              | GPT-5, Claude, DeepSeek, Llama 4           |
|                    | A I Cloudflare Workers 🆕      | **$0** (10K neuronov/den)               | ~150 odpovedí denne        | 50+ modelov, globálna hraničná kontrola    |
|                    | Scaleway A I (Nový) 🆕         | **$0** (spolu 1 milión tokens)          | Obmedzená sadzba           | EU/GDPR, Qwen3 235B, Llama 70B             |

> 🆕 **Dodia pridávajú novšie modely (Mar 2026): ** Rodina Lek-4 Fast v cene
> $0,20/$0,50/M (značený na benchmárkovej rýchlosti 1143ms - 30% rýchlej ako
> Gemini 2.5 Flash), GLM-5 pomocou Z.AI s 128K výstupom, MiniMax M2.5
> dôslednosť, DeepSeek V3.2 aktualizovaný cenový štart, Kimi K2.5 pomocou
> Moonshot priamo cez API.

**💡 $0 Combostack – Celý Bezplatný Nastavenie:**

```
# 🆓 Najlepší Beztúžinový Sklad 2026 – 11 Dodávateľov, $0 Našie
Kiro (kr/)             → Claude Sonnet/Haiku NEOBDRAŽO
iFlow (if/)            → kimi-k2-thinking, qwen3-coder-plus, deepseek-r1 NEOBDRAŽO
LongCat Lite (lc/)     → LongCat-Flash-Lite — 50M tokens/den 🔥
Pollinations (pol/)    → GPT-5, Claude, DeepSeek, Llama 4 — bez kľúča potrebného
Qwen (qw/)             → qwen3-coder-plus, qwen3-coder-flash, qwen3-coder-next NEOBDRAŽO
Gemini (gemini/)       → Gemini 2.5 Flash — 1 500 žiadosť zdarma denne API kľúč
Cloudflare A I (cf/)    → Llama 70B, Gemma 3, Mistral — 10K Neuronov/den
Scaleway (scw/)        → Qwen3 235B, Llama 70B — 1 milión zdarma tokens (EU)
Groq (groq/)           → Llama/Gemma extrémne rýchly — 14,4K žiadosť denne
NVIDIA NIM (nvidia/)   → 70+ otvorených modelov — 40 RPM navždy
Cerebras (cerebras/)   → Llama/Qwen svetovo najrýchlejšie — 1M tok/den
```

**Odtváraj odpočítavanie. Nie je vôbec zastavené.** Nastavte to ako jeden
kombinovaný úsek OmniRoute a všetky výpadek nastanú automaticky – nikdy sa
nestarete o manuálne presmerovanie.

---

---

## 🆓 Bezplatné Modely – Čo ste Skutočne Dostali

> Vzorká modely níže sú **100% výhodné so zlomkovou kartou[63X]. OmniRoute
> rýchlo prechádzajú automaticky medzi nimi a kombinovanie všetkých ich vám
> poskytne neprekroľateľný $0 kombinovaný produkt.

### 🔵 Mody CLAUDE (via Kiro – AWS kľúč)

| Model               | Predpona | Omezený limit | Limit sadzby                   |
| ------------------- | -------- | ------------- | ------------------------------ |
| `claude-sonnet-4.5` | `kr/`    | **Neomezený** | Žiadna denná akčná hranica     |
| `claude-haiku-4.5`  | `kr/`    | **Neomezený** | Žiadna denná akčná hranica     |
| `claude-opus-4.6`   | `kr/`    | **Neomezený** | Najnovšie modely Opus cez Kiro |

### 🟢 NÁRODY IFLOW (Bezplatný OAuth – Bez kreditnej karty)

| Model              | Predpona | Omezený limit | Limit sadzby                    |
| ------------------ | -------- | ------------- | ------------------------------- |
| `kimi-k2-thinking` | `if/`    | **Neomezený** | Nie je uvedená hraničná hodnota |
| `qwen3-coder-plus` | `if/`    | **Neomezený** | Nie je uvedená hraničná hodnota |
| `hlbnohaľ-r1`      | `if/`    | **Neomezený** | Nie je uvedená hraničná hodnota |
| `minimax-m2.1`     | `if/`    | **Neomezený** | Nie je uvedená hraničná hodnota |
| `kimi-k2`          | `if/`    | **Neomezený** | Nie je uvedená hraničná hodnota |

### 🟡 MODELY PREKLADENO Kľúč (Zariadenie kódovanie autentizácia)

| Model               | Predpona | Omezený limit | Limit sadzby                    |
| ------------------- | -------- | ------------- | ------------------------------- |
| `qwen3-coder-plus`  | `qw/`    | **Neomezený** | Nie je uvedená hraničná hodnota |
| `qwen3-coder-flash` | `qw/`    | **Neomezený** | Nie je uvedená hraničná hodnota |
| `qwen3-coder-next`  | `qw/`    | **Neomezený** | Nie je uvedená hraničná hodnota |
| `vizionové-model`   | `qw/`    | **Neomezený** | Multimódny (obrázky)            |

### 🟣 GEMINI CLI (Google OAuth)

| Model                    | Predpona | Omezený limit                      | Limit sadzby                 |
| ------------------------ | -------- | ---------------------------------- | ---------------------------- |
| `Gemini-3-Flash-Preview` | `gc/`    | **180K tokenov/mesiac** + 1K/den   | Obnovuje sa mesiac za mesiac |
| `Gemini-2.5-Pro`         | `gc/`    | 180K tokenu/mesiac (zdieľané pool) | Vysoká kvalita               |

### ⚫ NVIDIA NIM (Bezplatné kľúče API — build.nvidia.com)

| Trieda                         | Denný limit                    | Limit sadzby | Poznámky                                                                              |
| ------------------------------ | ------------------------------ | ------------ | ------------------------------------------------------------------------------------- |
| Bezplatné (rozvojárská verzia) | Nemajú obmedzený počet tokenov | **~40 RPM**  | 70+ modelov; prevrátenie na čisté obmedzenia stredného rýchlosti v polovicu roku 2025 |

Populárne slobodné modely: `moonshotai/kimi-k2.5` (Kimi K2.5), `z-ai/glm4.7`
(GLM 4.7), `deepseek-ai/deepseek-v3.2` (DeepSeek V3.2),
`nvidia/llama-3.3-70b-instruct`, `deepseek/deepseek-r1`

### ⚪ CEREBRAS (Bezplatné kľúče API — inference.cerebras.ai)

| Trieda  | Denný limit      | Limit sadzby        | Poznámky                                  |
| ------- | ---------------- | ------------------- | ----------------------------------------- |
| Zadarmo | 1M tokenov/den** | 60tis. TPM / 30 RPM | Súper rýchle LLM inercia; resetuje dennie |

K dispozícii zadarmo: `llama-3.3-70b`, `llama-3.1-8b`,
`deepseek-r1-distill-llama-70b`

### 🔴 GROQ (Súbor API kľúč — console.groq.com)

| Trieda  | Denný limit | Limit sadzby    | Poznámky                                               |
| ------- | ----------- | --------------- | ------------------------------------------------------ |
| Zadarmo | 14,4K RPD** | 30 RPM na model | Žiadne kreditná kártya; 429 na limit, nebolo vyhlásený |

K dispozícii zadarmo: `llama-3.3-70b-versatile`, `gemma2-9b-it`, `mixtral-8x7b`,
`whisper-large-v3`

### 🔴 LONGCAT AI (Súbor API kľúč — longcat.chat) 🆕

| Model                           | Predpona | Denní Zľava          | Poznámky                                  |
| ------------------------------- | -------- | -------------------- | ----------------------------------------- |
| ` LongCat-Flash-Lite `          | ` lc/`   | ** 50M tlačítok ** 💥 | Najväčšia zľava za zvýhodneného užívateľa |
| ` LongCat-Flash-Chat `          | ` lc/`   | 500K tlačítok        | Multipozvodie                             |
| ` LongCat-Flash-Thinking `      | ` lc/`   | 500K tlačítok        | Racionalizácia / CoT                      |
| ` LongCat-Flash-Thinking-2601 ` | ` lc/`   | 500K tlačítok        | Jan. 2026 verzia                          |
| ` LongCat-Flash-Omni-2603 `     | ` lc/`   | 500K tlačítok        | Multimódna                                |

> 100% zľava počas verejného beta testu. Zaregistrujte sa na
> [longcat.chat](https://longcat.chat) pomocou emailu alebo telefonu. Znova
> používanie denná o 00:00 UTC.

### 🟢 ROZMRAŇOVANIE A I (Žiadne API Kľúčy Sú Potrebné) 🆕

| Model      | Predpona | Limit sadzby  | Obslužujúci zastraniať |
| ---------- | -------- | ------------- | ---------------------- |
| `openai`   | `pol/`   | 1 žiadosť/15s | GPT-5                  |
| `claude`   | `pol/`   | 1 žiadosť/15s | Anthropic Claude       |
| `gemini`   | `pol/`   | 1 žiadosť/15s | Google Gemini          |
| `deepseek` | `pol/`   | 1 žiadosť/15s | DeepSeek V3            |
| `llama`    | `pol/`   | 1 žiadosť/15s | Meta Llama 4 Scout     |
| `mistral`  | `pol/`   | 1 žiadosť/15s | Mistral AI             |

> ✨ **Zerosťujúci tlač:** Nezadávajte si údržbu alebo API kľúč. Pridajte
> poskytovateľa Pollinácií s prázdny kľúčovými poli a funkcionuje nepretržite.

### 🟠 CLOUDFLARE WORKERS AI (Kľúč zdarma — cloudflare.com) 🆕

| Trieda  | Dnešných neuronových ustanov\ | Ekvivalent Používania                         | Poznámky                     |
| ------- | ----------------------------- | --------------------------------------------- | ---------------------------- |
| Zadarmo | [10 000]10 000**              | ~150 modelov LLM / 500s audio / 15K zobrazení | Globálne okraje, 50+ modelov |

Populárne zadarmo modely: [21X]@cf/meta/llama-3.3-70b-instruct`,
`@cf/google/gemma-3-12b-it`, `@cf/openai/whisper-large-v3-turbo` (zdarmo
audio!), `@cf/qwen/qwen2.5-coder-15b-instruct`

> Požaduje Token API + ID účtu z
> [dash.cloudflare.com](https://dash.cloudflare.com). Ulož ID účtu v
> nastaveniach poskytovateľa.

### 🟣 SCALEWAY AI (1M Zadarmo Tokenov — scaleway.com) 🆕

| Trieda  | Zadarmo Pomer          | Miesto       | Poznámky                                    |
| ------- | ---------------------- | ------------ | ------------------------------------------- |
| Zadarmo | [1 000 000]1M tokens** | 🇫🇷 Paríž, EU | Žiadny kreditná karta je potrebná do limítu |

Dostupné zadarmo: [16X]qwen3-235b-a22b-instruct-2507` (Qwen3
235B!), `llama-3.1-70b-instruct`, `mistral-small-3.2-24b-instruct-2506`,
`deepseek-v3-0324`

> EU/GDPR kompatibilné. Požaduje sa kľúč API na
> [console.scaleway.com](https://console.scaleway.com).

> [X]💡 Ďalší Umiestnenie Zadarmo (11 Poskytovateľov, $0 Navštetné):
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

| Provider         | Free Credits           | Best Model                                   | Limit sadzby                 |
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

Then v dashboard/media` → **Prepísané transkripcie** tab: nahrajte zvukové alebo
videový súbor → vyberte váš konfiguračnú bodku → získajte transkripciach vo
podporovaných formátoch.

## 💡 Hlavné riešenia

OmniRoute v2.0 je postavený ako operačný platforma, nie len ako proxy prenosový
server

### 🆕 Nové — Inšpirácie z KlawaRouter (Mar 2026)

| Funkcia                                                       | Čo urobí                                                                                                                          |
| ------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| ⚡ **Rýchly Grok-4 Fast Family**                               | AI modely v cene $0.20/$0.50/M — preskúmané 1143ms (30% rýchlejšie ako Gemini 2.5 Flash)                                          |
| 🧠 **GLM-5 pomocou Z.AI**                                      | 128K výstupny kontext, $0.5/1M — najnovšia vlajková loď z GLM rodiny                                                              |
| 🔮 **MiniMax M2.5**                                            | Dôvodné rozhodovanie + agentic úlohy v cene $0.30/1M — značkové upgrade od M2.1                                                   |
| 🎯 **toolCalling Vlajka pre model**                            | Modelová `toolCalling: true/false` v registriere — AutoKombinácia sa vyhýba tým modelom, ktoré nie sú schopné vykonávať nástroje  |
| 🌍 **Rozpoznávanie intencionnej vety v mnohoročných jazykoch** | Záverečné PT/ZH/ES/AR slov v skórovaní AutoKombinácie — lepšia volba modelu pre nenia-angl. obsah                                 |
| 📊 **Fallbacove správanie podľa benchmarkov**                  | Skutočné p95 tranzientné odovzdania liveho vyžiadania kormtujú skórovanie AutoKombinácie — AutoKombinácia sa učí podľa reálne dát |
| 🔁 **Duplikovanie žiadosť**                                    | Obsah-záhlavie základe dodup. okienko — bezpečné pre viacerých agentov, preváždzujuce zopakovaní zúžitie                          |
| 🔌 **Pluggable RouterStrategy**                                | Rozšíriteľné `RouterStrategy` rozhraním — pridajte vlastnú logiku prijímania správ ako pluginy                                    |

### 🚀 Predošlé v2.0.9+ — Playground, CLI Fingerprints & ACP

| Funkcia                                   | Čo urobí                                                                                                                                                                                                                                                                   |
| ----------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🎮 **Model Playground**                    | Priečinok nástrojov pre testovanie modelov pomocou poskytovateľa / modelu / koncového bodu - editor, tokovanie, ukončenie, časovanie                                                                                                                                       |
| 💻 **CLI Fingerprint Matching**            | Podoradenie hlavičky / tela providerom, aby sa zapodobalo pôvodnému podpisu CLI — zapnite pri každom poskytovatom v nastavení > Bezpečnosť. **Váš proxy IP je uchovávaný**                                                                                                 |
| 🤝 **ACP Support (Agent Client Protocol)** | Rozsah agentov (Codex, Claude, Goose, Gemini CLI, OpenClaw + 9 ďalších), spôsobenie procesu, `/api/acp/agents` koncový bod                                                                                                                                                 |
| 🤖 **ACP Agents Dashboard**                | DEBUG › Agents stráňa – súradnice 14 agentov s inštaláciou, verziou, ďalšimi zariadeniami pre ktorékoľvek nástroja CLI. **OpenCode** používateľom sa zobrazí tlačidlo "Stiahnite opencode.json", ktoré automatikky generuje pripraveniu konfiguráciu s dostupnými modelmi. |
| 🔧 **Custom Model `apiFormat` Routing**    | Pri použití `apiFormat: "responses"` sa modely spravidla ukladajú do API prečítavacej zodpovedností                                                                                                                                                                        |
| 🏢 **Codex Workspace Isolation**           | Nástroje multiple Codex priamoľubí po emailovej adrese - OAuth riadi rozlíšeniú spojení na základe Id workspacu                                                                                                                                                            |
| 🔄 **Electron Auto-Update**                | Desktop aplikácia kontroluje aktualizácie a automaticky ich nainštaluje po restarte                                                                                                                                                                                        |

### 🤖 Agent & Protocol Operations (v2.0)

| Funkcia                                      | Čo urobí                                                                                                                     |
| -------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| 🔧 **Hlavný server MCP (16 nástruh)**         | Ide/agenta nástroje cez 3 dopravné prostriedky: stdio, SSE (`/api/mcp/sse`), Streamable HTTP (`/api/mcp/stream`)             |
| 🤝 **Server A2A (JSON-RPC + SSE)**            | Spojenie agentov pre vykonanie úloh s sync a streamingovými tokmi                                                            |
| 🧭 **Stránka konsolidovaných endpointov**     | Stránka založená na nastavovaní tabov (Endpoint Proxy, MCP, A2A a API Endpoints)                                             |
| 🎚️ **Plochy povolení služieb**               | Switchy na ON/OFF pre MCP a A2A, vrátane ukladania nastavení (predvolené: OFF)                                               |
| 🛰️ **Biela srdcovinová čipka rýchlosti MCP** | Skutočný proces status (pid, doba prebiehania, vek bielich srdcovín, doprava, rozsahovací režim)                             |
| 📋 **Auditný súbor MCP**                      | Bazosobe zátvorený auditn ý rekord s úspechmi/ neúspechmi a vložením klíča                                                   |
| 🔐 **Použitie ochranných príkazov MCP**       | 9 tienou prístupných ochranných prísad pre reguláciu nástrojov                                                               |
| 📡 **Úpravou úloh v A2A**                     | Zoznam/filter úloh, inšpekcie udalostí/artikulov, zrušenie bežiacich úloh                                                    |
| 📋 **Objav kart agentov**                     | `/.well-known/agent.json` pre automatické objavovanie klientov                                                               |
| ✍️ **Protokoly E2E testová skúška **         | Skupina real MCP SDK + A2A klientké toky v `test:protocols:e2e`                                                              |
| ⚙️ **Kontroly operačných **                  | Prekrútenie kombinovaného tlačidla, aplikovanie odolnosti profilov, resetovanie prekrútenia od jedného kontrolovoúho povrchu |

### 🧠 Riešenie & Inteligencia

| Funkcia                                      | Čo urobí                                                                               |
| -------------------------------------------- | -------------------------------------------------------------------------------------- |
| 🎯 **Inteligentné 4-podlažné prehodnotenie ** | Automatické trasy: Rozsah → API Key → Cheape → Free                                    |
| 📊 **Reálna časová sledovanie kvóty **        | Aktuálny pocet tokenov + resetovaciečasového countdown per provider                    |
| 🔄 **Preklad formátov **                      | OpenAI ↔ Claude ↔ Gemini ↔ Odpovede s tvorením schema-bezpečného premenovanie          |
| 👥 **Pristup k jednotlivých účtom **          | Viacej účtov na zprovidere rýchlo inteligentnej selection                              |
| 🔄 **Automatizované odmeny tokenov **         | OAuth tokens premenia automaticky s obnovou úsť                                        |
| 🎨 **Zálohuj kombinovanie **                  | 6 strategie rovnováhy + kontrola prechodových rádiu                                    |
| 🌐 **Router s štítkami **                     | `poskytovateľ/*` dynamické routing                                                     |
| 🧠 **Úsilia na rozpočet                       | Spustenie cez, automatické, zásadné a prispôsobené rozmiestnenia počitavých limitov    |
| 🔀 **Modelové zmenu                           | Prepojovanie budovených + zásadných modelových zmen a bezpečnosť prevádzky             |
| ⚡ **Zadavana prevádzka znižania úsilia       | Prevedenie nízšich úsilia zadávaných pozadí úloh na lacnejších modeloch                |
| 🧪 **Súvetnám pamäť inteligentného navozíťu   | Automatické vyberanie modelu podľa obsahu (kódovanie, vizualizácia, analýza, zhrnutie) |
| 💬 **Vstučné injekcie používateľskeho promptu | Globálne riadenia chovania aplikované konzistnne                                       |
| 📄 **Zodpovedanie API kompatibilita           | Plná `/v1/responses` kompatibilita pre Codex a pokročilé agentic procesy               |

### 🎵 Multimodaľní API

| Funkcia                | Čo urobí                                                                                                                                                                   |
| ---------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🖼️ **obrazové výrobu   | `/v1/images/generations` s cloud a lokálnymi back-endmi                                                                                                                    |
| 📐 **Vloženie           | `/v1/embeddings` pre vyhľadávanie a RAG pipe-líniami                                                                                                                       |
| Zvukový prepis         | `/v1/audio/transcriptions` — 7 providers (Deepgram Nova 3, AssemblyAI, Groq Whisper, HuggingFace, ElevenLabs, OpenAI, Azure), auto-language detection, MP4/MP3/WAV support |
| 🔊 **Text-to-Speech**   | `/v1/audio/speech` — 10 providers (ElevenLabs, OpenAI, Deepgram, Cartesia, PlayHT, HuggingFace, Nvidia NIM, Inworld, Coqui, Tortoise) with correct error messages          |
| 🎬 **Video Generation** | `/v1/videos/generations` (ComfyUI + SD WebUI workflows)                                                                                                                    |
| 🎵 **Music Generation** | `/v1/music/generations` (ComfyUI workflows)                                                                                                                                |
| 🛡️ **Moderations**     | `/v1/moderations` safety checks                                                                                                                                            |
| 🔀 **Reranking**        | `/v1/rerank` for relevance scoring                                                                                                                                         |
| 🔍 **Web Search** 🆕     | `/v1/search` — 5 providers (Serper, Brave, Perplexity, Exa, Tavily), 6,500+ free/month, auto-failover, cache                                                               |

### 🛡️ Resilience, Security & Governance

| Funkcia                                                       | Čo urobí                                                                                        |
| ------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
| 🔌 **Circuit Breakers**                                        | Per-model trip/recover with threshold controls                                                  |
| 🎯 **Endpoint-Aware Models**                                   | 🛡️ [X3X]Ochrana proti bleskovému stádu[X25X]                                                    |
| Víreň + semaforová ochrana pri obnovení/chybových udalostiach | Znižovanie nákladov/zmršťovanie zvlaštšeností pomocou dvoch cachovacích úrovneí                 |
| 🧠 **Sémantická + Signatúrna Cache**                           | Znižovanie nákladov/zmršťovanie zvlaštšeností pomocou dvoch cachovacích úrovneí                 |
| ⚡ **Idempotencia požiadavky**                                 | Ochrana proti kopírovaniam v oknom                                                              |
| 🔒 **Rasťanie fingerprintu TLS**                               | Browser-like TLS fingerprint — **znižuje riziko detekcie botov a zákazníkov**                   |
| 💻 **CLI Fingerprint Matching**                                | Overie natívne nastrojenú žiadosť o signatúru — **znižuje riziko vylúčky a zachováva proxy IP** |
| 🌐 **Filtrovanie IP**                                          | Povolenie/zakázanie kontrol vystavených nasadení                                                |
| 📊 **Priamo úpravy obmedzení**                                 | Konfigurovateľné celosvetové/zväzové obmedzenie so persistenciou                                |
| 🔑 **Spravovanie API kľúčov + osahovanie**                     | Bezpečné vydanie/počiatočnosť kľúčov a modelov/providérov kontrol                               |
| 🛡️ **Chránená / môdi**                                        | Voliteľná autentifikácia a skrývanie poskytovateľov pre katalógy môdi                           |

### 📊 Náhlavie & Analýzy

| Funkcia                           | Čo urobí                                                           |
| --------------------------------- | ------------------------------------------------------------------ |
| 📝 **Žiadosť + Proxy Radylovanie** | Plná žiadosť/zodpoveď a proxy radylovanie                          |
| 📋 **Jednotný Logovacie Priečko**  | Žiadosť, proxy, audit a konsoleské územia na jedne strane          |
| 🔍 **Radionosiťelia Žiadosť**      | Latencia (p50, p95, p99) a vyžiadanie sledovanie                   |
| 🏥 **Zdravotný Priebeh**           | Pristupnosť, breaker stavy, blokovanie, cache štáty                |
| 💰 **Cenové sledovanie**           | Rozpočet kontrola a viditeľnosť cen modelu/prispievajúceho         |
| 📈 **Analytické vizualizácie**     | Infračnost modelu/ prispievajúceho a trendy úrovne                 |
| 🧪 **Framework na zhodnotenie**    | Zlaté sťahovanie testov s konfigurovateľnými taktikami pre zhodosť |

### ☁️ Riešenie & Platforma

| Funkcia                                             | Čo urobí                                                                           |
| --------------------------------------------------- | ---------------------------------------------------------------------------------- |
| 🌐 **Nastavenie akadie všade**                       | Súbor lokálneho počítača, VPS, Docker, oblasť Cloud                                |
| 💾 ** Syncrovacie Cloud**                            | Synchronizácia konfigurácií pomocou cloudového prácovného programu                 |
| 🔄 ** Zálohovanie/Zobnovovanie**                     | Fluxy exportovania/importovania a prevencie katastrof                              |
| 🧙 ** Asistova Magia pre Začiatkovcov**              | Prvé spustenie riadičkovej sady                                                    |
| 🔧 ** Dashboard pre Nákladné Prihlasovacie Príkazy** | Rýchla nainštalovanie populárnych nástrojov pre programovanie                      |
| 🎮 **Model Playground**                              | Výskum jakékolvek provider/model/endpoint z dashboardu                             |
| 🔏 ** Prívlastok pre Nákladný Náhlinský Prehľad**    | Pridelenie prívlastkov v závislosti od providera v Paneli Bezpečnosti > Bezpečnosť |
| 🌐 ** Mezinárodní lokalizácia (30 jazykov)**         | Plná lokalizácia dashboardu + dokumentácie s podporou RTL                          |
| 🧹 ** Odstrániť Všetky modely**                      | Klikanie jednostranými modelami v podrobnostoch providera                          |
| 📋 ** Šablóny pre Vytvoriť Projekt**                 | Štandardizované šablóny pre GitHub pre chyby a funkcie                             |
| 📂 ** Predvolené Slovenské Miesto pre Údaje**        | `ŠÍDEL_DIR` override pre ukladovacia lokácia                                       |

### HĽADANIE HLĽADEK V HLĽADANÍ

#### Inteligentné pádanie s praktickým riadením nákladov

```txt
Sbory: "môj-kódovací-stĺpec"
  1. cc/claude-opus-4-6
  2. nvidia/llama-3.3-70b
  3. glm/glm-4.7
  4. if/kimi-k2-thinking
```

Keď zlyhá cita, rátalebo zdravotné sústredenie, OmniRoute automaticky prechádza
na ďalší kandidát bez manuálneho prechodovania.

#### Správa protokolu, ktorá je viditeľná a operabilná

- MCP + A2A sú dostupné v UI a dokumentáci. Nie sú prekryté
- API protokolu sú preukazujúce živé operácie ( `/api/mcp/*`, `/api/a2a/*` )
- Deskovy dashboard obsahuje akcie pre denný údržbu (kombinované preklikače,
  breaker nápravy a zrušenie úlohy)

#### Prikladateľ, ktorý pridáva úpravy

priestor Prikladateľa obsahuje:

- **Hádzanky pre hlavolamom**: overenie preradenie kontrolných bodov
- **Kýmský Tester**: celkové vyžiadanie/zodpovedanie obojstranný prechádzať.
- **Testovo miesto**: viacero prípadov v jednom bežnem
- **V reálnom čase sledujem**: viditeľný prezrel útok a vidný.

Plus verifikácia protokolu so skutočnými klientmi cez `npm run
test:protokoly:e2e`

> 📖 **[MCP Server README](open-sse/mcp-server/README.md)** — Nástrojná
> priradzujúca, preukazujúca, IDE zobrazenie a ukotvené příklady.
> 
> 📖 **[A2A Server README](src/lib/a2a/README.md)** – Kľúčové prostriedky,
> JSON-RPC metódy, pričleňujúca a životnosť úlohy

## Triedy ľudi ( Evals )

Omnitrova Obsahuje vnutromnovenú rámcovú triedu pre ľudské vyčleňujúce obsah
proti zlatú sadu. Dostupný cez ** Analysts → Evals ** na dashboard.

### Integrovaná Zlatá sadzie

Predznačená "OmniRoute Zlatá sadzie" obsahuje príklady testovacích sadzieb pre:

- Predmety prírodných vied, geografické lokality, generovanie kódu
- Koherencia formátu JSON, prekladanie, generovanie markdownu
- Odmietnutie nebezpečného obsahu, počítanie, logika boolean

### Stratégie hodnotenia

| Stratégia            | Popis                                                               | Priejímací príklad                     |
| -------------------- | ------------------------------------------------------------------- | -------------------------------------- |
| `premierne`          | Výstup musí zároveň zhodovať                                        | `"4"`                                  |
| `obsahuje`           | Výstup musí obsahovať podsúbor (insenzitívne na veľký/i malý písmo) | `"Paríž"`                              |
| `šablonový výraz`    | Výstup musí zároveň vyhovovať šablonovému výrazu                    | `"1.*2.*3"`                            |
| `zákonom definovaný` | Zákonom definovaná funkcia JavaScriptov vráti true/false            | `(výtlač) =&gt; výtlač.length &gt; 10` |

---

## 📖 Príručka na začatie

### Nastavenie protokolu (MCP + A2A)

<details>
<summary><b>🧩 MCP Setup (Model Context Protocol)</b></summary>

Nastartovať prenos MCP v móde stdio:

```bash
omniroute --mcp
```

Doporučený postup validácie:

1. Pripojte svojho klienta MCP cez stdio.
2. Spustiť `omniroute_get_health`.
3. Spustiť `omniroute_list_combos`.
4. Otvoriť `/dashboard/mcp` pre potvrdenie heartbeat, aktivity a auditu.

Použitečné API pre automatizáciu:

- `GET /api/mcp/status`
- `GET /api/mcp/tools`
- `GET /api/mcp/audit`
- `GET /api/mcp/audit/stats`

</details>

<details>
<summary><b>🤝 A2A Setup (Agent2Agent)</b></summary>

Zistiť agenta:

```bash
curl http://localhost:20128/.well-known/agent.json
```

Odoslať úlohu:

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"setup-a2a","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"Summarize quota status."}]}}'
```

Spravovať životnosť cyklu:

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
- `Týždenné ` (VÝROBNO/VYPNUTO): uplatňuje sa pravidlo o taktovom výkonnej
  práve.
- Pružnosť škály: ak použitá okná dosiahne >= 90% výkonnej práve, účet sa
  vylučuje.
- Rotácia: OmniRoute riadi na ďalší dostupný účet Codex automaticky.
- Respektovaním štartovočas `resetAt`: účet sa dostane do výberu znova
  automaticky.

Scenáre:

- `5h VYPNUTÝ` + `Týždenné VÝROBNO`: účet sa vylučuje, ak aj napriek tomu
  zasiahne pravidlo o škále.
- `5h VYPNUTO` + `Týždenné VÝROBNO`: skôr sa vylučuje až vtedy, keď sa
  dosiahnutie 90% už nepokrývajú.
- `5h VYPNUTÝ` + `Týždenné VYPNUTO`: skôr sa vylučuje až vtedy, keď sa
  dosiahnutie 90% už nepokrývajú.
- `resetAt` prejde: účet sa automaticky vrátí do rotácie (bez manuálneho
  preaktivovania)

### Gemini CLI (FREE 180K/month!)

```bash
Nástroje → Prídavač → Pridaj Gemini CLI
→ Google OAuth
→ 180K úspešných dokončené priatokov + 1K priatokov denne

Modely:
  gc/gemini-3-skutočný-prezývka
  gc/gemini-2.5-pro
```

**Best Value:** Vynikajúce zadarmo! Použite to pred platnými tavenými vrstvami

### GitHub Copilot

```bash
Nástroje → Prídavače → Pridaj GitHub
→ OAuth pomocou GitHub
→ Mäsačný reset (1. deň mesiaca)

Modely:
  gh/gpt-5
  gh/claude-4.5-sonnet
  gh/gemini-3-pro
```

</details>

<details>
<summary><b>🔑 API Key Providers</b></summary>

### NVIDIA NIM (ZADARMO pre vývojárovky - 70+ modelov)

1. Zaregistrujte sa: [build.nvidia.com](https://build.nvidia.com)
2. Získať zadarmo API kľúč (2000 operácií prepočítaných úspešne)
3. Nástroje → Prídavať Prídavač → NVIDIA NIM :
   - Kľúč API: `nvapi-your-key`

**Modely:** `nvidia/llama-3.3-70b-instruct`, `nvidia/mistral-7b-instruct` a 50+
ďalších modelov

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
3. Prihlásenie na rozhraní:
   - Dodávateľ: `glm`
   - API kľúč: `váš kľúč`

**Použite:** `glm/glm-4.7`

**Pro tip:** Prieskumný plán Vám ponúka trojnásobný kľúč pri 1/7 cene!
Preloženie dennie 10:00 AM.

### MiniMax M2.1 ( reset 5h, $0.20/1M)

1. Prihlásenie: [MiniMax](https://www.minimax.io/)
2. Get API key
3. Rozhranie → Pridať API kľúč

**Použite:** `minimax/MiniMax-M2.1`

**Pro tip:** Najlevnejší úchop dlhodobej kontextu (1M tokenov)!

### Kimi K2 (9 $/ mesiac flat)

1. Prihlásenie: [Moonshot AI](https://platform.moonshot.ai/)
2. Get API key
3. Rozhranie → Pridať API kľúč

**Použite:** `kimi/kimi-latest`

**Pro tip:** Fixná cena 9 $/mesiac za 10M tokenov = $0,90/1M efektívna výška!

</details>

<details>
<summary><b>🆓 FREE Providers (Emergency Backup)</b></summary>

### iFlow (5 ZDARMA modelov prostredníctvom OAuth)

```bash
Rozhranie → Pripájanie iFlow
→ Überenie sa pomocou iFlow OAuth
→ Nezrozmerné využívanie

Modely:
  if/kimi-k2-thinking
  if/qwen3-coder-plus
  if/glm-4.7
  if/minimax-m2
  if/deepseek-r1
```

### Qwen (4 ZDARMA modely prostredníctvom Zariadenie kód)\

```bash
Dashboard → Spojiť Qwen
→ Autorizácia zdrojovej kódy zariadenia
→ Neomezená služba

Modely:
  qw/qwen3-coder-plus
  qw/qwen3-coder-flash
```

### Kiro (Claude FREE)

```bash
Dashboard → Spojiť Kiro
→ ID budovateľa AWS alebo Google/GitHub
→ Neomezená služba

Modely:
  kr/claude-sonnet-4.5
  kr/claude-haiku-4.5
```

</details>

<details>
<summary><b>🎨 Create Combos</b></summary>

### Príklad 1: Maximálna Subskenzia → Tlakom Cheap Backupu

```
Dashboard → Kombinácie → Vytvoriť Nové

Názov: premium-coding
Modely:
  1. cc/claude-opus-4-6 (Priamá účtovaná služba)
  2. glm/glm-4.7 (Mliečnú Cheap backup, 0,6 $/1M)
  3. minimax/MiniMax-M2.1 (Načajší prechod, 0,20 $/1M)

Použite v CLI: premium-coding
```

### Príklad 2: Neznačkové (Zdarma)

```
Názov: free-combo
Modely:
  1. gc/gemini-3-flash-preview (180K zdarma mesačne)
  2. if/kimi-k2-thinking (neomezená)
  3. qw/qwen3-coder-plus (neomezená)

Cena: 0 $ navždy!
```

</details>

<details>
<summary><b>🔧 CLI Integration</b></summary>

### Kurzor IDE

```
Nastavenia → Modely → Rozšírené:
  URL OpenAI API: http://localhost:20128/v1
  API OpenAI: [z OmniRute rozhrania]
  Model: cc/claude-opus-4-6
```

### Claude Kód

Použite **Stránku nástrojov CLI** v paneli správania pre jednosúťažné nastavenia
alebo manuálne upravte `~/.claude/settings.json`.

### Codex CLI

```bash
export OPENAI_BASE_URL="http://localhost:20128"
export OPENAI_API_KEY="vaš-omniroute-api-klúč"

codex "vaš vypočítaný vstup"
```

### OpenClaw

**Option 1 — Panel správania (používateľsky priateľskú verziu)**

```
Panel správania → Nástroje CLI → OpenClaw → Vyberte model → Použiť
```

**Option 2 — Ručne:** Upravte `~/.openclaw/openclaw.json`:

```json
{
  "modely": {
    "poskytovateľov": {
      "omniroute": {
        "baseUrl": "http://127.0.0.1:20128/v1",
        "apiKey": "sk_omniroute",
        "api": "openai-completions"
      }
    }
  }
}
```

> **Poznámka:** OpenClaw funguje iba s lokálnym OmniRutem. Použite `127.0.0.1`
> miesto `localhost` aby ste vyhnuli riešenia zdravie IPv6.

### Cline / ďalehrad / RooCode

```
Nastavenia → Konfigurovanie API:
  Poskytovä: Kompatibilný s OpenAI
  Základná adresa: http://localhost:20128/v1
  API klúč: [z OmniRoute dashboard]
  Model: if/kimi-k2-thinking
```

### OpenCode

**Krok 1:** Pridať OmniRoute ako uzľavného poskytovateľa:

```bash
opencode
/connect
# Vyberte "Iné" → Vkladajte ID: "omniroute" → Vkládajte váš OmniRoute API klúč
```

**Krok 2:** Vytvorte alebo upravte `opencode.json` vo vašom korotnom projekte:

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
        "if/kimi-k2-thinking": { "name": "Kimi K2 (Zdarma)" }
      }
    }
  }
}
```

**Krok 3:** Vyberte model v OpenCode:

```bash
/models
# Vyberte kterýkoľvek model OmniRoute zo zoznamu
```

> **Pokrok:** Pridať kterýkoľvek model k dispozícii v vašom OmniRoute
> `/v1/models` endpoint k `models` sekciu. Použité formát
> `poskytovateľ/model-id` od vašeho OmniRoute dashboard.

</details>

---

## Riešenie problémov

<details>
<summary><b>Click to expand troubleshooting guide</b></summary>

**"Model jazyka neposkytol správy"**

- Kvota poskytovateľa vyčerpaná → Pozrite si kvótne nastavenie na dashboard
- Riešenie: Použité kombináciu fallback alebo prepíname na tlačidlo s nižším
  príjemom

**Limitácia rátu**

- Použitá kvota odobredenia → Vrátime na GLM/MiniMax
- Pridaná kombinacia: `cc/claude-opus-4-6 → glm/glm-4.7 → if/kimi-k2-thinking`

**Zmerný token expired**

- Autorefréšenom od OmniRoute
- Ako problémy ostávajú: Dashboard → Poskytovateľ → Rekoenecťuj

**Vysoce drahé poplatky[X34X]

- Prehľad používania v pracovnej stani→ Náklady
- Previesť primárnu modelifikáciu na GLM/MiniMax
- Použiť bezplatnú tieru (Gemini CLI, iFlow) pre nedodatočné úlohy

**Prehľad/API porty sú chybné**

- `PORT` je kánonovým základovým portom (a portom API predvolaním)
- `API_PORT` preťažuje iba otvorenou OpenAI-kompatibilnú API poslucháča
- `DASHBOARD_PORT` preťažuje iba pracovňu prehľadu/Next.js poslucháča
- Nastaviť `NEXT_PUBLIC_BASE_URL` na vaše adresy prehľadu/public URL (pre OAuth
  návraty)

**Chyby synchronizácie cloudu**

- Over siú `BASE_URL`, či viesločiacia na vaše bežiacie zariadenie
- Over siú `CLOUD_URL`, či viesločiacia na vaše očakávané cloudu koncovú bod
- Udržiavať `NEXT_PUBLIC_*` hodnoty v súlade so hodnotami na serverovej strane

**Prvý prihlásenie sa nepodieľa**

- Preveri `INITIAL_PASSWORD` v `.env`
- Ak neschované, tak sa nastaví fallbackovacia heslá ako `123456`

**Žiadne požiadavky logy**

- Nastav `ENABLE_REQUEST_LOGS=true` v `.env`

**Konštantná skúšenka označuje „Neplatný“ pre providerov späťovkej
kompatibilných s OpenAI**

- Veľa zproviderov nenáhrado zvonca pre `/models` endpoint
- OmniRoute v1.0.6+ obsahuje fallbackovú overovanie poskytnutím pomocných
  vyrovnaní cez chat úlohy.
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

**6. OmniRoute restartuj**

```bash
# Ak používate npm:
npm run dev

# Ak používate Docker:
docker restart omniroute
```

**7. Skús sa pripojiť znovu**

Dashboard → Prylia → Antigravity (alebo Gemini CLI) → OAuth

Google však bude reťazovať správne na `https://jeho-správca-server.com/callback`
a autentifikácia funguje.

---

#### Prechodné riešenie (bez konfigurácie vlastných údajov)

Ak nechcete vytvárať vlastné údaje teraz, stále môžete použiť **manuálny prevod
URL**:

1. OmniRoute otvorí poľa googleovej autentifikácie
2. Po tejto autentifikácii Google zamedzí odkiaľ redirektovať na `localhost` (čo
   sa však nepodarí lokálnym serverom)
3. **Kopírujte úplnú adresu URL** so začiatočnej stránky vášho prekladacieho
   prostriedku (hoci stránky možno nebude znova stiahnutý)
4. Vložte túto úplnú adresu URL do pola, ktoré sa zobrazí v modálne rozbalenom
   príslušenstve pre pripojenie
5. Stlačte **"Pripojiť"**

> Ľahšie riešenie funguje, pretože je na url-ku kódu autorizácie vedena
> nezávisle na či sa reťaz zvlášť načítal alebo ne.

</details>

---

</details>

## 🛠️ Tech Stack

<details>
<summary><b>Click to expand tech stack details</b></summary>

- **Runtime**: Node.js 18–22 LTS (⚠️ Node.js 24+ nie je **Supported** —
  `better-sqlite3` doménne binárne súložicie sú nekompatibilné)
- **Programming language**: TypeScript 5.9 — **100% TypeScript** v celej `src/`
  a `open-sse/` (bez žiadnych `any` vo vnutrihladiná knižniciach od v2.0)
- **Framerwork**: Next.js 16 + React 19 + Tailwind CSS 4
- **Databáze**: LowDB (klasifikovanie JSON) + SQLite (doménne stavové údaje +
  proxy logs + MCP audit + routing decisions)
- **Schematic**: Zod (MCP nástroj I/O overenie, API zmluvy)
- **Protokoly**: MCP (stdio/HTTP) + A2A v0.3 (JSON-RPC 2.0 + SSE)
- **Prehľadávka**: Server-Sent Events (SSE)
- **Autentifikácia**: OAuth 2.0 (PKCE) + JWT + API Klíče + MCP Scenované
  Prístupové Rights
- **Testovanie**: Node.js Testovací Rámec + Vitest (900+ testov vrátane
  jednotkových testov, integračných testov, E2E)
- **CI/CD**: GitHub Actions (auto npm publish + Docker Hub na základe release)
- **Webová stránka**: [omniroute.online](https://omniroute.online)
- **Balíček**:
  [npmjs.com/package/omniroute](https://www.npmjs.com/package/omniroute)
- **Docker**:
  [hub.docker.com/r/diegosouzapw/omniroute](https://hub.docker.com/r/diegosouzapw/omniroute)
- **Používateľská odolnosť**: Obvodový prenášač, exponenciálny čakanie,
  anti-strela veľkého stredošia, TLS falšovanie, samoobnovný kombinácií

</details>

---

## Dokumentácia

| Dokument                                       | Popis                                                                    |
| ---------------------------------------------- | ------------------------------------------------------------------------ |
| [Ručné Prewoda](docs/USER_GUIDE.md)            | Dodávateľsko, kombinácie, integrač CL, nasadzanie                        |
| [Referenčný Zoznam API](docs/API_REFERENCE.md) | Všetky endpointy s primerami                                             |
| [MCP Server](open-sse/mcp-server/README.md)    | 16 nástrojov MCP, editorké konfigurácie, Python/TS/Go klienti            |
| [A2A Server](src/lib/a2a/README.md)            | Protokol JSON-RPC 2.0, kompetencie, prehľadávacia reťaž, riadenie úlohou |
| [Auto-Combo Motor](docs/auto-combo.md)         | Šestfaktorové skóre, módní balíčky, self-healing                         |
| [Troubleshooting](docs/TROUBLESHOOTING.md)     | Typické problémy a riešenia                                              |
| [Architecture](docs/ARCHITECTURE.md)           | Systémový architektúr a vnútorné zložky                                  |
| [Contributing](CONTRIBUTING.md)                | Nastavenie vývoja a prvé pokyny                                          |
| [OpenAPI Spec](docs/openapi.yaml)              | OpenAPI 3.0 zmluva                                                       |
| [Security Policy](SECURITY.md)                 | Prieskum únikov a bezpečnostné praktiky                                  |
| [VM Deployment](docs/VM_DEPLOYMENT_GUIDE.md)   | Kompletný príručka: VM + nginx + Cloudflare nastavovanie                 |
| [Features Gallery](docs/FEATURES.md)           | Prehľadný denník s vizuálnymi obrázkami                                  |
| [Release Checklist](docs/RELEASE_CHECKLIST.md) | Kroky pred vydavateľským overením                                        |

---

## 🗺️ Cestopis

OmniRoute má **210+ plánovaných prvov** v mnohých fázach vývoja. Nasledujúce
kľúčové oblasti:

| Kategória                           | Plánované riešenia | Hlavné body                                                                                                    |
| ----------------------------------- | ------------------ | -------------------------------------------------------------------------------------------------------------- |
| 🧠 **Riešenie cestu a inteligencie** | 25+                | Najnižšia latencia cesti, tagging, kvóty predprednosť, P2C účet vyber                                          |
| 🔒 **Zabezpečenie a Overenie**       | 20+                | Hardening SSRF, skrývanie hesiel, omezení limit na endpoint, managementová kľúčová skúsenosť                   |
| 📊 **Zistiťelnosť**                  | 15+                | Integration OpenTelemetry, reálne kótovací monitorovanie, sledovanie počtu na model                            |
| 🔄 **Integrácie dodávateľov**        | 20+                | Dynamický registračný model registráciu účtu, zatarasovanie dodávateľa, viac účtov Codex, parsing kvót Copilot |
| ⚡ **Verejnosť[System]**             | 15+                | Dual cache layer, cache promtu, cache odpovede, streamingu držíme žijúce, batch API                            |
| 🌐 **Ecosystem**                     | 10+                | WebSocket API, hot reload konfigurácie, distribuovaný registráciu účtu, komerčný režim                         |

### 🔜 Kompletne rýchlo

- 🔗 **OpenCode Integration** — Domáce komponujúce prijímače pre OpenCode AI
  kódovací IDE
- 🔗 **Integrácia TRAE** — Plná podpora pre vývojové rámenie TRAE AI
- 📦 **Rozpísaná API** — Asynchrónne rozpísače podkladových požiadaviek v
  množstve
- 🎯 **Routedľa taggingu** — Rozpísačky požiadaviek založené na custom tagách a
  metaúdajoch
- 💰 **Najnižšia-kódová stratégia** — Automaticky vyberaj najlacnejší dostupný
  poskytovateľ

> 📝 Podrobné štartové vlastnosti dostupné v
> [`docs/new-features/`](docs/new-features/) (217 podrobných štartových
> vlastností)

---

## 👥 Prispievatelia

[![Prispievatelia](https://contrib.rocks/image?repo=diegosouzapw/OmniRoute&max=100&columns=20&anon=1)](https://github.com/diegosouzapw/OmniRoute/graphs/contributors)

### Ako Prispievať

1. Fork repository
2. Vytvorte nový rozdelený konkrétny odnož ( `git checkout -b
   feature/amazing-feature` )
3. Zdieľte vaše zmeny ( `git commit -m 'Pridajte peknú funkcia'` )
4. Posťahujte odnož na server ( `git push origin feature/amazing-feature` )
5. Otvorte Pull request

Zisti v [CONTRIBUTING.md](CONTRIBUTING.md) podrobné štartové vedenia.

### Vydanie novej verzie

```bash
# Stvorujte novú verziu — vydanie sa uskutoční automatickej skrze npm
gh release create v2.0.0 --title "v2.0.0" --generate-notes
```

---

## 📊 História hviezd

## Hviezdy cez čas

## [![História hviezd cez čas](https://starchart.cc/diegosouzapw/OmniRoute.svg?variant=adaptive)](https://starchart.cc/diegosouzapw/OmniRoute)

## 🙏 Ďakujem

Ďakujeme **[9router](https://github.com/decolua/9router)**
**[decolua](https://github.com/decolua)** za to, že sa stal pôvodným projektom,
na čom sa zakladá táto fork. OmniRoute týmto zdokonaľuje báznivú založenie s
ďalšími funkciami, multi-modalnými API a úplnou prepísanou verziou pomocou
TypeScript-u.

Ďakujeme **[CLIProxyAPI](https://github.com/router-for-me/CLIProxyAPI)** —
originalnému implementácii v Go, ktorá inšpirovala táto JavaScriptovú
implementáciu.

---

## 📄 Licencia

Licencia MIT - pozri [LICENSE](LICENSE) pre podrobnosti.

---

<div align="center">
  <sub>Built with ❤️ for developers who code 24/7</sub>
  <br/>
  <sub><a href="https://omniroute.online">omniroute.online</a></sub>
</div>
<!-- GitHub Discussions enabled for community Q&A -->
