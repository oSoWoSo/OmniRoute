# 🚀 OmniRoute — היציאה החינם של AI

### ערבי אינטרנט - נאקל - "Never stop coding."  Smart routing to **חינם & low-cost AI models** with automatic fallback.

_ה-API שלך האוניברסלי — אחד endpoint, 67+ providers, זמן עבודה של 0. עכשיו עם
MCP & A2A agent orchestration._

**סיומת חברת Chat • Embeddings • Image Generation • Video • Music • Audio •
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

🌐 **נמצא ב:** 🇺🇸 [English](README.md) | 🇧🇷 [Português
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

> **Updating from v2.9.5?** — See the [full
> CHANGELOG](CHANGELOG.md#300--2026-03-22-release-candidate--not-yet-merged-to-main)
> for all changes.

| Area                        | Change                                                                                                                                                                    |
| --------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🔒 **CodeQL Security**       | Fixed 10+ CodeQL alerts: polynomial-redos, insecure-randomness, shell-injection remediation                                                                               |
| ✅ **Route Validation**      | All 176 API routes now validated with Zod schemas + `validateBody()` — CI `check:route-validation:t06` passes                                                             |
| 🐛 **omniModel Tag Leak**    | Internal `<omnimodel>` tags no longer leak to clients in SSE streaming responses (#585)</omnimodel>                                                                       |
| 🔑 **Registered Keys API**   | Auto-provision API keys via `POST /api/v1/registered-keys` with per-provider/account quota enforcement, idempotency, SHA-256 storage, and optional GitHub issue reporting |
| 🎨 **Provider Icons**        | 130+ סמלי ספקים via `@lobehub/icons` (SVG) עם זרימה מסובבת של PNG                                                                                                         |
| 🔄 תיאום אוטומטי של **מודל** | 29 שעות ופעמון + לחץ ידני על UI כדי לשגר רשימות מודלים לספקי built-in ונקיים פתוח-לא-אי (OpenAI-compatible providers)                                                     |
| 🌐 **OpenCode Zen/Go**       | שני ספקים חדשים מ @kang-heewon מגישים PR #530: תכונת השירות ב-1000 X‏ OpencodeExecutor`                                                                                   |
| 🐛 **Gemini CLI OAuth**      | הוצעה נעשתה כשהייתה `GEMINI_OAUTH_CLIENT_SECRET` חסורה ב- Docker (הייתה הצהרה מסתורית של Google)                                                                          |
| 🐛 **OpenCode config**       | `saveOpenCodeConfig()` כתב תווי- TOML נכון ל-`XDG_CONFIG_HOME`                                                                                                            |
| 🐛 **Pinned model override** | `body.model` נקבע `pinnedModel` בעקבות- context-cache הגנה                                                                                                                |
| 🐛 **Codex/Claude loop**     | `tool_result` מצומדות סרזה כעת ל- - כדי לעצור כיפוף- של-                                                                                                                  |
| 🐛 **Login redirect**        | [X0X]Login[] לא תדוע- כעת בעת-ברחב- עם- סקיפ- - יוצא                                                                                                                      |
| 🐛 **Windows paths**         | MSYS2 / Git - Bash pathways   (`/c/...`) נגמר - -                                                                                                                         |

---

## 🖼️ Dashboard ה-ראש

<div align="center">
  <img src="./docs/screenshots/MainOmniRoute.png" alt="OmniRoute Dashboard" width="800"/>
</div>

---

## 📸  תצוגה-

<details>
<summary><b>Click to see dashboard screenshots</b></summary>

| עמוד              | קופסת תמונה                                       |
| ----------------- | ------------------------------------------------- |
| **Providerim**    | ![Providerim](docs/screenshots/01-providers.png)  |
| **Combos**        | ![Combos](docs/screenshots/02-combos.png)         |
| **Analytics**     | ![Analytics](docs/screenshots/03-analytics.png)   |
| **Health**        | ![Health](docs/screenshots/04-health.png)         |
| **Translator**    | ![Translator](docs/screenshots/05-translator.png) |
| **Settings**      | ![Settings](docs/screenshots/06-settings.png)     |
| **CLI Tools**     | ![CLI Tools](docs/screenshots/07-cli-tools.png)   |
| **היעטות השימוש** | ![השימוש](docs/screenshots/08-usage.png)          |
| **Endpoints**     | ![Endpoints](docs/screenshots/09-endpoint.png)    |

</details>

---

### 🤖 מותג-מדרכי AI עבור העגון-ובהבעלים

_לחבר כל IDE שכלול IDE כלול API או CLI מערב איידי Omniroute — API ארע ״יאח — API
Gateway בחינם ובחינם לאלףוני ק

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

<sub>📡 הרמות כל האגנט דרך<code>http://localhost:20128/v1</code>
או<code>http://cloud.omniroute.online/v1</code> — אחד פמס (configuration) , אשר
שלולון models -</sub>

---

## 🤔  מדוע Omniroute?

**אספר- כפום **

- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  אשר (subscription quota) ננף (expired) (unused) זש (every) (month) –
  (unlimited)
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  אשר (rate limits) - (stopping) (you) mid-coding
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  API (expensive) ($20-50/month (per provider)
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  (מהלך switch) (manual) - (between) (providers)

**Omnimoute (fix) (solution) **

- ✅ **Maximize subscriptions** - (track) , (use) every (bit) (before) (reset) ,
  (unlimited)
- ✅ **Auto fallback** - (subscription) → (API Key) → (cheap) → (free) , (zero)
  (downtime)
- ✅ **Mulit-account** - (round-robin) ב- (between) (accounts) (per) (provider)
- ✅ **Universal** - (works) ע- (with) cluade code , (codex) , (gemini CLI) ,
  (curson) , (cline) , (openclaw) , (any) (CLI tool)

---

## 📧  (support)

> 💬 **Join (community! )**
> [(https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t) — ז] (help) ,
> share (tip) , (stay) updated.

- **Website : [OmniRoute. net](https://omniroute.online)
- **GitHub : [github.
  com/diegosouzapw/Omniroute](https://github.com/diegosouzapw/OmniRoute)
- **Ihues : [github.
  com/diegosouzapw/Omniroute/issues](https://github.com/diegosouzapw/OmniRoute/issues)
- **WhatsApp : [Community
  Group](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)
- **Contributing : (see) [CONTRIBUTING. mdc](CONTRIBUTING.md) , (open) (a pr) ,
  (or) (pick) a[65X]good first issue`
- **Original Project**: [9router by decolua](https://github.com/decolua/9router)

### Should We Report a BUG?

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

## איך זה עובד

```
┌─────────────┐
│  Your CLI   │  (Claude Code, Codex, Gemini CLI, OpenClaw, Cursor, Cline...)
│   Tool      │
└──────┬──────┘
       │ http://localhost:20128/v1
       ↓
┌─────────────────────────────────────────┐
│           OmniRoute (Smart Router)        │
│  • Annotate conversion (OpenAI ↔ Claude) │
│  • Account management + Embeddings + Images │
│  • Auto token refresh                   │
└──────┬──────────────────────────────────┐
       │
       ├─→ [Tier 1: SUBSCRIPTION] Claude Code, Codex, Gemini CLI
       │   ↓ quota exhausted
       ├─→ [Tier 2: KEY API] DeepSeek, Groq, xAI, Mistral, NVIDIA NIM, etc.
       │   ↓ budget limit
       ├─→ [Tier 3: CHEAP] GLM ($0.6/1M), MiniMax ($0.2/1M)
       │   ↓ budget limit
       └─→ [Tier 4: FREE] iFlow, Qwen, Kiro (limitless)

Result: Never stop programming, minimal cost
```

---

## What problem does OmniRoute solve — 30 real problems daily

> **Every programmer using AI tools faces these problems daily.** OmniRoute was
> built to solve them all — from cost overruns to regional blocks, from broken
> OAuth flows to protocol operations and enterprise observability.

<details>
<summary><b>💸 1. "I pay for an expensive subscription but still get interrupted by limits"</b></summary>

Developers pay $20–200/month for Claude Pro, Codex Pro, or GitHub Copilot. Even
paying, quota has a ceiling — 5h of usage, weekly limits, or per-minute rate
limits. Mid-coding session, the provider stops responding and the developer
loses flow and productivity.

**איך OmniRoute פותר אותו:**

- ** 4-Tier Smart fallback** - If subscription quota has expired, redirects
  automatically to API Key → Cheap → Free with zero user intervention
- **Real-Time Tracking** — Token consumption in real-time with 5 hour, weekly,
  daily countdown to reset
- **Multi-Account Support** — Multiple accounts per provider with automatic
  round-robin — when one is used up, switches to the next
- **Custom Combos** — Customizable fallback chains with 6 balancing strategies
  (fill-first, round-robin, P2C, random, least-used, cost-optimized)
- **Monitoring Business Quotas** — Business/Team workspace quota monitoring
  directly in the dashboard

</details>

<details>
<summary><b>🔌 2. "I need to use multiple providers but each has a different API"</b></summary>

OpenAI uses one format, Claude (Anthropic) uses another, Gemini yet another. If
a dev wants to test models from different providers or fallback between them,
they need to reconfigure SDKs, change endpoints, deal with incompatible formats.
Custom providers (FriendLI, NIM) have non-standard model endpoints.

**איך OmniRoute פותר אותו:**

- **Unified Endpoint** — A single `http://localhost:20128/v1` server serves as a
  proxy for all 67+ providers
- **Automatic Format Translation** — OpenAI ↔ Claude ↔ Gemini ↔ Responses API
- **Response Sanitization** — Strips non-standard fields (`x_groq`,
  `usage_breakdown`, `service_tier`) that break OpenAI SDK v1.83+
- **Role Normalization** — Converts `developer` → `system` for non-OpenAI
  providers; `system` → `user` for GLM/ERNIE
- **Think Tag Extraction** — Extracts `<think>` blocks from models like DeepSeek
  R1 into standardized `reasoning_content`
- **Structured Output for Gemini** — `json_schema` →
  `responseMimeType`/`responseSchema` automatic conversion
- **`stream` defaults to `false`** — Aligns with OpenAI spec, avoiding
  unexpected SSE in Python/Rust/Go SDKs

</details>

<details>
<summary><b>🌐 3. "My AI provider blocks my region/country"</b></summary>

Providers like OpenAI/Codex block access from certain geographic regions. Users
get errors like `unsupported_country_region_territory` during OAuth and API
connections. This is especially frustrating for developers from developing
countries.

**איך OmniRoute פותר אותו:**

- **3-Level Proxy Config** — Configurable proxy at 3 levels: global (all
  traffic), per-provider (one provider only), and per-connection/key
- **Color-Coded Proxy Badges** — Visual indicators: 🟢 global proxy, 🟡 provider
  proxy, 🔵 connection proxy, always showing the IP
- **OAuth Token Exchange Through Proxy** — OAuth flow also goes through the
  proxy, solving `unsupported_country_region_territory`
- **Connection Tests via Proxy** — Connection tests use the configured proxy (no
  more direct bypass)
- **SOCKS5 Support** — Full SOCKS5 proxy support for outbound routing
- **TLS Fingerprint Spoofing** — Browser-like TLS fingerprint via `wreq-js` to
  bypass bot detection
- **🔏 CLI Fingerprint Matching** — Reorders headers and body fields to match
  native CLI binary signatures, drastically reducing account flagging risk. The
  proxy IP is preserved — you get both stealth **and** IP masking simultaneously

</details>

<details>
<summary><b>🆓 4. "I want to use AI for coding but I have no money"</b></summary>

Not everyone can pay $20–200/month for AI subscriptions. Students, devs from
emerging countries, hobbyists, and freelancers need access to quality models at
zero cost.

**איך OmniRoute פותר אותו:**

- **Free Tier Providers Built-in** — Native support for 100% free providers:
  iFlow (5 unlimited models via OAuth: kimi-k2-thinking, qwen3-coder-plus,
  deepseek-r1, minimax-m2, kimi-k2), Qwen (4 unlimited models: qwen3-coder-plus,
  qwen3-coder-flash, qwen3-coder-next, vision-model), Kiro (Claude + AWS Builder
  ID for free), Gemini CLI (180K tokens/month free)
- **Ollama Cloud** — Cloud-hosted Ollama models at `api.ollama.com` with free
  "Light usage" tier; use `ollamacloud/<model>` prefix
- **Free-Only Combos** — Chain `gc/gemini-3-flash → if/kimi-k2-thinking →
  qw/qwen3-coder-plus` = $0/month with zero downtime
- **NVIDIA NIM Free Access** — ~40 RPM dev-forever free access to 70+ models at
  build.nvidia.com (transitioning from credits to pure rate limits)
- **Cost Optimized Strategy** — Routing strategy that automatically chooses the
  cheapest available provider

</details>

<details>
<summary><b>🔒 5. "I need to protect my AI gateway from unauthorized access"</b></summary>

When exposing an AI gateway to the network (LAN, VPS, Docker), anyone with the
address can consume the developer's tokens/quota. Without protection, APIs are
vulnerable to misuse, prompt injection, and abuse.

**איך OmniRoute פותר אותו:**

- **API Key Management** — Generation, rotation, and scoping per provider with a
  dedicated `/dashboard/api-manager` page
- **Model-Level Permissions** — Restrict API keys to specific models
  (`openai/*`, wildcard patterns), with Allow All/Restrict toggle
- **API Endpoint Protection** — Require a key for `/v1/models` and block
  specific providers from the listing
- **Auth Guard + CSRF Protection** — All dashboard routes protected with
  `withAuth` middleware + CSRF tokens
- **Rate Limiter** — Per-IP rate limiting with configurable windows
- **IP Filtering** — Allowlist/blocklist for access control
- **Prompt Injection Guard** — Sanitization against malicious prompt patterns
- **AES-256-GCM Encryption** — Credentials encrypted at rest

</details>

<details>
<summary><b>🛑 6. "My provider went down and I lost my coding flow"</b></summary>

AI providers can become unstable, return 5xx errors, or hit temporary rate
limits. If a dev depends on a single provider, they're interrupted. Without
circuit breakers, repeated retries can crash the application.

**איך OmniRoute פותר אותו:**

- **Circuit Breaker per-model** — Auto-open/close with configurable thresholds
  and cooldown (Closed/Open/Half-Open), scoped per-model to avoid cascading
  blocks
- **Exponential Backoff** — Progressive retry delays
- **Anti-Thundering Herd** — Mutex + semaphore protection against concurrent
  retry storms
- **Combo Fallback Chains** — If the primary provider fails, automatically falls
  through the chain with no intervention
- **Combo Circuit Breaker** — Auto-disables failing providers within a combo
  chain
- **Health Dashboard** — Uptime monitoring, circuit breaker states, lockouts,
  cache stats, p50/p95/p99 latency

</details>

<details>
<summary><b>🔧 7. "Configuring each AI tool is tedious and repetitive"</b></summary>

Developers use Cursor, Claude Code, Codex CLI, OpenClaw, Gemini CLI, Kilo
Code... Each tool needs a different config (API endpoint, key, model).
Reconfiguring when switching providers or models is a waste of time.

**איך OmniRoute פותר אותו:**

- **דשבורד CLIX0X] — דף ייעודי עם קישורים אחד-נקל ל-Claude Code, Codex CLI,
  OpenClaw, Kilo Code, Antigravity, Cline
- **מאמן GitHub Copilot** — מוציא `chatLanguageModels.json` ל-VS Code עם בחירה
  רב-עברית של דגימות
- **מדריך חבילה** — הצמדה מרוכזת ב-4 שלבים למשתמשים חדשים
- **אחד נקודת התעברות כל הדגימות** — הגדר `http://localhost:20128/v1` פעם אחת,
  גישה ל-67+ ספקים

</details>

<details>
<summary><b>🔑 8. "Managing OAuth tokens from multiple providers is hell"</b></summary>

Claude Code, Codex, Gemini CLI, Copilot — כולם משתמשים ב-OAuth 2.0 עם מסמכי
פנאות. המפיצים נדרשים לרשום מחדש באופן קבוע, para `client_secret האבוד`,
`redirect_uri_mismatch`, וכישלונות בשרתים רחוקים. OAuth ב-LAN/vps תואם במיוחד.

**איך OmniRoute פותר אותו:**

- **Auto Token Refresh** — הפעל מחדש של מסמכי OAuth ברקע לפני תום התקופה
- **OAuth 2.0 (PKCE) X27X] — זרם אוטומטי למוציא, Codex, Gemini CLI, Copilot,
  Kiro, Qwen, iFlow
- **Multi-Account OAuth** — מספרי חשבונות נפרדים באמצעות JWT/ID token הוצאה
- **OAuth Fix LAN/Remote** — זיהוי IP פרטי ל `redirect_uri` + צירוף URL מנותק
  לשרתי רחוק
- **OAuth Behind Nginx** —
- **מדריך השתלטות OAuth Remote** — מדריך צעד ב-Step לקבצי Google Cloud על
  VPS/Docker

</details>

<details>
<summary><b>📊 9. "I don't know how much I'm spending or where"</b></summary>

מפיצים נפרדים תולמים, אך אין מבט מרוכז אל

**איך OmniRoute פותר אותו:**

- **דשבורד Analysis of Costs** — מעקב אחר עלויות וניהול תקציב כל הספקים
- **Set- Limits by Layer** — Ceiling תקציב על-דרגה שמעלים fallback אוטומטי
- **Configuration Pricing by Model** — גודל [price per model
- **Usage Statistics by API Key** — העלאי- כ- [xapi][xLast-Used] by Key
- **Dashboard Analytics** — Chart cards, Usage of Models, table של provider
  success rate and latency

</details>

<details>
<summary><b>🐛 10. "I can't diagnose errors and problems in AI calls"</b></summary>

==WEBLATE_PART==\
[X0X]תיעוד בוקר עד-קולאס[X24X] — 4 טבלאות: תיעודי הבקשות, דוח נוטרי, איןפשי,
טכנולוגי

**איך OmniRoute פותר אותו:**

- **תוכן/VIEWer של לוג[X20X] — המקורה ב-Real-time terminal-style VIEWer, עם רמת
  צבע, גלגל AUTO-s, search, filter
- **SQLite Proxy Logs[X19X] — תיעוד חופשי ששרדי הפסקת שרת\
  ע
- **Playground של Translator[X23X] — 4 תצורות debugger: Playground (תרגום טפס),
  Chat Tester (round-trip), Test Bench (batch), Live Monitor (real-time)
- **תיעוד הבקשה[X19X] —\
  p50/p95/p99 latency + X-Request-Id tracing
- **תיעוד log עם file rotation[X34X] — Console interceptor captures everything
  to JSON log with size-based rotation
- **דוח אינפו של System[X20X] — [X25X]npm run system-info[X45X] generates
  [X57X]system-info.txt[X73X] with your full environment (Node version,
  OmniRoute version, OS, CLI tools, Docker/PM2 status). Attach it when reporting
  issues for instant triage.
- התקנה, הגדרה, ותחזוקת proxy AI מבוסס AI על ידי שוק(י)\
  X

</details>

<details>
<summary><b>🏗️ 11. "Deploying and maintaining the gateway is complex"</b></summary>

[X0X]npm global install[X20X] — [X25X]npm install -g omniroute &&
omniroute[X63X] — done

**איך OmniRoute פותר אותו:**

- **multi-platform Docker[X23X] — AMD64 + ARM64 native (Apple Silicon, AWS
  Graviton, Raspberry Pi)
- **Docker Profiles Compose[X25X] — [X30X]base[X35X] (no CLI tools) and
  [X56X]cli[X60X] (with Claude Code, Codex Code, OpenClaw)
- **Electron Desktop App[X22X] — Native app for Windows/macOS/Linux with system
  tray, auto-start, offline mode
- **Split-Port Mode[X17X] — API and Dashboard on separate ports for advanced
  scenarios (reverse proxy, container networking)
- **sync cloud[X12X] — Config synchronization across devices via Cloudflare
  Workers
- **DB Backups** — Automatic backup, restore, export and import of all settings
- צוותים במדינות ישראלים אי אנגלט שבדעד, xpectically וב אור בני-בע

</details>

<details>
<summary><b>🌍 12. "The interface is English-only and my team doesn't speak English"</b></summary>

[X0X]X[X0X] — languages languages languages languages languages languages
languages adoption and increase configuration errors.

**איך OmniRoute פותר אותו:**

- **מספור דשבורד i18n -- 30 שפות ** -- כל 500+ המפתחות תורגמו כולל ערבית,
  בולגרית, דנית, גרמנית, ספרדית, פינית, צרפתית, עברית, הינדי, הונגרית,
  אינדונזית, איטלקית, יפנית, קוריאנית, מלזית, הולנדית, נורווגית, פולנית,
  פורטוגזית (PT/BR), רומנית, רוסית, סלובקית, שוודית, תאילנדית, אוקראינית,
  וייטנאמית, סינית, טגלוג, אנגלית
- **תמיכה RTL** -- ממשק למעבר-קולני לעברית וערבית
- **READMEs בשפות שונות** -- 30 תעתיקים תחביריים מלאים
- **בחירת שפה** -- אייקון כדור עולם בראש הדף לצורך רישום מכוני

</details>

<details>
<summary><b>🔄 13. "I need more than chat — I need embeddings, images, audio"</b></summary>

AI אינו רק שלבי סיום-דברים. מפתחים צריכים לגנרט Image, לרשום Audio, לייצר
embeddings עבור RAG, לנרות תעתיקים, ליצור embeddings, ולמנסב content. כל API
ישנו נקודת-סי. ו פורמט

**איך OmniRoute פותר אותו:**

- **embeddings** -- embeddings/v1/embeddings` 6 providers 9+ models
- ** יצירת Image** -- /v1/images/generations` -- 10 providers 20+ models
  (OpenAI, xAI, Together, Fireworks, Nebius, Hyperbolic, NanoBanana,
  Antigravity, SD WebUI, ComfyUI)
- **Text-to-Video** -- /v1/videos/generations` -- ComfyUI (AnimateDiff, SVD)
  ו-SD WebUI
- **Text-to-Music** -- /v1/music/generations` -- ComfyUI (Stable Audio Open,
  MusicGen)
- **transcriptionAudio** -- /v1/audio/transcriptions` -- Whisper + Nvidia NIM,
  HuggingFace, Qwen3
- **Text-to-Speech** -- /v1/audio/speech` ElevenLabs, Nvidia NIM, HuggingFace,
  Coqui, Tortoise, Qwen3, Inworld, Cartesia, PlayHT, + providers
- **Moderations** -- /v1/moderations` Content safety checks
- **reranking** -- /v1/rerank` Document relevance reranking
- **Responses API** -- Full /v1/responses` support for Codex

</details>

<details>
<summary><b>🧪 14. "I have no way to test and compare quality across models"</b></summary>

מפתחים רוצים לדעת אילו מודל הוא הטוב ביותר עבור אתגר שלהם -- code, translation,
reasoning -- אבל עריכה בעל-ס, אלגוריתמי/אילנה יואב.\
-- אללה

**איך OmniRoute פותר אותו:**

- **LLM Evaluations** -- Golden set testing 10 pre-loaded cases greetings, math,
  geography, code generation, JSON compliance, translation, markdown, safety
  refusal
- **strategies 4 Match** -- exact`, contains`, regex`, custom` (JS function)
- **translator playground** -- Batch testing multiple inputs expected outputs,
  cross-provider comparison
- **Chat Tester** — מבחן שיחות מלא בעל תמונה-שני-כיוונים
- **Live Monitor** — זרם אמת-מה-עולם של כל בקשות העוברות דרך הפרוקסי

</details>

<details>
<summary><b>📈 15. "I need to scale without losing performance"</b></summary>

ככל שהכמות של בקשות הידלדל, עם פסילת מסוף אותו-אותו-שלב, אותו-אותו-נושא של
דואר-נפרד הוא עלות-כפול. אם ללא-ידידוא-עצי-פל, משלוחים-כף-שני-פעמים דורש
גמיל-מעד-שנתן-יד

**איך OmniRoute פותר אותו:**

- **Semantic Cache** — קצין-מסוף דו-שכבתי (חותם + סמנטי) מוריד
  זמן-הגאב-ואופ-מוה-קוסט
- **Request Idempotency** — 5 ה-מ-דב-ו-וי-שע-ד- חבורה-פח-ס-ב-ה-אות-מ-ב-הא-ל-ה
- **Rate Limit Detection** — עמיד-צ-ר-מ-ר-י-ם-י- (RPM), (min ) שע-ו-א- ש- -א-ה-
  -ה( -ן- - -
- **Editable Rate Limits** — ה- -א- - (Configure ) - - - (Settings → Resilience
  with persistence
- **API Key Validation Cache** — 3- - (tier cache (for performance (production
- **Health Dashboard with Telemetry** — p50/p95/p99 , latency, cache stats,
  uptime

</details>

<details>
<summary><b>🤖 16. "I want to control model behavior globally"</b></summary>

[x0x]m- --sׇ- - - (Developers who want all responses in a specific language,
with a specific tone, or want to limit reasoning tokens. - - - - - - - - (in
every tool/request is impractical

**איך OmniRoute פותר אותו:**

- **System Prompt Injection** — Global prompt injected to all requests
- **Thinking Budget Validation** — Reasoning token allocation control per
  request (passthrough, auto, custom, adaptive)
- **6 Routing Strategies** — Global strategies that determine how requests are
  distributed
- **Wildcard Router** —` provider/*` patterns routed dynamically to any provider
- **Combo Enable/Disable Toggle** — Toggle combos directly from the dashboard
- **Provider Toggle** — Enable/disable all connections for a provider with one
  click
- **Blocked Providers** — Exclude specific providers from `/v1/models` listing

</details>

<details>
<summary><b>🧰 17. "I need MCP tools as first-class product capabilities"</b></summary>

[x0x]m- - - (Many AI gateways expose MCP only as a hidden implementation detail.
Teams need a visible, manageable operation layer\
==WEBLATE_PART==

**איך OmniRoute פותר אותו:**

- כפליים מפבריק שיין (MCP) מופיע בתחום ההצפייה של הדפדפן ובעמוד הנורמה מפרוטוקול
  הסיוע
- דף ניהול מפבריק שיין, כולל: תהליכים, כלים, פרטים וסיכום
- שירות שקט כדי--mcp[x41]x להתקין omni route --mcp` וציבור ובור שבד

</details>

<details>
<summary><b>🧠 18. "I need A2A orchestration with sync + stream task paths"</b></summary>

מעקב עבודות נזרק השגה פאנל בזוהר החוורם-

**איך OmniRoute פותר אותו:**

- API של- JSON-RPC (`POST /a2a`)בעל `message/send` ו-`message/stream`
- זרימה SSE, תעבורה שפנב
- API חיים של פרו

</details>

<details>
<summary><b>🛰️ 19. "I need real MCP process health, not guessed status"</b></summary>

API MVC --MCP חי

**איך OmniRoute פותר אותו:**

- מכלול API--MCP
- Teams צבע פלוס אם MVC
- MCP status API- MVC --MCP

</details>

<details>
<summary><b>📋 20. "I need auditable MCP tool execution"</b></summary>

API MVC --MCP -

**איך OmniRoute פותר אותו:**

- API MVC --MCP
- API MVC --MCP
- API MVC --MCP +

</details>

<details>
<summary><b>🔐 21. "I need scoped MCP permissions per integration"</b></summary>

API MVC --MCP +\
\
\
\
(Translations that were not clear will be asked for clarification)

**איך OmniRoute פותר אותו:**

- 9 granular MCP scopes for controlled tool access
- Scope enforcement and visibility in MCP management UI
- Safe default posture for operational tooling

</details>

<details>
<summary><b>⚙️ 22. "I need operational controls without redeploying"</b></summary>

Teams need quick runtime changes during incidents or cost events.

**איך OmniRoute פותר אותו:**

- Switch combo activation directly from MCP dashboard
- Apply resilience profiles from pre-defined policy packs
- Reset circuit breaker state from the same operations panel

</details>

<details>
<summary><b>🔄 23. "I need live A2A task lifecycle visibility and cancellation"</b></summary>

Without lifecycle visibility, task incidents become hard to triage.

**איך OmniRoute פותר אותו:**

- Task listing/filtering by state/skill with pagination
- Drill-down on task metadata, events, and artifacts
- Task cancellation endpoint and UI action with confirmation

</details>

<details>
<summary><b>🌊 24. "I need active stream metrics for A2A load"</b></summary>

Streaming workflows require operational insight into concurrency and live
connections.

**איך OmniRoute פותר אותו:**

- Active stream counters integrated into A2A status
- Last task timestamp and per-state counts
- A2A dashboard cards for real-time ops monitoring

</details>

<details>
<summary><b>🪪 25. "I need standard agent discovery for clients"</b></summary>

External clients and orchestrators need machine-readable metadata for
onboarding.

**איך OmniRoute פותר אותו:**

- Agent Card נחשף ב`/.well-known/agent.json`
- יכולות ונכונות שמוצגות ב-UI של הניהול
- API A2A כוללת מתוחכמות גילוי עבור אוטומציה

</details>

<details>
<summary><b>🧭 26. "I need protocol discoverability in the product UX"</b></summary>

אם המשתמשים אינם יכולים לגלות פנאלים של פרוטוקול, יורדת איכות התמיכה ועקבות
השימוש

**איך OmniRoute פותר אותו:**

- עמוד ה-X13XEndpoints** האחיד שמותקן בדפדפות ל-Proxy, MCP, A2A, ו-API Endpoints
- הסוושה אס לאסטטוס של שירותים (Online/Offline) הישירה של MCP ו-A2A
- מעברים מהמערכת הכללי לחלונות הניהול המיוחדים

</details>

<details>
<summary><b>🧪 27. "I need end-to-end protocol validation with real clients"</b></summary>

המבחנים המוקיימים X13X אינם מספיקים כדי לא אמת מחדש תאימות הפרוטוקול הסופית לפני
יציאה

**איך OmniRoute פותר אותו:**

- רכבת הצד הסופי שמטען את האפליקציה ומשתמשת ב-MCP SDK ל-transport
- מבחני קולקטיב A2A לגבי גילוי, שליחה, זרימה, קבל, וביטול
- ביצועי אימות נגד API המעבר של MCP וAPI התיקונים של A2A

</details>

<details>
<summary><b>📡 28. "I need unified observability across all interfaces"</b></summary>

בפיצול אספקט האספקט האספקטית, נוצר פגע ארג"ט ו-A2A מעמיק-חד

**איך OmniRoute פותר אותו:**

- דפדפן מאוחד (דה) / מערכת (ל) /ב-Log anlystics
- -X11X (X13X) (X15X) בפרק ב-MCP- OpenAI -A2A layer
- API אופרציונליות לא-מעמ"י ורבים

</details>

<details>
<summary><b>💼 29. "I need one runtime for proxy + tools + agent orchestration"</b></summary>

רציית (X19X)שר (X24X)X19X) -X14X) - (X13X)X26X) ש- (X18X).

**איך OmniRoute פותר אותו:**

- stack של server של MCP ו-server של A2A תורם
- אימות חופשי, חוסן, חנות נתונים, ובחזרה
- דגם פוליסה תחומי התערבות

</details>

<details>
<summary><b>🚀 30. "I need to ship agentic workflows without glue-code sprawl"</b></summary>

קבוצות סובלות מאיבוד שפע בעת אסדקה חופשית

**איך OmniRoute פותר אותו:**

- אסטרטגיית הצגת פרוטוקול יחידה לצורכי הלקוח
- גישה אוטומטית לניהול פרוטוקול
- בסיסיות זמין (ביטחון, ההוצאה תפעול, חוסן, בקרה, וחמצה)

</details>

### דוגמאות לנוסחאות ([X0X] Playbooks)

** Playbook A: Maximize חברותך+Cheap Backup**

```txt
Combo: "Maximize Claude"
  1. cc/claude-opus-4-6
  2. glm/glm-4.7
  3. if/kimi-k2-thinking

עלות חודשית: $20 + יקרה שלחזר
עלייה: חסכונית, אפס תקלות.
```

** Playbook B: Zero-cost coding קטל

```txt
Combo: "Free Forever"
  1. gc/gemini-3-flash
  2. if/kimi-k2-thinking
  3. qw/qwen3-coder-plus

עלות חודשית:0
עלייה: קטל כ-מה-
```

** Playbook C: 24/7 Always-on chain

```txt
Combo: "Always-on"
  1. cc/claude-opus-4-6
  2. cx/gpt-5.2-codex
  3. glm/glm-4.7
  4. minimax/MiniMax-M2.1
  5. if/kimi-k2-thinking

עלייה: depth קפדן
```

** Playbook C: Agent ops בעזרת MCP + A2A

```txt
1)  Run MCP transport בתצרוך Tool-Driven
(` omni route --mcp`) 
2)  run A2A tasks Via ` message/send` 
  and ` message/stream`
3)  view on /dashboard/endpoint (MCP ומפשט)
4)  toggle services at status in line control
```

---

## 🐋     free — Cost Null

> Setup coding AI in minutes On-Board at ** $0 /month**. Connect free accounts
> using free combo של Built-in של ** Free Stack**\
> ==WEBLATE_PART==

| צעד | פעולה                                               | אספקנים מנותקים                                                    |
| --- | --------------------------------------------------- | ------------------------------------------------------------------ |
| 1   | התחבר **Kiro** (AWS Builder ID OAuth)               | סונט 4.5 של קלוד, 4.5 Haiku — **ללא הגבלה**                        |
| 2   | התחבר **iFlow** (Google OAuth)                      | kimi-k2-thinking, qwen3-coder-plus, deepseek-r1... — **ללא הגבלה** |
| 3   | התחבר **Qwen** (Device Code)                        | qwen3-coder-plus, qwen3-coder-flash... — **ללא הגבלה**             |
| 4   | התחבר **Gemini CLI** (Google OAuth)                 | gemini-3-flash, gemini-2.5-pro — **180K/חודש הרשות בחינם**         |
| 5   | `/dashboard/combos` → **Stack החינם (0$)** template | הסתיימו את כל האספקנים החינם ברשימה העדיפה                         |

**בחר קו קצה (IDE/CLI):** `http://localhost:20128/v1` · סיסמה: `קו קצה ` · סיום.

> **סיקור חינם (לא מחובר):** Groq API key (30 RPM free), NVIDIA NIM (40 RPM
> free, 70+ models), Cerebras (1M tok/day), LongCat API key (50M tokens/day!),
> Cloudflare Workers AI (10K Neurons/day, 50+ models).

## התחלה מהירה

### 1. התקן והפעל

```bash
npm install -g omniroute
omniroute
```

> **npm users:** רוץ npm approve-builds -g` אחרי התקנה כדי לאחד סקריפטי-ביניים
> מקוצרים דרושים על ידי `better-sqlite3` ו- `@swc/core`:
> 
> ```bash
> npm install -g omniroute
> npm approve-builds -g  # בחר כל החבילות מעבד
> omniroute
> ```

לוח המידע נפתח ב-X19X]http://localhost:20128` ו- API הבסיס
מנוי:`http://localhost:20128/v1`.

| תקשורת                  | תיאור                                                               |
| ----------------------- | ------------------------------------------------------------------- |
| `omniroute`             | הפעל שרת (PORT=20128`, API ואינטרפייס לאדמינסטרטורים - פורטים זהים) |
| `omniroute --port 3000` | עצים פורט קאנוניקל ו-API ל 3000                                     |
| `omniroute --mcp`       | הפעל שרת MCP (API ללא יכולת "open")                                 |
| `omniroute --no-open`   | דאגה לא פתח את הממשק תאריכל"                                        |
| `omniroute --help`      | הופצה סיוע                                                          |

אפשרות הפעלה במצב "ארג הפורטים" (ספליט-פורט):

```bash
PORT=20128 DASHBOARD_PORT=20129 omniroute
#API:      http://localhost:20128/v1
#          http://localhost:20129
```

### 2) התחבר לספקים ויצרו את מפתח ה-API

1. פתח את `הספקים` ב- Dashboard → והתחבר לספק סודי (OAuth או מפתח-API).
2. פתח את `התחברות` ב- Dashboard → ויצרו מפתח-API.
3. (אופציונלי) פתח את `המשחקים` ב- Dashboard → ובחרו את הזרימת-הפליטה הכפולה.

### 3) הפנה את כלי-העריכה שלך ל OmniRoute

```txt
URL בסיס: http://localhost:20128/v1
מפתח-API:  [העתק מעמוד התחברות]
מודל:    if/kimi-k2-thinking (או מושג-המסד האחסון של ספק או מודל)
```

תואם עם Claude Code, Codex CLI, Gemini CLI, Cursor, Cline, OpenClaw, OpenCode,
ובתיבות SDK שתואמות ל-OpenAI.

### 4) הפעל ואשר תקנות-ה-Protocols (v2.0)

**MCP (ל- tool-driven operations):**

```bash
omniroute --mcp
```

אז, התחבר את ל�IENT-client שלהם ל-`stdio` ובדוק כלים כמו:

- `omniroute_get_health`
- `omniroute_list_combos`

**A2A (ל- agent-to-agent workflows):**

```bash
curl http://localhost:20128/.well-known/agent.json
```

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"quickstart","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"Give me a short quota summary."}]}}'
```

### 5) אסור להשאיר-דבר-פתוח-סוף-של-ה- protocol-(recommented)

```bash
npm run test:protocols:e2e
```

בחבילה זו, מתבקש, ובדק את התקנות MCP- client-A2A נגד תוכניה-א- גרות-פעלת

### אופציה:  2 נוקד 2- A  נ"   ( -גם-  A  -  .)  2  (run-  02   - 0-  .  =- 4- .  a  09- 2  r 1- 8-  d 6-   )

```bash
cp .env.example .env
npm install
PORT=20128 DASHBOARD_PORT=20129 NEXT_PUBLIC_BASE_URL=http://localhost:20129 npm run dev
```

---

## 🐳 Docker

OmniRoute זמין כתדורות ציבורי ב-[Docker
Hub](https://hub.docker.com/r/diegosouzapw/omniroute).

[מצחין]Quick run:[12]

```bash
docker run -d \
  --name omniroute \
  --restart unless-stopped \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:latest
```

[מצחין]With environment file:[24]

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

[מצחין]Using Docker Compose:[23]

```bash
# Base profile (no CLI tools)
docker compose --profile base up -d

# CLI profile (Claude Code, Codex, OpenClaw built-in)
docker compose --profile cli up -d
```

| תמונה                             | תג               | גודל   | תיאור        |
| --------------------------------- | ---------------- | ------ | ------------ |
| [מצחין]diegosouzapw/omniroute[23] | [מצחין]latest[7] | ~250MB | איחוד אחרון: |
| [מצחין]diegosouzapw/omniroute[23] | [מצחין]1.0.3[6]  | ~250MB | גירסת הרצה   |

---

## 🖥️ Desktop App — Offline & Always-On

> 🆕 **חדש!** OmniRoute כעת זמין כיישום נטיבי (Native desktop application**) על
> Windows, macOS, ו-Linux.

רצה OmniRoute כיישום יישומי בודד (standalone desktop app) — כאן לא ישימים
(terminal), לא ג'ו (browser), לא זקוק (internet) כדי (to) שאבות (local models).

- 🖥️ **חלון נטיבי** — שורת אוויר (Dedicated app window) עם (with) שילוט (system
  tray integration)
- 🔄 **שיקוף (Auto-Start**) — (Launch OmniRoute ב-(system login)
- 🔔 **התרעות נטיביות** — (Get alerts ל-(quota exhaustion) או (provider issues)
- ⚡ **הגש (One-Click Install**) — NSIS (Windows), DMG (macOS), AppImage (Linux)
- 🌐 **שדה (Offline Mode**) — (Works על-(fully offline) (with) (bundled server)

### התחלה מהירה

```bash
# (development mode)
npm run electron:dev

# (build for your) (platform)
npm run electron:build         #(Current) (platform)
npm run electron:build:win     # (Windows) (.exe)
npm run electron:build:mac     # (macOS) (.dmg) — x64 &amp; arm64
npm run electron:build:linux   #(Linux) (.AppImage)
```

### סימניה (System Tray)

אזיק (When minimized), OmniRoute ב-(lives) (in) שילוט (your system tray) (with)
(quick actions:

- פתח את לוח המחוונים
- שנה (Change server) (port)
- סגור (Quit application)

📖 (Full documentation: [`electron/README.md`](electron/README.md)

---

## 💰 (Pricing at a Glance)

| מערכת ברירה      | ספק                        | עלות                          | אתח (Quota Reset)    | Best For                          |
| ---------------- | -------------------------- | ----------------------------- | -------------------- | --------------------------------- |
| **💳 מובטל**      | קלוד קוד (משתמש רגיל)      | $20/חודש                      | 5 שעות + שבועית      | הרשמה כבר נעשתה                   |
|                  | Codex (Plus/Pro)           | $20-200/חודש                  | 5 שעות + שבועית      | משתמשי OpenAI                     |
|                  | Gemini CLI                 | **FREE**                      | 180K/חודש + 1K/יום   | לכול!                             |
|                  | GitHub Copilot             | $10-19/חודש                   | חודשי                | משתמשי GitHub                     |
| **🔑 מפתח API**   | NVIDIA NIM                 | **FREE** (לדבוקא הנצחי)       | ~40 RPM              | 70+ מודלים פתוחים                 |
|                  | Cerebras                   | **FREE** (1M ‏טוק/יום)        | 60 אלף TPM / 30 RPM  | המהירים ביותר בעולם               |
|                  | Groq                       | **FREE** (30 RPM)             | 14.4 אלף RPD         | LLama/Gemma - מהיר אוטומט         |
|                  | DeepSeek V3.2              | $0.27/$1.10 ל-1M              | אין                  | תיעוד גובה-איכות טוב ביותר        |
|                  | xAI Grok-4 Fast            | **$0.20/$0.50 ל-1M** 🆕        | אין                  | מהיר וריבוי פעל                   |
|                  | xAI Grok-4 (סטנדרט)        | $0.20/$1.50 ל-1M 🆕            | אין                  | מגן-מנהיגות ל-xAI                 |
|                  | מיסטרל                     | חינם | שירותים בתשלום         | שיעור מוגבל          | אי.אי יורופאי                     |
|                  | OpenRouter                 | כריית וקבלת תשלום             | אין                  | יותר מ-100 דגמים בקבוצה           |
| ** 💰 זול**       | GLM-5 (via Z.A.I) 🆕        | 0.50/1,000,000                | 10 AM ביומי          | 128,000 כניסה, דגם חדש            |
|                  | GLM-4.7                    | 0.60/1,000,000                | 10 AM ביומי          | חיסכון לחיפזון                    |
|                  | MiniMax M2.5 🆕             | 0.30/1,000,000 כניסה          | 5 שעות נקוב          | תכנון + משימות בתקיפה             |
|                  | MiniMax M2.1               | 0.2 ₪/1,000,000               | 5 שעות נקוב          | אופציה הזולה ביותר                |
|                  | Kimi K2.5 (Moonshot API) 🆕 | כריית וקבלת תשלום             | אין                  | ממשק יaight ל-AAP Moonshot        |
|                  | Kimi K2                    | $9/mo flat                    | 10,000,000 tokens/mo | עלות נבונה                        |
| **🆓 קטיעה חינם** | iFlow                      | **P0**                        | ללא גבלה             | 5 דגמים ללא גבלה                  |
|                  | Qwen                       | **P0**                        | ללא גבלה             | 4 דגמים ללא גבלה                  |
|                  | Kiro                       | **P0**                        | ללא גבלה             | Claude Sonnet/Haiku (AWS Builder) |
|                  | LongCat Flash-Lite בנוסח 🆕 | **P0** (50,000,000 tok/day 🔥) | RPS 1                | Largest free quota on Earth       |
|                  | Pollinations AI 🆕          | **$0** (no key needed)        | 1 req/15s            | GPT-5, Claude, DeepSeek, Llama 4  |
|                  | Cloudflare Workers AI 🆕    | **$0** (10K Neurons/day)      | ~150 resp/day        | 50+ models, global edge           |
|                  | Scaleway AI 🆕              | **$0** (1M tokens total)      | שיעור מוגבל          | EU/GDPR, Qwen3 235B, Llama 70B    |

> 🆕 **New models added (Mar 2026):** Grok-4 Fast family at $0.20/$0.50/M
> (benchmarked at 1143ms — 30% faster than Gemini 2.5 Flash), GLM-5 via Z.AI
> with 128K output, MiniMax M2.5 reasoning, DeepSeek V3.2 updated pricing, Kimi
> K2.5 via Moonshot direct API.

**💡 $0 Combo Stack — The Complete Free Setup:**

```
# 🆓 Ultimate Free Stack 2026 — 11 Providers, $0 Forever
Kiro (kr/)             → Claude Sonnet/Haiku UNLIMITED
iFlow (if/)            → kimi-k2-thinking, qwen3-coder-plus, deepseek-r1 UNLIMITED
LongCat Lite (lc/)     → LongCat-Flash-Lite — 50M tokens/day 🔥
Pollinations (pol/)    → GPT-5, Claude, DeepSeek, Llama 4 — no key needed
Qwen (qw/)             → qwen3-coder-plus, qwen3-coder-flash, qwen3-coder-next UNLIMITED
Gemini (gemini/)       → Gemini 2.5 Flash — 1,500 req/day free API key
Cloudflare AI (cf/)    → Llama 70B, Gemma 3, Mistral — 10K Neurons/day
Scaleway (scw/)        → Qwen3 235B, Llama 70B — 1M free tokens (EU)
Groq (groq/)           → Llama/Gemma ultra-fast — 14.4K req/day
NVIDIA NIM (nvidia/)   → 70+ open models — 40 RPM forever
Cerebras (cerebras/)   → Llama/Qwen world-fastest — 1M tok/day
```

**Zero cost. Never stops coding.** Configure this as one OmniRoute combo and all
fallbacks happen automatically — no manual switching ever.

---

---

## 🆓 Free Models — What You Actually Get

> All models below are **100% free with zero credit card required**. OmniRoute
> auto-routes between them when one quota runs out — combine them all for an
> unbreakable $0 combo.

### 🔵 CLAUDE MODELS (via Kiro — AWS Builder ID)

| דגם                 | קידומת | מגבלה     | מגבלת שיעור           |
| ------------------- | ------ | --------- | --------------------- |
| `claude-sonnet-4.5` | `kr/`  | **בחינם** | אין מגבלה שוטפנית     |
| `claude-haiku-4.5`  | `kr/`  | **בחינם** | אין מגבלה שוטפנית     |
| `claude-opus-4.6`   | `kr/`  | **בחינם** | אופוס האחרון דרך Kiro |

### 🟢 אפלזמים IFLOW (OAuth חינם — אין כרטיס אשראי)

| דגם                | קידומת | מגבלה     | מגבלת שיעור     |
| ------------------ | ------ | --------- | --------------- |
| `kimi-k2-thinking` | `if/`  | **בחינם** | אין מגבלה שוטפת |
| `qwen3-coder-plus` | `if/`  | **בחינם** | אין מגבלה שוטפת |
| `deepseek-r1`      | `if/`  | **בחינם** | אין מגבלה שוטפת |
| `minimax-m2.1`     | `if/`  | **בחינם** | אין מגבלה שוטפת |
| `kimi-k2`          | `if/`  | **בחינם** | אין מגבלה שוטפת |

### 🔴  MODELS (Device Code Auth)

| דגם                 | קידומת | מגבלה     | מגבלת שיעור         |
| ------------------- | ------ | --------- | ------------------- |
| `qwen3-coder-plus`  | `qw/`  | **בחינם** | אין מגבלה שוטפת     |
| `qwen3-coder-flash` | `qw/`  | **בחינם** | אין מגבלה שוטפת     |
| `qwen3-coder-next`  | `qw/`  | **בחינם** | אין מגבלה שוטפת     |
| `vision-model`      | `qw/`  | **בחינם** | Multimodal (תמונות) |

### 🟣 CLI לגמיני (Google OAuth)

| דגם                   | קידומת | מגבלה                       | מגבלת שיעור      |
| --------------------- | ------ | --------------------------- | ---------------- |
| `ג'מיני-3-סקיצת פלאש` | `gc/`  | **180K טוק/לחודש** + 1K/יום | ניתוק מחדש בחודש |
| `ג'מיני-2.5-פרו`      | `gc/`  | 180K/לחודש (אפשרות שיתופית) | איכות גבוהה      |

### ⚫ NVIDA NIM (API Key חינם — build.nvidia.com)

| מערכת ברירה  | מגבלה יומית | מגבלת שיעור | הערות                                         |
| ------------ | ----------- | ----------- | --------------------------------------------- |
| חינם (פיתוח) | עיקוי טוק   | **~40 RPM** | 70+ דגמים; העברה למוגבלים פוריים באמצע ה-2025 |

דגמים פופולריים חינם: `moonshotai/kimi-k2.5` (Kimi K2.5), `z-ai/glm4.7` (GLM
4.7), `deepseek-ai/deepseek-v3.2` (DeepSeek V3.2),
`nvidia/llama-3.3-70b-instruct`, `deepseek/deepseek-r1`

### ⚪ CEREBRAS (API Key חינם — inference.cerebras.ai)

| מערכת ברירה | מגבלה יומית           | מגבלת שיעור         | הערות                                      |
| ----------- | --------------------- | ------------------- | ------------------------------------------ |
| חינם        | **1M בקרי סחורה/יום** | 60 אלף TPM / 30 RPM | מתוך ה-LLM המהיר ביותר; חוזר ומחדש מדי יום |

זמין בחינם: `llama-3.3-70b`, `llama-3.1-8b`, `deepseek-r1-distill-llama-70b`

### 🔴 GROQ (Authorization Free API Key — console.groq.com)

| מערכת ברירה | מגבלה יומית   | מגבלת שיעור           | הערות                                   |
| ----------- | ------------- | --------------------- | --------------------------------------- |
| חינם        | **14.4K RPD** | 30 RPM למודל לעת מועד | אין כרטיס אשראי; 429 כאשר גבל, לא ישויך |

זמין בחינם: `llama-3.3-70b-versatile`, `gemma2-9b-it`, `mixtral-8x7b`,
`whisper-large-v3`

### 🔴 LONGCAT AI (Authorization Free API Key — longcat.chat) 🆕

| דגם                              | קידומת  | מתכונת חינם יומית      | הערות                     |
| -------------------------------- | ------- | ---------------------- | ------------------------- |
| `LongCat-Flash-Lite-X19X         | `lc-X4X | **50M סימני שקיפה**  💥 | החסימה החינם הגדולה ביותר |
| `LongCat-Flash-Chat-X19X         | `lc-X4X | 500K סימני שקיפה       | שיחה מסלולית              |
| `LongCat-Flash-ThinkingX23X      | `lc-X4X | 500K סימני שקיפה       | התבוננות / CoT            |
| `LongCat-Flash-Thinking-2601X28X | `lc-X4X | 500K סימני שקיפה       | גרסת ינואר 2026           |
| `LongCat-Flash-Omni-2603X24X     | `lc-X4X | 500K סימני שקיפה       | היקש הרב-ערוצי            |

> 100% חינם בעת באת הבטא. הרשם ב-longcat.chat{}1 בעשרה או בטלפון. מתעדכן יומית,
> 00:00 UTC.

### 🟢 שאלת-קלות AI (אין חיוב API לרצועה) 🆕

| דגם        | קידומת | מגבלת שיעור | הספק מאחורי           |
| ---------- | ------ | ----------- | --------------------- |
| `openai`   | `pol/` | 1 req/15s   | GPT-5                 |
| `claude`   | `pol/` | 1 req/15s   | Claude של Anthropic   |
| `gemini`   | `pol/` | 1 req/15s   | Gemini של Google      |
| `deepseek` | `pol/` | 1 req/15s   | DeepSeek V3           |
| `llama`    | `pol/` | 1 req/15s   | Llama 4 Scout של Meta |
| `mistral`  | `pol/` | 1 req/15s   | Mistral AI            |

> ✨ **ללא דיסקורד: ** ללא הרשמה, ללא מפתח API. הוסף נותן ספק Pollinations עם שדה
> מפתח API ריק והוא עבד כל עת.

### 🟠 עובדי העולם של CLOUDFLARE (API Key - cloudflare.com) 🆕

| מערכת ברירה | נוירונים יומיים | אמצע ניצול                           | הערות                    |
| ----------- | --------------- | ------------------------------------ | ------------------------ |
| חינם        | **10,000**      | כּ-150 GPM / 500s audio / 15K embeds | גְלובאל edge, 50+ models |

דגמי-בניסיון חינם: `@cf/meta/llama-3.3-70b-instruct`,
`@cf/google/gemma-3-12b-it`, `@cf/openai/whisper-large-v3-turbo` (אודיו-חינם!),
`@cf/qwen/qwen2.5-coder-15b-instruct`

> מחיית API + Account ID מ- [dash.cloudflare.com](https://dash.cloudflare.com).
> שמור Account ID בהגדרות הספק.

### 🟣 SCALEWAY AI (1M Tokens- חינם — scaleway.com) 🆕

| מערכת ברירה | חינם Quota    | מיקום        | הערות                               |
| ----------- | ------------- | ------------ | ----------------------------------- |
| חינם        | **1M tokens** | 🇫🇷 Paris, EU | אין צורך בקרטיס כרטיסי חיים בתחומים |

זמינים חינם: `qwen3-235b-a22b-instruct-2507` (Qwen3 235B!),
`llama-3.1-70b-instruct`, `mistral-small-3.2-24b-instruct-2506`,
`deepseek-v3-0324`

> EU/GDPR compliant.קבל גישה API ב-
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

| ספק              | Free Credits           | Best Model                                   | מגבלת שיעור                  |
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

Then in `/דשבורד/מדיה` → **תרגום** tab: upload any audio or video file → select
your combo endpoint → get transcription in supported formats.

## 💡 מאפייני ראש

OmniRoute v2.0 is built as an operational platform, not just a relay proxy.

### 🆕 חדש — שיפורים שהשראויו ClawRouter (מרץ 2026)

| מאפיין                              | מה זה עושה                                                                                    |
| ----------------------------------- | --------------------------------------------------------------------------------------------- |
| ⚡ **פקח-4 אקספר ספאמ' **            | דגימות AI עבור $0.20/$0.50/M — השוואה 1143ms (30% מהירה יותר מ-Gemini 2.5  תקליט)             |
| 🧠 **GLM - 5 דרך Z.AI**              | 128K קונטקסט מוצא, $0.5/1M — הונרנגסק שלטנר  אחד ה-GLEך                                       |
| 🔮 **MiniMax M2.5**                  | logicheskaia + agenchtiscai tasks at $0.30/1M — significant upgrade from M2.1                 |
| 🎯 **flagtoolCalling per Model**     | Model per  `flagtoolCalling: true/false` in registry — Skip AutoCombo non-tool-capable models |
| 🌍 **Multilingual Intent Detection** | PT/ZH/ES/AR keywords in AutoCombo scoring — better model selection for non - English content  |
| 📊 **Benchmark-Driven Fallbacks**    | Real p95 latency from live requests feeds combo scoring — AutoCombo learns from actual data   |
| 🔁 **Request Deduplication**         | CONTENT-hashes based dedup window — multi-agent safe, prevents duplicate charges              |
| 🔌 **שליף סטרטגיה Router**           | Extensible `שליף סטרטגיה Router` interface — add custom routing logic as plugins              |

### 🚀 Previous v2.0.9+ — Playground, CLI Fingerprints & ACP

| מאפיין                                    | מה זה עושה                                                                                                                                                                                                                              |
| ----------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🎮 **Playground דגם**                      | Dashboard page to test any model directly — provider/model/endpoint selectors, Monaco Editor, streaming, abort, timing                                                                                                                  |
| 🔏 **CLI זיהוי חותמת**                     | Per-provider header/body ordering to match native CLI signatures — toggle per provider in Settings > Security. **Your proxy IP is preserved**                                                                                           |
| 🤝 **תמיכת ACP (Agent Client Protocol)**   | CLI agent discovery (Codex, Claude, Goose, Gemini CLI, OpenClaw + 9 more), process spawner, `/api/acp/agents` endpoint                                                                                                                  |
| 🤖 **דפדפן ACP מנווט**                     | Debug › Agents page — grid of 14 agents with install status, version, custom agent form for any CLI tool. **OpenCode** users get a "Download opencode.json" button that auto-generates a ready-to-use config with all available models. |
| 🔧 **מודל כותרת כוזר `apiFormat` Routing** | Custom models with `apiFormat: "responses"` now correctly route to the Responses API translator                                                                                                                                         |
| 🏢 **עבודה-מרחב Codex בידוד**              | Multiple Codex workspaces per email — OAuth correctly separates connections by workspace ID                                                                                                                                             |
| 🔄 **העדכון אלקטרון אוטומטי**              | Desktop app checks for updates + auto-install on restart                                                                                                                                                                                |

### 🤖 תפעול שליח והתקשרות (v2.0)

| מאפיין                                        | מה זה עושה                                                                                         |
| --------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| 🔧 **שרת MCP (16 כלים)**                       | IDE/agent tools via 3 transports: stdio, SSE (`/api/mcp/sse`), Streamable HTTP (`/api/mcp/stream`) |
| 🤝 **שרת A2A (JSON-RPC + SSE)**                | Execution of tasks between agents with sync and streaming flows                                    |
| 🧭 **דף קווי פתיחה מאוחד**                     | Tabbed management page with Endpoint Proxy, MCP, A2A, and API Endpoints tabs                       |
| 🎚️ **אוטומציות שירות Enable/Disable Toggles** | ON/OFF switches for MCP and A2A with settings persistence (default: OFF)                           |
| 🛰️ **לב הבעת MCP**                            | Real process status (pid, uptime, heartbeat age, transport, scope mode)                            |
| 📋 **עקבת MCP**                                | Filterable audit logs with success/failure and key attribution                                     |
| 🔐 **ניהול גישה MCP**                          | 9 granular scope permissions for controlled tool access                                            |
| 📡 **ניהול חיים טלאי A2A**                     | List/filter tasks, inspect events/artifacts, cancel running tasks                                  |
| 📋 **חיפוש כרטיס שולית**                       | `/.well-known/agent.json` for client auto-discovery                                                |
| 🧪 **Protocol E2E Test Harness**               | משחק תקשורת E2E באוצר `test:protocols:e2e`                                                         |
| ⚙️ **Operational Controls**                   | בכפתור החלפה, חינם פרופילי חוזריות, מחק עקובים מאחד סט עקיפה                                       |

### 🧠 Routing & Intelligence

| מאפיין                          | מה זה עושה                                                                                                       |
| ------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| 🎯 **Smart 4-Tier Fallback**     | ניווט אוטומטי: תזכור- [X2X]Subscription[X25X] → API התזכור ת[ X2X]Key[X25X] → [X2X]Cheap[X25X] → [X2X]Free[X25X] |
| 📊 **Real-Time Quota Tracking**  | ספירת טובות הזמן LIVE + [X2X]reset[X25X] ניגוד ספירה חי זמן מספק                                                 |
| 🔄 **Format Translation**        | OpenAI ↔ Claude ↔ Gemini ↔ Gemini ↔ Conversions מ- [X2X]schema[X25X]-safe                                        |
| 👥 **Multi-Account Support**     | סתגלות [X2X]MultiAccounts[X25X] בספקים דרך [X2X]intelligent[X25X] הנבחר                                          |
| 🔄 **Auto Token Refresh**        | Token OAuth תוכנן [X2X]retires[X25X] [X2X]automatically[X25X]                                                    |
| 🎨 **Custom Combos**             | 6 שטרת פיוס + [X2X]chain[X25X] אפשרי                                                                             |
| 🌐 **Wildcard Router**           | `provider/*` Routing דינאמית                                                                                     |
| 🧠 **משאבות תכניות               | Passthrough, auto, custom, and adaptive reasoning limits                                                         |
| 🔀 **אלייסים של דגימה**          | Built-in + custom model aliasing and migration safety                                                            |
| ⚡ **התרדש של רקע**              | Route low-priority background tasks to cheaper models                                                            |
| 🧪 ** Smart Routing - צלאל קשב** | Auto-select model by content type (coding/vision/analysis/summarization)                                         |
| 💬 **ההרעש של נושא**             | Global behavior controls applied consistently                                                                    |
| 📄 **תואמות API - הגירה**        | Full `/v1/responses` support for Codex and advanced agentic workflows                                            |

### 🎵 APIs ביצועי-תגובה

| מאפיין                   | מה זה עושה                                                                                                                                                                 |
| ------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🖼️ ** ייצור תמונות**     | `/v1/images/generations` with cloud and local backends                                                                                                                     |
| 📐 **המזהים**             | `/v1/embeddings` for search and RAG pipelines                                                                                                                              |
| 🎤 **Transkripcia Audio** | `/v1/audio/transcriptions` — 7 providers (Deepgram Nova 3, AssemblyAI, Groq Whisper, HuggingFace, ElevenLabs, OpenAI, Azure), auto-language detection, MP4/MP3/WAV support |
| 🔊 **Text-to-Speech**     | `/v1/audio/speech` — 10 providers (ElevenLabs, OpenAI, Deepgram, Cartesia, PlayHT, HuggingFace, Nvidia NIM, Inworld, Coqui, Tortoise) with correct error messages          |
| 🎬 **הפקת וידאו**         | `/v1/videos/generations` (ComfyUI + SD WebUI workflows)                                                                                                                    |
| 🎵 **הפקת מוזיקה**        | `/v1/music/generations` (ComfyUI workflows)                                                                                                                                |
| 🛡️ **ביקורת**            | `/v1/moderations` safety checks                                                                                                                                            |
| 🔀 **Reranking**          | `/v1/rerank` for relevance scoring                                                                                                                                         |
| 🔍 **חיפוש ובן** 🆕        | `/v1/search` — 5 providers (Serper, Brave, Perplexity, Exa, Tavily), 6,500+ free/month, auto-failover, cache                                                               |

### 🛡️ [X4X] Resilience, Security & Governance

| מאפיין                             | מה זה עושה                                                                             |
| ---------------------------------- | -------------------------------------------------------------------------------------- |
| 🔌 **Circuit Breakers**             | Per-model trip/recover with threshold controls                                         |
| 🎯 **Models Aware Endpoint**        | Custom models declare supported endpoints + API format                                 |
| 🛡️ **Anti-Thundering Herd**        | Mutex + semaphore protections on retry/rate events                                     |
| 🧠 **Semantic + Signature Cache**   | Cost/latency reduction with two cache layers                                           |
| ⚡ **Request Idempotency**          | Duplicate protection window                                                            |
| 🔒 **TLS Fingerprint Spoofing**     | Browser-like TLS fingerprint — **reduces bot detection and account flagging**          |
| 🔏 **CLI זיהוי חותמת**              | Matches native CLI request signatures — **reduces ban risk while preserving proxy IP** |
| 🌐 **IP Filtering**                 | Allowlist/blocklist control for exposed deployments                                    |
| 📊 **Editable Rate Limits**         | Configurable global/provider-level limits with persistence                             |
| 🔑 **API Key Management + Scoping** | Secure key issuance/rotation and model/provider controls                               |
| 🛡️ **Protected `/models`**         | Optional auth gating and provider hiding for model catalog                             |

### 📊 Observability & Analytics

| מאפיין                   | מה זה עושה                                                |
| ------------------------ | --------------------------------------------------------- |
| 📝 **בקשה + תאגיד רשתים** | לוגין מלא של בקשות/תשובות ותאגיד רשתים                    |
| 📋 **לוח מנהל אספקת יחד** | הצצה לעמוד אחד של בקשות, תאגיד רשתים, ניתוח וצפיית קונסול |
| 🔍 **טלאומטריה של רפלקס** | תזמון לקווי ג'50,95,99 ולאגירת בקשות                      |
| 🏥 **מחשבון בריאות**      | זמן עבודה, מצבי נפח, שולי, סטטיסטי קצר                    |
| 💰 **עקבת עלויות**        | בקרה על התקציב ונגישות ברמה המודל                         |
| 📈 **תחזיות אנליטי**      | ידיות של שימוש במודלים ונגישות ברמה הספק                  |
| 🧪 **תשתי הערכה**         | ניסויי קן זהב ברב ראשי לתאגיד                             |

### ☁️ התקנה ותשתי

| מאפיין                          | מה זה עושה                                               |
| ------------------------------- | -------------------------------------------------------- |
| 🌐 **התקן [נקודת]**              | localhost, VPS, Docker, Cloud environments               |
| ☁️  **מערכת־ענן**               | Configuration sync via cloud worker                      |
| 🔄  **Backup/Restore**           | Export/import and disaster recovery flows                |
| 🧙  **מדריך ההרשמה**             | First-run guided setup                                   |
| 🔧  **דשבורד של CLI Tools**      | One-click setup for popular coding tools                 |
| 🎮 **Playground דגם**            | Test any provider/model/endpoint from the dashboard      |
| 🔏  **אפשרות זיהוי CLI**         | Per-provider fingerprint matching in Settings > Security |
| 🌐  **i18n (30 languages)**      | Full dashboard + docs language support with RTL coverage |
| 🧹  **Clear All Models**         | One-click model list clearing in provider details        |
| 📋  **Issue Templates**          | Standardized GitHub templates for bugs and features      |
| 📂  **Directory of Custom Data** | `אישור תיקייה נתונים` override למיקום קובצי תיקייה       |

### דיעות שדה בעומק

#### האפקטולוגיה "smart fallback" עם גל השקעה מעשי

```txt
combo: "my-coding-stack"
  1. cc / claude-opus-4-6
  2. nvidia / llama-3.3-70b
  3. glm / glm-4.7
  4. if / kimi-k2-thinking
```

אומנירוט מעבר אוטומטי למועמד לבא בעקבות שגיאת קוורטו, שער, או מצב בריאות

#### אפליקציה של טכנולוגיה שהיא ראויה ופעיל

- MCP ו-AAA היינו זרימים באתר ומסמכים (לא מסתורין)
- API של מצבי טכנולוגיה (ג'ל ` , /api/`\
  ` /api/a2a /* ` )
- דשבורד כולל פעולות עבודה ביומו-שני (כפתורי כביסת קופסא ) , [X0X]reset[X7X]
  breaker, cancellation of tasks)

#### מעבד+דמות הביקורת

אזור [X0X]The Translator[X12X] כולל:

- **Playground**: יצירת חקירה
- **Chat Tester**: סיור שאילת-תגובה
- **Test Bench**: פעילות בעת ניסוי
- **Live Monitor**: מבט וממשק

נוסף: בדיקת פרוטוקול

> 📖 **[MCP Server README](open-sse/mcp-server/README.md)** — קשר לפגית, IDE
> configs, ודוגמאות לרשתות
> 
> 📖 **[A2A Server README](src/lib/a2a/README.md)** — כשלים, JSON-RPC methods,
> streaming, וצדקנים

## 🧪 אבחון

אומנירוט כולל תוכנית/מקוו פרטאומני ** Analytics → Evals** \
==WEBLATE_PART==

### הסט האורנג' של OmniRoute

האתחול "OmniRoute Golden Set" כולל תקריות ניתוח ל:

- ברכות, מתמטיקה, גאוגרפיה, יצירת קוד
- תקינות JSON, תרגום, יצירת markdown
- נסיון סירוב (תוכן הרמי), מניעת ספירה, הגייה בוליאנית

### אסטרטגיות הערכה

| אסטרטגיה      | תיאור                           | דוגמה                                 |
| ------------- | ------------------------------- | ------------------------------------- |
| `דוקטי`       | התאמה צביעה                     | `"4"`                                 |
| `מכיל`        | דוקטים המכילים תחת (בעל שם-מלא) | `"Paris"`                             |
| `תבנית רגולר` | תדמית התאימה תבנית רגולר        | `"1.*2.*3"`                           |
| `אוטומטי`     | פנקס JS אוטומטי חוזר true/false | `(פלט) =&gt; פלט.ל[ת].length &gt; 10` |

---

## מדריך הגדרה

### הגדרת פרוטוקול (MCP + A2A)

<details>
<summary><b>🧩 MCP Setup (Model Context Protocol)</b></summary>

התחל MCP transport במערכת הפעלה סטנדרטית:

```bash
omniroute --mcp
```

אבחנת זרימת השגיאה המומלצת:

1. שאיל את הלקוח MCS אל הסטנדרטית.
2. התחל `omniroute_get_health`.
3. התחל `omniroute_list_combos`.
4. פתח `/dashboard/mcp` כדי לאשש נפח, פעילות וביקורת.

APIים חשובות לאוטומציה:

- `GET /api/mcp/status`
- `GET /api/mcp/tools`
- `GET /api/mcp/audit`
- `GET /api/mcp/audit/stats`

</details>

<details>
<summary><b>🤝 A2A Setup (Agent2Agent)</b></summary>

גלה את האג'נט:

```bash
curl http://localhost:20128/.well-known/agent.json
```

שלח תפקיד:

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'פלג-תוכן: application/json' \
  -d '{"jsonrpc":"2.0","id":"setup-a2a","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"SUMMARIZE סטטוס-האגירה."}]}}'
```

נהל חיים:

- `GET /api/a2a/תצוגתעבודה`
- `GET /api/a2a/מטבעות`
- `GET /api/a2a/מטבעות /:id`
- `POST /api/a2a/מטבעות /:id/ביטול`

Active UI:

- `/dasborad/a2a` לצורכי תצוגתעבודה בזמן-אמת ומעשי רתמות

</details>

<details>
<summary><b>🧪 End-to-end protocol validation</b></summary>

Valida שני פרוטוקולים עם לקלקלים אמיתיים:

```bash
npm run test:protocols:e2e
```

זה מאשר:

- לקוח MCP SDK connect / list / call
- חיפוש A2A send / stream / get / cancel
- Cross-check נתונים ב-MCP audit ו-API A2A for task management

</details>

<details>
<summary><b>💳 Subscription Providers</b></summary>

### קלוד Code (Pro/Max)

```bash
Dashboard → ספקים → Connect Claude Code
→ OAuth login → Auto תעדכן טוקן
→ 5-שעות + שבועי עקבת
לקבלת Model :
  cc / claude-opus-4-6
  cc / claude-sonnet-4-5-20250929
  cc / claude-haiku-4-5-20251001
```

** Pro Tip: ** make use of Opus for complex tasks , Sonnet for speed . OmniRoute
tracks quota per model!

### OpenAI Codex (Plus/Pro)

```bash
Dashboard → Providers → Connect Codex
→ OAuth login (port 1455)
→ 5-שעות + restore שבועי

לקבל Model:
  cx / gpt-5.2-codex
  cx / gpt-5.1-codex-max
```

#### צב חשבון Codex Limit Management (5h + Weekly)

בכל חשבונות Codex ישן policy toggles תוך `Dashboard -&gt; Providers`:

- `5h` (ON/Off): enforce של 5 - שעה window threshold policy.
- `שבועי` (ON/OFF): enforce the weekly window threshold policy.
- התנהגות הגבול: כאשר חלון מוקטן ניגש ל- >=90%, חשבון זה מופנה אחורה.
- התנהגות הסתר: OmniRoute מעביר באופטימוס לחשבון Codex הבא האלוג'יבילי.
- התנהגות Reset: כאשר חבילת ה[ X34X ]Reset At` חל ב- time, החשבון נהייה
  אלוג'יבילי שוב סיבות-אוטומטי.

תאוריות:

- `5h ON` + `Weekly ON`: החשבון SKIPPED כאשר חלון כלשהו 닿 threshold.
- `5h OFF` + `Weekly ON`: ניתן SHUT ל-Weekly usage BLOCK החשבון.
- `5h ON` + `Weekly OFF`: 닿 ה-5- Usage BLOCK החשבון.
- `Reset At` passed: החשבון נכנס שוב rotation אוטומטית (א- Enable שאל).

### Gemini CLI (FREE 180K/month!)

```bash
דפדפן → Providers → Connect Gemini CLI
→ Google OAuth
→ 180K completions/month + 1K/day

Models:
  gc/gemini-3-flash-preview
  gc/gemini-2.5-pro
```

**Best Value:** Huge free tier! Use this before paid tiers.

### GitHub Copilot

```bash
דפדפן → Providers → Connect GitHub
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
3. דפדפן → Add Provider → NVIDIA NIM:
   - API Key: `nvapi-your-key`

**Models:** `nvidia/llama-3.3-70b-instruct`, `nvidia/mistral-7b-instruct`, and
50+ more

**תיפתח:** API-OpenAI לגמרי עובד - סינכרון אל תוך שפת אשכולות OmniRoute!

### DeepSeek

1. הרשמה: [platform.deepseek.com](https://platform.deepseek.com)
2. קבל את האי-PI
3. חדשות - > התווית מספק - > DeepSeek

**הדגמים:** `deepseek/deepseek-chat`, `deepseek/deepseek-coder`

### Groq (גרסה חינם)

1. הרשמה: [console.groq.com](https://console.groq.com)
2. קבל את האי-Pi (כלול בגרסה חিঠם)
3. חדשות - > התווית מספק - > Groq

**הדגמים:** `groq/llama-3.3-70b`, `groq/mixtral-8x7b`

**תיפתח:** מסונכרן עבור משתמש - המדויק ביותר לקוד ריאל-טיימ!

### OpenRouter (100+ הדגמים)

1. הרשמה: [openrouter.ai](https://openrouter.ai)
2. קבל את האי-PI
3. חדשות - > התווית מספק - > OpenRouter

**הדגמים:** הגיש 100+ הדגמים מכל ספקים גדולים, דרך [email protected]

</details>

<details>
<summary><b>💰 Cheap Providers (Backup)</b></summary>

### GLM-4.7 (לקושט בסיבוב, כ- $0.6 / 1M)

1. הרשמה: [Zhipu AI](https://open.bigmodel.cn/)
2. קבל את האי-Pi מ-Coding וה'כלי'\
   ==WEBLATE_PART==
3. יישום המוצף - הוספת מפתח API:
   - מספק: `glm`
   - מפתח API: `your-key`

**שימוש:** `glm/glm-4.7`

**עיפרון:** מתוכנת-כרטיס המציע 3X שקל 1/7! נרגיל כל יום ב-10:00 AM.

### MiniMax M2.1 (5h reset, $0.20/1M)

1. הרשמה: [MiniMax](https://www.minimax.io/)
2. קבל את האי-PI
3. יישום המוצף - הוספת מפתח API

**שימוש:** `minimax/MiniMax-M2.1`

**עיפרון:** אפשרות הירושה 1M tokens)!

### Kimi K2 ($9/month flat)

1. השתלם: [Moonshot AI](https://platform.moonshot.ai/)
2. קבל את האי-PI
3. יישום המוצף - הוספת מפתח API

**שימוש:** `kimi/kimi-latest`

**עיפרון:** 9$/חודש 1M tokens = $0.90/1M העלויות האפקטיביות!

</details>

<details>
<summary><b>🆓 FREE Providers (Emergency Backup)</b></summary>

### iFlow (5 FREE models via OAuth)

```bash
יישום המוצף -   iFlow
→ iFlow OAuth login
→ שימוש חופשי

מודלים:
  if/kimi-k2-thinking
  if/qwen3-coder-plus
  if/glm-4.7
  if/minimax-m2
  if/deepseek-r1
```

### Qwen (4 FREE models via Device Code)

```bash
==WEBLATE_PART==
תֵּיבָה שָׂנִי Kwen
→ קוד בַּמַשִּׁין
→ מְחִיר כְּלָל

מְדָנים:
  qwen/qwen3-coder-plus
  qwen/qwen3-coder-flash
```

### קִירו (קלוד שָׂנֶה)

```bash
תֵּיבָה שָׂנִי Kiro
→ AWS Builder ID או Google / GitHub
→ מְחִיר כְָל

מְדָנים:
  kr/claude-sonnet-4.5
  kr/claude-haiku-4.5
```

</details>

<details>
<summary><b>🎨 Create Combos</b></summary>

### דָּגָם 1: ' אכְלוּס'\

```
תֵּיבָה שָׂנִי - 'Combos' → 'בָּנָה חָדָש'
שם: 'premium-coding'
מְדָנים:
  1. cc/claude-opus-4-6 (אֶחְרָבָה רִאשׁוֹנה)
  2. glm/glm-4.7 (זוּל 'חֵפשׁ', 0.6/1M)
  3. minimax/MiniMax-M2.1 (זוּל 'מְנֻצָּה', 0.20/1M)

שִׁימוש בCLI: 'premium-coding'
```

### דָּגָם 2: 'זוּל שָׂנֶה (אֲפֵס)'

```
שם: 'free-combo'
מְדָנים:
  1. gc/gemini-3-flash-preview (180K חָרוּשׁ 'חָדָש')
  2. if/kimi-k2-thinking (בְּאין מְגָב)
  3. qwen/qwen3-coder-plus (בְּאין מְגָב)

מִמְחָל'
!= פָּעַם!
```

</details>

<details>
<summary><b>🔧 CLI Integration</b></summary>

### הסמן IDE

```
'  תאֹמ
תָּבנִית:
  OpenAI API Base URL: http://localhost:20128/v1
  OpenAI API Key: [from OmniRoute dashboard]
  Model: cc/claude-opus-4-6
```

### קלוד קוד

שִׁימוש 'CLI Tools** 'CLI**' \
בָּןֵה ' - ' בָּנָה' \
ישִׁימ שׂ" 'CLI` 'פּ'~/.claude/settings.json`' א'א

### 'C CLI

```bash
export OPENAI_BASE_URL="http://localhost:20128"
export OPENAI_API_KEY="your-omniroute-api-key"

codex "your prompt"
```

### 'אנ'ל

**דָּגָם 1 - 'דָּפו' **

```
'דָּפו' → CLI Tools → OpenClaw → Select Model → Apply
```

** 1 - ' ' \
` ' ' ~`:

```json
{
  'models": {
    "providers": {
      "omniroute": {
        'baseUrl": "http://127.0.0.1:20128/v1",
        'apiKey": "sk_omniroute",
        'api": "openai-completions"
      }
    }
  }
}
```

> **ה ** \
> "OpenClaw פעְ 'Open[I]' \
> ['127.0.0.1` 127.0.0.1` ' 'localhost` ' .

### '  / / RooCode\

```
Settings → תצורה API:
  מספק: OpenAI Compatible
  URL מסיסת בסיס: http://localhost:20128/v1
  מפתח API: [מאצנס OmniRoute דירוטשט]
  Model: if/kimi-k2-thinking
```

### OpenCode

**Step 1:** Add OmniRoute כמספק מקורי:

```bash
opencode
/connect
# בחר "Other" → הכנס ID: "omniroute" → הכנס את ה-API key של OmniRoute שלך
```

**Step 2:** הוסף/ערך `opencode.json` בתיקיית [X51X]root[X62X] של project שלך:

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

**Step 3:** Select מדלל ב- OpenCode:

```bash
/models
# בחר כל OmniRoute model מהרשימה
```

> **Tip:** הוספה של [X13X]Any model[X21X] זמין ב- בסיס OmnriRoute
> [X38X]v1/models` endpoint ל `models[X95X] סיקס. שת ת
> [X121X]provider/model-id[X136X] [X145X] from your OmniRoute Dashboard.

</details>

---

## פתרון בעיות

<details>
<summary><b>Click to expand troubleshooting guide</b></summary>

**"model בעי תש נ **languagedid not provide messages"[X59X]

- Provider quota exhausted → Check dashboard dashboard quota tracker
- Solution: Use combo fallback or switch to cheaper tier

**Rate limiting**

- Subscription quota out → Fallback to GLM/MiniMax
- Add combo: `cc/claude-opus-4-6 → glm/glm-4.7 → if/kimi-k2-thinking[X65X]

**OAuth token expired**

- Auto-refreshed by Omniroute
- If issues persist: dashboard -> provider -> reconnect

**High costs**

- בדוק סטטיסטיקות שימוש בדשבורד → עלויות
- שנה את המודל הראשי ל-GLM/MiniMax
- את הגיטאר (Gemini CLI, iFlow) לאשליות אינטראקטיביות

[ X0X ]דשבורד/API נמנע פורטים[ X31X ]

- [ X0X ]PORT[ X5X ] הוא פורט הבסיס (וה-API על ידי הגדרת הרשמה)
- [ X0X ]API_PORT[ X9X ]תוודא תורכ רק מאזן ה-API הפתיר ע" ית Jerusalem OpenAI
- [ X0X ]DASHBOARD_PORT[ X15X ] תוודא רק את קולית/Next.js שט
- הגדר [ X4X ]NEXT_PUBLIC_BASE_URL[ X25X ] את כתובת URL של דשבורד /public
  (לשיחות OAuth )

[ X0X ]שגיאות sync בעולם**

- אשר [ X7X ]BASE_URL[ X16X ] דלמעקב א
- אשר [ X7X ]CLOUD_URL[ X17X ] דלאק
- אח"ק [ X5X ]NEXT_PUBLIC_ *[ X19X ] שיצב ע" Y

[ X0X ]לא Xfirst login X not working**

- אשור [ X6X ]INITIAL_PASSWORD[ X23X ] ב[ X28X ].env`
- אם אין, תחל_ [ X31X ]123456 `

[ X0X ]No request logs**

- הגדר [ X4X ]ENABLE_REQUEST_LOGS= true` ב[ X34X ].env`

[ X0X ]Connection test shows "Invalid" for OpenAI-compatible providers**

- רב providers דור" not expose a /models endpoint
- OmnimRoute v1.0.6 + includes fallback validation via chat completions
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

**4. Save and copy the **קרדיטאליות**

אחרי יצירה, Google יראה את **Client ID** ואת **Client Secret**.

**5. Set environment variables**

ב-`.env` (או אתרי הסברה דוקר):

```bash
# ל-Antigravity:
ANTIGRAVITY_OAUTH_CLIENT_ID=your-client-id.apps.googleusercontent.com
ANTIGRAVITY_OAUTH_CLIENT_SECRET=GOCSPX-your-secret

# ל-Gemini CLI:
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

דשבורד → ספקים → Antigravity (או Gemini CLI) → OAuth

Google ישלח כעת ל-`https://your-server.com/callback`.

---

#### תצורה זמנית (ללא קרדיטאליות ידניות)

אם אינך רוצה להקים קרדיטאליות משלך כרגע, ניתן עוד להשתמש ב-**manual URL flow**:

1. OmniRoute פותחת URL של אישור Google
2. אחרי אישור, Google נוסה לשלוח אל `localhost` (אשר נכשל על השרת המרוחק)
3. **Copy the full URL** מ-הדילוג של הדפדפן (אפילו אם הדף לא נטען)
4. הדביק לתיבה שמוצגת בחופן שידור OmniRoute
5. לחץ **"Connect"**

> זה עובד כי הקוד באושר ב-URL ל-גמיש.

---

<details>
<summary><b>🇧🇷 Versão em Português</b></summary>

#### למה OAuth של Antigravity / Gemini CLI נכשל בשרתים רחוקים?

הספקים **Antigravity** ו-**Gemini CLI** השתמשים **Google OAuth 2.0** לאיזורי
אותנציפציה. Google דואג `redirect_uri` שמופעל בהחזקים OAuth להיות **מדויק** אחת
מ-URIs שהושבעה מראש ל- Google Cloud Console של האפליקציה.

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

**6. הפעל את האומנירוט**

```bash
# אם משתמשים בnpm:
npm run dev

# אם משתמשים בDocker:
docker restart omniroute
```

**7. נסה להתחבר שנית**

Dashboard → Providers → Antigravity (או Gemini CLI) → OAuth

כעת הגוגל יגדיר את `https://seu-servidor.com/callback` וההתקנה תתקן.

---

#### עבודה זמנית (ללא הפעלת יישומים)

אם לא רוצים להשלים את ההפעלה של הרב-ערכים עתה, יש לכם את האפשרות להשתמש ב[
X78X]שטח URL**:

1. אומנירוט יפתח [X0X]URL של אישור[X22X] של הגוגל
2. אחרי שאתם התחתנו, [X47X]http://localhost` (המקום הזה לא פועל בשרת הרחוק)
3. **Copy URL במלאי** של [X25X] Browser[X35X]
4. Copie זאת [X0X]URL של [X47X]seu-servidor.com/callback[X81X]
5. **"Connect"**

> זה [X50X] עבודה[X65X] שהקוד העוטף ב [X47X]URL[X66X] קיים.

</details>

---

</details>

## 🛠️ Tech Stack

<details>
<summary><b>Click to expand tech stack details</b></summary>

- ** Runtime**: Node.js 18–22 LTS (⚠️ Node.js 24+ is **not supported** —
  `better-sqlite3` native binaries are incompatible)
- **Language**: TypeScript 5.9 — ה- **100% TypeScript** גם אחרי ` src/`
  ו-`open-sse/`
- ** Framework**: Next.js 16 + React 19 + Tailwind CSS 4
- ** Database**: LowDB (JSON) + SQLite (domain state + proxy logs + MCP audit +
  routing decisions)
- ** Schemas**: Zod (MCP tool I/O validation, API contracts)
- ** Protocols**: MCP (stdio/HTTP) + A2A v0.3 (JSON-RPC 2.0 + SSE)
- **Streaming**: Server-Sent Events (SSE)
- **Auth**: OAuth 2.0 (PKCE) + JWT + API Keys + Authorization Scoped to MCP
- **Testing**: Node.js test runner + Vitest (900+ tests including unit,
  integration, E2E)
- **CI/CD**: GitHub Actions (auto publish npm + Docker Hub on release)
- **Website : [OmniRoute. net](https://omniroute.online)
- **Package**:
  [npmjs.com/package/omniroute](https://www.npmjs.com/package/omniroute)
- **Docker**:
  [hub.docker.com/r/diegosouzapw/omniroute](https://hub.docker.com/r/diegosouzapw/omniroute)
- **Resilience**: Circuit Breaker, Backoff Exponential, Anti-thundering Herd,
  TLS Spoofing, Auto-combo Self-healing

</details>

---

## תיעוד

| תעוד                                           | תיאור                                           |
| ---------------------------------------------- | ----------------------------------------------- |
| [דרך המשתמש](docs/USER_GUIDE.md)               | תפקודי MKP, combos, API של התגזמות, השבתה       |
| [מדריך API](docs/API_REFERENCE.md)             | כל נקודת ממשק עם דוגמאות                        |
| [Server ה- MCP](open-sse/mcp-server/README.md) | 16 כלי SDK, הגדרות IDE, קליינטים: Python/TS/Go  |
| [Server A2A](src/lib/a2a/README.md)            | הסכם RPC 2.0, skills, streaming, ניהול missions |
| [מנגנון Auto-Combo](docs/auto-combo.md)        | 6-גורמי ציון, קבצי פורמט, תיקון עצמי            |
| [תקנות](docs/TROUBLESHOOTING.md)               | בעיות נפוצות ופתרונות                           |
| [ארכיטקטורה](docs/ARCHITECTURE.md)             | ארכיטקטורה ואבחנת היבטים                        |
| [תרומה](CONTRIBUTING.md)                       | הקמת והגדרות מערכת                              |
| [פרטי API פתוח](docs/openapi.yaml)             | פרטי API 3.0 מספרית                             |
| [מדיניות ביטחון](SECURITY.md)                  | דוחות חולשות ומערכות בטיחות                     |
| [התקני VM](docs/VM_DEPLOYMENT_GUIDE.md)        | הדרך המלאה: VM + nginx + Cloudflare התקנה       |
| [תצוגה של יישומון מאוחד](docs/FEATURES.md)     | מסלולי נסיעה ביזמיות, עם מסקרינים               |
| [רשימת תקנות שחרור](docs/RELEASE_CHECKLIST.md) | עצה שחרור מראש, צעדי אבחנה                      |

---

## 🗺️ היצ'ום

OmniRoute חזה **210+ יישום שארה יבשים פעיל. ה

| קטגוריה                         | מצוקת תכונות | כותרות                                                                                             |
| ------------------------------- | ------------ | -------------------------------------------------------------------------------------------------- |
| 🧠 **תסצנת הורדת & אינטליגנציה** | 25+          | החבילה הנמוכה ביותר של דרייב, החבילה המבוססת על מאפיינים, רישום מוקדם של קווטה, P2C תמיכה בחשבונות |
| 🔒 **בטחון & תנאים**             | 20+          | החזקת SSRF, צלפות של כרתי, מגבלת טווח אחידה, מצוקת מפתח                                            |
| 📊 **נגישות**                    | 15+          | בינג' הפתוח של OpenTelemetry, פיקוח און-ליין של קווטה, עקבה הקצאה מחיר                             |
| 🔄 **התקשרות ספק                 | 20+          | Dynamic model registry, provider cooldowns, multi-account Codex, Copilot quota parsing             |
| ⚡ **ביצוע**                     | 15+          | Dual cache layer, prompt cache, response cache, streaming keepalive, batch API                     |
| 🌐 **אקוסיסטם**                  | 10+          | WebSocket API, config hot-reload, distributed config store, commercial mode                        |

### 🔜 כצמד

- 🔗 **OpenCode Integration** — Native provider support for the OpenCode AI
  coding IDE
- 🔗 **TRAE Integration** — Full support for the TRAE AI development framework
- 📦 **Batch API** — Asynchronous batch processing for bulk requests
- 🎯 **Tag-Based Routing** — Route requests based on custom tags and metadata
- 💰 **Lowest-Cost Strategy** — Automatically select the cheapest available
  provider

> 📝 Full feature specifications available in
> [`docs/new-features/`](docs/new-features/) (217 detailed specs)

---

## 👥 Contributors

[![Contributors](https://contrib.rocks/image?repo=diegosouzapw/OmniRoute&max=100&columns=20&anon=1)](https://github.com/diegosouzapw/OmniRoute/graphs/contributors)

### How to Contribute

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

See [CONTRIBUTING.md](CONTRIBUTING.md) for detailed guidelines.

### Releasing a New Version

```bash
# Create a release — npm publish happens automatically
gh release create v2.0.0 --title "v2.0.0" --generate-notes
```

---

## 📊 Star History

## Stargazers over time

## [![Stargazers over time](https://starchart.cc/diegosouzapw/OmniRoute.svg?variant=adaptive)](https://starchart.cc/diegosouzapw/OmniRoute)

## 🙏 Acknowledgments

תודות מיוחדות ל **[ CLIProxyAPI ](https://github.com/decolua/9router)[X36X] —
גרסה המקורית שהשפיעה על גרסה זו של JavaScript.

OmniRoute מבנה על הבסיס הגדול הזה, עם תכונות נוספות, APIs אוטומטיים מרובי-שיטות
ושחזור מחדש ב-ToTypeScript.

---

## הסכם רישיון 📄

רישיון MIT - ראה [LICENSE](LICENSE) על פרטים\
==WEBLATE_PART==

---

<div align="center">
  <sub>Built with ❤️ for developers who code 24/7</sub>
  <br/>
  <sub><a href="https://omniroute.online">omniroute.online</a></sub>
</div>
<!-- GitHub Discussions enabled for community Q&A -->
