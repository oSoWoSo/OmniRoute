# 🚀 OmniRoute — The Free AI Gateway

### Никога не преставайте да програмирате. Интелигентно маршрутиране до **МОВНИ И БАЛСОВИ ИНТЕЛИГЕНТНИ МОДЕЛИ** със съществена fallback.

_Вашата универсална API-посредник — едно endpoint, 67+ провайдъра, никакъв
downtime. Сега със **MCP & A2A** агентна координация._

**Чатовите допълвания • Ингредиенти • Изобразяване на слики • Видео • Музика •
Аудио • Опитуване на резултатите • **Пътеводител за Веб** • MCP Server • A2A
Protocol • 100% TypeScript**

---

<div align="center">

[![npm
версия](https://img.shields.io/npm/v/omniroute?color=cb3837&logo=npm)](https://www.npmjs.com/package/omniroute)
[![npm
сваляния](https://img.shields.io/npm/dm/omniroute?color=cb3837&logo=npm&label=npm%20downloads)](https://www.npmjs.com/package/omniroute)
[![Docker
Hub](https://img.shields.io/docker/v/diegosouzapw/omniroute?label=Docker%20Hub&logo=docker&color=2496ED)](https://hub.docker.com/r/diegosouzapw/omniroute)
[![Свала на
Docker](https://img.shields.io/docker/pulls/diegosouzapw/omniroute?logo=docker&color=2496ED&label=docker%20pulls)](https://hub.docker.com/r/diegosouzapw/omniroute)
[![Лиценз](https://img.shields.io/github/license/diegosouzapw/OmniRoute)](https://github.com/diegosouzapw/OmniRoute/blob/main/LICENSE)
[![Уебсайт](https://img.shields.io/badge/Website-omniroute.online-blue?logo=google-chrome&logoColor=white)](https://omniroute.online)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-Community-25D366?logo=whatsapp&logoColor=white)](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

[🌐 Уебсайт](https://omniroute.online) • [🚀 Бърза поява](#-quick-start) • [💡
Функции](#-key-features) • [📖 Документация](#-documentation) • [💰
Цени](#-pricing-at-a-glance) • [💬
WhatsApp](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

</div>

🌐 **Достъпен в:** 🇺🇸 [Американска](README.md) | 🇧🇷 [Португалски
(Бразилия)](docs/i18n/pt-BR/README.md) | 🇪🇸 [Испански](docs/i18n/es/README.md) |
🇫🇷 [Френски](docs/i18n/fr/README.md) | 🇮🇹 [Италиански](docs/i18n/it/README.md) |
🇷🇺 [Руски](docs/i18n/ru/README.md) | 🇨🇳 [Китайски
(прости)](docs/i18n/zh-CN/README.md) | 🇩🇪 [Немски](docs/i18n/de/README.md) | 🇮🇳
[Хинди](docs/i18n/in/README.md) | 🇹🇭 [タイ](docs/i18n/th/README.md) | 🇺🇦
[Українське](docs/i18n/uk-UA/README.md) | 🇸🇦 [Арабски](docs/i18n/ar/README.md) |
🇯🇵 [Японски](docs/i18n/ja/README.md) | 🇻🇳 [Виетнамски](docs/i18n/vi/README.md) |
🇧🇬 [Български](docs/i18n/bg/README.md) | 🇩🇰 [Датски](docs/i18n/da/README.md) |
🇫🇮 [Фински](docs/i18n/fi/README.md) | 🇮🇱 [Ебреишки](docs/i18n/he/README.md) | 🇭🇺
[Унгарски](docs/i18n/hu/README.md) | 🇮🇩 [Индонезийски](docs/i18n/id/README.md) |
🇰🇷 [Corean](docs/i18n/ko/README.md) | 🇲🇾 [Малайски](docs/i18n/ms/README.md) | 🇳🇱
[Нидерландски](docs/i18n/nl/README.md) | 🇳🇴 [Норвежки](docs/i18n/no/README.md) |
🇵🇹 [Португалски (Португалия)](docs/i18n/pt/README.md) | 🇷🇴
[Румънски](docs/i18n/ro/README.md) | 🇵🇱 [Польски](docs/i18n/pl/README.md) | 🇸🇰
[Словакийски](docs/i18n/sk/README.md) | 🇸🇪 [Шведски](docs/i18n/sv/README.md) |
🇵🇭 [Филипийски](docs/i18n/phi/README.md) | 🇨🇿 [Чешки](docs/i18n/cs/README.md)

---

## 🆕 Що е новото в v3.0.0.

> **Предиствувам от v2.9.5?** — Вижте [цялото
> CHANGELOG](CHANGELOG.md#300--2026-03-22-release-candidate--not-yet-merged-to-main)
> за всички промени.

| Оblast                                            | Смениние                                                                                                                                                                  |
| ------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🔒 **CodeQL Security**                             | Справили над 10 аларми на CodeQL: polynomial-redos, insecure-randomness, shell-injection Remediation                                                                      |
| ✅ **Route Validation**                            | Сега са валидирани всички 176 API-рути с Zod схеми + `validateBody()` — CI `check:route-validation:t06` завършва                                                          |
| 🐛 **omniModel Tag Leak**                          | Вътрешните `&lt;омни модели&gt;` марки не излизат до клиентите в SSE струящи отговори (#585)                                                                              |
| 🔑 **Registered Keys API**                         | Авто-предоставяне на API ключове чрез `POST /api/v1/registered-keys` с една на provider/счетовка квота, идентичност, SHA-256 съхранение и възможно GitHub issue reporting |
| 🎨 **Provider Icons**                              | 130+ провайдърски лого чрез `@lobehub/icons` (SVG) с fallback на PNG                                                                                                      |
| 🔄 Автоматично синхронизиране със събота **Модел** | 24-часовият шпилон и ръчно UI настройки за синхронизиране на списъци на моделите за вградени и кастомни провайдъри, съвместими с OpenAI                                   |
| 🌐 **Открит код Зен/Го**                           | Двата нови провайдъра от @kang-heewon чрез PR #530: безплатен тариф + абонаментен тариф чрез `OpencodeExecutor`                                                           |
| 🐛 **Северен блик OAuth**                          | Актуализирано извеждане на баводейства при липса на `GEMINI_OAUTH_CLIENT_SECRET` в Docker (беше криптирано гуглово извеждане)                                             |
| 🐛 **Открит код конфигуранти**                     | `saveOpenCodeConfig()` сега коректно записва TOML в `XDG_CONFIG_HOME`                                                                                                     |
| 🐛 **Близки модел override**                       | `body.model` сега коректно е поставен на `pinnedModel` на защита на контекстно-кеш                                                                                        |
| 🐛 **Кодекс Клод луп**                             | `tool_result` блокове сега преобразувани в текст за да спрят неограничени петли                                                                                           |
| 🐛 **Пренавеждане за вход**                        | Входът вече не замразява след пропускането на настройката за парола                                                                                                       |
| 🐛 **Патейки за Windows**                          | Патѐйки за MSYS2/Git-Bash (`/c/...`) нормализирани автоматично към `C:\...`                                                                                               |

---

## 🖼️ Основно Dashboard

<div align="center">
  <img src="./docs/screenshots/MainOmniRoute.png" alt="OmniRoute Dashboard" width="800"/>
</div>

---

## 📸 Преглед на Dashboard

<details>
<summary><b>Click to see dashboard screenshots</b></summary>

| Страница               | Збирка                                                   |
| ---------------------- | -------------------------------------------------------- |
| **Обработчици**        | ![Обработчици](docs/screenshots/01-providers.png)        |
| **Комбита**            | ![Комбита](docs/screenshots/02-combos.png)               |
| **Анализи**            | ![Анализи](docs/screenshots/03-analytics.png)            |
| **Здраве**             | ![Здраве](docs/screenshots/04-health.png)                |
| **Приеведател**        | ![Приеведател](docs/screenshots/05-translator.png)       |
| **Наличи настройки**   | ![Наличи настройки](docs/screenshots/06-settings.png)    |
| **Инструменти за CLI** | ![Инструменти за CLI](docs/screenshots/07-cli-tools.png) |
| **Изходни лози**       | ![Изходни](docs/screenshots/08-usage.png)                |
| ** Края точки**        | ![Края точки](docs/screenshots/09-endpoint.png)          |

</details>

---

### 🤖 Free AI Provider за Вашите любими програми за програмиране

_Намери която Ai-jак потовно IDE или CLI инструмент през OmniRoute — безплатен
API gateway за безкрайно programиране._

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

<sub>📡 Всички агенти се свързват през <code>http://localhost:20128/v1</code> или
<code>http://cloud.omniroute.online/v1</code> – един конфигурация, безкрайни
модели и квота</sub>

---

## 🤔 Защо OmniRoute?

**Запомнини да не губиш пари и грешното ограничаване:**

- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Квотата за абонамента изтича неназначена всеки месец
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Лимитите на цената те спрат сред програмирането
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Държавните API ($20-50/month per провайдър)
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Ръчно мъркане между провайдъри

**OmniRoute решава това:**

- ✅ **Максимизирай абонаментите** – monitor квотата, използвай всяка грамата
  преди reset
- ✅ **Автоматично fallback** – Abonent → API Key → Cheap → Free, zero down time
- ✅ **Multi-account** – circle robin между акунти per провайдър
- ✅ **Universal** – Работи с Claude Code, Codex, Gemini CLI, Cursor, Cline,
  OpenClaw,всякакви_CLI tool

---

## 📧 Поддръжка

> 💬 **Приєднайте се към нашата общност!** [WhatsApp
> Group](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t) – Получете
> помощ, споделете съвети и останете актуален

- **Вебстайтове**: [omniroute.online](https://omniroute.online)
- **Гитхаб**:[github.com/diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute)
- **Проблеми**:
  [github.com/diegosouzapw/OmniRoute/issues](https://github.com/diegosouzapw/OmniRoute/issues)
- **Whatsapp**: [Community
  Group](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)
- **Принос**: Вижте [CONTRIBUTING.md](CONTRIBUTING.md), отворете PR или
  избравте[ X65X ][good first issue`
- **Оригинален Проект**: [9рутер от деколуа](https://github.com/decolua/9router)

### 🐛 Отчет на Бага?

При създаването на проблема, моля, изпращате систем-инфо командата и прикрепите
генерираното файл:

```bash
npm run систем-инфо
```

Това генерира `систем-инфо.txt` с вашата версия на Node.js, версия на OmniRoute,
детайли на операционната система, инсталирани CLI команди (iflow, gemini,
claude, codex, antigravity, droid и т.н.), статус на Docker/PM2, системни пакети
и всичко онова, нужно за бързо възпроизвеждане на проблема. Прикрепете файла
директно към проблем в GitHub.

---

## Как работи

```
┌─────────────┐
│  Твоят CLI   │  (Claude Code, Codex, Gemini CLI, OpenClaw, Cursor, Cline...)
│   Уред      │
└──────┬──────┘
       │ http://localhost:20128/v1
       ↓
┌─────────────────────────────────────────┐
│           OmniRoute (Умна Рутер)        │
│  • Преобразуване на формат (OpenAI ↔ Claude) │
│  • Monitoring на квоти + Embeddings + Images │
│  • Автоматично обновяване на токенове │
└──────┬──────────────────────────────────┘
       │
       ├─→ [Tier 1: ПОДПИСКА] Claude Code, Codex, Gemini CLI
       │   ↓ квота изчерпана
       ├─→ [Tier 2: АПИ КЛЮЧ] DeepSeek, Groq, xAI, Mistral, NVIDIA NIM и т.н.
       │   ↓ лимит на бюджета
       ├─→ [Tier 3: БИЖНО] GLM ($0.6/1M), MiniMax ($0.2/1M)
       │   ↓ лимит на бюджета
       └─→ [Tier 4: БЕЗПЛАЩЕН] iFlow, Qwen, Kiro (без ограничения)

Резултат: Никога да не спиеш, минимален излишек от пари
```

---

## 🎯 Що OmniRoute Вижда срещу – 30 реални проблеми и употреби

> **Всеки разработчик, използващ AI инструменти, среща тези проблеми
> ежедневно.** OmniRoute е създаден, за да реши всички тях – от излишъци на пари
> до регионални блокове, от пречуплени OAuth протоци към протоколи за наблюдение
> и предприемачески наблюдаване.

<details>
<summary><b>💸 1. "I pay for an expensive subscription but still get interrupted by limits"</b></summary>

Разработчиците плащат 20–200 долара на месец за Claude Pro, Codex Pro или GitHub
Copilot. И също така, квотата има ограничение – 5 часа на използване, седмичен
лимит или лимит на потребени минути. Сред сесията на писане, провайдъра спира да
отговаря и разработчикът губи протокола и ефективността.

**Както OmniRoute решава това:**

- **Базиран на умно fallback system** — Ако квотата за подписка спира да
  функционира, автоматично преминава към АПИ КЛЮЧ → БИЖНО → БЕЗПЛАЩЕНО без
  въздействие от ръка
- **В реално време отслежване на квоти** — Показва потребеният token в реално
  време с гумен countdown (5h, дневен, седмичен)
- **Подподкрепа за множество сметки** — Подсметки за множество провайдъра с
  автоматично кръгово затваряне — когато едната спира да функционира, преминава
  към другата
- **Personalni комбинации** — Самоусъвършителни fallback вериги с 6 стратегии за
  балансиране (първоначално запълвате, кръгово затваряне, P2C, случайно,
  най-малките използвани, оптимизирано по затрябващи)
- **Monitoring на квоти за бизнес за Codex** — Monitoring на квоти за бизнес
  спрямо заишн на бизнес/Създадено в Тима справка директно в пилот таблици

</details>

<details>
<summary><b>🔌 2. "I need to use multiple providers but each has a different API"</b></summary>

OpenAI ползва един формат, Claude (Anthropic) другият, Gemini и другите пак. Ако
един разработчик иска да тества моделите от различни провайдъри или fallback
между тях, трябва да пре-соединит SDK-итe, да сменят иенда за достъп, да се
справят със самостоятелния формат. Външни предоставители (FriendLI, NIM) имат
разходна структура на модели за конзолиране.

**Както OmniRoute решава това:**

- **Единен точак за достъп** — Висококачествена `http://localhost:20128/v1` за
  да се използва като прокси за всички 67+ провайдъри
- **Преобразуване на формат** — Автоматично и транспарентно: OpenAI ↔ Claude ↔
  Gemini ↔ API на респонсите
- [Razreshvane na sanitizaciq na otgovor**] — Otriče neprijatelstveni polja
  (`x_groq`, `usage_breakdown`, `service_tier`) koito lomjavat OpenAI SDK v1.83+
- [ Normalizacija na vloga**] — Prevede `developer` → `system` za non-OpenAI
  provideri; `system` → `user` za GLM/ERNIE
- [Ekstrakciq na tag na Think**] — Izvadja `<think>` blokova от моделите като
  DeepSeek R1 в standardizirani `reasoning_content`</think>
- [Strukturni izhod za Gemini**] — `json_schema` →
  `responseMimeType`/`responseSchema` automatska преTransition
- ['stream' по подразбиране e 'false' **] — Coordinirata s OpenAI spec, evitajqi
  neizchektani SSE в Python/Rust/Go SDK-ove

</details>

<details>
<summary><b>🌐 3. "My AI provider blocks my region/country"</b></summary>

Providerite като OpenAI/Codex блокиран достъп от определени географични региони.
Изнайдетитe грешки като `unsupported_country_region_territory` по време на OAuth
и API свързания. Това е особено безнадежно за създатели от развиващи се държави.

**Както OmniRoute решава това:**

- [Konfiguracija на 3-нивиен прокси**] — Настройка на прокси на трите нива:
  глобален (всички трафик), на ниво на потребител (само на една потребителска
  услуга) и на ниво на връзка/чип
- [Kраен с цветни етикетки**] — Виждими индикатори: 🟢 глобален прокси, 🟡
  потребителски прокси, 🔵 връзъчна установка, винаги показва IP адреса
- [Обмен на token OAuth чрез прокси**] — token OAuth flow също става през
  проксия, решавайки проблемите `unsupported_country_region_territory`
- [Тестове на връзката чрез прокسی**] — Тестовете на връзката използват
  настроените проксита (не така директното еклипсаене)
- Поддръжка на SOCKS5**] — Пълна поддръжка на SOCKS5 прокси за изходен трафик
- [Побъркане на TLS fingerprint**] — Browser-like TLS fingerprint чрез `wreq-js`
  за избягване на детекцията на ботове
- [Скрийнсайтинг чрез КЛАЙМИТАР на CLI**] — Премахва главите и полетата от
  тялото на заявката за съответствие с клиентските API, понижавайки риска от
  блокиране на профила

</details>

<details>
<summary><b>🆓 4. "I want to use AI for coding but I have no money"</b></summary>

Не всеки може да плати 20–200 / месец за поддръжка на AI. Студенти, разработчици
от развиващи се държави, хобиити и свободни професионалисти изпитват нужда да
acces към висококачествените модил на zereo стойност.

**Както OmniRoute решава това:**

- [Модели за вградена бесплатна поддръжка**] — Текуща поддръжка за 100%
  безплатни provider: iFlow (5 безплатни модели по OAuth: kimi-k2-thinking,
  qwen3-coder-plus, deepseek-r1, minimax-m2, kimi-k2), Qwen (4 безплатни модели:
  qwen3-coder-plus, qwen3-coder-flash, qwen3-coder-next, vision-model), Kiro
  (Claude + AWS Builder ID за безплатна поддръжка), Gemini CLI (180K token /
  месец безплатно )
- [Област за хранене в облако**] — Cloud-hosted Ollama модели в `api.ollama.com`
  с безплатен ниво ' Light usage'; ползвайте префикса
  `ollamacloud/<model>`</model>
- [Комбиниране само с безплатни модели**] — Свързване на `gc/gemini-3-flash →
  if/kimi-k2-thinking → qw/qwen3-coder-plus` = безплатен месечен биланс без
  прекъсвания
- [Бесплатно достъп до NVIDIA NIM**] — ~40 RPM безплатен достъп до 70+ модел в
  build.nvidia.com (преход от кредита кърата храненост)
- Стратегия за оптимизираност на стойностите на СТРАНГА **СТРАНГА** — routing
  стратегия, която автоматично избира най-евтина достъпна провайдър

</details>

<details>
<summary><b>🔒 5. "I need to protect my AI gateway from unauthorized access"</b></summary>

При използване на AI gateway във мрежата (LAN, VPS, Docker), всяка лиценз за
потребление на потребителя може да получи достъп до token-ите/квотите на
разработчика. Без защита, апи серверните са на рисък от злоупотреби, инжуки за
стимул на реч, и злоупотреби.

**Както OmniRoute решава това:**

- **Управление за API ключове** — Generations per provider with scoping
  dashboard/api-manager` съсърмер
- **Уровен за позволение на модели** — Задържаните API ключове до конкретните
  модели (`openai/*`, wildcard patterns), с пултел за разрешаване или закъснение
- **Защита на API endpoint** — Изисква ключ за достъп за `/v1/models` и забрана
  на достъп за конкретни провайдър
- **Припрат и защита с CSRS** — Всяки routes за dashboard натюрщи с `withAuth`
  middleware + CSRF tokens
- **Rate limiter** — Limitiranе на потреблението на IP
- **Филтриране на IP** — позволит за блокиране или позволяване за достъп
- **Припрат за.inject на стимул на реч** — Санитация срещу оповестявания за
  злоупотреби
- **AES-256-GCM ENCRIPTION** — Кредетали шифрани във репо със съвърмерно

</details>

<details>
<summary><b>🛑 6. "My provider went down and I lost my coding flow"</b></summary>

Услужители за AI може да станат нестабилни, да връщат 5xx грешк или да изпадат в
непостоянство на времето. Ако разработчик съизползва провайдърите със едно, се
появяват проблемите. Без брейкаутър, повторени опити за достъп ще причинят
разкъсване.

**Както OmniRoute решава това:**

- **Брейкаутър по модели** — Авт. откриване/закриване, с конфигуративните
  порогове и периоден съвърмер
- **Постепенно нарастваща продължителност** — Денови опити за възстановяване със
  прогресивни задождявания
- **Бара да бъде сваляно от стража** — Мюхтес + семафороден пазар против
  снимките злоупотреби
- **Множен fallback съедиѝи** — Ако основният провайдър се уврежда, да се
  премести съюза в касово като
- **.Combo брейкаут съедиѝи** — Авт. изключване на провайдърите съвета в
  съедиѝита касково
- **Демонстрационно дисплеи на здравето** — Упрощаване на достъпните
  статистически данни, брейкаут съведености, блоки на отсъствие, статистика за
  кеша, първо 50%, 95%, 99%

</details>

<details>
<summary><b>🔧 7. "Configuring each AI tool is tedious and repetitive"</b></summary>

Разработчиките използват Cursor, Claude Code, Codex CLI, OpenClaw, Gemini CLI,
Kilo Code... Всяко свое изделие има различна конфигурация (АПИ ендпоитот,
ключове, модели). Следващо конфигурирайки при претражване на провайдъра или
модела е излишен проблем със съвърмер.

**Както OmniRoute решава това:**

- **Панел за инструменти CLI** — Дediciran съветен екран за еднократно
  подготвяване за Claude Code, Codex CLI, OpenClaw, Kilo Code, Antigravity,
  Cline
- **Конфигуриратор на GitHub Copilot** — Generira `chatLanguageModels.json` за
  VS Code с масова селекция на модели
- **Упателният водач за записване** — Управляем 4-стъпково подготвяне за първи
  пълнолетен потребител
- **Една точка за всички модели** — Конфигурирайте `http://localhost:20128/v1`
  веднъж, за да получите достъп до 67+ провайдъра

</details>

<details>
<summary><b>🔑 8. "Managing OAuth tokens from multiple providers is hell"</b></summary>

Claude Code, Codex, Gemini CLI, Copilot — всички използват OAuth 2.0 със
експирайващи потвърждения. Разработчици се налага да изпълняват повторно
аутентикация постоянно, да се справят с `мислището за клиентска секритна дума`,
`съвпадението на релайзаURI`, и неуспехите на отдалечени сървъри. OAuth в
LAN/VPS е особено проблематично.

**Както OmniRoute решава това:**

- **Автоматично препращане на потвърждение** — Потвърдителните знаци на OAuth се
  актуализират в заден план преди изтичането им
- **Съвместна аутентикация OAuth 2.0 (PKCE)** — Автоматична връзка за Claude
  Code, Codex, Gemini CLI, Copilot, Kiro, Qwen, iFlow
- **Множествено-accoнта в системата OAuth** — Множество счета зад уеб провайдъра
  чрез извличане JWT/ID токена
- **Приватно решение за аутентикация OAuth** — Детекция на личната IP адреса за
  `реляса URI` + ръчен мод за отдалечени сървъри
- **Решение за конфигуриране на аутентикация OAuth зад Nginx** — Използва
  `window.location.origin` за съвместимост с обратен прокс
- **Упателна статия за аутентикация OAuth отдалечно** — Стъп- по-стъп стойностна
  практика за настройването на сървъри Google Cloud на VPS/Docker

</details>

<details>
<summary><b>📊 9. "I don't know how much I'm spending or where"</b></summary>

Разработчиците използват множество платени провайдъра, но нямат обединен поглед
и трошковата им. Каждият провайдър има свои платен ефирна панел, но тази е
единственият. Негативни трошкови безвозвратно наслоят.

**Както OmniRoute решава това:**

- **Панела за анализа на трошковите** — Тръкване на трошките и управление на
  бюджета във всякакъв уеб провайдър
- **Плъзнитлената седловка на бюджета по тир** — Седловка върху наложените
  трошкови по every tier
- **Конфигуриране на цената за модели** — Конфигурийте цената на модела
- **Статистика на използваните модел** — Счетане на използваните заявки и
  последната използвана дата за уеб ключа
- **Панел за анализа** — Карти и успехови статистики за услугата и стойностите
  със задно време

</details>

<details>
<summary><b>🐛 10. "I can't diagnose errors and problems in AI calls"</b></summary>

==WEBLATE_PART==\
Если извикването на извикване е фалило, разработчика не известява дали причината
е лимит за скорост, изтекъл токен, грешка в формата или грешка на провайзъруто.
Разкъсаните дневници с различни терминали. Без наблюдение, дебъгването е проб и
погибел.

**Както OmniRoute решава това:**

- **Обединени Лози за Мониторинг** — 4 глави: Пулитен Дневник, Прокси Дневник,
  Наблюдателен Дневник, Конзолен Девайс
- **Представител за Конзолен Дневник** — Реално врееме, терминално представител
  с цветов за ниво, аутоскоролинг, търсене, филтриране
- **SQLite Дявник на Проксираща Система** — Съществувайки дневници, които
  издържат перезаваряване на сървъра
- **Айгледжи за Преход на Език** — 4 мода за дебагване: Поле за Игре
  (представяне на преход на език), Поглед с Хат (обратна връзка), Пътека за Тест
  (серия), Жив Ключник (реално врееме)
- **Телеметрия за Извиквания** — п50/п95/п99 злополучие + следиране
  X-Резолютна-Идентификатор
- **Файлово-основанът Логически Дневник с Ротация** — Конзолен представител
  капитурва съществувайки JSON дневник с ротация по потребителска база
- **Справочник за Системата** — `npm скарти сървис-инфо` генерира
  `система-инфо.txt` с цяла среда (версия на Node,, версия на Omiroute,
  операционна система, инструменти за CLI, статус на Docker\PM2). Добавете го
  когато отчетвайте проблеми за тотошния триаж.

</details>

<details>
<summary><b>🏗️ 11. "Deploying and maintaining the gateway is complex"</b></summary>

Установяване, конфигуриране и поддържане на аи-прокси в различни среди (локална,
VPS, Docker, облако) е тежко. Проблеми като-hardcoded пътища, `EACCES` в
директории, конфликти между портове, и крос-платформен билд добавят вълнение.

**Както OmniRoute решава това:**

- **Установяне на npm global** — `npm инсталиране -г -омнироути &amp;&amp;
  навигатор на Omiroute` — дело е завършено
- **Docker Multi-Platform** — AMD64 + ARM64 native (Apple Silicon, AWS Graviton,
  Raspberry Pi)
- **Docker Compose Profiles** — `base` (без инструменти за CLI) и `cli` (с
  Claude Code, Codex, OpenClaw)
- **Electron Desktop App** — Нативно приложение за Windows/macOS/Linux с
  системна тряба, саморазтегляне, режим offline
- **Разделен Режим(X17X) — API и Конзолен Девайс на раздели портове за
  изкуствени сценарии (ревърс-прокси, контейнерен мрежов)
- **Режим за Плънка в Облака** — Синхронизация на конфигурации между устройства
  чрез Cloudflare Raboki
- **Режим за Запазване на БД** — Автоматично запазване, възстановяване, експорт
  и импорт на всички настройки

</details>

<details>
<summary><b>🌍 12. "The interface is English-only and my team doesn't speak English"</b></summary>

Тимове в държави където не се говори езиково на английски, особено в Латинска
Америка, Азия и Европа, имат проблеми с английските интерфейси. Следните бариери
намаляват приците и увеличават грешките при конфигурнирането.

**Както OmniRoute решава това:**

- **Панел за дисплей i18n — 30 езика** — Всички 500+ ключове преведени,
  включително арабски, български, датски, германски, испански, фински, френски,
  еврейски, хинди, унгарски, индонезийски, италиански, японски, корейски,
  малайски, нидерландски, норвежки, полски, португалски (PT/BR), румънски,
  руски, словашки, шведски, тайски, украински,вьетнамски, китайски, филипински,
  английски
- **RTL Поддръжка** — Поддръжка за правоСлъвска писменост за арабски и еврейски
- **Многоезични README** — 30 пълни документирани превода
- **Seletor за езици** — Иконка „Глобус“ в главна настройва на лицето за реално
  вреъме съблекане

</details>

<details>
<summary><b>🔄 13. "I need more than chat — I need embeddings, images, audio"</b></summary>

Инженерите не са само за хълковане. Те трябва да генерират изображения,
транскрибират език, създават отражения за RAG, поновявт документите, и правят
съдържание по-сигурното. Къдя АПИ има различни точки от стартове и формат.

**Както OmniRoute решава това:**

- **Отражения** — /v1/embeddings` с 6 провайдер и 9+ модел
- **Генерация на Изображения** — /v1/images/generations` с 10 провайдер и 20+
  модел (OpenAI, xAI, Together, Fireworks, Nebius, Hyperbolic, NanoBanana,
  Antigravity, SD WebUI, ComfyUI)
- **Текст-Джинаерация на Видео** — /v1/videos/generations` — ComfyUI
  (AnimateDiff, SVD) и SD WebUI
- **Текст-Джинаерация на Музика** — /v1/music/generations` — ComfyUI (Stable
  Audio Open, MusicGen)
- **Транскрибировка на Аудио** — /v1/audio/transcriptions` — Whisper + Nvidia
  NIM, HuggingFace, Qwen3
- **Текстъръзползватели Текст–на-Глас** — /v1/audio/speech` — ElevenLabs, Nvidia
  NIM, HuggingFace, Coqui, Tortoise, Qwen3, **Inworld**, **Cartesia**,
  **PlayHT**, + съществуващи провайдер
- **Промитания** — /v1/moderations` — Съдържание на сигурнотсти
- **Реранкира** — /v1/rerank` — Реранкира на документи на съдържание
- **Отвечения API** — Пълна /v1/responses` поддръжка за Codex

</details>

<details>
<summary><b>🧪 14. "I have no way to test and compare quality across models"</b></summary>

Инженерите искат да знаят, кой модел е най-добър за техния случай на използване
— код, превод, изчисления — но сравнителното изпълнение бързо. Няма интегрирана
оценка.

**Както OmniRoute решава това:**

- **Оценки на LLM** — Златните случаи от тестване с 10 предназначени случаи
  обхващат приветствия, математика, география, код генерация, ЮSON, превод,
  маркирани, отхвърлитя съдържание за сигурнотти
- **4 Стратегии за съответствие** — ,`точен`, `содържание`, `регекс`,
  `произвольни`, (JS функция)
- **Игрище за Преводач** — Бизнес преводилник с масови входове и очаквани
  резултата, съподоршкона сравнение
- Разширена чат тестяра ** -- Пълно затворно със визуално отражение
- [Live Monitor]** — Реално-временна струя на всички заявки, протичащи през
  прокси

</details>

<details>
<summary><b>📈 15. "I need to scale without losing performance"</b></summary>

След като броят на заявките засилява, без промена на същите въпроси те генерират
двойката разходи. Без единствено изпълнение, повтарящи се заявки троше
разпространение. Производителите имат да бъдат спазвани единични данъци за
връзки.

**Както OmniRoute решава това:**

- [Semantic Cache]** – Двуяркова промяна в цената и зад 延ение на кеша (сигнатурa
  + semantic) намалява разхода и задvigod
- [Request Idempotency]** – 5с защита на показване за идентични заявки
- [Rate Limit Detection]** – На единичния произвeдителски РПМ, минимален отстъп,
  и максимум за съвпадения запис
- [Editable Rate Limits]** — Променимите данни като дефолти при Настройки →
  Резилienza с предаващи се данни
- [API Key Validation Cache]** – Трият кеш за производителна перформанса
- [Health Dashboard with Telemetry]** – Latenciya p50/p95/p99, кеш статистика,
  пълна работност

</details>

<details>
<summary><b>🤖 16. "I want to control model behavior globally"</b></summary>

Разработчиките, които искат цялото съждение в даден език, със с предвидяне или с
поддръжка на допълнителни ресурси. Накладването на това в всеки
инструмент/заявка е наведнъчно немисливо.

**Както OmniRoute решава това:**

- [System Prompt Injection]** – Глобален предвидяне наложен на всички заявки
- [Thinking Budget Validation]** – Алокация на ресурс за съждение пер заявка
  (преход, авто, персонализирано, адаптивно)
- [6 Routing Strategies]** – Глобални стратегии, които определят кои заявки са
  рутвани
- [Wildcard Router]** – ` произвeдител.provider/*` шаблони рутват динамично до
  произвeдителтe
- [Combo Enable/Disable Toggle]** – Изключвате комбинацията директно от
  контролера
- [Provider Toggle]** – Включвате/исключвате съвмесимостта на поведения на
  произвeдителите с един щелк
- [Blocked Providers]** – Изключвате съвмесимостта на специфични произвeдителe
  от `/v1/models` списъка заяви

</details>

<details>
<summary><b>🧰 17. "I need MCP tools as first-class product capabilities"</b></summary>

Много АИ гейти exposing MCP само като секретен реализирування. Тъмниците за
източник на MCP имат да представят видимо, управляемо, операционно ниво.

**Както OmniRoute решава това:**

- Харесаеми конзола МСП използва се в навигацията на дейскапа и в тази на
  протокола за конечен брой
- Една специална страница за управление на МСП с процеси, инструменти, домени и
  аудира
- Вграден бърза старт за omniroute --mcp и клиентско въвождане

</details>

<details>
<summary><b>🧠 18. "I need A2A orchestration with sync + stream task paths"</b></summary>

Потребите на агентските събития включват както директните отговори, така и
дългосрочните потоци с етап контрола.

**Както OmniRoute решава това:**

- А2А JSON-RPC точка за крайна точка ([ТПОСТ /a2a] с [message/send] и
  [message/stream])
- Потокова потокова потокова транзакция с терминална предаване
- API-то за животнието на задълженията за работа за [tasks/get] и [tasks/cancel]

</details>

<details>
<summary><b>🛰️ 19. "I need real MCP process health, not guessed status"</b></summary>

Тимовете за експлоатация трябва да знаят, дали МСП съществува, а не само дали
API-то е достъпна.

**Както OmniRoute решава това:**

- Файл с бягане на работа в реално време с PID, маркировки, превоз, брой
  използвани инструменти и мод същност
- API-то за състоянието на MCP, което хибридира бягането на работа и недавната
  дейност
- Статусни карти на дейскапа за процес/възпиране/свежест на бегане на работа

</details>

<details>
<summary><b>📋 20. "I need auditable MCP tool execution"</b></summary>

Когато инструментите модифицират сефигурация или уреждат оперативно действие,
тимовете потребяват линейна следпаметност.

**Както OmniRoute решава това:**

- Аудира, поддръжана от SQLite, за извикванията към инструментите на МСП
- Филтри, удрождени по инструмент, успех/неуспех, ключ за API и страници за
  разчети
- Табелна за аудира на дейскапа и конечни точки за статистики за автоматизация

</details>

<details>
<summary><b>🔐 21. "I need scoped MCP permissions per integration"</b></summary>

Различни клиенти все пак трябва да имат наименително достъп до групите по
инструменти.

**Както OmniRoute решава това:**

- 9 дребни множества за контролиран достъп до мощен инструмент
- Навигация и видимост на MCP в управлящия интерфейс
- Безопасен по подразбиране на настройката на операционни инструменти

</details>

<details>
<summary><b>⚙️ 22. "I need operational controls without redeploying"</b></summary>

Кomitентите имат бързи промени на runtime по време на инциденти или събития със
затежение на стойността

**Както OmniRoute решава това:**

- Активиране на комбинираните надстройки direкто от dashboard на MCP
- Примена на профили на отражаване от предефинирани пакети с политика
- Избутване на състоянието на breaker за циркулация от същата пейна на операции

</details>

<details>
<summary><b>🔄 23. "I need live A2A task lifecycle visibility and cancellation"</b></summary>

Без визуализация на етапите, инцидентите на задачите стават трудни да се
трирате.

**Както OmniRoute решава това:**

- Сортиране и филтриране на задачата по състояние/умения със страница на
  интервализация
- Ръчен преглед на метаданни, събития и артефакти на задачата
- Пунеж на endpoint и UI на отмяна на задачата със потвърждение.

</details>

<details>
<summary><b>🌊 24. "I need active stream metrics for A2A load"</b></summary>

Текущите потоци изискват операционна видимост в конкуренция и на живи връзки.

**Както OmniRoute решава това:**

- Активни счетчики на поток в интегрирани в статус A2A
- Last данен за задача и посотискти спреженя
- Карти за dashboard A2A за реално време за мониторинг на операции

</details>

<details>
<summary><b>🪪 25. "I need standard agent discovery for clients"</b></summary>

Клиентите и на оркестраторите изискват машиночитими данни за въвеждане на
клиента.

**Както OmniRoute решава това:**

- Аджент карта излага се в `/.well-known/agent.json`
- Възможности и skills показват в управлевния интерфейс на управление
- Статус на A2A API включва разкрита информация за автоматизацията

</details>

<details>
<summary><b>🧭 26. "I need protocol discoverability in the product UX"</b></summary>

Ако потребителите не изобретат ендпоинтовите поверхности на протокола,
качеството на приятелите на сервиса и съпортата се намалява.

**Както OmniRoute решава това:**

- Консолидираната страница с ендпоинтови, с тabelle за Proxy, MCP, A2A и API
  Endpoints
- Активатори за онлайн/офилен статус на сервисите inline (Онлайн/Офライン) за MCP и
  A2A
- Сообщения, свързани с извеждането, водят до посочена мениджмънт табове

</details>

<details>
<summary><b>🧪 27. "I need end-to-end protocol validation with real clients"</b></summary>

Мок тества не се използват за валидация на съвместимостта на протокол за излиза
на услуга.

**Както OmniRoute решава това:**

- Пълна система, която започва приложението и използва реален клиент за
  транспорт на съобщения на MCP SDK
- Тествата клиентската A2A за изобретение, изпрощване, потека и заявки за
  стойност за потвърждение и за отменяне
- Кросовърките при извадени твръждения срещу MCP заявки и задачи A2A API

</details>

<details>
<summary><b>📡 28. "I need unified observability across all interfaces"</b></summary>

Разделяването на наблюдаването по протоколи създава слепота по място и по-дълъга
ВМТР.

**Както OmniRoute решава това:**

- Единни dashboard + лози/анализии на продуктите в едно произведение
- Здраве + аудира + попитите телеметрии в едно издание за продукта
- Оперативните api за статус и аутоматизация

</details>

<details>
<summary><b>💼 29. "I need one runtime for proxy + tools + agent orchestration"</b></summary>

Изпълнение на повече от един и същи сервис се повишава и по-задължителната
оперативния разход и случаите във фазата на ломеане.

**Както OmniRoute решава това:**

- Суъязан сървър за OpenAI, MCP сървър и A2A сървър в една стака
- Надяснено авторизация, резилienza, данни за хранене и наблюдаемост
- Еднолично политическо модело през цялото взаимодействие

</details>

<details>
<summary><b>🚀 30. "I need to ship agentic workflows without glue-code sprawl"</b></summary>

Тимовете губят скорост когато въвеждат няколко едноцилинни услуги и сценарии.

**Както OmniRoute решава това:**

- Еднолично стратегия за връзка с края за клиенти и агенти
- Вградени интерфейси за управление на протоколови и пътеки за изпитвания на
  дима
- Производствени съвместими основи (сигурност, логгироване, резилienza, защита)

</details>

### Примерни плејбуък (интегрирани случаи за използване)

**Плејбуък А: Максимизиране на заплащащите подписки + дълбока защита**

```txt
Combo: "maximize-claude"
  1. cc/claude-opus-4-6
  2. glm/glm-4.7
  3. if/kimi-k2-thinking

Месечен старт: 20 долара + малка тарифа за защита
Изход: по-високо качество, близък зазор за изключвания
```

**Плејбуък Б: Нулеви сметки за програмиране в стака**

```txt
Combo: "free-forever"
  1. gc/gemini-3-flash
  2. if/kimi-k2-thinking
  3. qw/qwen3-coder-plus

Месечен старт: 0 долара
Изход: съвместима с програмистко заявление
```

**Плејбуък С: 24/7 винаги в работа fallback верига**

```txt
Combo: "always-on"
  1. cc/claude-opus-4-6
  2. cx/gpt-5.2-codex
  3. glm/glm-4.7
  4. minimax/MiniMax-M2.1
  5. if/kimi-k2-thinking

Изход: дълбок fallback за строго настройки крайни срокове
```

**Плејбуък D: Съвместими операции със сървърите MCP + A2A**

```txt
1) Заряди MCP транспорта (`омнирута --mcp`) за инструмент-оориентирани операции
2) изпълни задачи за A2A чрез `предаване на съобщение` и `предаване на поток`
3) следи виртуалните таблоои (/dashboard/endpoint - MCP и A2A таблооии)
4) включи услугите чрез inline статусни контроли
```

---

## Инициирай Безплатно — Нулеви конфигурации за тариф

> Настрой влоговете на AI програмиране за минути 0 долара в **месечно място**.
> Присъединете тези бесплатни сметки и използвайте вградените **съвместими
> програмиране в стака** комбинации.

| Изпойвай следващият етап | Действие                                              | Разрешено приложение за провайдъри                                   |
| ------------------------ | ----------------------------------------------------- | -------------------------------------------------------------------- |
| 1                        | Вклъвай **Кириъ** (AWS Builder ID OAuth)              | Клод Сонет 4.5, Хаику 4.5 — **безограничен**                         |
| 2                        | Вклъвай **иФлоъ** (Google OAuth)                      | кими-к2-мисълен, qwen3-кодър-плюс, deepseek-r1... — **безограничен** |
| 3                        | Вклъвай **Qwen** (Device Code)                        | qwen3-кодър-плюс, qwen3-кодър-флаш... — **безограничен**             |
| 4                        | Включи **Гемини КЛИъ** (Google OAuth)                 | gemini-3-флаш, gemini-2.5-професионал — **180K/месеца безплатно**    |
| 5                        | `/dashboard/combos` → **Безплатна стака ($0)** шаблон | Ротация на всички безплатни провайдъри автоматично                   |

**Налагай любимата ВИ за:** `http://localhost:20128/v1` · API ключ:
`койсотвоено-стрингъсъ,X76X] · Готово.

> **Допитека приложение за покритие (не задължително и безплатно):** ключ за API
> на Groq (30 RPM безплатно), NVIDIA NIM (40 RPM безплатно, 70+ модели),
> Cerebras (1M токенове на ден), ключ за API на LongCat (50 милиона токенове на
> ден!), Cloudflare Workers AI (10K токенови ден, 50+ модели).

## Бърз старт

### 1. Инсталирайте и стартирайте

```bash
npm инсталирай -g omniroute
омнируте
```

> **pnpm потребители:** Изпълни `pnpm съгласува-изграждане -g` след инсталиране,
> за да активираш native скриптове за изграждане, изисквани от `better-sqlite3`
> и `@swc/core`:
> 
> ```bash
> pnpm инсталирай -g omniroute
> pnpm съгласува-изграждане -g   # Изберете всички пакети → съгласувай
> омнируте
> ```

Дashboard отваря се на `http://localhost:20128` и базовата URL на API-та е
`http://localhost:20128/v1`.

| Нареждане               | Описание                                                                     |
| ----------------------- | ---------------------------------------------------------------------------- |
| `омнируте`              | Почни уеб-сервер (вдъхновено от `PORT=20128`, API и Dashboard на същия порт) |
| `омнируте --порт 3000`  | Настрой фоки-порт на 3000                                                    |
| `омнируте --mcp`        | Почни MCP-сервер (stdio-транспорт)                                           |
| `омнируте --не-открива` | Не избирай се в някой браузър                                                |
| `омнируте --помощ`      | Покажи помощ                                                                 |

Допълнителен режим за разделяне на портове:

```bash
PORT=20128 DASHBOARD_PORT=20129 omniroute
# API:       http://localhost:20128/v1
# Dashboard: http://localhost:20129
```

### 1) Разкonnekцияни и създаване на твоичница

1. Отвори Дейскотоп — > `Повеќици` и сложи поне една повеќица (OAuth или
   тичница).
2. Отвори Дейскотоп — > `Крайни точки[X37X] и създай тичница (API).
3. (Затворено) Отвори Дейскотоп — > `Кораблетчета` и сложи fallback верига.

### 3) Покажи свой кодинг инструмент към OmniRoute

```txt
Основна база URL: http://localhost:20128/v1
Тичница (API):  [копирай от Краи точки]
Модел:  ако/kими-ки2-мислий (или какъвто и да е повеќи-на-модел префикс)
```

Функционира с Claude Code, Codex CLI, Gemini CLI, Cursor, Cline, OpenClaw,
OpenCode и OpenAI-коматибилни SDK-ове.

### 4) enabling и валидиране на протоколи (v2.0)

**МПС-Е (за инструмент-ориентирана работа): **

```bash
omniroute --mcp
```

Затим свържи МПС-Е клиент чрез `stdio` и тествай инструменти като:

- `omniroute_get_health`
- `omniroute_list_combos`

**А2А (за агент-агент програмиране): **

```bash
curl http://localhost:20128/.well-known/agent.json
```

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"quickstart","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"Give me a short quota summary."}]}}'
```

### 5) Валидиране на всичко от краен край (по избор)

```bash
npm run test:protocols:e2e
```

Този бенчмарк валидира реален МПС-Е и А2А клиентов скрещения с работаща
приложение.

### Замясто: работи от източник.

```bash
cp .env.example .env
npm install
PORT=20128 DASHBOARD_PORT=20129 NEXT_PUBLIC_BASE_URL=http://localhost:20129 npm run dev
```

---

## Докър

OmniRoute е достъпна под формата на обществено Докър изображение на [Docker
Hub](https://hub.docker.com/r/diegosouzapw/omniroute).

**Бързо стартиране:**

```bash
docker run -d \
  --name omniroute \
  --restart unless-stopped \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:latest
```

**С фаил с настройки:**

```bash
#\n Копирайте и редактирайте за пръв път .env\n#
docker run -d \
  --name omniroute \
  --restart unless-stopped \
  --env-file .env \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:latest
```

**С използване на Докър Къмпоз:**

```bash
#\n Профилът база (без инсталирани програми\n#
docker compose --profile base up -d

#\nКлиентския профил (Claude Code, Codex, OpenClaw build-int)\n#
docker compose --profile cli up -d
```

| Изображение              | Таг      | Размер  | Описание                   |
| ------------------------ | -------- | ------- | -------------------------- |
| `diegosouzapw/omniroute` | `latest` | ~250 MB | Последната стабилна версия |
| `diegosouzapw/omniroute` | `1.0.3`  | ~250 MB | Aktualna версия            |

---

## 🖥️ Десктоп приложение — Offline & Always-On

> 🆕 **НОВО** OmniRoute сега е достъпна като **начална десктоп приложенение** на
> Windows, macOS и Linux.

Използвайте OmniRoute като самостоятелно десктоп приложение – без терминал, без
връзка в интернет за локални модели. Апликацията, базирана на Electron, включва:

- 🖥️ **Нативна Вижина** – посветена приложителна Вижина с интеграция в системния
  куфар
- 🔄 **Автоматично Възпира** – стартирате OmniRoute на логин в системата
- 🔔 **Нативни Изключваня** – получавате известия за износкване на квота или
  проблеми с провайдъра
- ⚡ **Еднократно Инсталиране** – NSIS (Windows), DMG (macOS), AppImage (Linux)
- 🌐 **Арендов_MODE** – действа напълно без интернет с вграден сървър

### Бърз старт

```bash
# Разработъчно състояние
npm run electron:dev

# Сгради за вашата платформа
npm run electron:build         # Текуща платформа
npm run electron:build:win     # Windows (.exe)
npm run electron:build:mac     # macOS (.dmg) — x64 и arm64
npm run electron:build:linux   # Linux (.AppImage)
```

### Системен купер

Когато се минимизиращи, OmniRoute съществува в системния купер с бързи дейности:

- Отворете таблото за управление
- Смени сървърския порт
- Излез от приложението

📖 Цялата документация: [`electron/README.md`](electron/README.md)

---

## 💰 Сметка при поглед

| Тарифа                 | Provider                   | Сметка                                | Повторно префармуване на квота | Най-добре за теб                             |
| ---------------------- | -------------------------- | ------------------------------------- | ------------------------------ | -------------------------------------------- |
| [Х0Х]💳 АБОНAMENT[Х16Х] | Клауд Код (Про)            | $20/мес                               | 5h + седмично                  | Уже подписан                                 |
|                        | Кодекс (Плюс/Про)          | $20-200/мес                           | 5h + седмично                  | Използватели на OpenAI                       |
|                        | Gemini CLI                 | [Х0Х]_FREE[Х6Х]                       | 180K/мес + 1K/ден              | Всеки!                                       |
|                        | Копилот на GitHub          | $10-19/мес                            | Месечно                        | Използватели на GitHub                       |
| [Х0Х]🔑 КЛЮЧ ЗА АПИ**   | NVIDIA NIM                 | [Х0Х]_FREE[Х6Х] (development вечност) | 30 RPM                         | Премахнати над 70 модели                     |
|                        | Cerebras                   | **ЗАТВОРАВАНО** (1M ток/day)          | 60K TPM / 30 RPM               | Световен рекорднa по скорост                 |
|                        | Groq                       | **ЗАТВОРАВАНО** (30 RPM)              | 14,4K RPD                      | Ултра-бързи Llama/Gemma                      |
|                        | DeepSeek V3.2              | $0.27/$1.10 за 1M                     | Няма                           | Най-добро цено-качествено съODBрзяние        |
|                        | xAI Grok-4 Бавен           | **$0.20/$0.50 за 1M** 🆕               | Няма                           | Бавен + въвеждане на инструменти, ультралова |
|                        | xAI Grok-4 (стандарт)      | $0.20/$1.50 за 1M 🆕                   | Няма                           | Лидер за съODBрзяние от xAI                  |
|                        | Мистрал                    | Gratis пробно + платно                | Ограничена скорост             | Европейски АИ                                |
|                        | OpenRouter                 | Платен според използването            | Няма                           | 100+ модели агр.                             |
| ** 💰 ШИРОКИ💰 **        | GLM-5 (чрез Z.AI) 🆕        | $0.5/1M                               | Събота 10:00                   | 128К изход, новият флагмански                |
|                        | GLM-4.7                    | $0.6/1M                               | Събота 10:00                   | Бюджетна защита                              |
|                        | MiniMax M2.5 🆕             | $0.3/1M вход                          | 5-часовно въртене              | Откриващия + задачи на агентите              |
|                        | MiniMax M2.1               | 0,2$/1M                               | 5-часовно въртене              | Най-евтин вариант                            |
|                        | Kimi K2.5 (Moonshot API) 🆕 | Платен според използването            | Няма                           | Пряkelig вход до Moonshot API                |
|                        | Kimi K2                    | $9/mese фиксна цена                   | 10M токена/mese                | Предсказуема стойност                        |
| **🆓 ЗА СВОБОДА**       | iFlow                      | **$0**                                | Несъкновимо                    | 5 модели без限制                               |
|                        | Qwen                       | **$0**                                | Несъкновимо                    | 4 модели без ограничения                     |
|                        | Kiro                       | **$0**                                | Несъкновимо                    | Claude Sonnet/Haiku (AWS Builder)            |
|                        | LongCat Flash-Lite 🆕       | **$0** (50M tok/day 🔥)                | 1 РПС                          | Най-големият безплатен квота на Земята       |
|                        | Продължаващи AI            | **$0** (без ключ)                     | 1 запит/15с                    | GPT-5, Claude, DeepSeek, Llama 4             |
|                        | Cloudflare Workers AI      | **$0** (10K Неурони ден)              | ~150 отговора/ден              | 50+ модели, глобален ръчай                   |
|                        | Scaleway AI                | **$0** (1M вътрешни знака общо)       | Ограничена скорост             | EU/GDPR, Qwen3 235B, Llama 70B               |

> ** Добавени нови модели (**):** Grok-4 Бърз семейство за $0.20/$0.50/М (върху
> база 1143ms — 30% по-бавен от Gemini 2.5 Flash), GLM-5 чрез Z.AI с 128K изход,
> MiniMax M2.5 логика на съждението, DeepSeek V3.2 обновено ценообразуване, Kimi
> K2.5 чрез Moonshot директна API.

**💡 $0 comboСтак — Всички безплатно настройки:**

```
# 🆓 Ultimate безплатен Стак 2026 — 11 провайдъри, $0 Forever
Kiro (kr/)             → Клод Сонет/Хайку НЕОГРАНЕН
iFlow (if/)            → Кимик2.5-на мисленето,  qwen3-coder-plus, deepseek-r1 НЕОГРАНЕН
LongCat Lite (lc/)     → LongCat-Flash-Lite — 50M знака/ден 🔥
Pollinations (pol/)    → GPT-5, Клод, DeepSeek, Llama 4 — без ключ
Qwen (qw/)             → qwen3-coder-plus, qwen3-coder-flash, qwen3-coder-next НЕОГРАНЕН
Gemini (gemini/)       → Gemini 2.5 Flash — 1 500 запит/ден безплатен API ключ
Cloudflare AI (cf/)    → Llama 70B, Gemma 3, Mistral — 10K Неурони/ден
Scaleway (scw/)        → Qwen3 235B, Llama 70B — 1M безплатни знака (EU)
Groq (groq/)           → Llama/Gemma ускорен — 14.4K запит/ден
NVIDIA NIM (nvidia/)   → 70+ отворени модели — 40 RPM навеки
Cerebras (cerebras/)   → Llama/Qwen най-бърз — 1M знака/ден
```

** Zero затрат. Никога не спират кодирането.** Конфигурирай този като едно
OmniRoute комбо и всички fallback отива непринудително — никаква ръчна
премълчавка във всеки caso.

---

---

## 🆓 Безплатни модели — Може да получите нещо

> Всички модели по-долу са **100% безплатни с нула заявки потребителски карти**.
> OmniRoute изпраща автоматично между тях, когато съответнощ квота изтича —
> съединете ги на съчетавайте ги за неотриваем комбо на $0.

### 🔵 КЛУД MODEЛЯ (чрез КIRO — AWS стройчик ID)

| Модел                      | Префикс       | Граница         | Лимит на скоростта                 |
| -------------------------- | ------------- | --------------- | ---------------------------------- |
| [U0U]Klaud-sonet-4.5[U18U] | [U0U]кр/[U4U] | Без ограничения | Няма съобщавано дnevno oграничение |
| [U0U]Klaud-haiku-4.5[U17U] | [U0U]кр/[U4U] | Без ограничения | Няма съобщавано дnevno oграничение |
| [U0U]Klaud-опус-4.6[U16U]  | [U0U]кр/[U4U] | Без ограничения | Най-новия Opus чрез Киро           |

### 🟢 Режим на Kлауд модели (Безплатен авторизация — Безвкусна Кредитна карта)

| Модел                       | Префикс       | Граница         | Лимит на скоростта            |
| --------------------------- | ------------- | --------------- | ----------------------------- |
| [U0U]кими-к2-mышление[U17U] | [U0U]if/[U4U] | Без ограничения | Няма допълнителна ограничение |
| qwen3-coder-plus            | [U0U]if/[U4U] | Без ограничения | Няма допълнителна ограничение |
| deepseek-r1                 | [U0U]if/[U4U] | Без ограничения | Няма допълнителна ограничение |
| minimax-m2.1                | [U0U]if/[U4U] | Без ограничения | Няма допълнителна ограничение |
| kimi-k2                     | [U0U]if/[U4U] | Без ограничения | Няма допълнителна ограничение |

### 💛 МОДЕЛИ QWEN (Контактно-поръчнопредприятие)

| Модел             | Префикс | Граница         | Лимит на скоростта            |
| ----------------- | ------- | --------------- | ----------------------------- |
| qwen3-coder-plus  | qw/     | Без ограничения | Няма допълнителна ограничение |
| qwen3-coder-flash | qw/     | Без ограничения | Няма допълнителна ограничение |
| qwen3-coder-next  | qw/     | Без ограничения | Няма допълнителна ограничение |
| Модел на визия    | qw/     | Без ограничения | Мултимодална (снимки)         |

### 🟣 CLI ГЕМИНИ (Google OAuth)

| Модел                            | Префикс | Граница                      | Лимит на скоростта |
| -------------------------------- | ------- | ---------------------------- | ------------------ |
| `Gemini-3-фаиловото-преди-превю` | `gc/`   | **180K token/mese** + 1K/den | Месечен сблъсък    |
| `gemini-2.5-официален`           | `gc/`   | 180K/месец (Споделена пул)   | Висока качество    |

### Нерисовките NVIDIA NIM (Нebо API Key — build.nvidia.com)

| Тарифа      | Дневен лимит              | Лимит на скоростта | Бележки                                                       |
| ----------- | ------------------------- | ------------------ | ------------------------------------------------------------- |
| Небен (Dev) | Без ограничения за токени | **~40 RPM**        | 70+ модели; достъп до чисти пределите през средата на 2025 г. |

Популярни безплатни модели: `moonshotai/kimi-k2.5` (Kimi K2.5), `z-ai/glm4.7`
(GLM 4.7), `deepseek-ai/deepseek-v3.2` (DeepSeek V3.2),
`nvidia/llama-3.3-70b-instruct`, `deepseek/deepseek-r1`

### Нерисовките CEREBRAS (Нebо API Key — inference.cerebras.ai)

| Тарифа    | Дневен лимит           | Лимит на скоростта | Бележки                                                |
| --------- | ---------------------- | ------------------ | ------------------------------------------------------ |
| безплатно | **1М дана tokens/day** | 60K TPM / 30 RPM   | Световният най-бърз инференция на LLM; resetира събота |

Наличен безплатно: `llama-3.3-70b`, `llama-3.1-8b`,
`deepseek-r1-distill-llama-70b`

### 🔴 GROQ (Безплатна API ключ — console.groq.com)

| Тарифа    | Дневен лимит  | Лимит на скоростта | Бележки                                              |
| --------- | ------------- | ------------------ | ---------------------------------------------------- |
| безплатно | **14.4K RPD** | 30 RPM за модел    | Няма кредитна карта; 429 на лимит, не взимат платени |

Наличен безплатно: `llama-3.3-70b-versatile`, `gemma2-9b-it`, `mixtral-8x7b`,
`whisper-large-v3`

### 🔴 LONGCAT AI (Безплатна API ключ — longcat.chat) 🆕

| Модел                                   | Префикс | Дnevna безплатна квота | Бележки                          |
| --------------------------------------- | ------- | ---------------------- | -------------------------------- |
| `Дългата Мачка-Петля-Лайт`              | ` lc/`  | ** 50M токена** 💥      | Най-голяма безплатна квота икога |
| ` Дългата мачка-Петля-Чат`              | ` lc/`  | 500K токена            | Мултиターн чат                     |
| ` Дългата мачка-Петля-Разсъждение`      | ` lc/`  | 500K токена            | Реализация / CoT                 |
| ` Дългата мачка-Петля-Разсъждение-2601` | ` lc/`  | 500K токена            | Версия от януари 2026 г.         |
| ` Дългата мачка-Петля-Омни-2603`        | ` lc/`  | 500K токена            | Мултимодален                     |

> 100% безплатен по време на публичен бета етап. Регистрирайте се на
> [longcat.chat](https://longcat.chat) с имейл или телефон. Обновяване на
> квотата всеки дневен 00:00 UTC.

### 🟢 ПОЛИНАЦИИ АИ (Без потребителски ключ, потребен) 🆕

| Модел      | Префикс | Лимит на скоростта | Създател зад гръб  |
| ---------- | ------- | ------------------ | ------------------ |
| `openai`   | `пол/`  | 1 запит/15с        | GPT-5              |
| `claude`   | `пол/`  | 1 запит/15с        | Антropic Claude    |
| `gemini`   | `пол/`  | 1 запит/15с        | Google Gemini      |
| `deepseek` | `пол/`  | 1 запит/15с        | DeepSeek V3        |
| `lldma`    | `пол/`  | 1 запит/15с        | Meta Llama 4 Scout |
| `mistral`  | `пол/`  | 1 запит/15с        | Мистрал АИ         |

> ✨ ** Zero тег: ** Изрично: Вход със потвърждение, ни кой API ключ. Добавете
> услуга Pollinations с празно поле за ключ и тя започва да работи на миг.

### 🟠 КЛАУДФЛОР УРКЕР УАЙ (Бесплатен API ключ — cloudflare.com) 🆕

| Тарифа    | Дневни Neuroscience | Недопълнителна употреба                     | Бележки                           |
| --------- | ------------------- | ------------------------------------------- | --------------------------------- |
| безплатно | 10,000              | ~150 ЛМ олимпия / 500с аудии / 15К елементи | Глобална крайна точка, 50+ модели |

На популярените безплатни модели: `@cf/meta/llama-3.3-70b-instruct`,
`@cf/google/gemma-3-12b-it`, `@cf/openai/whisper-large-v3-turbo` (всъщност
безплатен аудий!), `@cf/qwen/qwen2.5-coder-15b-instruct`

> Трябва да е информиран API Token + Account ID от
> [dash.cloudflare.com](https://dash.cloudflare.com). Разположете Account ID в
> настройките на провайдъра.

### 🟣 ИНФОРМАЦИОННОЕ СУПЕРИОРНОСТИ НА СКОЛ (10M Безплатни Кредитна карта — scaleway.com) 🆕

| Тарифа    | Безплатна квота   | Място        | Бележки                                    |
| --------- | ----------------- | ------------ | ------------------------------------------ |
| безплатно | 10 mилиона токена | 🇫🇷 Париж, ЕС | Няма потребност от кредитна карта в лицата |

Базирана на API достъпна за безплатно: `qwen3-235b-a22b-instruct-2507` (Qwen3
235B!), `llama-3.1-70b-instruct`, `mistral-small-3.2-24b-instruct-2506`,
`deepseek-v3-0324`

> EU/GDPR съответстъвност. Получете API ключа на
> [console.scaleway.com](https://console.scaleway.com).

> 💡 Всенародно безплатно разширение на фундаменталитетите (11 Функции Сътрудника
> – $0 Вечно):**
> 
> ```
> Кирил (kr/)             → Claude Сонет/Хаику БЕЗГРАНИЦНО
> иФлоу (if/)            → кими-ки2-мисъл, qwen3-кодер-плюс, deepseek-r1 БЕЗГРАНИЦНО
> Дългата Съiska Lite (lc/) → Дългата Съiska-Лайт — 50M токени/ден 🔥
> Полинации (pol/)    → GPT-5, Клод, DeepSeek, Llama 4 — без ключ
> Qwen (qw/)             → qwen3-кодер модели БЕЗГРАНИЦНО
> Гемини (gemini/)       → Гемини 2.5 Лайт — 1 500 req/ден безплатно
> Cloudflare AI (cf/)    → 50+ модели — 10K Неврони/ден
> Scaleway (scw/)        → Qwen3 235Б, Llama 70Б — 1M безплатни токени (EU)
> Groq (groq/)           → Llama/Гемма — 14.4K req/ден超-бързо
> NVIDIA NIM (nvidia/)   → 70+ отворени модели — 40 RPM навеки
> Cerebras (cerebras/)   → Llama/Qwen световно-бързо — 1M ток/ден
> ```

## 🎙️ Бесплатно transcription комбо

> Претоварявайте каквито и дълбочина за **$0** — Deepgram води с $200 бесплатно,
> AssemblyAI $50 fallback, Groq Whisper като безграничен еквипиров backup.

| Provider         | Безплатни кредити           | Най-добрият модел                              | Лимит на скоростта                                |
| ---------------- | --------------------------- | ---------------------------------------------- | ------------------------------------------------- |
| 🟢 **Deepgram**   | **$200 бесплатно** (signup) | `nova-3` — най-висока точност, 30+ езици       | Не е ограничено при ползване на безплатни кредити |
| 🔵 **AssemblyAI** | **$50 бесплатно** (signup)  | `universal-3-pro` — главна части, мненипе, ПИI | Не е ограничено при ползване на безплатни кредити |
| 🔴 **Groq**       | **Всегда безплатно**        | `whisper-large-v3` — OpenAI Whisper            | 30 RPM (ограничено с регистрачка)                 |

**Поръчително комбо в `/dashboard/combos`:**

```
Име: free-transcription
Стратегия: Приоритет
Ноди:
  [1] deepgram/nova-3          → използва $200 бесплатно първо
  [2] assemblyai/universal-3-pro → fallback когато Deepgram кредитите изтичат
  [3] groq/whisper-large-v3    → бесплатно навеки, еквипиров backup.
```

Тогава в /dashboard/media` → Media**Transcription** таб: Uploadай качеството си
на аудио или видефайл → изберете конекшън на вашата комбо → получете
транскрипция в поддържани формати.

## 💡 Главни функции

OmniRoute v2.0 е постройен като операционна платформа, а не само като релейний
прокси.

### 🆕 Новите – вдъхновени от ClawRouter подобрения (март 2026)

| Функция                                       | Що е то                                                                                                     |
| --------------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| ⚡ **Grok-4 Бърз Фамилия**                     | xCибер-интелектуални модели от $0.20/$0.50/M — мерени 1143ms (30% бързо от Gemini 2.5 Флаш)                 |
| 🧠 **GLM-5 чрез Z.AI**                         | 128K изходен контекст, $0.5/1M — най-новия флагман от бялотофамилия GLM                                     |
| 🔮 **MiniMax M2.5**                            | Решаване на проблеми + задачи с енегентно поведение от $0.30/1M — значително подобряване от M2.1            |
| 🎯 **toolCalling Значен флаг за модела**       | Персонализиран `toolCalling: true/false` в реестъра — комбо прескача модели, които нямат такива възможности |
| 🌍 **Модернираема дума в Интент Разпознаване** | ПТ/ЖЗ/ЕС/АР ключови думи в комбо оценка — по-добра селекция на модела за неанглийски съдържание             |
| 📊 **Benchmark-Driven Падения на Падения**     | Реални p95 задържание от реалнии запитвания обслужва комбо оценка — комбо учи от действителни данни         |
| 🔁 **Повторна Задачна Дупликация**             | Съдържание Хеш базирани дупликация — за безопасен, запазва да не платите повторно за тази съдържание.       |
| 🔌 **Продаваем РоутерСтратегия**               | Универсален `РоутерСтратегия` интерфейс — добави превъзходна маршрутизираща логика като плагини             |

### 🚀 Предишно v2.0.9+ — Игрище за изпитване, CLI Извличане на Спечения & ACP

| Функция                                                | Що е то                                                                                                                                                                                                                                                                                                                 |
| ------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🎮 Пул Х2 ХМодел Плейграунд Х20 Х                       | Панел за изпитване на модели директно — селектори на провайдър, модел и точка на вход, Monaco Editor, стрийминг, забавяне, време                                                                                                                                                                                        |
| 🔏 **Повторнопречиство на данните за CLI **             | Сортиране на главни и тела на провайдър, за да отговарят на автентификите на native CLI сървър — настройки за секуритета за избор на провайдър. **Вашата прокси IP е запазена**                                                                                                                                         |
| 🤝 **Поддръжка на ACP (AGENT CLIENT PROTOCOL)**         | Открива агенти CLI (Codex, Claude, Goose, Gemini CLI, OpenClaw + 9 други), процес за стартиране, `/acp/api/agents` точка на вход                                                                                                                                                                                        |
| 🤖 **Подборка на ACP Агенти**                           | Открива Агенти › страничка за отмяна в grid на 14 агенти, състояние на инсталиране, версия, форма за въвеждане на кастомни агенти за всички CLI системи. **Потребители на OpenCode** получават бутон "Зареди опенсорсния файл" за автоматическо-генериране на готов-да-използва конфигурация за всички достъпни модели. |
| 🔧 **Сщедствено моделиering `apiFormat` Маршрутизация** | Сщедствено моделиering с `apiFormat: "отговори"` сега ще коретно маршутират към Responses API трансляция                                                                                                                                                                                                                |
| 🏢 **Работни пояси на Codex Изаляция**                  | Няколко работни пояси на Codex на електронна поща — единственият OAuth отделянетя от ръкав на работните пояси по ИД                                                                                                                                                                                                     |
| 🔄 **Авто-update на Electron**                          | Десктоп приложите проверяват актуализиране + извеждат при ново зачитване                                                                                                                                                                                                                                                |

### 🤖 Operации и съръгментиране на извеждатя и протоколи (v2.0)

| Функция                                                     | Що е то                                                                                                                                 |
| ----------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| 🔧 [Х2Х]Сервер MCP (16 инструменти)[Х25Х]                    | IDE/агентови инструменти през 3 транспортни методи: stdio, SSE ([Х46Х]/api/mcp/sse[X59Х]), Нарежимен HTTP ([Х80Х]/api/mcp/stream[X96Х]) |
| 🤝 [Х2Х]Сервер A2A (JSON-RPC + SSE)[Х31Х]                    | Изпълнение задач между агенти с синхронна и поточна експлоатация                                                                        |
| 🧭 [Х2Х]Пейдж за Обединени точки[X31Х]                       | Изградена страница с табове за Endpoint Proxy, MCP, A2A и API точки                                                                     |
| 🎚️ [Х3Х]Включения/Изключения на услугите[X35Х]              | Предimmerки ОН/ОФ за MCP и A2A, със съхраняване на зададените мустики (по подразбиране: ОФ)                                             |
| 🛰️ [Х3Х]Реално състояние на МакРан时代[X26Х]                  | Истинско състояние на процеса (pid, uptime, старезина на сърцата, транспорт, scope режим)                                               |
| 📋 [Х2Х]Документацията за аудит MCP[X19Х]                    | Можество за филтриране на аудитни записи с успех/неуспех и ключове                                                                      |
| 🔐 [Х2Х]Накладите за опирание на Scope MCP[X25Х]             | 9 грануларни множения за контрол на достъпните инструменти                                                                              |
| 📡 [Х2Х]Мениджъмента на жизнения цикъл на задачите A2A[X33Х] | Списъци за филтриране и изрязване на задачите и инспектиране на събитията и артефакти, отмяната на бъдещите задачи                      |
| 📋 [Х2Х] Откриване на карта на агент[X24Х]                   | `/.well-known/agent.json` за клиентска самота на разпознаване                                                                           |
| 💡 **Protocol E2E Test Harness**                             | Реален MCP SDK + A2A клиентски потоци в  `test:protocols:e2e`                                                                           |
| ⚙️ **Operational Controls**                                 | Постреждащ комбо, прилагане на профили за резистентност, префилтриране на бронтажери от една конзола за управление                      |

### 🧠 Рутингове & Интелектуалност

| Функция                                        | Що е то                                                                            |
| ---------------------------------------------- | ---------------------------------------------------------------------------------- |
| 🎯 **Smart 4-Tier Fallback**                    | Авторутване: Подписка → API Ключ → Cheaper → Безплатен                             |
| 📊 **Real-Time Quota Tracking**                 | Време реално брой токени + брой на пресметванията за перезареждане за провайдър    |
| 🔄 **Format Translation**                       | OpenAI ↔ Claude ↔ Gemini ↔ Отговора с защита на схемата                            |
| 👥 **Multi-Account Support**                    | Като предоставяне на множество сметки за провайдърите с интелигентно подбиране     |
| 🔄 **Auto Token Refresh**                       | OAuth токените се рестартират автоматически с повторна опитка                      |
| 🎨 **Custom Combos**                            | 6 стратегии за балансиране + кръгова връзка за контрол на последиците              |
| 🌐 **Wildcard Router**                          | `провайдер/*` динамичен рутинг                                                     |
| 🧠udget за мислене контроли[Х28Х]               | Прехвърляне, ауто, кастомизирана и адаптивна граница на разсъжденията              |
| 🔀  Алиаси на модели                            | Натрупвани + кастомизирани алиаси на модели и безопасност на изместбво             |
| ⚡ Падащо разсъждение в позадина                | Канализация на понишен степен на задачи за съвестни модели                         |
| 🧪 Интелигентно упражнение със задача           | АUTO-селекция на модела от съдържание (кодироване/изобразяване/анализа/сумарне)    |
| 💬 Иначеряване на система за системна подсказка | Глобални контроли за поведение се прилагат в съответствие                          |
| 📄 Обща спрашваща API за отговори               | Пълно [Х5Х]/v1/responses[X19Х] поддръжка за Codex и напреднали агентствени процеси |

### 🎵 Multi-Modal APIs

| Функция                         | Що е то                                                                                                                                                                                |
| ------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🖼️  Производство на изображения | `/v1/images/generations[X23Х] със облака и местен превод                                                                                                                               |
| 📐 Вградени векторни размерности | `/v1/embeddings[X15Х] за търсене и RAG канали                                                                                                                                          |
| 🎤 **Аудио Транскрипция**        | `/v1/audio/transcriptions` — 7 поставители (Deepgram Nova 3, AssemblyAI, Groq Whisper, HuggingFace, ElevenLabs, OpenAI, Azure), автоматично детекция на езика, подкрепа за MP4/MP3/WAV |
| 🔊 **Текст на говор**            | `/v1/audio/speech` — 10 поставители (ElevenLabs, OpenAI, Deepgram, Cartesia, PlayHT, HuggingFace, Nvidia NIM, Inworld, Coqui, Tortoise) с точно синхронизирани съобщения за грешки     |
| 🎬 **Видео Генерация**           | `/v1/videos/generations` (ComfyUI + SD WebUI workflows)                                                                                                                                |
| 🎵 **Музикален Генерация**       | `/v1/music/generations` (ComfyUI workflows)                                                                                                                                            |
| 🛡️ **Модерации**                | `/v1/moderations` сигурностни проверки                                                                                                                                                 |
| 🔀 **Повторна класиране**        | `/v1/rerank` за релевантност на класиране                                                                                                                                              |
| 🔍 **Уеб Сърс** 🆕                | `/v1/search` — 5 поставители (Serper, Brave, Perplexity, Exa, Tavily), 6,500+免费/месец, автоматичен фейлфовър, кеш                                                                      |

### 🛡️ Заштита, сигурност и управление

| Функция                                                                     | Що е то                                                                                    |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------ |
| 🔌 **Релевантни Превключвателя**                                             | Пер-моделна разлука/възстановяване с контроли за порог                                     |
| 🎯 **Модели със завъртане на края на пътя**                                  | Customни модели обявяват поддръжкани точки за настройка + формат на API                    |
| ⚓️ **Защита от гръмихането на стад **                                       | Семафор + мьютекс за защита на рибут и тарев събития                                       |
| Облекчаващи механизми за намаляване на загуба и задържане с две касови слоя | Намаляване на затратите и задържането с две касови слоя                                    |
| ⚡ **Повторнопречистване **                                                  | Protect от повторни сърдечни с токов window                                                |
| 🔒 **Аутентичност за TLS FingerPrinting **                                   | Browser-like TLS fingerPrinting — **намаляване на бот и flaggings **                       |
| 🔏 **Повторнопречиство на данните за CLI **                                  | Matching за native CLI request — **намаляване на риска, докато се запазва IP на проксита** |
| 🌐 **Проверка на IP Address **                                               | Премахване на изложените деплояма със разрешителна/запречителна лента                      |
| 📊 **Редовие граница на скоростите **                                        | Състъпна/множествена граница, съхраняваща се и с перзистентна връзка                       |
| 🔑 **Управление на ключове за API и разпределение **                         | Сигурно издание и повтаряне на ключове със също така модел/предложителните ограничения     |
| 🛡️ **Защитеното / модели **                                                 | Вариантна защита с ползваемо и скриваща се съобщаваща на модела като каталог               |

### 📊 Пазвеждиване, анализа и анализа в real time.

| Функция                            | Що е то                                                                     |
| ---------------------------------- | --------------------------------------------------------------------------- |
| 📝 **Петиция за Proxy Logout[X1X7X] | Пълният запит/отговор и излог на прокси                                     |
| 📋 **Обединени Панел за Лoğlu       | Настойки за запит, прокси, аудит и конзола в една страница                  |
| 🔍 **Наблюдаване на Запит           | П50/%p95/%p99 latency и търсене на запит                                    |
| 🏥 **Логов на Здраве                | Достъпност, състояние на преимущество, заблоки, статистики за кеш           |
| 💰 **Следене на Стойност            | Контрол на бюджет и видимост на стойността на модела                        |
| 📈 **Анализа на Визуализации        | Казуси и тенденции за използване на модела и предаване                      |
| 🧪 **Фреймворк за Оценка            | Тестове с латински комплект със съгласимите се на стратегии за съпоставител |

### ☁️ Разпространение и Платформа

| Функция                                      | Що е то                                                                              |
| -------------------------------------------- | ------------------------------------------------------------------------------------ |
| 🌐 **Разпространение в любое Място\           | Локалホスト, VPS, Docker, Nube environmenti                                             |
| 💾 Пул Х2 ХСинк в Облакото Х14 Х              | Синхронизация на конфигурация чрез облако работник                                   |
| 🔄 Пул Х2 ХБекъп/Ристори Х18 Х                | Експорт-импортиране и намаляване на бедности                                         |
| 🧙 Пул Х2 ХОнбординг Визард Х21 Х             | Първото сработване водено ръчно построяване                                          |
| 🔧 Пул Х2 ХКЛИ Утваряне на Борда Х23 Х        | Едноекликово поставяне на популярни програми за сътрудничество                       |
| 🎮 Пул Х2 ХМодел Плейграунд Х20 Х             | Изпробвай каквато и да е услуга-модел-точки от уеб-интерфейса                        |
| 🔏 Пул Х2 ХКЛИ Чиштир за Следи Х26 Х          | Суспоставящи следи в Сетингс > Безопасност                                           |
| 🌐 Пул Х2 ХI18N (30 езици) Х23 Х              | Активиране на всяка езикова поддръжка сRTL покриваща на уеб-интерфейсите и докуманти |
| 🧹 Пул Х2 ХИзчистване на всички Модули Х20 Х  | Кликнате за изчистване на модулите от уеб-интерфейса на услугата                     |
| 📋 Пул Х2 ХШаблон за Повдигнати Въпроси Х19 Х | Стандартизирани шаблони за GitHub за задълженията и приноси                          |
| 📂 Пул Х2 ХПотребителска директория Х25 Х     | `Директория_ДАННИ` override за местоположение на сървър за съхранение                |

### Актуаленъ view

#### Умна fallback с практически контрол на себестоимость

```txt
Комбо: "моя-комплект_за_razrabotka"
  1. cc/claude-opus-4-6
  2. nvidia/llama-3.3-70b
  3. glm/glm-4.7
  4. if/kimi-k2_myslleniye
```

Когато квота, скорост или здраве претърпят отказ, клиент автоматично преминава
към следващия кандидат без ръчна промяна.

#### Управлението на протокола, видимо и използваемо

- MCP + A2A могат да се открият в UI и в докуметиращия документ
- Апите за протокола изявят живата експлоатистваема данни от
  (`/ap/MCP/*`,`/ap/2Aa/*`)
- Панелите включват действия за дневен оперативен труд (представяне на комбо,
  сбойни пресекания и отмяната на задачи)

#### Стенографията на преводача + валидация на протокола

Полето за преводача включва:

- **Залата за игра** : превод чекове на проверка
- **Тестер за общащение**: полен превод в общащение и отговор
- **Тестов център**: множество случаи в един превод
- **Очакван визор**: реално-травящо гледане на трафика

Плюс конверсия на протокола със стена клиентите чрез `npm run тест е2е`.

> 📖 **[Наука по MCP-сервера](open-sse/mcp-server/README.md)** - набля на
> инструментите, презадължения с ИДЕ и примерни клиент
> 
> 📖 **[Наука на A2A-сервера](src/lib/a2a/README.md)** - знания, методи за
> JSON-RPC, стрийм и жизиен цикъл на задачи

## 🧪 Оценочни експерименти (Евал.)

Вграденият в OmniRoute оценочен експериментен фреймворк дава възможност за
изпитване на изправеността на лятна отговорност на клиентите срещу златно
сърцево набля. Достават се чрез **Анализи → Евал.X135X] на панеля\
==WEBLATE_PART==

### Интегрираният Златен Сет

Предлаганото вградено "OmniRoute Златен Сет" съдържа тестови случая за:

- Здравейте, математика, география, генериране на код
- Съответствието на формата на JSON, превод, генериране на маркиране
- Отказ за изчервяване на вредни данни, регистрация, булеви логически изрази

### Стратегии за оценка

| Стратегия         | Описание                                                                           | Пример                               |
| ----------------- | ---------------------------------------------------------------------------------- | ------------------------------------ |
| `изявчено`        | Изходът трябва да отговаря съвпадения                                              | `"4"`                                |
| `съдържа`         | Изходът трябва да съдържа подсвиргаема подпоследователност (без учет на регистъра) | `"Париж "`                           |
| `регуларен израз` | Изходът трябва да съответства на регуларен израз                                   | `"1.*2.*3"`                          |
| `задължителен`    | Задължителен(JS функция) връща true/false                                          | `(вивод) =&gt; вывод.размер &gt; 10` |

---

## 📖 Управление настройките

### Настройка Протокола (MCP + A2A)

<details>
<summary><b>🧩 MCP Setup (Model Context Protocol)</b></summary>

Започнете транспорта MCP в режим стдио:

```bash
omniroute --mcp
```

Приемливо потвърждаване на протокола:

1. Наеме соединение с MCP разпространител в режим стдио.
2. Изпълнете `омнироут_геит_здраве`.
3. Изпълнете `омнироут_списъци_комбо`.
4. Отворете `/dashboard/mcp`, за да потвърдитеheartbeat, активност и аудит.

Полезни API-и за автоматизация:

- `GET /api/mcp/status`
- `GET /api/mcp/tools`
- `GET /api/mcp/audit`
- `GET /api/mcp/audit/stats`

</details>

<details>
<summary><b>🤝 A2A Setup (Agent2Agent)</b></summary>

Открийте агента:

```bash
curl http://localhost:20128/.well-known/agent.json
```

Изпратете задача:

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'съдържание-type: приложение/json' \
  -d '{"jsonrpc":"2.0","id":"setup-a2a","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"Съобщи за статус на квотата."}]}}'
```

Управление на живота:

- `GET /апи/a2a/статус`
- `GET /апи/a2a/задачи`
- `GET /апи/a2a/задачи/:ид`
- `POST /апи/a2a/задачи/:ид/отмена`

Операционна UI:

- `/панел за мониторинг/a2a` за наблюдение за задачите, състоянията и потоците и
  за изпъляване на действия за събиране на данни

</details>

<details>
<summary><b>🧪 End-to-end protocol validation</b></summary>

Верифицирайте повърхността на клиентите и с реалните клиенти:

```bash
npm run test:protocols:e2e
```

Това потвърждава:

- Клиент на MCP SDK: свързване/списък/понеждане
- Очертаване A2A: разпознаване/отпращане/поток/получаване/отмена
- Кръстосна проверка на данните в MCP аудит и API-източник за управление на
  задачите A2A

</details>

<details>
<summary><b>💳 Subscription Providers</b></summary>

### Клод Коуд (Про/Макс)

```bash
Панел за наблюдение → Провайдър → Свържуване Клод Коуд
→ Понеждано логване → Автоматично подновяване на токена → Следенуване на квотата за 5 часа + седмичен квотова режим

Модели:
  cc/claude-opus-4-6
  cc/claude-sonnet-4-5-20250929
  cc/claude-haiku-4-5-20251001
```

**Професионална тачка:** Използвайте Опус за сложни задачи, Сонет за бързост.
OmniRoute отслужва квотата на модела!

### Отворен кодекс Ай (Пъл/Професионал)

```bash
Панел за наблюдение → Провайдър → Свържуване Содекс
→ Понеждано логване (порта 1455)
→ 5-часов + седмичен изхождане на квотата

Модели:
  cx/gpt-5.2-codex
  cx/gpt-5.1-codex-max
```

#### Управление на квотите на Содекса (5ч + седмичен квотова режим)

Що също така още Содекс има селекторите на квотите в `Панел за наблюдение -&gt;
Провайдер`:

- `5ч` (ОН/ОТ): извършване на 5 часовата граница на квотата на политика.
- [Х0Х]Неделно[Х7Х] (ДА/ОТКАЗИВАМ СЕ): изпълване на политиката за минимален
  етап.
- Behaviour при гранична граница: когато позволената прозоречна граница направи
  >= 90% потребление, съответната сметка е пропусната.
- Rotation поведение: OmniRoute нарежда следващият позволен кодекс отчет
  автоматично.
- Мъничави поведения: след като връщането на пружината `resetAt` миграция
  минава, сметката се връща отново наред автоматично.

Сценарии:

- `5h ON` + `Неделно ON`: ако сметката се запърости когато или оба прозоречни
  граници достигнат минимум.
- `5h OFF` + `Неделно ON`: само неделената употреба може да оневоли сметката.
- `5h ON` + `Неделно OFF`: само часовото намаление може да блокира сметката.
- `resetAt` вече е минувала: съответната сметка се връща в ротационата рамка
  автоматично (никоя самия рибник ряз.

### Гемини КЛИ (ЗА СВИНЕ БЕЗПЛАТНО 180К/месец!)

```bash
Общи панели → Providers → Връзване с Гемини КЛИ
→ Google OAuth
→ 180K завършени изпълнения/месец + 1K/день

Модели:
  gc/gemini-3-скицеви-премиерна-демонстрация
  gc/gemini-2.5-професионален
```

**Лучшата стойност:** голям безплатен план! Използвайте го преди платените
планове.

### Копилот на GitHub

```bash
Общи панели → Providers → Връзване GitHub
→ OAuth натписа GitHub
→ Месечно възстановяване (1 в месец)

Модели:
  gh/gpt-5
  gh/claude-4.5-сонет
  gh/gemini-3-професионален
```

</details>

<details>
<summary><b>🔑 API Key Providers</b></summary>

### НВИДИА НИМ (БЕЗПЛАТЕН АКЕС ЗА РАЗработвачи — 70+ модели)

1. Регистрирай се: [build.nvidia.com](https://build.nvidia.com)
2. Активирайте безплатен API ключ (включвали 1000 импликации кредита)
3. Общи панели → Добавяне на услуга → НВИДИА НИМ:
   - Ключ: `nvapi-ваш-ключ`

**Модели:** `нвидия/лаама-3.3-70б-инструкции`, `нвидия-мистрал-7б-инструкции` и
още 50+\
==WEBLATE_PART==

**Противопрепятствие:** Открийте AI-兼容ен API — работи безпроблемно с
преобразуване на OmniRoute!

### DeepSeek

1. Регистрация: [platform.deepseek.com](https://platform.deepseek.com)
2. Получи API ключ
3. Перйти на главната страница → Добави Provider → DeepSeek

**Модели:** `.deepseek/deepseek-chat`, `.deepseek/deepseek-coder`

### Groq (Нямат такса)

1. Регистрация: [console.groq.com](https://console.groq.com)
2. Получете ключа на API (вкл. в безплатнитея версия)
3. Перйти на главната страница → Добави Provider → Groq

**Модели:** `.groq/llama-3.3-70b`, `.groq/mixtral-8x7b`

**Противопрепятствие:**超скоро инференция — най-добре за реално време за
програмиране!

### OpenRouter (100+ Модели)

1. Регистрация: [openrouter.ai](https://openrouter.ai)
2. Получи API ключ
3. Перйти на главната страница → Добави Provider → OpenRouter

**Модели:** Достъп до 100+ модели от всички основни провайдъри чрез един ключ на
API.

</details>

<details>
<summary><b>💰 Cheap Providers (Backup)</b></summary>

### GLM-4.7 (_daily_reset, $0.6/1M)

1. Регистрация: [Zhipu AI](https://open.bigmodel.cn/)
2. Получете ключа на API от Кодинговия план
3. Контролен панел → добави API ключ:
   - Провайдър: `glm`
   - API ключ: `your-key`

**Use:** `glm/glm-4.7`

**Pro Tip:** Планът за програмиране пълни 3x квота на 1/7 от затратата! Сброи се
ежедневно на 10:00 часа сутринта.

### MiniMax M2.1 (5-часов преизход, $0.20/1М)

1. Заръ417и се: [MiniMax](https://www.minimax.io/)
2. Получи API ключ
3. Контролен панел → добави API ключ

**Use:** `minimax/MiniMax-M2.1`

**Pro Tip:** Нисшата цена за дълъг контекст (1M знака)!

### Kimi K2 (9 долара/месец flatt rate)

1. Регистрирай се: [Moonshot AI](https://platform.moonshot.ai/)
2. Получи API ключ
3. Контролен панел → добави API ключ

**Use:** `kimi/kimi-latest`

**Pro Tip:** Фиксирано 9 долара/месец за 10М знака = $0.90/1M ефективна цена!

</details>

<details>
<summary><b>🆓 FREE Providers (Emergency Backup)</b></summary>

### iFlow (5 безплатни модели чрез OAuth)

```bash
Контролен панел → свържи iFlow
→ вхождение в OAuth профила
→ безкръгова употреба

Модели:
  if/kimi-k2-thinking
  if/qwen3-coder-plus
  if/glm-4.7
  if/minimax-m2
  if/deepseek-r1
```

### Qwen (4 безплатни модели чрез устройствен код)\

```bash
Dashboard → Свържи Qwen
→ Авторизация чрез устройствен код
→ Безограничен достъп

Модели:
  qw/qwen3-coder-plus
  qw/qwen3-coder-flash
```

### Киโร (Форс ФРИ)

```bash
Dashboard → Свържи Киโร
→ AWS Builder ID или Google/GitHub
→ Безограничен достъп

Модели:
  kr/claude-sonnet-4.5
  kr/claude-haiku-4.5
```

</details>

<details>
<summary><b>🎨 Create Combos</b></summary>

### Пример 1: Максимизирай Абонамент → Счепа Backup

```
Dashboard → Комбинирай → създай нова

Име: premium-coding
Модели:
  1. cc/claude-opus-4-6 (Основен абонамент)
  2. glm/glm-4.7 (Счепа резервна копия, $0.6/1M)
  3. minimax/MiniMax-M2.1 (Най-евтин заместник, $0.20/1M)

Испотреби в CLI: premium-coding
```

### Пример 2: Безплатно съоръжение (Нула Стоимость)

```
Име: free-combo
Модели:
  1. gc/gemini-3-flash-preview (180K безпл. мес.)+
  2. if/kimi-k2-thinking (безграничен)
  3. qw/qwen3-coder-plus (безграничен)

Стоимост: $0 навечер!
```

</details>

<details>
<summary><b>🔧 CLI Integration</b></summary>

### Курсор IDE

```
Настройки → Модели → Разширени:
  URL на базово API на OpenAI: http://localhost:20128/v1
  API ключ на OpenAI: ( от OmniRoute)
  Модел: cc/claude-opus-4-6
```

### Клод Код

Използвайте страницата **CLI Tools** в dashboard за едновременна конфигурация
или редактирай `~/.claude/settings.json` ръчностно.

### Кодекс CLI

```bash
експорт OPENAI_BASE_URL="http://localhost:20128"
експорт OPENAI_API_KEY="Ваш-омнироут-API-ключ"

кодекс "вашия вход"
```

### Отворен чашкослоп

[Х0Х]Вариант 1 — Dashboard (recommended):[Х37Х]

```
Dashboard → CLI Tools → OpenClaw →Select Модел → Примени
```

[Х0Х]Вариант 2 — Ръчна поставка:[Х20Х] редактирай
[Х28Х]~/.openclaw/openclaw.json`:

```json
{
  "models": {
    "providers": {
      "омнироут": {
        "baseUrl": "http://127.0.0.1:20128/v1",
        "apiKey": "sk_omniroute",
        "api": "openai-completions"
      }
    }
  }
}
```

> [Х0Х]Примечание:[Х7Х] Отворен чашкослоп работи само с локален OmniRoute.
> Използвайте [Х56Х]127.0.0.1` по място на [Х79X]localhost` за да избегнете
> проблемите с резолюция на IPV6.

### Linia / Продължи / Стрела на Kodice

```
Настройки → Конфигурация API:
  Провайдер: OpenAI Compatible
  Базов URL: http://localhost:20128/v1
  API Ключ: [от OmniRoute панел]
  Модел: if/kimi-k2-thinking
```

### Опенкод

**Шаг 1:** Добавете OmniRoute като личен провайдър:

```bash
opencode
/connect
# Изберете " Други" → Въведете ID: "omniroute" → Въвъдете Вашата OmniRoute API ключ
```

**Шаг 2:** Създайте/потвърдете `опendcode.json` в корена на своя проект:

```json
{
  "$schema": "https://opencode.ai/config.json",
  "провайдър": {
    "omniroute": {
      "npm": "@ai-sdk/openai-compatible",
      "имe": "OmniRoute",
      "опции": {
        "базов URL": "http://localhost:20128/v1"
      },
      "модели": {
        "cc/claude-sonnet-4-20250514": { "имe": "Claude Sonnet 4" },
        "gg/gemini-2.5-pro": { "имe": "Gemini 2.5 Pro" },
        "if/kimi-k2-thinking": { "имe": "Kimi K2 (Free)" }
      }
    }
  }
}
```

**Шаг 3:** Селектирайте модела в Опенкод:

```bash
/models
# Изберете каквото и да е OmniRoute модел от списъка
```

> **Съвет:** Добавете към `/v1/models` endpoint в OmniRoute панела модела.
> Използвайте формата `provider/model-id`.

</details>

---

## Отстраняване на неизправности

<details>
<summary><b>Click to expand troubleshooting guide</b></summary>

**"Лингвистическият модел не е предоставил съобщения"**

- Изчерпан квота на провайдъра → Проверете квотата в панела на прозорчетата
- Решение: Използвайте комбинация на fallback или премахнете на дамска
  приставаца кратната

**Мерни граници**

- Изчерпан квота. Използвайте комбинация на GLM/MiniMax
- Добавте комбинацията: `cc/claude-opus-4-6 → glm/glm-4.7 → if/kimi-k2-thinking`

**Изтичащо се нарастване**

- Ауторефрешван от OmniRoute
- Ако проблемите продължават: Панел → Провайдър → Съединете се отново.

**Държавни разходи**

- Прегледайте използваните статистики в Панел → Разходи
- Свържете основна модел с GLM/MiniMax
- Използвайте свободен тариф (Gemini CLI, iFlow) за непритежните задачи

**Dashboard/API портов са грешни**

- `Порт` е основният базов (и API) порт по подразбиране
- `API_PORT` преоствува само за OpenAI съпоставими API съществуващи уведомления
- `DASHBOARD_PORT` преоствува само за dashboard/Next.js съществуващи уведомления
- Налагайте `NEXT_PUBLIC_BASE_URL` на вашия публикуван URL на dashboard (за
  OAuth уведомления)

**Грешки при облачна синхронизация**

- Проверявайте дали `BASE_URL` показва пълен ваша завършена версия
- Проверявайте дали `CLOUD_URL` показва вашето зададено облаково кръси
- Държите `NEXT_PUBLIC_*` координати намерени на сървърната страна

**Първ ентер не работи**

- Проверявайте `INITIAL_PASSWORD` в `.env`
- Ако не е зададена, предвидимата парола е `123456`

**Няма изпратени логове**

- Налагайте `ENABLE_REQUEST_LOGS=true` в `.env`

**Тест по свръзката показва " невалиден" за OpenAI съпоставими провайдъри**

- Много доставчии не използват endpoint за моделите
- Omnidirect v1.0.6+ включва fallback validation от чат за свършване
- Задържане URL включва[Н25Н]/v1[Н29Н] префикс

### Възпламенено при пулта на страна. Офис на достъп на много отдалечена централа

<a name="oauth-on-a-remote-server"></a> <a name="oauth-em-servidor-remoto"></a>

> [Х0Х]⚠️ Важно за потребителите, които използват OmniRoute в VPS, Docker или
> която година друга страна централа[Х81Х]

#### Защо OAuth Antigravity / Gemini CLI няма в работата отдалечена централа?

Преподавателят [Х4Х]Гравитация[X17Х] и [Х24Х]Gemini CLI[X36Х] доставчиките
ползват [Х53Х]Google OAuth 2.0[X71Х]. Google изисква [Х95Х]указателен URI[X108Х]
в подхода за възпламенение на достъп, който да бъде точен от пулта на предишните
зарегистрирани URI в профила на Google Cloud Console.

Шифрите за OAuth, свързани със сървъра OmniRoute са зарегистрирани
[Х58Х]исключително за `localhost`[Х80Х]. Когато достъпите OmniRoute на удалена
централа, Google отхвърля възпламенението на входите:

```
Ошибка 400: направил URI_mismatch
```

#### Решение: Настройване на собствени ключове за достъп на Оауътър

Вие трябва да създадете [Х22Х]клиентен идентификатор OAuth 2.0[X43Х] в профила
на Google Cloud Console с URI на вашата централа.

#### Хороскоп

[Х0Х]1. Отворете профила на Google Cloud Console[X30Х]

Идете на:
[https://console.cloud.google.com/apis/credentials](https://console.cloud.google.com/apis/credentials)

[Х0Х]2. Създайте нов клиентен идентификатор за OAuth 2.0[X37Х]

- Натиснете [Х6Х]"+ Създайте кредити"[X30Х] → [Х35Х]"Клиент за OAuth"[Х54Х]
- Тип: [Х18Х]"Web приложение"[Х37Х]
- Име: що ви искаете (например [Х30Х]OmniRoute отдалечена централа[X47Х])

[Х0Х]3. добавете разрешени URI за връщане в подхода на входите[X33Х]

В полета за разрешени Ввръщане URI добавете:

```
https://вашият-сервер.домен/{callback}
```

> Заменете [Х8Х]вашият-сервер.домен` с домейн или IP на вашата централа
> (включвайте порта, ако е нужен, например
> [Х92Х]http://45.33.32.156:20128/връщане`).

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

Кредитите OAuth, вградени в OmniRoute са регистрирани ** само за `localhost` **.
Когато достъпите OmniRoute в отдален сървър (например,
`https://omniroute.meyservidor.com`), Google отхвърля възможността за
autentикация:

```
Ошибка 400: направил URI_mismatch
```

#### Солuzione: Конфигурирайте собствените си OAuth-кредитии

Ви трябва да създадете **OAuth 2.0 Client ID** в Google Cloud Console с URI на
вашата служба.

#### Шагове към решенията:

**1. Включете Google Cloud Console**

Отворете:
[https://console.cloud.google.com/apis/credentials](https://console.cloud.google.com/apis/credentials)

**2. създайте нов OAuth 2.0 Client ID**

- Кликнете на **"+ Create Credentials"** → **"OAuth client ID"**
- Тип на приложение: **"Web приложение"**
- Име: избирете каквото желаете (например, `OmniRoute отдален`)

**3. Добавете позволениredi URIs**

В полето **"Authorized redirect URIs"**, добавете:

```
https://seu-servidor.com/callback
```

> Заместете `seu-servidor.com` с домейн или IP адрес на сървърата си (включете
> порта, когато е необходимо, например: `http://45.33.32.156:20128/callback`).

**4. Спряхне и копирайте кредити**

След като създадете тях, Google ще покаже **Client ID** и серии клиент **.

**5. Конфигуриращи се environment переменни**

На вашето `.env` (или environment переменни на Docker):

```bash
# За Antigravity:
ANTIGRAVITY_OAUTH_CLIENT_ID=seu-client-id.apps.googleusercontent.com
ANTIGRAVITY_OAUTH_CLIENT_SECRET=GOCSPX-seu-secret

# За Gemini CLI:
GEMINI_OAUTH_CLIENT_ID=seu-client-id.apps.googleusercontent.com
GEMINI_OAUTH_CLIENT_SECRET=GOCSPX-seu-secret
GEMINI_CLI_OAUTH_CLIENT_SECRET=GOCSPX-seu-secret
```

**6. Натиснете Restart на OmniRoute**

```bash
# В случае използване npm:
npm run dev

# В случай използване Docker:
docker restart omniroute
```

**7. Опитайте да се свържете пак**

Дashboard → Providers → Antigravity (или Gemini CLI) → OAuth

Сега Google ще обръща правилно обратно в `https://ваш-сервер.com/callback` и
автентикацията ще функционира.

---

#### Мъгълно решение за краткосрочно време (без настройка на собствени цреда)

Ако не искате да направите собствени креденцили сега, все още е възможно да
използвате потока **мана на URL**:

1. Оmniroute ще отвори URL за авторизация на Google
2. След като разрешите, Google ще опита да обръща в `localhost` (който се
   проваля тук на сървъра)
3. **Копирате цяла URL** от адресния ред в вашия browser ( дори ако страницата
   не се зареди)
4. Вкарвате тази URL в полето, който излиза в модала за свързване на OmniRoute
5. Натиснете **"Connect"**

> Това мъгълно решение работи защото аутентикационния код от URL-ът е валиден
> независимо от да се зареди или не.

</details>

---

</details>

## 🛠️ Tech Stack

<details>
<summary><b>Click to expand tech stack details</b></summary>

- **Runtime**: Node.js 18–22 LTS (⚠️ Node.js 24+ не е **подкрепен** – native
  начините за Бета-сървър SQL не са съвместими)
- **Език**: TypeScript 5.9 — **100% TypeScript** по цялото `src/` и `open-sse/`
  ( нула `any` в основни модули от версия 2.0)
- **Фреймворк**: Next.js 16 + React 19 + Tailwind CSS 4
- **База данни**: LowDB (JSON) + SQLite (домейнни стойности + проспири сега +
  МСП аудит + рутинни решения)
- **Схеми**: Zod (инструмент за МСП I/O валидация, API контакти)
- **Повеъни протоколи**: MCP (stdio/HTTP) + A2A v0.3 (JSON-RPC 2.0 + SSE)
- **Преглед на потока[Х11X]: Серверно-отдавани събития (SSE)
- **Потвърждаване[Х6X]: OAuth 2.0 (PKCE) + JWT + API Кики + МКП Създадено
  одобрение
- **Тестване[Х9X]: Тестов сървър Node.js + Vitest (900+ тестове включващи
  единичностни тести, интеграционни тести и Е2Е)
- **CI/CD[Х7X]: GitHub Actions (автоматично публикуване на npm + Docker Hub при
  издаване)
- **Вебстайтове**: [omniroute.online](https://omniroute.online)
- **Пакет[Х9X]:
  [npmjs.com/package/omniroute](https://www.npmjs.com/package/omniroute)
- **Докер[Х8X]:
  [hub.docker.com/r/diegosouzapw/omniroute](https://hub.docker.com/r/diegosouzapw/omniroute)
- **Съпротивяваща се способност[Х12X]: Чиркова кутия, експоненциално
  оповрждение, противоречие на стадия при хердата, симулация TLS, саможивот на
  комбиниране

</details>

---

## Документация

| Документ                                                | Описание                                                                |
| ------------------------------------------------------- | ----------------------------------------------------------------------- |
| [Потребителска справка](docs/USER_GUIDE.md)             | Съпроводители, комбинации, интеграция на командния линей, разпределение |
| [Sправочник на API-та](docs/API_REFERENCE.md)           | Всички края на точката на изход с примери                               |
| [Сървър MCP](open-sse/mcp-server/README.md)             | 16 инструменти MCP, конфигурации на IDE, клиенти Python/TS/Go           |
| [Сървър A2A](src/lib/a2a/README.md)                     | Протокол JSON-RPC 2.0, умения, потокове, управление на задачи           |
| [Аутоматизиран комбиниран двигател](docs/auto-combo.md) | Шестифакторско осмянивание, модове пакети, самозаваряване               |
| [Трубоустройство](docs/TROUBLESHOOTING.md)              | Общи проблеми и решения                                                 |
| [Архитектура](docs/ARCHITECTURE.md)                     | Архитектура и вътрешни механизми на системата                           |
| [Принос](CONTRIBUTING.md)                               | Налагане на разработка и ръководството                                  |
| [Отворена API спецификация](docs/openapi.yaml)          | Отворена API спсификация 3.0                                            |
| [Безопасностен политик](SECURITY.md)                    | Отчитане на недостатъчности и използване на безопасни трайктики         |
| [Виртуално разпределение](docs/VM_DEPLOYMENT_GUIDE.md)  | Пълен пук: виртуално + nginx + Cloudflare комплект                      |
| [Галерия с функции](docs/FEATURES.md)                   | Визуален тур на dashboard със снимки                                    |
| [Списък на изданието](docs/RELEASE_CHECKLIST.md)        | Шагове за предизданието                                                 |

---

## 🗺️ Карта на развитието

OmniRoute има **210+ програмирани фичи**, разпределени в множество етапи. Тук са
ключовите области:

| Категория                                    | Планирани Функции | Акценти                                                                                                              |
| -------------------------------------------- | ----------------- | -------------------------------------------------------------------------------------------------------------------- |
| 🧠 Мозъката **Routing & Интелигенция**        | 25+               | Рутинг с най-ниска задействаност, рутинг с тагове, префильтроваване на квоти, избор на акаунт P2C                    |
| 🔒 **Безопасност & Съхраняване съобразяване** | 20+               | Покачване на SSRF, скриваене на достъп, нормализиране на достъп на един точек и определение ключове на управление    |
| 📊 **Визиятинност**                           | 15+               | Засегател на OpenTelemetry, реално времени обозначащо квоти, отслеждане на стойностите за модели                     |
| 🔄 **Вградени интеграции**                    | 20+               | Динамично създаване на моделни реестри, рестартиране на провайдъри, много-кратен Кода, парсване на квоти за Copilot  |
| ⚡ **Извършение**                             | 15+               | Двойна подслояна кеш лоя, кеш за запита, кеш за отговори, поточен поток за живот, пакетно API                        |
| 🌐 **Екосистема**                             | 10+               | Откриваща API за web socket, гореща рехайл конфигурация, разпределено съхраняване на конфигурации, комерсиален режим |

### 🔜 Скоро

- 🔗 **ОПЕНКОД Интеграция** — Натуалнаподдържана интеграция с AI кoding IDE на
  OpenCode
- 🔗 **УДК Интеграция** — Полна поддръжка на рамката за развитие на УДК AI
- 📦 **Интеграционна API** — Асинхронна интеграционна обработка за множество
  заявки
- 🎯 **Тег-подредбен маршрутизиране** — Рутване на заявки по кратни тагове и
  метаданни
- 💰 **Нискоустойчива тактика** — Автоматично избирете най-евтиния достъпен
  услуговодител

> 📝 Полни характеристики към [`docs/new-features/`](docs/new-features/) (217
> подробни характеристики)

---

## 👥 Автори

[![Автори](https://contrib.rocks/image?repo=diegosouzapw/OmniRoute&max=100&columns=20&anon=1)](https://github.com/diegosouzapw/OmniRoute/graphs/contributors)

### Как да контрибуете

1. Зафъркираният репзиторий
2. Създайте фичния клон (`git checkout -b feature/amazing-feature`)
3. Настроечите своите промени (`git commit -m 'Добавете уникална фичата'`)
4. Изпратете промяната (`git push origin feature/amazing-feature`)
5. Отворете Pull Request

Вижте CONTRIBUTING.md за обстоятелства.

### Публикуване на нова версия

```bash
# Създайте Release — npm publish става автоматично
gh release create v2.0.0 --title "v2.0.0" --generate-notes
```

---

## 📊 Историия на Старите

## Старатели върху време

## [![Старатели върху време](https://starchart.cc/diegosouzapw/OmniRoute.svg?variant=adaptive)](https://starchart.cc/diegosouzapw/OmniRoute)

## 🙏 Благодарности

У особено голяко благодарим на
**[CLIProxyAPI](https://github.com/decolua/9router)[X36X] — източника на
произвежената този fork. OmniRoute предграденето върху този голям фундамент с
нови функции, multi-modal API и полна перезапишеност на TypeScript.

У особено голяма благодарим на проекта
**[9router](https://github.com/router-for-me/CLIProxyAPI)** — оригинален проект,
който вдъхнови този fork. OmniRoute продължава върху тази изключителна основа с
допълнителни функции, multi-modal API и полна перезапис с TypeScript.

---

## 📄 Ловса за използване

Ловса за използване MIT - съдържа повече информация в [LICENSE](LICENSE).

---

<div align="center">
  <sub>Built with ❤️ for developers who code 24/7</sub>
  <br/>
  <sub><a href="https://omniroute.online">omniroute.online</a></sub>
</div>
<!-- GitHub Discussions enabled for community Q&A -->
