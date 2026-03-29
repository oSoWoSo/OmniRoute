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

| Area                              | Change                                                                                                                                                                    |
| --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🔒 **CodeQL Security**             | Fixed 10+ CodeQL alerts: polynomial-redos, insecure-randomness, shell-injection remediation                                                                               |
| ✅ **Route Validation**            | All 176 API routes now validated with Zod schemas + `validateBody()` — CI `check:route-validation:t06` passes                                                             |
| 🐛 **omniModel Tag Leak**          | Internal `<omniModel>` tags no longer leak to clients in SSE streaming responses (#585)                                                                                   |
| 🔑 **Registered Keys API**         | Auto-provision API keys via `POST /api/v1/registered-keys` with per-provider/account quota enforcement, idempotency, SHA-256 storage, and optional GitHub issue reporting |
| 🎨 **Provider Icons**              | 130+ icone dei provider tramite `@lobehub/icons` (SVG) con filaggine a fallback PNG generico                                                                              |
| 🔄 **Model Sync Auto**             | 24h programmazione e toggle di utilizzo manuale per sincronizzare le liste dei modelli per i provider integrati e personalizzati compatibili con OpenAI                   |
| 🌐 **OpenCode Zen/Go**             | Due nuovi provider da @kang-heewon via Pull Request #530: tariffa gratuita + tariffa a sottoscrizione tramite `OpencodeExecutor`                                          |
| 🐛 **CLI OAuth di Gemini**         | Errore azionario quando `GEMINI_OAUTH_CLIENT_SECRET` è mancante in Docker (era un errore criptico di Google)                                                              |
| 🐛 **Configurazione OpenCode**     | `saveOpenCodeConfig()` scrive ora correttamente TOML in `XDG_CONFIG_HOME`                                                                                                 |
| 🐛 **Override del model avvinato** | `body.model` impostato correttamente a `pinnedModel` nella protezione della cache di contesto                                                                             |
| 🐛 **Buco di Codex/Claude**        | `tool_result` adesso blocco i loop infiniti                                                                                                                               |
| 🐛 **Ridirezione di accesso**      | L'accesso non si blocca più dopo aver saltato l'impostazione della password                                                                                               |
| 🐛 **Percorsi di Windows**         | I percorsi MSYS2/Git-Bash (`/c/...`) sono normalizzati automaticamente a `C:\...`                                                                                         |

---

## 🖼️ Dashboard Principale

<div align="center">
  <img src="./docs/screenshots/MainOmniRoute.png" alt="OmniRoute Dashboard" width="800"/>
</div>

---

## 📸 Anteprima di Dashboard

<details>
<summary><b>Click to see dashboard screenshots</b></summary>

| Pagina              | Schermo                                             |
| ------------------- | --------------------------------------------------- |
| **Fornitori**       | ![Fornitori](docs/screenshots/01-providers.png)     |
| **Combini**         | ![Combini](docs/screenshots/02-combos.png)          |
| **Analisi**         | ![Analisi](docs/screenshots/03-analytics.png)       |
| **Salute**          | ![Salute](docs/screenshots/04-health.png)           |
| **Traduttore**      | ![Traduttore](docs/screenshots/05-translator.png)   |
| **Impostazioni**    | ![Impostazioni](docs/screenshots/06-settings.png)   |
| **Strumenti CLI**   | ![Strumenti CLI](docs/screenshots/07-cli-tools.png) |
| **Log di utilizzo** | ![Log"(docs/screenshots/08-usage.png)]              |
| **Endpoint**        | ![Endpoint](docs/screenshots/09-endpoint.png)       |

</details>

---

### 🤖 Fornitore AI gratuito per i tuoi agenti di codifica preferiti

_Connect any AI-powered IDE or CLI tool through OmniRoute — free API gateway for
unlimited coding._

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

<sub>📡 All agents connect via <code>http://localhost:20128/v1</code> or
<code>http://cloud.omniroute.online/v1</code> — one config, unlimited models and
quota</sub>

---

## 🤔 Why OmniRoute?

**Stop wasting money and hitting limits:**

- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Subscription quota expires unused every month
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Rate limits stop you mid-coding
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Expensive APIs ($20-50/month per provider)
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Manual switching between providers

**OmniRoute solves this:**

- ✅ **Maximize subscriptions** - Track quota, use every bit before reset
- ✅ **Auto fallback** - Subscription → API Key → Cheap → Free, zero downtime
- ✅ **Multi-account** - Round-robin between accounts per provider
- ✅ **Universal** - Works with Claude Code, Codex, Gemini CLI, Cursor, Cline,
  OpenClaw, any CLI tool

---

## 📧 Support

> 💬 **Join our community!** [WhatsApp
> Group](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t) — Get help,
> share tips, and stay updated.

- **Website**: [omniroute.online](https://omniroute.online)
- **GitHub**:
  [github.com/diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute)
- **Issues**:
  [github.com/diegosouzapw/OmniRoute/issues](https://github.com/diegosouzapw/OmniRoute/issues)
- **WhatsApp**: [Community
  Group](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)
- **Contributing**: See [CONTRIBUTING.md](CONTRIBUTING.md), open a PR, or pick a
  `good first issue`
- **Progetto Originale**: [9router by
  decolua](https://github.com/decolua/9router)

### 😒 Segnala un Bug?

Quando si apre un problema, per favore esegui il comando system-info e incollare
il file generato:

```bash
npm run system-info
```

Ciò genera un `file system-info.txt` con la versione di Node.js, la versione di
OmniRoute, i dettagli del sistema operativo, le tool CLI installate (se iflow,
gemini, claude, codex, antigravity, droid, ecc.), lo stato Docker/PM2, e i
pacchetti del sistema — tutto ciò che ci serve per riprodurre rapidamente il
nostro problema. Incollare il file direttamente nella tua issue di GitHub.

---

## Come funziona

```
┌─────────────┐
│  Tuo CLI   │  (Claude Code, Codex, Gemini CLI, OpenClaw, Cursor, Cline...)
│   Strumento │
└──────┬──────┘
       │ http://localhost:20128/v1
       ↓
┌─────────────────────────────────────────┐
│           OmniRoute (Router Inteligente)        │
│  • Formattazione translation (OpenAI ↔ Claude) │
│  • Tracciamento de quota + Embeddings + Images │
│  • Aggiornamento token automatico                   │
└──────┬──────────────────────────────────┘
       │
       ├─→ [Piano 1: ABONAMENTO] Claude Code, Codex, Gemini CLI
       │   ↓ quota esaurita
       ├─→ [Piano 2: CHIAVE API] DeepSeek, Groq, xAI, Mistral, NVIDIA NIM, ecc.
       │   ↓ limite di budget
       ├─→ [Piano 3: CUSTO BASSO] GLM ($0,6/1M), MiniMax ($0,2/1M)
       │   ↓ limite di budget
       └─→ [Piano 4: GRATIS] iFlow, Qwen, Kiro (senza limite)

Risultato: continua sempre a codificare, minimo costo
```

---

## 🎯 Cos'è OmniRoute - 30 Punti di Dolore e Casi di Utilizzo Reali

> **Ogni sviluppatore che utilizza strumenti AI incontra questi problemi
> quotidianamente.** OmniRoute è stato costruito per risolverli tutti — dai
> costi esorbitanti ai blocchi regionali, dalle flussi OAuth rotti alle
> operazioni di protocollo e all'osservabilità d'impresa.

<details>
<summary><b>💸 1. "I pay for an expensive subscription but still get interrupted by limits"</b></summary>

Gli sviluppatori pagano 20-200 €/mese per Claude Pro, Codex Pro o GitHub
Copilot. Nonostante il pagamento, la quota ha un limite — 5h di utilizzo, limiti
settimanali o per minuto. In una sessione di codifica in corso, il fornitore
smette di rispondere e lo sviluppatore perde la fluidità e la produttività.

** Come OmniRoute risolve il problema**:

- **Fallback Intelligente 4-Tier** — se la quota del piano di abbonamento è
  esaurita, viene automaticamente reindirizzato a Chiave API → Custo Basso →
  Gratis con nessuna interazione manuale
- **Tracciamento della Quota in Tempo Reale** — Mostra la consumo di token in
  tempo reale con il conteggio di reset (5h, quotidiano, settimanale)
- **Supporto Multi-Documento** — supporto per documenti multipli per provider
  con rotazione automatica — quando uno esaurisce la quota, passa al successivo
- **Combinazioni Personalizzate** — fallback personalizzati con strategie di
  bilanciamento 6 (fill-first, round-robin, P2C, random, least-used,
  cost-optimizzato)
- **Quota di Business Codex** — monitoraggio diretto della quota di lavoro di
  business/ditutto nel dashboard

</details>

<details>
<summary><b>🔌 2. "I need to use multiple providers but each has a different API"</b></summary>

OpenAI utilizza una formattazione, Claude (Anthropic) ne utilizza un'altra,
Gemini ne utilizza un'altra ancora. Se un dev ne vuole testare modelli da
provider diversi o fallback tra loro, devono ri.configurare gli SDKs, cambiare
gli endpoint, trattare con formati incompatibili. Provider personalizzati
(FriendLI, NIM) hanno punti di accesso dei modelli non standard.

** Come OmniRoute risolve il problema**:

- **Punto Unico di Accesso** — un unico `http://localhost:20128/v1` funziona
  come proxy per tutti i 67+ provider
- **Traduzione di Formattazione** — automatica e trasparente: OpenAI ↔ Claude ↔
  Gemini ↔ API di Risposta
- **Sintetizzazione Risposta** — Elimina campi non standard (`x_groq`,
  `usage_breakdown`, `service_tier`) che compromettono OpenAI SDK v1.83+
- **Normalizzazione Ruolo** — Converte `sviluppatore` → `sistema` per provider
  non OpenAI; `sistema` → `utente` per GLM/ERNIE
- ** Estrazione Etichetta Pensiero** — Estrarre `` blocchi dai modelli tipo
  DeepSeek R1 nella formato `ragionamento_contenuto`
- ** Output Strutturato per Gemini** — `json_schema` →
  `responseMimeType`/`responseSchema` conversione automatica
- ** `stream` è impostato su `falso`** — Coincide con la specifica OpenAI,
  evitando l'apparizione dell'SSE inaspettata nelle librerie Python/Rust/Go SDKs

</details>

<details>
<summary><b>🌐 3. "My AI provider blocks my region/country"</b></summary>

Gli provider come OpenAI/Codex bloccano l´accesso da certe regioni geografiche.
Gli utenti ricevono errori come `regione_città_territorio_supportato` durante la
connessione OAuth e API. Ciò è particolarmente frustrante per gli sviluppatori
da paesi in via di sviluppo.

** Come OmniRoute risolve il problema**:

- ** Configurazione Proxy 3 Livelli** — Configurazione customizzabile del proxy
  a 3 livelli: globale (tutta la traffico), per fornitore (un provider solo), e
  per connessione/chiave
- ** Badges di Proxy Colorati** — Indicatori visivi: 🟢 proxy globale, 🟡 provider
  proxy, 🔵 proxy della connessione, mostrando sempre l‚IP
- ** Scambio Token OAuth Attraverso Proxy** — Il flusso OAuth passa attraverso
  proxy, risolvendo `regione_città_territorio_supportato`
- ** Test di Connettività Attraverso Proxy** — I test di connettività utilizzano
  la configurazione proxy (nessun bypass diretto più)
- ** Supporto SOCKS5** — Il proxy SOCKS5 completo per la routing outwards
- ** Spoofing Marcatura Firma TLS** — Marcatura TLS come un browser tramite
  `wreq-js` per eludere la detezione dei bot
- ** 🔏 Coincidenza Firma CLI** — Riassegna i header e campo dei corpi per
  coincidere dei firme binary nativi in CLI, per ridurre drasticamente il
  rischio di scartare l‚account. Si preserva l‚IP di proxy — ottenere entrambi
  simultaneamente la furtività **e** mascheramento dell‚indirizzo IP

</details>

<details>
<summary><b>🆓 4. "I want to use AI for coding but I have no money"</b></summary>

Non tutti possono pagare $20-200/mese per le abbonamenti AI. Studenti,
sviluppatori da paesi in via di sviluppo, appassionati e freelancers necessitano
accesso a modelli qualitativi a costo zero

** Come OmniRoute risolve il problema**:

- ** Provider Livello di Grazia Incorporati** — Supporto nativo per gli provider
  gratuiti del 100 %: iFlow (5 modelli illimitati tramite OAuth:
  kimi-k2-thinking, qwen3-coder-plus, deepseek-r1, minimax-m2, kimi-k2), Qwen (4
  modelli illimitati: qwen3-coder-plus, qwen3-coder-flash, qwen3-coder-next,
  modello visivo ), Kiro (Claude + Builder ID AWS gratuito per free ), Gemini
  CLI (180K ombre del token/mese gratuito )
- ** Nuvoletta Cloud** — le nuvolette spostate ospitate Ollama modelli in
  `api.ollama.com` con grado di "uso leggero" gratuito; utilizare `ollamacloud/`
  prefisso
- ** Combos Esclusivamente Gratuiti** — Mettere `gc/gemini-3-flash →
  if/kimi-k2-thinking → qw/qwen3-coder-plus` = $0/mese con zero rallentamento
- ** Accesso NVIDIA NIM Gratuito** — libero accesso a 70+ modelli (in
  transizione da credito a limiti puri di velocità) circa 40 RPM presso sito
  build.nvidia.com per sviluppatori che lo devono
- Strategia Ottimizzata per i Costi ** — Strategia di routing che sceglie
  automaticamente il fornitore più economico disponibile

</details>

<details>
<summary><b>🔒 5. "I need to protect my AI gateway from unauthorized access"</b></summary>

Esponendo un gateway di AI alla rete (LAN, VPS, Docker), chiunque abbia
l'indirizzo può utilizzare i token/licenze del sviluppatore senza protezione,
rendendo le API vulnerabili all'abuso, all'iniezione di incitamenti e all'abuso.

** Come OmniRoute risolve il problema**:

- Gestione delle chiavi API ** — Generazione, rotazione e scoping per fornitore
  con pagina dedicata /dashboard/api-manager`
- Permessi Modelli ** — Limitare le chiavi API ai modelli specifici (` openai/
  \*`, pattern di wildcard), con pulsante di blocco/toggle
- Protezione dei punti di accesso API ** — Richiedere una chiave per
  `/v1/models` e bloccare fornitori specifici dalla lista
- Guardiano dell'autenticazione + protezione CSRF ** — Tutte le rotte di
  dashboard protette dal middleware ` withAuth` + token CSRF
- Limite di tariffe ** — Limitazione di tariffe per IP con finestre
  configurabili
- Filτρα IP ** — Liste di autorizzazione/blocco di accesso
- Guardiano dell'iniezione di incitamento ** — Sanitizzazione contro pattern di
  stimoli maliziosi
- Crittografia AES-256-GCM ** — Credenziali crittografate per le interazioni

</details>

<details>
<summary><b>🛑 6. "My provider went down and I lost my coding flow"</b></summary>

I fornitori di AI possono diventare instabili, restituire errori 5xx o colpire
limpi limiti di tariffe temporanei. Senza i breakers di circuito, i tentativi
ripetuti possono bloccare l'applicazione.

** Come OmniRoute risolve il problema**:

- Breaker di circuito per-modello ** — Apri/chiudi automaticamente con soglie
  configurabili e cooldown (Chiuso/Aperto/Mezzo-Aperto), ricollegato per-modello
  per evitare blocchi di cascata
- Ritardi esponenziali ** — Ritardi di tentativi progressivi
- Anti-Thundering Herd ** — Mutex + semaforo per proteggere i balzi di ritento
  congiunti
- Combo Chain di Caduta ** — Se il fornitore primario fallisce, automaticamente
  cade lungo la catena senza interferire
- Combo Breaker di circuito ** — Blocchi automaticamente gli alimentatori
  falliti entro una catena di combo
- Pannello di controllo della salute ** — Monitoraggio dell'uptime, stati dei
  breaker di circuito, blocco, statistiche della cache, latenza p50/p95/p99

</details>

<details>
<summary><b>🔧 7. "Configuring each AI tool is tedious and repetitive"</b></summary>

I sviluppatori utilizzano Cursor, Claude Code, Codex CLI, OpenClaw, Gemini CLI,
Kilo Code... Ogni strumento necessita di un config diverso (end point API,
chiave, modello). La ricongiunzione quando si passa dai fornitori o dai modelli
è una perdita di tempo.

** Come OmniRoute risolve il problema**:

- **CLI Tools Dashboard** — Dedicated page with one-click setup for Claude Code,
  Codex CLI, OpenClaw, Kilo Code, Antigravity, Cline
- **GitHub Copilot Config Generator** — Generates `chatLanguageModels.json` for
  VS Code with bulk model selection
- **Onboarding Wizard** — Guided 4-step setup for first-time users
- **One endpoint, all models** — Configure `http://localhost:20128/v1` once,
  access 67+ providers

</details>

<details>
<summary><b>🔑 8. "Managing OAuth tokens from multiple providers is hell"</b></summary>

Claude Code, Codex, Gemini CLI, Copilot — all use OAuth 2.0 with expiring
tokens. Developers need to re-authenticate constantly, deal with `client_secret
is missing`, `redirect_uri_mismatch`, and failures on remote servers. OAuth on
LAN/VPS is particularly problematic.

** Come OmniRoute risolve il problema**:

- **Auto Token Refresh** — OAuth tokens refresh in background before expiration
- **OAuth 2.0 (PKCE) Built-in** — Automatic flow for Claude Code, Codex, Gemini
  CLI, Copilot, Kiro, Qwen, iFlow
- **Multi-Account OAuth** — Multiple accounts per provider via JWT/ID token
  extraction
- **OAuth LAN/Remote Fix** — Private IP detection for `redirect_uri` + manual
  URL mode for remote servers
- **OAuth Behind Nginx** — Uses `window.location.origin` for reverse proxy
  compatibility
- **Remote OAuth Guide** — Step-by-step guide for Google Cloud credentials on
  VPS/Docker

</details>

<details>
<summary><b>📊 9. "I don't know how much I'm spending or where"</b></summary>

Developers use multiple paid providers but have no unified view of spending.
Each provider has its own billing dashboard, but there's no consolidated view.
Unexpected costs can pile up.

** Come OmniRoute risolve il problema**:

- **Cost Analytics Dashboard** — Per-token cost tracking and budget management
  per provider
- **Budget Limits per Tier** — Spending ceiling per tier that triggers automatic
  fallback
- **Per-Model Pricing Configuration** — Configurable prices per model
- **Usage Statistics Per API Key** — Request count and last-used timestamp per
  key
- **Analytics Dashboard** — Stat cards, model usage chart, provider table with
  success rates and latency

</details>

<details>
<summary><b>🐛 10. "I can't diagnose errors and problems in AI calls"</b></summary>

==WEBLATE_PART==\
Quando un richiamo fallisce, il dev non sa se è un limite alle richieste, un
token scaduto, un formato sbagliato o un errore del fornitore. I log frammentati
su terminali diversi senza una visibilità corretta ne impedisce il debug, che
diventa un'esperienza "a tentativo e errore".

** Come OmniRoute risolve il problema**:

- **Unified Logs Dashboard** — 4 schede: Request Logs, Proxy Logs, Audit Logs,
  Console
- **Visualizzatore dei Log Console** — Visualizzatore in tempo reale con stili
  di colore, scorrimento automatico, ricerca, filtro
- **SQLite Proxy Logs** — Log persistenti che sopravvivono ai riavvii del server
- **Translator Playground** — 4 modalità di debug: Playground (traduzione del
  formato), Chat Tester (viaggio a ritroso), Test Bench (batch), Live Monitor
  (tempo reale)
- **Request Telemetry** — latenza p50/p95/p99 + X-Request-Id tracing
- **logging con file e rotazione** — Interfaccia in console cattura tutto il
  traffico in un log JSON con rotazione basata sulla dimensione
- **Rapporto di informazioni sul sistema** — `npm run system-info` genera
  `system-info.txt` con la tua intera ambiente (versione Node, versione
  OmniRoute, OS, strumenti CLI, stato Docker/PM2). Attaccalo quando segnali
  problemi per un triage istantaneo.

</details>

<details>
<summary><b>🏗️ 11. "Deploying and maintaining the gateway is complex"</b></summary>

L'installazione, la configuraizoni e la manutenzione di un proxy AI in ambienti
diversi (locale, VPS, Docker, cloud) è un processo laborioso. Problemi come
percorsi hardcoded, `EACCES` sui directory, conflitti di porta, costruzioni
cross-platforme e altri fanno frizione.

** Come OmniRoute risolve il problema**:

- **npm install globale** — `npm install -g omniroute &amp;&amp; omniroute` —
  fatto
- **Docker Multi-Platform** — AMD64 + ARM64 nativo (Apple Silicon, AWS Graviton,
  Raspberry Pi)
- **Profilo di composizione Docker** — `base` (senza strumenti CLI) e `cli` (con
  Claude Code, Codex, OpenClaw)
- **App desktop con Electron** — App nativa per Windows/macOS/Linux con icone
  sistem, avvio automatico, modalità offline
- **Modalità Split-Port** — API e Dashboard su porte separate per scenari
  avanzati (reverse proxy, rete dei container)
- **Sincronizzazione Cloud** — Configurazione sincronizzata tra dispositivi
  tramite Cloudflare Workers
- ** Backup della base dati** — Backup automatico, ripristino, esportazione e
  importazione di tutte le impostazioni

</details>

<details>
<summary><b>🌍 12. "The interface is English-only and my team doesn't speak English"</b></summary>

Le squadre in paesi non di lingua inglese, specialmente in America Latina, Asia
e Europa, hanno difficoltà con interfacce in lingua inglese. Ostacoli
linguistici riducono l'adottazione e aumentano gli errori di configurazione.

** Come OmniRoute risolve il problema**:

- ==WEBLATE_PART==\
  Painello Dashboard i18n — 30 linguaggi[31] — Tutti più di 500 tasti tradotti,
  inclusi Arabo, Bulgaro, Danese, Tedesco, Spagnolo, Finale, Francese, Ebraico,
  Hindi, Ungherese, Indonesiano, Italiano, Giapponese, Coreano, Malese,
  Olandese, Norvegese, Polacco, Portoghese (PT/BR), Rumeno, Russo, Slovacco,
  Svedese, Thai, Ucraino, Vietnamita, Cinese, Filipino, Inglese
- Supporto RTL** — Supporto da sinistra a destra per l'Arabo e l'Ebraico
- Panoramica Multi-Lingua dei README** — 30 traduzioni complete della
  documentazione
- Semplificatore delle Lingue** — Icona della Terra per l'accesso in tempo reale

</details>

<details>
<summary><b>🔄 13. "I need more than chat — I need embeddings, images, audio"</b></summary>

L'intelligenza artificiale non è solo la completazione dei dialoghi. Gli
sviluppatori devono generare immagini, trascrivere audio, creare embedding per
RAG, riarrendere i documenti e moderare il contenuto. Ogni API ha un endpoint e
un formato diversi.

** Come OmniRoute risolve il problema**:

- **Embedding** — `/v1/embedding` con 6 fornitori e 9+ modelli
- **Generazione delle Immagini** — `/v1/images/generazioni` con 10 fornitori e
  20+ modelli (OpenAI, xAI, Together, Fireworks, Nebius, Hiperbolic, NanoBanana,
  Antigravità, SD WebUI, ComfyUI)
- **Testo-Video** — `/v1/videos/generazioni` — ComfyUI (AnimateDiff, SVD) e SD
  WebUI
- **Testo-Musica** — `/v1/musica/generazioni` — ComfyUI (Audio stabile aperto,
  MusicGen)
- **Trascrizione Audio** — `/v1/audio/trascrizioni` — Whisper + Nvidia NIM,
  HuggingFace, Qwen3
- **Testo-in-Voce** — `/v1/audio/voce` — ElevenLabs, Nvidia NIM, HuggingFace,
  Coqui, Tortoise, Qwen3, **Inmondo**, **Cartesia**, **GiocaHT**, + fornitori
  esistenti
- **Moderazioni** — `/v1/moderazioni` — Verifiche di sicurezza del contenuto
- **Riordinamento** — `/v1/riordinamento` — Riordinamento della rilevanza dei
  documenti
- **API delle Risposte** — Supporto completo di `/v1/risposte` per Codex

</details>

<details>
<summary><b>🧪 14. "I have no way to test and compare quality across models"</b></summary>

Gli sviluppatori vogliono sapere quale modello è più adatto per il loro utilizzo
del caso — codice, traduzione, ragionamento — ma confrontare manualmente è
lento. Nessuno strumento di valutazione integrato esiste.

** Come OmniRoute risolve il problema**:

- **Valutazioni LLM** — Test da oro con 10 casi pre-caricati che coprono cenni
  di saluto, matematica, geografia, generazione di codice, conformità JSON,
  traduzione, markdown, rifiuto di sicurezza
- ** Strategie di Corrispondenza a 4** — `esatto`, `contiene`, `regex`,
  `personalizzato` (funzione JS)
- **Banchettino per Test Translatability** — Test di banchetto con input
  multipli e outputs previsti, confronto incrociato dei provider
- **Chat Tester** — Full round-trip con feedback visivo
- **Monitor in Tempo Reale** — Flusso in tempo reale di tutte le richieste che
  fluiscono attraverso il proxy

</details>

<details>
<summary><b>📈 15. "I need to scale without losing performance"</b></summary>

Man mano che la quantità di richieste cresce, senza caching le stesse domande
generano costi duplicati. Senza idempotenza, richieste duplicate sprecano
processor. I limiti di tariffa per-provider devono essere rispettati.

** Come OmniRoute risolve il problema**:

- **Cache Semantico** — Cache a due livelli (firma + semantico) riduce costo e
  latenza
- **Idempotenza delle Richieste** — Finestra di 5s per la deduplicazione di
  richieste identiche
- **Detezione dei Limite di Tariffa** — Tracciamento dei provider per RPM,
  minimo intervallo e massimo concorrente
- **Limite di Tariffa Modificabile** — Defalt di configurazione nei Settings →
  Resilienza con persistenza
- **Cache di Validazione delle Chiavi API** — Cache a 3 livelli per prestazioni
  in produzione
- **Dashborad di Salute con Telemetria** — Latenza p50/p95/p99, statistiche del
  cache, uptime

</details>

<details>
<summary><b>🤖 16. "I want to control model behavior globally"</b></summary>

Gli sviluppatori che desiderano tutte le risposte in una determinata lingua, con
un determinato tono o che desiderano limitare i token di ragionamento.
Configurare questo in ogni tool/richiesta è poco pratico.

** Come OmniRoute risolve il problema**:

- **Iniezione di Promp del Sistema** — Promp globale applicato a tutte le
  richieste
- **Validazione del Budget di Pensiero** — Controllo delle assegnazioni dei
  token di ragionamento per richiesta (passaparte, auto, personalizzato,
  adattativo)
- **6 Strategie di Routing** — Strategie globali che determinano come le
  richieste sono distribuite
- **Router Wildcard** — `provider/*` pattern invia dinamicamente a qualsiasi
  provider
- **Abilitazione/Sbattimento Combo** — Abilita/disabilita combo direttamente dal
  dashboard
- **Seleziona Provider** — Abilita/disabilita tutte le connessioni per un
  provider con un solo clic
- **Provider Bloccati** — Escludi provider specifici da /v1/models/X67X/ listare

</details>

<details>
<summary><b>🧰 17. "I need MCP tools as first-class product capabilities"</b></summary>

Molti gateway AI espongono MCP solo come dettaglio implementativo occulto. Gli
team hanno bisogno di uno strato di gestione visibile e gestibile.

** Come OmniRoute risolve il problema**:

- Navigazione della dashboard e scheda protocollo endpoint con MCP
- Pagina dedicata alla gestione di MCP con processi, strumenti, ambiti e audit
- Livello base per `omniroute --mcp` e sulla gestione del client

</details>

<details>
<summary><b>🧠 18. "I need A2A orchestration with sync + stream task paths"</b></summary>

Gli flussi di lavoro dell'agente richiedono entrambe risposte dirette e
esecuzioni a lungo corso con caricamento a ciclo di vita.

** Come OmniRoute risolve il problema**:

- Punto finale JSON-RPC A2A (`POST /a2a`) con `inviare messaggio` e `flusso di
  messaggio`
- Stream di eventi con propagazione dello stato dei termini
- API del ciclo di vita delle attività per `ottieni attività` e `annulla
  attività`

</details>

<details>
<summary><b>🛰️ 19. "I need real MCP process health, not guessed status"</b></summary>

Le squadre di operazioni devono sapere se MCP è realmente attiva, non solo se un
API è raggiungibile.

** Come OmniRoute risolve il problema**:

- File di feedback di runtime con PID, timestamp, trasporto, contatore degli
  strumenti e modalità di ambito
- API del status di MCP combinando feedback + attività recente
- Carte di status nella UI per uptime/processo/freschezza del feedback

</details>

<details>
<summary><b>📋 20. "I need auditable MCP tool execution"</b></summary>

Quando gli strumenti modificano la configurazione o attivano azioni di
operazione, le squadre hanno bisogno di tracciabilità forense.

** Come OmniRoute risolve il problema**:

- Log di audit supportati dal database SQLite per le chiamate del tool MCP
- Filtro da strumento, successo/fallimento, API key e pagination
- Tabella di audit della dashboard + punti finale per la statistica
  dell'automazione

</details>

<details>
<summary><b>🔐 21. "I need scoped MCP permissions per integration"</b></summary>

I client diversi dovrebbero avere accesso alle categorie degli strumenti con
privilegi di minori perenti.

** Come OmniRoute risolve il problema**:

- 9 ambiti di autorizzazione di accesso a strumenti dettagliati e controllabile
- Rispetto e visibilità del piano di controllo nell'interfaccia di
  amministrazione del MCP
- Postura predefinita sicura per attrezzature operative

</details>

<details>
<summary><b>⚙️ 22. "I need operational controls without redeploying"</b></summary>

Gli team necessitano di modifiche velocizzate del runtime durante incidenti o
eventi di costo.

** Come OmniRoute risolve il problema**:

- Attivazione di comb della commuta direttamente dall'interfaccia di dashboard
  del MCP
- Applicazione di profili di resilienza da pacchetti di politiche predefinite
- Azzeramento dello stato blocca circuito direttamente dal pannello di
  operazioni

</details>

<details>
<summary><b>🔄 23. "I need live A2A task lifecycle visibility and cancellation"</b></summary>

Senza visibilità del ciclo di vita, gli incidenti di compito diventano difficili
da triare.

** Come OmniRoute risolve il problema**:

- Elenco e filtri dei compiti per stato/skill con paginazione
- Zoom di compito sul metadata, eventi e artefatti
- Indicatore di annullamento del compito con conferma endpoint e UI

</details>

<details>
<summary><b>🌊 24. "I need active stream metrics for A2A load"</b></summary>

I flussi di lavoro in streaming richiedono visibilità operativa nel concorso e
connessioni vive.

** Come OmniRoute risolve il problema**:

- Conticadori di flusso attivi integrati nello stato A2A
- Ultimo timestamp del compito e conteggi per stato
- Carte della dashboard A2A per monitoraggio opp a tempo reale

</details>

<details>
<summary><b>🪪 25. "I need standard agent discovery for clients"</b></summary>

I clienti esterni e orchestratori richiedono metadata a lettura macchina per
l'accesso.\
==WEBLATE_PART==

** Come OmniRoute risolve il problema**:

- Agent Card exposed at `/.well-known/agent.json`
- Capabilities and skills shown in management UI
- A2A status API includes discovery metadata for automation

</details>

<details>
<summary><b>🧭 26. "I need protocol discoverability in the product UX"</b></summary>

If users cannot discover protocol surfaces, adoption and support quality drop.

** Come OmniRoute risolve il problema**:

- Consolidated **Endpoints** page with tabs for Proxy, MCP, A2A, and API
  Endpoints
- Inline service status toggles (Online/Offline) for MCP and A2A
- Links from overview to dedicated management tabs

</details>

<details>
<summary><b>🧪 27. "I need end-to-end protocol validation with real clients"</b></summary>

Mock tests are not enough to validate protocol compatibility before release.

** Come OmniRoute risolve il problema**:

- E2E suite that boots app and uses real MCP SDK client transport
- A2A client tests for discovery, send, stream, get, and cancel flows
- Cross-check assertions against MCP audit and A2A tasks APIs

</details>

<details>
<summary><b>📡 28. "I need unified observability across all interfaces"</b></summary>

Splitting observability by protocol creates blind spots and longer MTTR.

** Come OmniRoute risolve il problema**:

- Unified dashboards/logs/analytics in one product
- Health + audit + request telemetry across OpenAI, MCP, and A2A layers
- Operational APIs for status and automation

</details>

<details>
<summary><b>💼 29. "I need one runtime for proxy + tools + agent orchestration"</b></summary>

Running many separate services increases operational cost and failure modes.

** Come OmniRoute risolve il problema**:

- Proxy compatibile con OpenAI, server MCP e server A2A in un unico stack
- Auth condivisa, resilienza, archiviazione dei dati e visibilità
- Modello di politica coerente per tutte le superfici delle interazioni

</details>

<details>
<summary><b>🚀 30. "I need to ship agentic workflows without glue-code sprawl"</b></summary>

Gli equipaggi perdono velocità quando devono integrare più servizi e script
ad-hoc.

** Come OmniRoute risolve il problema**:

- Strategy di endpoint unificata per i clienti e gli agenti
- Interfacce di dialogo di protocollo integrate e percorsi di validazione al
  fumo
- Basi di produzione pronte per essere utilizzate (sicurezza, logging,
  resilienza, backup)

</details>

### Esempi di Playbook (Utilizzo Integrato)

**Playbook A: massimizzazione della sottoscrizione a pagamento + backup
economico**

```txt
Combo: “massimizza-claude”
  1. cc/claude-opus-4-6
  2. glm/glm-4.7
  3. if/kimi-k2-thinking

Costo mensile: $20 + spesa per backup di piccole dimensioni
Outcome: maggiore qualità, zero interruzioni
```

**Playbook B: stack di codifica zero-costante**

```txt
Combo: “gratuito-forever”
  1. gc/gemini-3-flash
  2. if/kimi-k2-thinking
  3. qw/qwen3-coder-plus

Costo mensile: $0
Outcome: flusso di lavoro di codifica stabile e gratuito
```

**Playbook C: catena di fallback 24/7 sempre attiva**

```txt
Combo: “sempre attivo”
  1. cc/claude-opus-4-6
  2. cx/gpt-5.2-codex
  3. glm/glm-4.7
  4. minimax/MiniMax-M2.1
  5. if/kimi-k2-thinking

Outcome: profonda profondità di fallback per carichi di lavoro critici per la scadenza
```

**Playbook D: operazioni degli agenti con MCP + A2A**

```txt
1) Avvia il trasporto MCP (`omniroute --mcp`) per operazioni guidate dalle tool
2) Esecuzione delle attività A2A tramite `messaggio/envia` e `messaggio/stream`
3) Osserva tramite /dashboard/endpoint (pannelli MCP e A2A)
4) Attiva/disattiva le funzionalità tramite controlli di stato inline
```

---

## 🆓 Inizia a utilizzare gratuitamente — Nesso Costo di Configurazione

> Configura la codifica AI in pochi minuti al costo di **$0/mese**. Collega
> questi conti gratuitamente e utilizza la combinazione di **stack Gratuito**.

| Etapa | Azione                                               | Provider sbloccati                                                    |
| ----- | ---------------------------------------------------- | --------------------------------------------------------------------- |
| 1     | Connetti **Kiro** (ID di costruttore AWS OAuth)      | Claude 4.5, Haiku 4.5 — **senza limiti**                              |
| 2     | Connetti **iFlow** (Google OAuth)                    | kimi-k2-thinking, qwen3-coder-plus, deepseek-r1... — **senza limiti** |
| 3     | Connetti **Qwen** (Codice dispositivo)               | qwen3-coder-plus, qwen3-coder-flash... — **senza limiti**             |
| 4     | Connetti **Gemini CLI** (Google OAuth)               | gemini-3-flash, gemini-2.5-pro — **180K/mese gratuito**               |
| 5     | `/dashboard/combos` → **Pila Gratuito ($0)** modello | Distribuisci tutte le provider gratuite automaticamente               |

**Point qualsiasi IDE/CLI a:** `http://localhost:20128/v1` · Chiave API:
`qualsiasi-stringa` · Completato.

> **Copertura extra facoltativa (anche gratuita):** Chiave API Groq (30 RPM
> gratuita), NVIDIA NIM (40 RPM gratuita, 70+ modelli), Cerebras (1M
> tok/giorno), Chiave API LongCat (50M token/giorno!, Cloudflare Workers AI (10K
> Neuroni/giorno, 50+ modelli).

## Avvio rapido

### 1. Installa ed esegui

```bash
npm install -g omniroute
omniroute
```

> **pnpm users:** Run `pnpm approve-builds -g` after install to enable native
> build scripts required by `better-sqlite3` and `@swc/core`:
> 
> ```bash
> pnpm install -g omniroute
> pnpm approve-builds -g   # Select all packages → approve
> omniroute
> ```

Dashboard opens at `http://localhost:20128` and API base URL is
`http://localhost:20128/v1`.

| Command                 | Description                                                 |
| ----------------------- | ----------------------------------------------------------- |
| `omniroute`             | Start server (`PORT=20128`, API and dashboard on same port) |
| `omniroute --port 3000` | Set canonical/API port to 3000                              |
| `omniroute --mcp`       | Start MCP server (stdio transport)                          |
| `omniroute --no-open`   | Don't auto-open browser                                     |
| `omniroute --help`      | Show help                                                   |

Optional split-port mode:

```bash
PORT=20128 DASHBOARD_PORT=20129 omniroute
# API:       http://localhost:20128/v1
# Dashboard: http://localhost:20129
```

### 1) Collega gli fornitori e crea la tua chiave API

1. Apri la Dashboard → `Fornitori` e collega almeno un provider (OAuth o chiave
   API).
2. Apri la Dashboard → `Endpoint` e crea una chiave API.
3. (Opzionale) Apri la Dashboard → `Combo` e impostare la tua catena fallback.

### 3) Puntala tua strumento di sviluppo a OmniRoute

```txt
URL di base: http://localhost:20128/v1
Chiave API:  [copia dalla pagina Endpoint]
Modello:    se/kimi-k2-thinking (o qualsiasi prefisso provider/model)
```

Funziona con Claude Code, Codex CLI, Gemini CLI, Cursor, Cline, OpenClaw,
OpenCode e SDK compatibili con OpenAI.

### 4) Attiva e valida i protocolli (v2.0)

**MCP (per operazioni guidate dalla strumentazione):**

```bash
omniroute --mcp
```

Poi colleghi il tuo client MCP attraverso `stdio` e testa gli strumenti come:

- `omniroute_get_health`
- `omniroute_list_combos`

**A2A (per workflow di agente-agente):**

```bash
curl http://localhost:20128/.well-known/agent.json
```

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"quickstart","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"Dacci una breve riassunto della quota."}]}}'
```

### 5) Valida tutto all'interno di un flusso end-to-end (consigliato)

```bash
npm run test:protocollo:e2e
```

Questo suite valuta flussi reali di MCP e A2A clienti contro una finestra di
esecuzione.

### Altrimenti: esegui da sorgente.

```bash
cp .env.example .env
npm install
PORT=20128 DASHBOARD_PORT=20129 NEXT_PUBLIC_BASE_URL=http://localhost:20129 npm run dev
```

---

## 🐳 Container

OmniRoute è disponibile come immagine di Docker pubblica su [Docker
Hub](https://hub.docker.com/r/diegosouzapw/omniroute).

**Esegui velocemente:**

```bash
docker run -d \
  --name omniroute \
  --restart unless-stopped \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:latest
```

**Con file di ambiente:**

```bash
# Copia e modifica .env prima
cp .env.example .env

docker run -d \
  --name omniroute \
  --restart unless-stopped \
  --env-file .env \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:latest
```

**Utilizza Docker Compose:**

```bash
# Profilo di base (nessun strumento CLI)
docker compose --profile base up -d

# Profilo CLI (Claude Code, Codex, OpenClaw integrato)
docker compose --profile cli up -d
```

| Immagine                 | Etichetta     | Misurare | Description             |
| ------------------------ | ------------- | -------- | ----------------------- |
| `diegosouzapw/omniroute` | `più recente` | ~250MB   | Ultima versione stabile |
| `diegosouzapw/omniroute` | `1.0.3`       | ~250MB   | Versione corrente       |

---

## Scheda di lavoro Desktop — Offline e Sempre disponibile

> 🆕 **NUOVO ** OmniRoute è ora disponibile come applicazione desktop nativa **
> nativa per Windows, macOS e Linux.

Esegui OmniRoute come'applicazione desktop stante — non è richiesto terminale,
browser o connessione internet per i modelli locali. L'app, basata su Electron,
include:

- 🖥️ **Finestra Nativa** — finestra app dedicata con integrazione di sistema del
  pannello di sistema
- 🔄 **Avvio automatico** — lancia OmniRoute all'avvio del sistema
- 🔔 **Notifiche native** — ricevi aggiornamenti per la esaustione del
  quantitativo o le problematiche dei fornitori
- ⚡ **Installesione rapida con un sol click** — NSIS (Windows), DMG (macOS),
  AppImage (Linux)
- 🌐 **Modalità offline** — funziona completamente in modalità offline con server
  integrato

### Avvio rapido

```bash
# Modo di sviluppo
npm run electron:dev

# Costruisci il tuo platform
npm run electron:build         # Platform corrente
npm run electron:build:win     # Windows (.exe)
npm run electron:build:mac     # macOS (.dmg) — x64 &amp; arm64
npm run electron:build:linux   # Linux (.AppImage)
```

### Pannello del sistema

Quando minimizzato, OmniRoute vive nel pannello del sistema con azioni rapide:

- Apri Dashboard
- Cambia porta del server
- Esci dall'applicazione

📖 Documentazione completa: [`electron/README.md`](electron/README.md)

---

## 💰 Prezzi in un'occhiata

| Livello                | Provider                      | Costo                                     | Ricarica del quantitativo           | Migliore per te                            |
| ---------------------- | ----------------------------- | ----------------------------------------- | ----------------------------------- | ------------------------------------------ |
| **💳 ABONAMENTO**       | Claude Codice (Pro)           | $20/a mese                                | 5h + settimanale                    | Sono già abbonato                          |
|                        | Codex (Plus/Pro)              | $20-200/a mese                            | 5h + settimanale                    | Utilizzatori di OpenAI                     |
|                        | Gemini CLI                    | **FREE**                                  | 180K/a mese + 1K/al giorno          | Tutti!                                     |
|                        | Copilota GitHub               | $10-19/a mese                             | Mensile                             | Utilizzatori di GitHub                     |
| **🔑 CHIAVE API**       | NVIDIA NIM                    | **FREE** (per sempre in fase di sviluppo) | 40 RPM                              | 70+ modelli aperti                         |
|                        | Cerebras                      | **GRAZIE** (1M tok/giorno)                | 60.000 TPM / 30 RPM                 | Più veloce del mondo                       |
|                        | Groq                          | **GRAZIE** (30 RPM)                       | 14.400 RPD                          | Tecnologia Llama/Gemma ultra veloce        |
|                        | DeepSeek V3.2                 | $0,27/$1,10 per 1M                        | Nessuno                             | Meglio rispetto ad altri perché            |
|                        | xAI Grok-4 Rilevamento rapido | **$0,20/$0,50 per 1M**                    | Nessuno                             | Migliore velocità + chiamate da strumenti  |
|                        | xAI Grok-4 (standard)         | $0,20/$1,50 per 1M                        | Nessuno                             | Bandiera per la ragionamento di xAI        |
|                        | Mistral                       | Prova gratuita + a pagamento              | Tariffa limitata                    | Intelligenza artificiale europea           |
|                        | OpenRouter                    | Pagamento a consumo                       | Nessuno                             | Aggregazione di 100+ modelli               |
| ** 💰 CHEAP **          | GLM-5 (via Z.AI)  🆕           | $ 0,50/1M                                 | Ogni giorno alle 10 AM              | 128K output, nuovo flagship                |
|                        | GLM-4.7                       | $ 0,60/1M                                 | Ogni giorno alle 10 AM              | Backup di budget                           |
|                        | MiniMax M2.5  🆕               | $ 0,30/1M di input                        | Rolling della finestra oraria 5 ore | Compito di ragionamento + esercizio agente |
|                        | MiniMax M2.1                  | $0,2/1M                                   | Rolling della finestra oraria 5 ore | Opzione più economica                      |
|                        | Kimi K2.5 (API Moonshot) 🆕    | Pagamento a consumo                       | Nessuno                             | Accesso diretto all'API Moonshot           |
|                        | Kimi K2                       | $9/a/mo flat                              | 10M token/mo                        | Costo prevedibile                          |
| ** 🆓 GRAZIE Gratuito** | iFlow                         | **$0**                                    | Senza limiti                        | 5 modelli illimitati                       |
|                        | Qwen                          | **$0**                                    | Senza limiti                        | 4 modelli illimitati                       |
|                        | Kiro                          | **$0**                                    | Senza limiti                        | Claude Sonnet/Haiku (AWS Builder)          |
|                        | LongCat Flash-Lite 🆕          | **$0** (50M token/giorno 🔥)               | 1 RPS                               | La tariffa libera più grande sulla terra   |
|                        | Pollinazione AI 🆕             | **$0** (nessuna chiave necessaria)        | 1 req/15s                           | GPT-5, Claude, DeepSeek, Llama 4           |
|                        | Cloudflare Workers AI 🆕       | **$0** (10K Neuroni/giorno)               | ~150 resp/giorno                    | 50+ modelli, edge globale                  |
|                        | Scaleway AI 🆕                 | **$0** (1M tokeni totali)                 | Tariffa limitata                    | UE/GDPR, Qwen3 235B, Llama 70B             |

> 🆕 **Modelli nuovi aggiunti (marzo 2026):** Famiglia Grok-4 Rapido a
> $0,20/$0,50/M (verificato a 1143ms - 30% più veloce di Gemini 2.5 Flash),
> GLM-5 via Z.AI con 128K output, MiniMax M2.5 ragionamento, DeepSeek V3.2
> prezzi aggiornati, Kimi K2.5 via Moonshot API diretta.

**💡 Combo Gratuito Stacked - La configurazione completa e gratuita:**

```
# 🆓 Stacca Free Ultimate 2026 - 11 Provider, $0 Forever
Kiro (kr/)             → Claude Sonnet/Haiku SENZA LIMITI
iFlow (if/)            → kimi-k2-pensiero, qwen3-coder-plus, deepseek-r1 SENZA LIMITI
LongCat Lite (lc/)     → LongCat-Flash-Lite — 50M tokens/giorno 🔥
Pollinazioni (pol/)    → GPT-5, Claude, DeepSeek, Llama 4 — nessuna chiave necessaria
Qwen (qw/)             → qwen3-coder-plus, qwen3-coder-Flash, qwen3-coder-next SENZA LIMITI
Gemini (gemini/)       → Gemini 2.5 Flash — 1.500 req/giorno gratuito API chiave
Cloudflare AI (cf/)    → Llama 70B, Gemma 3, Mistral — 10K Neuroni/giorno
Scaleway (scw/)        → Qwen3 235B, Llama 70B — 1M tokeni gratuiti (UE)
Groq (groq/)           → Llama/Gemma ultra-veloce — 14.400 req/giorno
NVIDIA NIM (nvidia/)   → 70+ modelli aperti — 40 RPM per sempre
Cerebras (cerebras/)   → Llama/Qwen il più rapido del mondo — 1M tok/giorno
```

**A zero costo. Mai smette di codificare.** Configura questo come un combo
OmniRoute a zero costo e tutti i fallback avvengono automaticamente - non è mai
necessario effettuare un cambio manuale.

---

---

## 🆓 Modelli gratuiti — Cosa otteni effettivamente

> Tutti i modelli sotto sono **del 100% gratuito con zero carta di credito
> richiesta**. OmniRoute rinvia automaticamente tra di loro quando uno quota
> esaurisce — combinarli tutti per un combo intangibile a $0.

### 🔵 MODELLI DI CLAUDE (via Kiro — ID del costruttore AWS)

| Model               | Prefisso | limit            | Limite di velocità                  |
| ------------------- | -------- | ---------------- | ----------------------------------- |
| `claude-sonnet-4.5` | `kr/`    | **Senza limiti** | Nessuna cappa giornaliera riportata |
| `claude-haiku-4.5`  | `kr/`    | **Senza limiti** | Nessuna cappa giornaliera riportata |
| `claude-opus-4.6`   | `kr/`    | **Senza limiti** | Ultime opere tramite Kiro           |

### 🟢 MODELLI SEQUENZIALI DI I-FLOW (OAuth gratuito – Nessuna carta di credito richiesta)

| Model                 | Prefisso | limit            | Limite di velocità      |
| --------------------- | -------- | ---------------- | ----------------------- |
| `kimi-k2-thinking`    | `if/`    | **Senza limiti** | Nessuna cappa riportata |
| `qwen3-coder-plus`    | `if/`    | **Senza limiti** | Nessuna cappa riportata |
| `Ricerca Avanzata-d1` | `if/`    | **Senza limiti** | Nessuna cappa riportata |
| `minimax-m2.1`        | `if/`    | **Senza limiti** | Nessuna cappa riportata |
| `kimi-k2`             | `if/`    | **Senza limiti** | Nessuna cappa riportata |

### 🟡 MODELLI QWEN (Codice Autenticazione Device)

| Model                  | Prefisso | limit            | Limite di velocità      |
| ---------------------- | -------- | ---------------- | ----------------------- |
| `qwen3-coder-plus`     | `qw/`    | **Senza limiti** | Nessuna cappa riportata |
| `qwen3-coder-flash`    | `qw/`    | **Senza limiti** | Nessuna cappa riportata |
| `qwen3-coder-prossimo` | `qw/`    | **Senza limiti** | Nessuna cappa riportata |
| `modello visione`      | `qw/`    | **Senza limiti** | Multimodale (immagini)  |

### 🟣 CLI di GEMINI (Google OAuth)

| Model                    | Prefisso | limit                            | Limite di velocità |
| ------------------------ | -------- | -------------------------------- | ------------------ |
| `gemini-3-flash-preview` | `gc/`    | **180K tok al mese** + 1K/giorno | Ricompensa mensile |
| `gemini-2.5-pro`         | `gc/`    | 180K al mese (piscina condivisa) | Qualità superiore  |

### NVIDIA NIM (Chiave API gratuita — build.nvidia.com)

| Livello      | Limite giornaliero  | Limite di velocità | Note                                                          |
| ------------ | ------------------- | ------------------ | ------------------------------------------------------------- |
| Gratis (Dev) | No limite dei token | **~40 RPM**        | 70+ modelli; transizione a limiti di tariffe pure a metà 2025 |

Modelli gratuiti popolari: `moonshotai/kimi-k2.5` (Kimi K2.5), `z-ai/glm4.7`
(GLM 4.7), `deepseek-ai/deepseek-v3.2` (DeepSeek V3.2),
`nvidia/llama-3.3-70b-instruct`, `deepseek/deepseek-r1`

### CEREBRAS (Chiave API gratuita — inference.cerebras.ai)

| Livello  | Limite giornaliero   | Limite di velocità  | Note                                                                   |
| -------- | -------------------- | ------------------- | ---------------------------------------------------------------------- |
| Gratuito | **1M tokeni/giorno** | 60.000 TPM / 30 RPM | Velocità di inferenza dell'LTRD più veloce al mondo; reset ogni giorno |

Disponibile gratuitamente: `llama-3.3-70b`, `llama-3.1-8b`,
`deepseek-r1-distill-llama-70b`

### 🔴 GROQ (Chiave API gratuita — console.groq.com)

| Livello  | Limite giornaliero | Limite di velocità | Note                                                                             |
| -------- | ------------------ | ------------------ | -------------------------------------------------------------------------------- |
| Gratuito | **14.4K RPD**      | 30 RPM per modello | Nessuna carta di credito; 429 al raggiungimento del limite, non viene addebitato |

Disponibile gratuitamente: `llama-3.3-70b-versatile`, `gemma2-9b-it`,
`mixtral-8x7b`, `whisper-large-v3`

### 🔴 LONGCAT AI (Chiave API gratuita — longcat.chat) 🆕

| Model                         | Prefisso | Quote quotidiano gratuito | Note                                |
| ----------------------------- | -------- | ------------------------- | ----------------------------------- |
| `LongCat-Flash-Lite`          | `lc/`    | **50M token** 💥           | Quota gratuita più grande mai vista |
| `LongCat-Flash-Chat`          | `lc/`    | 500K token                | Chat a piu domande                  |
| `LongCat-Flash-Thinking`      | `lc/`    | 500K token                | Ragionamento / CoT                  |
| `LongCat-Flash-Thinking-2601` | `lc/`    | 500K token                | Versione gennaio 2026               |
| `LongCat-Flash-Omni-2603`     | `lc/`    | 500K token                | Multimodale                         |

> 100% gratuito fino alla pubblicazione beta. Iscrivetevi a
> [longcat.chat](https://longcat.chat) con la mail o telefono. Si resetta ogni
> giorno 00:00 UTC.

### 🟢 POLITIA DI INTELLOTTO (Non richiede Chiave API) 🆕

| Model      | Prefisso | Limite di velocità | Fornitore Dietro   |
| ---------- | -------- | ------------------ | ------------------ |
| `openai`   | `pol/`\  | 1 req/15s          | GPT-5              |
| `claude`   | `pol/`\  | 1 req/15s          | Antropico Claude   |
| `gemini`   | `pol/`\  | 1 req/15s          | Google Gemini      |
| `deepseek` | `pol/`\  | 1 req/15s          | DeepSeek V3        |
| `llama`    | `pol/`\  | 1 req/15s          | Meta Llama 4 Scout |
| `mistral`  | `pol/`\  | 1 req/15s          | Mistral AI         |

> ✨ **Assenza di frizione:** Nessuna registrazione, nessuna API key. Aggiungi il
> fornitore Pollinations con un campo tasti vuoto e funziona immediatamente.

### 🟠 LAVORATORI CLOUDFLARE AI ( Chiave API gratuita — cloudflare.com) 🆕

| Livello  | Neuroni Giornalieri | Usaggio Equivalente                           | Note                            |
| -------- | ------------------- | --------------------------------------------- | ------------------------------- |
| Gratuito | 10.000**20.000**    | ~150 modello LLM ogni 500s audio / 15K embeds | Estensione globale, 50+ modelli |

Modelli di tipo libero: `@cf/meta/llama-3.3-70b-instruct`,
`@cf/google/gemma-3-12b-it`, `@cf/openai/whisper-large-v3-turbo` (audio
gratuito!), `@cf/qwen/qwen2.5-coder-15b-instruct`

> È richiesto un Token API + ID Account da
> [dash.cloudflare.com](https://dash.cloudflare.com). Memorizza l'ID Account
> negli impostazioni del provider.

### SCALEWAY AI (1M token gratuiti — scaleway.com) 🆕

| Livello  | Quota Gratuito                  | Localizzazione | Note                                             |
| -------- | ------------------------------- | -------------- | ------------------------------------------------ |
| Gratuito | 10.000 token gratuiti**20.000** | 🇫🇷 Parigi, UE  | Non è necessaria carta di credito entro i limiti |

Disponibile gratuitamente: `qwen3-235b-a22b-instruct-2507` (Qwen3 235B!),
`llama-3.1-70b-instruct`, `mistral-small-3.2-24b-instruct-2506`,
`deepseek-v3-0324`

> In conformità con la normativa UE/GDPR. Otteni la chiave API al
> [console.scaleway.com](https://console.scaleway.com).

> ** 💡 La Stacks di Tipo Libero Definitivo (11 Provider, 0€ Per sempre):**
> 
> ```
> Kiro (kr/)             → Claude Sonnet/Haiku ILLIMITATI
> iFlow (if/)            → kimi-k2-thinking, qwen3-coder-plus, deepseek-r1 ILLIMITATI
> LongCat Lite (lc/)     → LongCat-Flash-Lite — 50M token/day  🔥
> Pollinations (pol/)    → GPT-5, Claude, DeepSeek, Llama 4 — nessuna chiave necessaria
> Qwen (qw/)             → qwen3-coder model ILLIMITATI
> Gemini (gemini/)       → Gemini 2.5 Flash — 1.500 req/day gratuito
> Cloudflare AI (cf/)    → 50+ modelli — 10K Neuron/day
> Scaleway (scw/)        → Qwen3 235B, Llama 70B — 1M token gratuito (EU)
> Groq (groq/)           → Llama/Gemma — 14.400 req/day ultra-scelto
> NVIDIA NIM (nvidia/)   → 70+ modelli aperti — 40 RPM per sempre
> Cerebras (cerebras/)   → Llama/Qwen il mondo più velocissimo — 1M tok/day
> ```

## 🎙️ Combo Transcrizione Gratuita

> Trascrivi qualsiasi audio/video per **$0** — Deepgram tiene con $200 gratuito,
> AssemblyAI $50 fallback, Groq Whisper come backup di emergenza illimitato.

| Provider         | Crediti Gratuiti               | Modello Migliore                              | Limite di velocità                           |
| ---------------- | ------------------------------ | --------------------------------------------- | -------------------------------------------- |
| 🟢 **Deepgram**   | **$200 gratuito** (iscrizione) | `nova-3` — miglior accuratezza, 30+ lingue    | Limite RPM non applicato ai crediti gratuiti |
| 🔵 **AssemblyAI** | **$50 gratuito** (iscrizione)  | `universal-3-pro` — capitoli, sentimento, PII | Limite RPM non applicato ai crediti gratuiti |
| 🔴 **Groq**       | **Gratuito per sempre**        | `whisper-large-v3` — OpenAI Whisper           | 30 RPM (limitato al tasso)                   |

**Combo consigliato in `/dashboard/combos`:**

```
Nome: trascrizione-gratuita
Strategy: Priorità
Nodi:
  [1] deepgram/nova-3          → utilizza i $200 gratuiti per primo
  [2] assemblyai/universal-3-pro → fallback quando i crediti Deepgram sono esauriti
  [3] groq/whisper-large-v3    → gratuito per sempre, fallback di emergenza
```

Poi in `/dashboard/media` → **Trascrizione** scheda: caricare qualunque file di
audio o video → selezionare il proprio endpoint di combinazione → ottenere la
trascrizione nei formati supportati.

## 💡 Funzioni chiave

OmniRoute 2.0 è costruito come piattaforma operativa e non solo come un proxy di
trasferimento.

### 🆕 Nuovo — Miglioramenti ispirati da ClawRouter (Mar 2026)

| Funzione                               | Cos'è fatto esattamente                                                                                                   |
| -------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| ⚡ **Grok-4 Fast Family**               | Modelli AI per $0,20/$0,50/M — misurato in 1143ms (30% più veloce del Gemini 2.5 Flash)                                   |
| 🧠 **GLM-5 via Z.AI**                   | Contesto di output di 128K, $0,5/1M — nuovo spigot di testa della famiglia GLM                                            |
| 🔮 **MiniMax M2.5**                     | Compiti di ragionamento + agente ad $0,30/1M — notevole miglioramento rispetto a M2.1                                     |
| 🎯 **flag di chiamata per Modello**     | [XX]flag di chiamata` per modello nel registro: v true/false — AutoCombo salta i modelli non capaci di strumenti          |
| 🌍 **Detezione di Intento Multilingue** | Parole chiave PT/ZH/ES/AR in AutoCombo per stimare — scelta migliore del modello per contenuti non inglesi                |
| 📊 **Fallback guidati dai Benchmark**   | Latenza reale p95 dalle richieste live in scoraggiamento combinazione — AutoCombo impara dai dati reali                   |
| 🔁 **Deduplicazione Richiesta**         | Finestra di deduplicazione basata sulla hash dei contenuti — sicuro per agenti multipli, prevenzione di carichi duplicati |
| 🔌 **Router di strategia plugabble**    | Interfaccia di estensione `RouterStrategy` — aggiungi logica di routing personalizzata come plugin                        |

### 🚀 V2.0.9+ precedente — Gioco di prova, CLI Fingerprints & ACP

| Funzione                                                   | Cos'è fatto esattamente                                                                                                                                                                                                                                                                                               |
| ---------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🎮 **Playground del modello**                               | Pagina periferica per testare qualsiasi modello direttamente — selezionatori provider/modello/endpoint, Monaco Editor, streaming, aborto, timing                                                                                                                                                                      |
| 🔏 **Inquadramento dei CLI per il match**                   | Ordinamento header/body per provider per sincronizzare con le firme native CLI — abilita/disabilita per provider nelle Impostazioni > Sicurezza. **Il tuo indirizzo IP proxy non viene modificato**                                                                                                                   |
| 🤝 **Supporto ACP (Protocollo Cliente Agente)**             | Scoperta dell'agente CLI (Codex, Claude, Goose, Gemini CLI, OpenClaw + 9 altri), avviamento processo, `/api/acp/agenty` endpoint                                                                                                                                                                                      |
| 🤖 **Dashbord degli Agenti ACP**                            | Pagina di debug ‹ Agenti — griglia dei 14 agenti con stato di installazione, versione, forma customizzata dell'agente per qualsiasi strumento CLI. **Utenti di OpenCode** hanno un pulsante "Scarica opencode.json" che genera automaticamente un file configurazione pronto all'uso con tutti i modelli disponibili. |
| 🔧 **Routing personalizzato dell' `apiFormat` del modello** | Modelli personalizzati con `apiFormat: "risposte"` correttamente inviano all'API di traduzione delle risposte                                                                                                                                                                                                         |
| 🏢 **Isolamento dello spazio di lavoro Codex**              | Più spazi di lavoro Codex per e-mail — OAuth separa correttamente le connessioni per ID dello spazio di lavoro                                                                                                                                                                                                        |
| 🔄 **Aggiornamento Automatico di Electron**                 | L'app di desktop controlla gli aggiornamenti + auto-installa all'avvio                                                                                                                                                                                                                                                |

### 🤖 Operazioni dell'Agente e del Protocollo (v2.0)

| Funzione                                                  | Cos'è fatto esattamente                                                                                              |
| --------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| 🔧 **Server MCP (16 strumenti)**                           | IDE/strumento agente tramite 3 trasporti: stdio, SSE (`/api/mcp/sse`), HTTP flusso gestibile (`/api/mcp/stream`)     |
| 🤝 **Server A2A (JSON-RPC + SSE)**                         | Esecuzione task agente-agente con flussi di sincronizzazione e streaming                                             |
| 🧭 ** pagina di estremi consolidati**                      | Pagina di gestione tabulata con endpoint proxy, MCP, A2A e endpoint dell'API                                         |
| 🎚️ **Regolatori di abilitazione/disenabili dei servizi**  | Scommutatori di selezione (ON/OFF) con persistenza dell'impostazione (predefinito: OFF)                              |
| 🛰️ **Heartbeat runtime del MCP**                          | Stato del processo reale (id processo, uptime, età heart, trasporto, modalità scope)                                 |
| 📋 **Tracciato di audit del MCP**                          | Log di audit filtrabili con successo/fallimento e attribuzione chiave                                                |
| 🔐 **Implementazione dell'attribuzione del scope del MCP** | 9 diritti di attribuzione del scope dettagliati per l'accesso ai strumenti controllati                               |
| 📡 **Gestione del ciclo di vita dei task A2A**             | Lista/articoli task, evento/articoli dettagli, annullamento dei task in esecuzione                                   |
| 📋 **Scoperta della scheda agente**                        | `/.well-known/agent.json` per la scoperta auto-dell'agente del client                                                |
| 🧪 **Protocolo E2E Test Harness**                          | Real MCP SDK + client flussi A2A in `test:protocols:e2e`                                                             |
| ⚙️ **Controllo Opzionale**                                | Combobox del pulsante, applica profili di resilienza, resettare i traghettatori da un'interfaccia di controllo unica |

### 🧠 Rilevamento & Intelligenza

| Funzione                                       | Cos'è fatto esattamente                                                                                     |
| ---------------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| 🎯 **Fallback Avanzato Smart 4-Tier**           | Inoltro automatico: Sottoscrizione → Chiave API → Economico → Gratuito                                      |
| 📊 **Monitoraggio dei Quoti in Tempo Reale**    | Conteggio in tempo reale dei token + conteggio di reset per provider                                        |
| 🔄 **Conversione del Format**                   | OpenAI ⇌ Claude ⇌ Gemini ⇌ Risposte con conversioni sicure dello schema                                     |
| 👥 **Supporto per Account Molti**               | Più account per provider con selezione intelligente                                                         |
| 🔄 **Rinnovo di Token Automatico**              | I token OAuth si rinnovano automaticamente con riprova                                                      |
| 🎨 **Combinazioni Custoizziate**                | 6 strategie di bilanciamento + controllo della catena di fallback                                           |
| 🌐 **Router Universale**                        | `fornitore/*` routing dinamico                                                                              |
| 🧠 **Budget dei Controlli di Pensiero**         | Tecniche di passaggio automatico, personalizzate e limiti di ragionamento adattive                          |
| 🔀 **Alias dei Modelli**                        | Il supporto integrato + le abilità di aliasaggio dei modelli personalizzato e la sicurezza della migrazione |
| ⚡ **Decrescita in Background**                 | Trasferisci le attività di background a basso priorità ai modelli più economici                             |
| 🧪 **Smart Routing Consapevole delle Task**     | Scegli automaticamente il modello in base al tipo di contenuto (codifica/visione/analisi/sommarizzazione)   |
| 💬 **Iniezione di Prompt alla Stringa Sistema** | Controlli di comportamento globali applicati in modo coerente                                               |
| 📄 **Compatibilità dell'API delle Risposte**    | Supporto completo per Codex e flussi agenziali avanzati delle classi [/v1/responses`                        |

### 🎵 API Multi-Modali

| Funzione                       | Cos'è fatto esattamente                                                                                                                                                                |
| ------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🖼️ **Generazione di Immagini** | Genera [/v1/images/generations` con back-end in cloud e locale                                                                                                                         |
| 📐 **Embeddings**               | [/v1/embeddings` per ricerca e pipeline RAG                                                                                                                                            |
| 🎤 Trascrizione audioricorda**  | `/v1/audio/trascrizioni` — 7 fornitori (Deepgram Nova 3, AssemblyAI, Groq Whisper, HuggingFace, ElevenLabs, OpenAI, Azure), rilevamento di lingua automatico, supporto per MP4/MP3/WAV |
| 🔊 **Testo a voce**             | `/v1/audio/parola` — 10 fornitori (ElevenLabs, OpenAI, Deepgram, Cartesia, PlayHT, HuggingFace, Nvidia NIM, Inworld, Coqui, Tortoise) con messaggi di errore corretti                  |
| 🎬 **Generazione video**        | `/v1/videos/generazioni` (ComfyUI + SD WebUI flussi di lavoro)                                                                                                                         |
| 🎵 **Generazione musica**       | `/v1/music/generazioni` (ComfyUI flussi di lavoro)                                                                                                                                     |
| 🛡️ **Moderazioni**             | `/v1/moderazioni` controlli di sicurezza                                                                                                                                               |
| 🔀 **Riparazione scala**        | `/v1/rerank` per la valutazione della rilevanza                                                                                                                                        |
| 🔍 **Ricerche web** 🆕           | `/v1/cerca` — 5 fornitori (Serper, Brave, Perplexity, Exa, Tavily), 6.500+ gratuiti/otto, fall-back automatico, cache                                                                  |

### 🛡️ Resilienza, Sicurezza & Governance

| Funzione                                 | Cos'è fatto esattamente                                                                |
| ---------------------------------------- | -------------------------------------------------------------------------------------- |
| 🔌 **Circuit breaker**                    | Rilancio a modello/tolleranza con controlli delle soglie                               |
| 🎯 **Modelli-consapevoli endpoint**       | Custom models declare supported endpoints + API format                                 |
| 🛡️ **Anti-Thundering Herd**              | Mutex + semaphore protections on retry/rate events                                     |
| 🧠 **Semantic + Signature Cache**         | Cost/latency reduction with two cache layers                                           |
| ⚡ **Request Idempotency**                | Duplicate protection window                                                            |
| 🔒 **TLS Fingerprint Spoofing**           | Browser-like TLS fingerprint — **reduces bot detection and account flagging**          |
| 🔏 **Inquadramento dei CLI per il match** | Matches native CLI request signatures — **reduces ban risk while preserving proxy IP** |
| 🌐 **IP Filtering**                       | Allowlist/blocklist control for exposed deployments                                    |
| 📊 **Editable Rate Limits**               | Configurable global/provider-level limits with persistence                             |
| 🔑 **API Key Management + Scoping**       | Secure key issuance/rotation and model/provider controls                               |
| 🛡️ **Protected `/models`**               | Optional auth gating and provider hiding for model catalog                             |

### 📊 Observability & Analytics

| Funzione                             | Cos'è fatto esattamente                                               |
| ------------------------------------ | --------------------------------------------------------------------- |
| 📝 Richiesta ** + Logging Proxy**     | Registrazione richiesta/risposta e logging proxy completo             |
| 📋 **Dashboard di logging unificati** | Visualizzazione richiesta, proxy, audit e console in una pagina unica |
| 🔍 **Telerilevamento richiesta**      | Latenza p50/p95/p99 e seguitura richiesta                             |
| 🏥 **Dashboard di salute**            | Uptime, stato blocco, lockout, statistiche cache                      |
| 💰 **Tracking dei costi**             | Controllo del budget e visibilità di prezzo per modello               |
| 📈 **Visualizzazioni di analytics**   | Ispirazioni e tendenze del modello e fornitore                        |
| 🧪 **Frammento di valutazione**       | Test con insieme d'oro con strategie di abbinamento configurabili     |

### ☁️ Deploy e Piattaforma

| Funzione                                        | Cos'è fatto esattamente                                                                     |
| ----------------------------------------------- | ------------------------------------------------------------------------------------------- |
| 🌐 **Déploiement ovunque**                       | Locale locale, ambiente VPS, Docker, Cloud                                                  |
| 💾 **Cloud Sync**                                | Syncronizzazione configurazione tramite cloud worker                                        |
| 🔄 **Backup/Restore**                            | Flussi di export/import e di ripristino da emergenza                                        |
| 🧙 **Assistant all'avvio**                       | Setup guidato al primo avvio                                                                |
| 🔧 **Pannello di controllo degli strumenti CLI** | Impostazione rapida dei popolari strumenti di programmazione                                |
| 🎮 **Playground del modello**                    | Testare qualsiasi provider/modelo/endpoint dal pannello di controllo                        |
| 🔏 **Alta sicurezza dei dati CLI**               | Abilitazione di comparazione dei fingerprint per provider nel menu Impostazioni > Sicurezza |
| 🌐 **Internazionalizzazione (30 lingue)**        | Supporto totale della lingua per dashboard e documentazione, inclusa copertura di RTL       |
| 🧹 **Pulisci tutte le modellazioni**             | Pulizia rapida dell'elenco dei modelli con un clic in dettaglio del provider                |
| 📋 **Template per issue**                        | Modelli GitHub standardizzati per bug e feature                                             |
| 📂 **Squadra dati personalizzata**               | `CARTELLO_DIR` override per località di archiviazione                                       |

### Deep Dive sui Feature

#### Fallback intelligente con controllo dei costi pratici

```txt
Combo: "la mia stack di codifica"
  1. cc/claude-opus-4-6
  2. nvidia/llama-3.3-70b
  3. glm/glm-4.7
  4. if/kimi-k2-thinking
```

Quando quota, tariffa o salute falliscono, OmniRoute si muove automaticamente al
prossimo candidato senza l'intervento manuale.

#### La gestione dei protocolli è visibile e azionabile

- MCP + A2A sono discovering nella UI e nel doc (non nascosti)
- Le API del status dei protocolli espongono dati operativi in tempo reale
  (`/api/mcp/*`, `/api/a2a/*`)
- Le console includono azioni per day-2 ops (combusto, reset dei spezzoni,
  annullamento dei task)

#### Flusso di lavoro del traduttore + validazione

L'area del traduttore include:

- **Tessera di gioco**: controlli di trasformazione di richiesta
- **Tester di chat**: viaggio di richiesta/risposta completo
- **Banchetto di prova**: casi multiple in un run
- **Monitor in tempo reale**: visualizzazione della traffic in tempo reale

Insieme alla validazione dei protocolli con client reali tramite `npm run
test:protocolli:e2e`.

> 📖 **[README Server MCP](open-sse/mcp-server/README.md)** — Riferimento alla
> tool, configurazioni del IDE e esempi di clienti
> 
> 📖 **[README Server A2A](src/lib/a2a/README.md)** — Abilità, metodi JSON-RPC,
> trasmissione e ciclo di vita dei task

## 🧪 Valutazioni (Evals)

OmniRoute include un framework di valutazione integration per testare la qualità
delle risposte LLM a fronte di un insieme di riferimento d'oro. Accesso tramite
**Analytics → Evals** della dashboard.

### Set di test golden preloadato

Il precaricato "OmniRoute Set golden" contiene casi di test per:

- Ciao, matematica, geografia, generazione codice
- Compatibilità JSON, traduzione, generazione markdown
- Rifiuto della sicurezza (contenuti dannosi), conteggio, logica booleana

### Strategie di valutazione

| Strategia    | Description                                                | Esempio                                |
| ------------ | ---------------------------------------------------------- | -------------------------------------- |
| `esatto`     | Deve uscire identico                                       | ` " contiene"`                         |
| ` contiene ` | Deve contenere la sottostringa (senza distinzione di caso) | `"Parigi"`                             |
| `regex`      | Deve uscire in base a un modello di espressione regolare   | ` "1.* 2 .* 3"`                        |
| `custom`     | Funzione JS personalizzata restituisce true/false          | `(uscita) =&gt; uscita.length &gt; 10` |

---

## 📖 Guida alla configurazione

### Configurazione del protocollo (MCP + A2A)

<details>
<summary><b>🧩 MCP Setup (Model Context Protocol)</b></summary>

Avvia il trasporto MCP in modalità stdio:

```bash
omniroute --mcp
```

Flusso di validazione raccomandato:

1. Connetti il tuo client MCP su stdio.
2. Avvia `omniroute_get_ salute`.
3. Avvia `omniroute_elencare_ combinazioni`.
4. Apri `/dashboard/mcp` per confermare il battito d'anima, l'attività e
   l'audit.

API utili per l'automazione:

- `GET /api/mcp/status`
- `GET /api/mcp/i strumenti`
- `GET /api/mcp/audit`
- `GET /api/mcp/audit/stats`

</details>

<details>
<summary><b>🤝 A2A Setup (Agent2Agent)</b></summary>

Scopri l'agente:

```bash
curl http://localhost:20128/.well-known/agent.json
```

Invia una task:

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"setup-a2a","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"Riepilogo dello stato dei limiti di quota."}]}}'
```

Gestisci la vita ciclo:

- `GET /api/a2a/stato`
- `GET /api/a2a/taski`
- `GET /api/a2a/taski/:id`
- `POST /api/a2a/taski/:id/annulla`

Interfaccia di utilizzo operativa:

- `/piano di controllo/a2a` per l'osservabilità e le azioni di fumo per
  compiti/stato/flusso

</details>

<details>
<summary><b>🧪 End-to-end protocol validation</b></summary>

Verificare entrambi i protocolli con client reali:

```bash
npm run test:protocollo:e2e
```

Ciò verifica:

- MCP SDK client connect/list/call
- A2A discovery/send/stream/get/cancel
- Confrontare i dati nel MCP audit e negli atti di gestione delle attività A2A
  API

</details>

<details>
<summary><b>💳 Subscription Providers</b></summary>

### Claude Code (Pro/Max)

```bash
Pannello di controllo → Fornitori → Collega Claude Code
→ Accesso OAuth → Rinnovo token automatico
→ Tracciamento della quota a 5 ore + settimanale

Modelli:
  cc/claude-opus-4-6
  cc/claude-sonnet-4-5-20250929
  cc/claude-haiku-4-5-20251001
```

**Pro Tip:** Utilizza Opus per compiti complessi, Sonnet per prestazioni
elevate. OmniRoute segue la quota per modello!

### OpenAI Codex (Plus/Pro)

```bash
Pannello di controllo → Fornitori → Collega Codex
→ Accesso OAuth (porta 1455)
→ 5 ore + reset settimanale

Modelli:
  cx/gpt-5.2-codex
  cx/gpt-5.1-codex-max
```

#### Gestione delle limitazioni dell'account Codex (5h + Reset)

Ora ogni account Codex dispone di toggle di politica nella sezione `Pannello di
controllo -&gt; Fornitori`:

- `5h` (ATTIVA/DISATTIVA): applicare la politica del trascorso della finestra di
  5 ore con un limite.
- `Settimanale` (ACCESSIONE/SPENSIIONE): attiva la politica di soglia di
  finestra settimanale.
- Comportarsi la soglia: quando una finestra abilitata raggiunge >=90% di uso,
  il relativo account viene ignorato.
- Comportamento di rotazione: OmniRoute invia automaticamente il traffico al
  prossimo account Codex ammissibile.
- Comportamento di resettamento: quando la data e ora nella quale il provider è
  resettato trascorre, l'account diventa nuovamente ammissibile automaticamente.

Casi di uso:

- `5 ore ON` + [X9X]Settimanale ON[X19X]: l'account viene ignorato quando
  raggiunge la soglia con o con la finestra.
- `5 ore OFF` + [X10X]Settimanale ON[X20X]: solo l'utilizzo settimanale può
  bloccare l'account.
- `5 ore ON` + [X9X]Settimanale OFF[X20X]: solo l'utilizzo delle 5 ore può
  bloccare l'account.
- `resettato[X9X] prima della data: l'account è nuovamente disponibile per la
  rotazione automaticamente (nessuna riabilitazione manuale).

### Gemini CLI (GRAZIA 180.000/180.000/mese!)

```bash
Dashboard → Provider → Collega Gemini CLI
→ Google OAuth
→ 180.000 completamenti al mese + 1.000 al giorno

Modelli:
  gc/gemini-3-rilievo-del-prodotto-di-previsione
  gc/gemini-2.5-pro
```

**Meglio:** Ottima libera fascia oraria! Usa questo prima delle fasce paganti.

### Copilota GitHub

```bash
Dashboard → Provider → Collega GitHub
→ OAuth via GitHub
→ Reset mensile (primo di ogni mese)

Modelli:
  gh/gpt-5
  gh/claude-4.5-sonnet
  gh/gemini-3-pro
```

</details>

<details>
<summary><b>🔑 API Key Providers</b></summary>

### NVIDIA NIM (ACCESSO GRATUITO per sviluppatori — 70+ modelli)

1. Iscriviti: [build.nvidia.com](https://build.nvidia.com)
2. Ottera chiave API (1.000 crediti di inferenza inclusi)
3. Dashboard → Aggiungi fornitore → NVIDIA NIM:
   - Chiave API: [X0X]nvapi-vai-chiave-tuo[X25X]

**Modelli:[X8X] `nvidia/llama-3.3-70b-istruzioni[X44X] ,
[X46X]nvidia/mistral-7b-istruzioni[X73X] e 50+ altri

Pro Tip: ** Raccomandazione esperta: ** ApriAI-API compatibile — funziona in
modo senza problemi con la traduzione del formato di OmniRoute!

### DeepSeek

1. Iscriviti: [platform.deepseek.com](https://platform.deepseek.com)
2. Ottenere scheda API
3. Pannello di controllo → Aggiungi fornitore → DeepSeek

**Modelli:** `deepseek/deepseek-chat`, `deepseek/deepseek-coder`

### Groq (Disponibile a livello gratuito!)

1. Iscriviti: [console.groq.com](https://console.groq.com)
2. Ottenere scheda API (livello gratuito incluso)
3. Pannello di controllo → Aggiungi fornitore → Groq

**Modelli:** `groq/llama-3.3-70b`, `groq/mixtral-8x7b`

**Raccomandazione esperta:** Inferenza estremamente veloce — best per le
esigenze di tempo reale!

### OpenRouter (100+ Modelli)

1. Iscriviti: [openrouter.ai](https://openrouter.ai)
2. Ottenere scheda API
3. Pannello di controllo → Aggiungi fornitore → OpenRouter

**Modelli:** Accesso a 100+ modelli da tutti i principali fornitori attraverso
una sola chiave API.

</details>

<details>
<summary><b>💰 Cheap Providers (Backup)</b></summary>

### GLM-4.7 (Reset giornaliero, $0,6/1M)

1. Iscriviti: [Zhipu AI](https://open.bigmodel.cn/)
2. Ottenere scheda API dal Pianificazione Coding
3. Pannello di controllo → Aggiungi chiave API:
   - Fornitore: `glm`
   - Chiave API: `your-key`

**Usa:** `glm/glm-4.7`

**Pro consiglio:** Il piano di codifica offre 3 volte la quota a un costo di
1/7!

### Risorsa mancia M2.1 (5 ore, $0,20/1 milione)

1. Iscriversi: [MiniMax](https://www.minimax.io/)
2. Ottenere scheda API
3. Pannello di controllo → Aggiungi chiave API

**Usa:** `minimax/MiniMax-M2.1`

**Pro consiglio:** Opzione più economica per contesti lunghi (1 milione di
token)!

### Kimi K2 ($9/mese fissa)

1. Iscrevisi: [Moonshot AI](https://platform.moonshot.ai/)
2. Ottenere scheda API
3. Pannello di controllo → Aggiungi chiave API

**Usa:** `kimi/kimi-latest`

**Pro consiglio:** $9/mese fissa per 10 milioni di token = $0,90/1 milione di
costo effettivo!

</details>

<details>
<summary><b>🆓 FREE Providers (Emergency Backup)</b></summary>

### iFlow (5 modelli gratuiti via OAuth)

```bash
Pannello di controllo → Collega iFlow
→ accesso OAuth a iFlow
→ Utilizzo illimitato

Modelli:
  if/kimi-k2-thinking
  if/qwen3-coder-plus
  if/glm-4.7
  if/minimax-m2
  if/deepseek-r1
```

### Qwen (4 modelli gratuiti via Codice dispositivo)

```bash
Dashboard → Connetti Qwen
→ Autenticazione del codice di dispositivo
→ Utilizzo illimitato

Modello:
  qw/qwen3-coder-plus
  qw/qwen3-coder-flash
```

### Kiro (Claude GRATIS)

```bash
Dashboard → Connetti Kiro
→ ID del costruttore di AWS o Google/GitHub
→ Utilizzo illimitato

Modello:
  kr/claude-sonnet-4.5
  kr/claude-haiku-4.5
```

</details>

<details>
<summary><b>🎨 Create Combos</b></summary>

### Esempio 1: Maximize Subscription → Backup a basso costo

```
Dashboard → Combos → Crea un Nuovo

Nome: code-premium
Modello:
  1. cc/claude-opus-4-6 (Abbonamento principale)
  2. glm/glm-4.7 (Backup a basso costo, $0.6/1M)
  3. minimax/MiniMax-M2.1 (Fallback più economico, $0.20/1M)

Utilizza in CLI: code-premium
```

### Esempio 2: Solo Gratis (Costo 0)

```
Nome: combo-gratis
Modello:
  1. gc/gemini-3-flash-preview (180K gratuiti al mese)
  2. if/kimi-k2-thinking (illimitato)
  3. qw/qwen3-coder-plus (illimitato)

Costo: $0 per sempre!
```

</details>

<details>
<summary><b>🔧 CLI Integration</b></summary>

### Cursore IDE

```
Impostazioni → Modelli → Avanzate:
  URL di base dell'API OpenAI: http://localhost:20128/v1
  Chiave dell'API OpenAI: [imposta dalla dashboard OmniRoute]
  Modello: cc/claude-opus-4-6
```

### Codice Claudio

Utilizza la pagina **CLI Tools** del dashboard per una configurazione a un clic,
o modifica `~/.claude/settings.json` manualmente.

### CLI Codex

```bash
esporta OPENAI_BASE_URL="http://localhost:20128"
esporta OPENAI_API_KEY="tua-chiave-omniroute-api"

codex "tua richiesta"
```

### OpenClaw

**Opzione 1 – Dashboard (consigliata):**

```
Dashboard → CLI Tools → OpenClaw → Seleziona Modello → Applica
```

**Opzione 2 – Manuale:** Modifica `~/.openclaw/openclaw.json`:

```json
{
  "modelli": {
    "provider": {
      "omniroute": {
        "baseUrl": "http://127.0.0.1:20128/v1",
        "apiKey": "sk_omniroute",
        "api": "openai-completions"
      }
    }
  }
}
```

> **Nota:** OpenClaw funziona solo con OmniRoute locale. Utilizza `127.0.0.1` al
> posto di `localhost` per evitare problemi di risoluzione IPv6.

### Cline / Continua / RooCode

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

## Risoluzione dei problemi

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

- Controlla le statistiche d'uso nella Dashboard → Costi
- Imposta il modello primario su GLM/MiniMax
- Utilizza il livello free (Gemini CLI, iFlow) per le funzioni non critiche

[Dashboard/API ports are wrong]

- [X]PORT[X] è la porta di base canonica (e la porta API predefinita)
- [X]API_PORT[X] sovrascrive solo l'ascoltatore di API compatibile con OpenAI
- [X]DASHBOARD_PORT[X] sovrascrive solo l'ascoltatore di dashboard/Next.js
- Imposta [NEXT_PUBLIC_BASE_URL] sulla tua URL pubblica di dashboard/pubblica
  (per gli callback di OAuth)

[X]Cloud sync errors[X]

- Verifica che [BASE_URL] si rechi al tuo istanza in esecuzione
- Verifica che [CLOUD_URL] si rechi al tuo punto di fineCloud atteso
- Mantieni [NEXT_PUBLIC_*] synchroni con i valori associate al lato server

[X]Il primo accesso non funziona[X]

- Controlla [INITIAL_PASSWORD] in [.env]
- Se non è impostata, il password predefinito è [123456]

[X]Non sono presenti i registri richiesta[X]

- Imposta [ENABLE_REQUEST_LOGS=true] in [.env]

[X]Il test di connessione mostra "Invalid" per i providers compatibili con
OpenAI[X]

- Molti provider non espongono un endpoint [/models]
- OmniRoute v1.0.6+ include la validation di fallback mediante completamenti di
  chat
- Assicurarsi che l'URL di base includa la suffisso `/v1`

### 🔒 OAuth in un Server Remoto

<a name="oauth-on-a-remote-server"></a> <a name="oauth-em-servidor-remoto"></a>

> **⚠️ Importante per gli utenti che eseguono OmniRoute su un VPS, Docker o
> qualsiasi server remoto**

#### Perché il processo di OAuth Antigravity / Gemini CLI fallisce sui server remoti?

I **provveditori Antigravity** e **Gemini CLI** utilizzano **Google OAuth 2.0**.
Google richiede il `redirect_uri` nel flusso OAuth per corrispondere esattamente
a uno dei URI registrati nella console di Google Cloud.

Le credenziali di autenticazione OAuth inclusi in OmniRoute sono registrate
**solo per `localhost`**. Quando accedi a OmniRoute su un server remoto (ad
esempio `https://omniroute.myserver.com`), Google respinge l'autenticazione con:

```
Errore 400: redirect_uri_mismatch
```

#### Soluzione: Configura le proprie credenziali di autenticazione con OAuth

Hai bisogno di creare un **ID Client OAuth 2.0** nella console di Google Cloud
con l'URI del tuo server.

#### Seguo i passaggi

**1. Apri la console di Google Cloud**

Vai a:
[https://console.cloud.google.com/apis/credentials](https://console.cloud.google.com/apis/credentials)

**2. Crea un nuovo ID Client OAuth 2.0**

- Clicca **"+ Crea credenziali"** → **"ID Client OAuth"**
- Tipo di applicazione: **"Applicazione web"**
- Nome: qualsiasi cosa che desideri (ad es. `OmniRoute Remoto`)

**3. Aggiungi indirizzi di reindirizzamento autorizzati**

Nel campo **"Indirizzi di reindirizzamento autorizzati"**, aggiungi:

```
https://your-server.com/callback
```

> Sostituisci `your-server.com` con il dominio o l'indirizzo IP del tuo server
> (compreso il porta se necessario, ad es.
> `http://45.33.32.156:20128/callback`).

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

As credenciais OAuth integrate no OmniRoute sono registrate solo in
**localhost**. Quando accedi al OmniRoute su un server remoto (ad esempio
`https://omniroute.meuservidor.com`), Google rifiuta l'autenticazione con:

```
Errore 400: redirect_uri_mismatch
```

#### Soluzione: Configura le tue credenziali OAuth di tuo pugno

Hai bisogno di creare uno **ID di client OAuth 2.0** nel Console di Google Cloud
con l'URI del tuo server.

#### Passo a passo

**1. Accedi al Console di Google Cloud**

Apri:
[https://console.cloud.google.com/apis/credentials](https://console.cloud.google.com/apis/credentials)

**2. Crea un nuovo ID di client OAuth 2.0**

- Clicca su **"+" Nuova credenziale"** → **"ID di client OAuth"**
- Tipo di applicazione: **"App web"**
- Nome: scegli un nome qualsiasi (ad esempio `OmniRoute Remote`)

**3. Aggiungi le Uniformi di ritorno autorizzate**

Nel campo **"Uniformi di ritorno autorizzate"**, aggiungi:

```
https://seu-servidor.com/callback
```

> Sostituisci `seu-servidor.com` con il dominio o l'indirizzo IP del tuo server
> (incluso la porta se necessario, ad esempio
> `http://45.33.32.156:20128/callback`).

**4. Salva e copia le credenziali**

Appena creato, Google mostrerà l' **ID di client** e il **Segreto di client**.

**5. Configura le variabili di ambiente**

Nel tuo `.env` (o nelle variabili di ambiente del Docker):

```bash
# Per Antigravity:
ANTIGRAVITY_OAUTH_CLIENT_ID=seu-client-id.apps.googleusercontent.com
ANTIGRAVITY_OAUTH_CLIENT_SECRET=GOCSPX-seu-secret

# Per Gemini CLI:
GEMINI_OAUTH_CLIENT_ID=seu-client-id.apps.googleusercontent.com
GEMINI_OAUTH_CLIENT_SECRET=GOCSPX-seu-secret
GEMINI_CLI_OAUTH_CLIENT_SECRET=GOCSPX-seu-secret
```

**6. Riavvia l'OmniRoute**

```bash
# Se utilizzando npm:
npm run dev

# Se utilizzando Docker:
docker restart omniroute
```

**7. Tenta collegarti nuovamente**

Dashboard → Fornitori → Antigravity (o Gemini CLI) → OAuth

Adesso Google invierà correttamente a `https://il-tuo-servidor.com/callback` e
l'autenticazione funzionerà.

---

#### Workaround temporaneo (senza configurare le credenziali proprietarie)

Se non vuoi creare le credenziali proprietarie ora, puoi ancora usare il flusso
**manuale delle URL**:

1. L'OmniRoute aprirà l'URL di autorizzazione di Google
2. Dopo aver autorizzato, Google cercherà di inviare a `localhost` (che fallisce
   sul server remoto)
3. **Copia l'URL completa** dalla barra degli indirizzi del tuo browser (anche
   se la pagina non si carica)
4. Incolla quell'URL nel campo che compare nel modal di connessione
   dell'OmniRoute
5. Clicca su **"Connettiti"**

> Questo workaround funziona perché il codice di autorizzazione nell'URL è
> valido indipendentemente dal redirect sia stato caricato o meno.

</details>

---

</details>

## 🛠️ Tech Stack

<details>
<summary><b>Click to expand tech stack details</b></summary>

- **Runtime**: Node.js 18–22 LTS (⚠️ Node.js 24+ non è **supportato** —
  `better-sqlite3` binari nativi non sono compatibili)
- **Lingua**: TypeScript 5.9 — **100% TypeScript** all'interno di `src/` e
  `open-sse/` (zero `qualsiasi` module di base dal v2.0)
- **Framework**: Next.js 16 + React 19 + Tailwind CSS 4
- **Database**: LowDB (JSON) + SQLite (stato del dominio + registri di proxy +
  audit di MCP + scelte di routing)
- **Schemi**: Zod (strumento di validazione I/O MCP, contratti API)
- **Protocolli**: MCP (stdio / HTTP) + A2A v0.3 (JSON-RPC 2.0 + SSE)
- Streaming**: Streaming**: Eventi del server (SSE)
- Auth**: OAuth 2.0 (PKCE) + JWT + API Keys + Autorizzazione del dominio MCP
- Testing**: Esecuzione dei test Node.js + Vitest (900+ test compresi unit,
  integrazione, E2E)
- CI/CD**: GitHub Actions (pubblicazione automatica di npm + Docker Hub alla
  rilascio)
- **Website**: [omniroute.online](https://omniroute.online)
- Package**:
  [npmjs.com/package/omniroute](https://www.npmjs.com/package/omniroute)
- Docker**:
  [hub.docker.com/r/diegosouzapw/omniroute](https://hub.docker.com/r/diegosouzapw/omniroute)
- Resilience**: Circuit breakers, backoff esponenziale, anti-turbamento del
  gregge, spoofing TLS, self-healing automatico combinato

</details>

---

## Documentazione

| Documenta                                      | Description                                                          |
| ---------------------------------------------- | -------------------------------------------------------------------- |
| Guida utente (docs/USER_GUIDE.md)              | Combinate, interfacce CLI, deployment                                |
| [API Reference](docs/API_REFERENCE.md)         | Tutti gli endpoint con esempi                                        |
| [MCP Server](open-sse/mcp-server/README.md)    | 16 strumenti MCP, configs IDE, client Python/TS/Go                   |
| [A2A Server](src/lib/a2a/README.md)            | Protocollo JSON-RPC 2.0, abilità, streaming, gestione delle attività |
| [Auto-Combo Engine](docs/auto-combo.md)        | Punteggio di 6 fattori, pack di modalità, autosanamento              |
| [Troubleshooting](docs/TROUBLESHOOTING.md)     | Problemi comuni e soluzioni                                          |
| [Architecture](docs/ARCHITECTURE.md)           | Architettura e interni del sistema                                   |
| [Contributing](CONTRIBUTING.md)                | Impostazioni e linee guida di sviluppo                               |
| [OpenAPI Spec](docs/openapi.yaml)              | Specificazione OpenAPI 3.0                                           |
| [Security Policy](SECURITY.md)                 | Denuncia di vulnerabilità e pratiche di sicurezza                    |
| [VM Deployment](docs/VM_DEPLOYMENT_GUIDE.md)   | Guida completa: VM + nginx + Cloudflare                              |
| [Features Gallery](docs/FEATURES.md)           | Tour guidato con screenshot della dashboard visiva                   |
| [Release Checklist](docs/RELEASE_CHECKLIST.md) | Passaggi di validazione pre-rilascio                                 |

---

## 🗺️ Plancia di comando

OmniRoute ha **210+ caratteristiche previste** in diverse fasi di sviluppo. Ecco
le principali aree:

| Categoria                    | Funzionalità previste | Highlights                                                                             |
| ---------------------------- | --------------------- | -------------------------------------------------------------------------------------- |
| 🧠 **Routing & Intelligence** | 25+                   | Lowest-latency routing, tag-based routing, quota preflight, P2C account selection      |
| 🔒 **Security & Compliance**  | 20+                   | SSRF hardening, credential cloaking, rate-limit per endpoint, management key scoping   |
| 📊 **Observability**          | 15+                   | OpenTelemetry integration, real-time quota monitoring, cost tracking per model         |
| 🔄 **Provider Integrations**  | 20+                   | Dynamic model registry, provider cooldowns, multi-account Codex, Copilot quota parsing |
| ⚡ **Performance**            | 15+                   | Dual cache layer, prompt cache, response cache, streaming keepalive, batch API         |
| 🌐 **Ecosystem**              | 10+                   | WebSocket API, config hot-reload, distributed config store, commercial mode            |

### In arrivo

- 🔗 **OpenCode Integration** — Native provider support for the OpenCode AI
  coding IDE
- 🔗 **INTEGRAZIONE TRAE** — Supporto full per il framework di sviluppo AI TRAE
- 📦 **API in Batch** — Elaborazione batch asincrona per richieste di bulk
- 🎯 **Routedistintivo per tag** — Routedi richieste in base a tag e metadata
  personalizzati
- 💰 **Strategy di costo minimo** — Selezione automatica del provider più
  economico disponibile

> 📝 Specifiche complete delle funzionalità disponibili in
> [`docs/new-features/`](docs/new-features/) (217 specifiche dettagliate)

---

## 👥 Contribuenti

[![Contribuenti](https://contrib.rocks/image?repo=diegosouzapw/OmniRoute&max=100&columns=20&anon=1)](https://github.com/diegosouzapw/OmniRoute/graphs/contributors)

### Come Contribuire

1. Fork il repository
2. Crea una nuova branca (`git checkout -b feature/amazing-feature`)
3. Aggiorna il commit (`git commit -m 'Aggiungi feature straordinaria'`)
4. Spedisce la modifica (`git push origin feature/amazing-feature`)
5. Avvia una Richiesta di modifica

Consulta [[CONTRIBUTING.md](CONTRIBUTING.md)] per linee guida dettagliate.

### Rilascio di una Nuova Versione

```bash
# Crea un nuovo rilascio — il rilascio avviene automaticamente con `npm publish`
gh release create v2.0.0 --title "v2.0.0" --generate-notes
```

---

## 📊 Cronologia delle Stelle

## Stelle ricevute nel tempo

## [![Stelle ricevute nel tempo](https://starchart.cc/diegosouzapw/OmniRoute.svg?variant=adaptive)](https://starchart.cc/diegosouzapw/OmniRoute)

## 🙏 Ringrazioni

Grazie infinite a ** [X36X] (https://github.com/decolua/9router) da **
[decolua](https://github.com/decolua) ** — il progetto originale che ha ispirato
questa fork. OmniRoute costruisce inoltre sulla fondazione incredibile con
funzionalità aggiuntive, interfacce API multimediali e una complete
riimplementazione con TypeScript.

Grazie infinite a ** [CLIProxyAPI](https://github.com/router-for-me/CLIProxyAPI)
** — l'implementazione Go originale che ha ispirato questa versione JavaScript.

---

## 📄 Licenza

Licenza MIT - consulta [LICENSE](LICENSE) per maggiori dettagli.

---

<div align="center">
  <sub>Built with ❤️ for developers who code 24/7</sub>
  <br/>
  <sub><a href="https://omniroute.online">omniroute.online</a></sub>
</div>
<!-- GitHub Discussions enabled for community Q&A -->
