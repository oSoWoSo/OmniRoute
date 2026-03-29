# 🚀 OmniRoute — Свободный AI-шлюз

### Никогда не останавливайтесь, кодите. Умная маршрутизация к **БЕСПЛАТНЫМ и низкозатратным моделям AI** с автоматической подстановкой defaultValue.

_Ваша универсальная proxy API — один endpoint, 67+ поставщиков, ни один
downtime. Теперь с агентом **MCP & A2A** для оркестровки агентов._

**Полнокомплектные решения Chat Completions • Embeddings • Image Generation •
Video • Music • Audio • Reranking • **Поиска по вебу** • Сервер MCP • Протокол
A2A • 100% TypeScript**

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

[🌐 Сайт](https://omniroute.online) • [🚀 Быстрый старт](#-quick-start) • [💡
Функции](#-key-features) • [📖 Документация](#-documentation) • [💰
Цены](#-pricing-at-a-glance) • [💬
WhatsApp](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

</div>

🌐 {**Доступно в:**} 🇺🇸 [Английский](README.md) | 🇧🇷 [Португальский
(Бразилия)](docs/i18n/pt-BR/README.md) | 🇪🇸 [Испанский](docs/i18n/es/README.md)
| 🇫🇷 [Французский](docs/i18n/fr/README.md) | 🇮🇹
[Итальянский](docs/i18n/it/README.md) | 🇷🇺 [Русский](docs/i18n/ru/README.md) |
🇨🇳 [Китайский (упрощенное)](docs/i18n/zh-CN/README.md) | 🇩🇪
[Немецкий](docs/i18n/de/README.md) | 🇮🇳 [Хинди](docs/i18n/in/README.md) | 🇹🇭
[Тайский](docs/i18n/th/README.md) | 🇺🇦 [Украинский](docs/i18n/uk-UA/README.md) |
🇸🇦 [Арабский](docs/i18n/ar/README.md) | 🇯🇵 [Японский](docs/i18n/ja/README.md) |
🇻🇳 [Тьет Вьет](docs/i18n/vi/README.md) | 🇧🇬 [Болгарский](docs/i18n/bg/README.md)
| 🇩🇰 [Датский](docs/i18n/da/README.md) | 🇫🇮 [Финский](docs/i18n/fi/README.md) |
🇮🇱 [Иврит](docs/i18n/he/README.md) | 🇭🇺 [Венгерский](docs/i18n/hu/README.md) |
🇮🇩 [Индонезийский](docs/i18n/id/README.md) | 🇰🇷
[Корейский](docs/i18n/ko/README.md) | 🇲🇾 [Малайский](docs/i18n/ms/README.md) |
🇳🇱 [Нидерландский](docs/i18n/nl/README.md) | 🇳🇴
[Норвежский](docs/i18n/no/README.md) | 🇵🇹 [Португальский
(Португалия)](docs/i18n/pt/README.md) | 🇷🇴 [Румынский](docs/i18n/ro/README.md) |
🇵🇱 [Польский](docs/i18n/pl/README.md) | 🇸🇰 [Словак](docs/i18n/sk/README.md) | 🇸🇪
[Шведский](docs/i18n/sv/README.md) | 🇵🇭 [Филиппинский](docs/i18n/phi/README.md)
| 🇨🇿 [Чешский](docs/i18n/cs/README.md)

---

## 🆕 Что нового в версии 3.0.0

> **Обновляю из v2.9.5?** — Смотрите полный CHANGELOG для всех изменений.

| Площадка                           | Изменение                                                                                                                                                                                      |
| ---------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🔒 **CodeQL Безопасность**          | Исправлены 10+ alertов CodeQL: polynomial-redos, insecure-randomness, shell-injection remediation                                                                                              |
| ✅ **Регистрация маршрутов**        | Все 176 API-рутоны теперь валидированы с помощью шаблонов Zod + `validateBody()` — CI `check:route-validation:t06` проходит                                                                    |
| 🐛 **омниМодель Случайная метка**   | Внутренние `&lt;омниМодель&gt;` метки больше не передаются клиентам в SSE-струйных ответах (#585)                                                                                              |
| 🔑 **Зарегистрированные API-Ключи** | Автоматически создавайте API-ключи через `POST /api/v1/зарегистрированные-ключи` с ежемесячной квотой на провайдера/аккаунт, idempotency, SHA-256, и требующей необязательного отчета о GitHub |
| 🎨 **Иконки поставщиков**           | 130+ логотипов провайдеров через `@lobehub/icons` (SVG) со сбоями на PNG → цепочке generic fallback                                                                                            |
| 🔄 Автосинхронизация ** модели**    | 24-часовая задача и ручной UI-кнопка для синхронизации списков моделей для встроенных и настраиваемых провайдеров OpenAI                                                                       |
| 🌐 **OpenCode Zen/Go**              | Два новых провайдера от @kang-heewon через PR #530: бесплатный тариф и подписной тариф через `OpencodeExecutor`                                                                                |
| 🐛 **Gemini CLI OAuth**             | Отображение ошибки при отсутствии `GEMINI_OAUTH_CLIENT_SECRET` в Docker (была криптическая ошибка Google)                                                                                      |
| 🐛 **OpenCode конфиг**              | `saveOpenCodeConfig()` теперь корректно записывает конфиг TOML в `XDG_CONFIG_HOME`                                                                                                             |
| 🐛 **Закреплённая модель**          | `body.model` теперь корректно устанавливается в `pinnedModel` на защиту кэша контекстов                                                                                                        |
| 🐛 **Методика Кодекс/Клод.loop**    | `tool_result` теперь конвертируется в текст, чтобы остановить бесконечный цикл                                                                                                                 |
| 🐛 **Перенаправление авторизации**  | Авторизация artık не блокируется после пропуска настройки пароля                                                                                                                               |
| 🐛 **Пути Windows**                 | Пути MSYS2/Git-Bash (`/c/...`) нормализуются в `C:\...` автоматически                                                                                                                          |

---

## 🖼️ Основная Ленты Новостей

<div align="center">
  <img src="./docs/screenshots/MainOmniRoute.png" alt="OmniRoute Dashboard" width="800"/>
</div>

---

## 📸 Предварительный просмотр Ленты Новостей

<details>
<summary><b>Click to see dashboard screenshots</b></summary>

| Страница                         | Скриншот                                                           |
| -------------------------------- | ------------------------------------------------------------------ |
| **Поставщики**                   | ![Поставщики](docs/screenshots/01-providers.png)                   |
| **Комбошки**                     | ![Комбошки](docs/screenshots/02-combos.png)                        |
| **Аналитики**                    | ![Аналитики](docs/screenshots/03-analytics.png)                    |
| **Здоровье**                     | ![Здоровье](docs/screenshots/04-health.png)                        |
| **Переводчик**                   | ![Переводчик](docs/screenshots/05-translator.png)                  |
| **Настройки**                    | ![Настройки](docs/screenshots/06-settings.png)                     |
| **Инструменты командной строки** | ![Инструменты командной строки](docs/screenshots/07-cli-tools.png) |
| **Журналы использования**        | ![Журналы использования](docs/screenshots/08-usage.png)            |
| [K2X]Кнопка Ботом                | ![Поставщики](docs/screenshots/09-endpoint.png)                    |

</details>

---

### Аи Бот служит бесплатным провайдером для любимых технических акцентов!

_Подключите любой IDE или CLI-инструмент с поддержкой ИИ через OmniRoute —
бесплатный API-шлюз для неограниченного кодинга._

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

<sub>📡 Всі агенты подключаются через <code>http://localhost:20128/v1</code> или
<code>http://cloud.omniroute.online/v1</code> — одна конфигурация,
неограниченные модули и квота</sub>

---

## 🤔 Почему OmniRoute?

**Не тратите деньги и не превышайте лимиты:**

- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Срок действия подписки истекает ежемесячно и остается незатраченным
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Лимиты тарифов останавливают работу по кодингу посредине
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Дорогие API ($20-50/месяц на провайдера)
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Переключение между провайдерами вручную

**OmniRoute решает эту проблему:**

- ✅ **Максимизируйте подписки** - Следите за квотой, используйте каждую часть до
  сброса
- ✅ **Авто fallback** - Подписание → АИДИ -> Cheap → Бесплатно, нулевой сбой
- ✅ **Многоаккаунты** - Включение-выключение между аккаунтами на провайдера
- ✅ **Универсальность** - Работает с Claude Code, Codex, Gemini CLI, Cursor,
  Cline, OpenClaw, любым CLI-инструментом

---

## 📧 Поддержка

> 💬 **Подключитесь к нашей сообществе!** [WhatsApp
> Группа](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t) — Получите
> помощь, поделитесь подсказками и обновляйтесь.

- **Сайт**: [omniroute.online](https://omniroute.online)
- **GitHub**:
  [github.com/diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute)
- **Иссьюс**:
  [github.com/diegosouzapw/OmniRoute/issues](https://github.com/diegosouzapw/OmniRoute/issues)
- **WhatsApp**: [Группа
  компьютера](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)
- **Привычение**: Подайте ПР, или выберите `хороший первый вопрос`
- **Оригинальный Проект**: [9роутер от
  decolua](https://github.com/decolua/9router)

### 🐛 ЗАПОМНИТЕ ПРОБЛЕМУ?

Когда создаёте выпад, пожалуйста, запустите команду system-info и приложите
сгенерированный файл:

```bash
npm run system-info
```

Этот файл — `system-info.txt` — содержит версию Node.js, версию OmniRoute,
подробности ОС, установленные командные инструменты (iflow, gemini, claude,
codex, antigravity, droid и тд), статус Docker/PM2 и системные пакеты — всё, что
нужно для быстрого воспроизведения вашей проблемы. Приложите файл напрямую к
выпаду GitHub.

---

## Как это работает

```
┌─────────────┐
│  Ваша CLI   │  (Claude Code, Codex, Gemini CLI, OpenClaw, Cursor, Cline...)
│   Инструмент │
└──────┬──────┘
       │ http://localhost:20128/v1
       ↓
┌─────────────────────────────────────────┐
│           OmniRoute (Smart Router)        │
│  • Редактирование формата (OpenAI ↔ Claude) │
│  • Трекинг квоты + Embeddings + Images │
│  • Автоперезагрузка токенов                  │
└──────┬──────────────────────────────────┘
       │
       ├─→ [Тариф 1: ПОДПИСКА] Claude Code, Codex, Gemini CLI
       │   ↓ квота exhausted
       ├─→ [Тариф 2: API KEY] DeepSeek, Groq, xAI, Mistral, NVIDIA NIM, и тд
       │   ↓ лимит бюджета
       ├─→ [Тариф 3: ДОСТАНОВКА] GLM (0,6 доллара/млн), MiniMax (0,2 доллара/млн)
       │   ↓ лимит бюджета
       └─→ [Тариф 4: БЕСПЛАТНО] iFlow, Qwen, Kiro (безлимитные)

Результат: Никогда не останавливайте кодирование, минимальные затраты
```

---

## 🎯 Решение, которое предлагает OmniRoute — 30 актуальных проблем и сценариев использования

> **У каждого разработчика есть проблемы с АИ-инструментами, которые встречаются
> каждый день.** OmniRoute создан для решения всех них — от превышения бюджета
> до региональных блокировок, от перечеркнутых OAuth-flow до операций протоколов
> и корпоративной наблюдаемости.

<details>
<summary><b>💸 1. "I pay for an expensive subscription but still get interrupted by limits"</b></summary>

Развлекатели платят $20–200/месяц за Claude Pro, Codex Pro или GitHub Copilot. И
даже платя, квота имеет потолок — 5h использования, еженедельные ограничения или
ограничение одной минуты. В середине сессии разработчик теряет поток и
продуктительность.

**Как OmniRoute решает проблему:**

- **Умная 4-уровневаяFallback** — при истечение квоты подписки автоматически
  перенаправляет на API Key →Cheap →БЕСПЛАТНО с нулевым вмешательством
- **Реальное время Трекинг-quota** — показывает потребление токенов в реальном
  времени с подсчётом сброса (5h, дневное, еженедельное)
- **Многоуровневая поддержка Подписки** — множество Подписок на одного
  провайдера с АВТО-моментом
- **Связанные КOMBos** — пользовательские цепочки Перехода с 6 стратегиями
  балансирования (Первым, Круговым, РУ П2К, Случайным, Используемым, Быстрым)
- **Ограничения квоты для Клауде-Бизнес** — подсчет квот бизнес/командного
  рабочего места непосредственно в панели управления

</details>

<details>
<summary><b>🔌 2. "I need to use multiple providers but each has a different API"</b></summary>

OpenAI использует один формат, Клауде (Anthropic) — другой, Gemini — ещё один.
Если дев хочет протестировать модели с разных провайдеров или переключаться
между ними, нужно перепрограммировать SDK, измениить конечные точки, справиться
с неподдерживаемыми форматами. Кастом-браузеры (FriendLI, NIM) имеют нетипичные
конечные точки.

**Как OmniRoute решает проблему:**

- **Одного конечного уравнения** — один `http://localhost:20128/v1` играет роль
  прокси для всех 67+ провайдеров
- **Перевод формата** — Авторизованный и прозрачный: OpenAI ↔ Claude ↔ Gemini ↔
  Responses API.
- **Обработка Ответов** — Устраняет некондиционные поля (`х_groq`,
  `использование_в расчета`, `обслуживаемый_уровень`) от OpenAI SDK v1.83+
- **Нормализация Роли** — Преобразует `разработчик` → `системный` для
  провайдеров, не являющихся OpenAI; `системный` → `пользователь` для GLM/ЕРНИ
- **Извлечение Блоков <think> ** — Извлекает `<think>` блоки из моделей, таких
  как DeepSeek R1 и предназначает их для стандартизированного `содержимого
  reasonign`</think></think>
- **Структурированный Вывод для Жемини** — Automatic конвертация json_schema` в
  responseMimeType`/responseSchema`
- ** `stream` по умолчанию равно `false`** — Поддерживает спецификацию OpenAI,
  избегая неожиданных SSE в Python/E.Rust/Go SDK-ах

</details>

<details>
<summary><b>🌐 3. "My AI provider blocks my region/country"</b></summary>

Провайдеры, такие как OpenAI/Кодекс, блокируют доступ из определенных
географических регионов. Пользователи сталкиваются с ошибками, такими как `не
поддерживаемая страна/регион/территория` во время OAuth и API-соединений, что
особенно frustrates разработчиков из развивающихся стран.

**Как OmniRoute решает проблему:**

- **3-Уровневая конфигурация прокси** — Конфигурируемый прокси на 3 уровня:
  глобальный (всё трафик), на основе провайдера ( только для провайдера) и на
  основе соединения/ключа
- **Количественные Индикаторы Прокси** — Визуальные индикаторы: 🟢 глобальный
  прокси, 🟡 на основе провайдера, 🔵 для соединения прокси; всегда отображать IP
- **Обмен OAuth через Прокси** — OAuth-flow проходит через прокси и решает `не
  поддерживаемая стран/регион/территория`
- **Проверка Соединения через Прокси** — Проверка соединения использует
  настроенный прокси (без прямого обхода)
- **Поддержка SOCKS5** — Полная поддержка SOCKS5 прокси для маршрутизации данных
- **Уловка Фингерпринта TLS** — Browser-like фингерпринт TLS, используемый в
  wreq_js`, для обмана бот-детекции
- **CLI- совместимое Умение Печать Фингерпринта** — Переставляет заголовки и
  поля тела, чтобы совпадать с естественной фирмой CLI, существенно уменьшая
  риск флаги счета. Прокси IP сохраняется для предоставления одновременно
  stealth ** и IP-скрытия **

</details>

<details>
<summary><b>🆓 4. "I want to use AI for coding but I have no money"</b></summary>

Не каждый может поддерживать стоимость $20–200/месяц для подписки AI. Студенты,
разработчики из развивающихся стран, хоббисты и freelancers нуждаются в доступе
к качественным моделям, обходящимся им в ноль.

**Как OmniRoute решает проблему:**

- **Нативная поддержка Политекий Провайдер[Т30X] — Поддержка провайдеров за 100%
  бесплатных: iFlow (5 моделей нетаких, к примеру: kimi-k2-thinking,
  qwen3-coder-plus, deepseek-r1, minimax-m2, kimi-k2), qwen3-coder-plus (4
  модели безлимитных: qwen3-coder-plus, qwen3-coder-flash, qwen3-coder-next,
  vision-model), Kiro (Claude + AWS-Buidler ID за бесплатно) для Gemini CLI
  (180K токенов/месяц бесплатных)
- **Оболас Cloud** — Хостинг облаци для модели Олламы через api.ollama.com`;
  free 'Light Использование' уровень; использовать prefix ollamacloud/
  &lt;модель&gt;`
- **Свободные Режимы Моделей** — Поскольку gc/gemini-3-flash →
  if/kimi-k2-thinking → qw/qwen3-coder-plus` = $0/месяц без паузы
- **НУВИДА Free Access** — Равно 40 RPM разряда для модели forever для free, в
  70+ моделей через build.nvidia.com (переход из кредитов на чистые линции
  ограничение)
- **ОптимизированнаяStrategy поCost** — маршрутная стратегия, автоматически
  выбирающая дешевый доступный провайдер

</details>

<details>
<summary><b>🔒 5. "I need to protect my AI gateway from unauthorized access"</b></summary>

Когда вы exposing AI-шлюз в сеть (LAN, VPS, Docker), любой пользователь с
адресом может потреблять токены/квоту разработчика. Без защиты API уязвимы для
злоупотребления, внедрения заплат и злоупотреблений.

**Как OmniRoute решает проблему:**

- **Управление API-ключами** — Генерация, вращение и ограничение по провайдеру с
  помощью отдельной `страницы Контроль API-ключами/dashboard/api-manager`
- **Уровневая регулинка модели** — Ограничить API-ключи конкретными моделями
  (`openai/*`, шаблоны дирижанного значения), с Allow All./Restrict
  переключателем
- **Защита API-конца** — требует ключа для `/v1/models` и блокирует конкретных
  провайдеров из списка
- **Защита при авторизации + Защиту CSRF/** — Все маршруты панели защиты с
  `withAuth` middleware + токенами CSRF
- **Ограничик скорости** — Ограничик скорости для IP по умолчанию
- **Фильтрация IP** — Допустимый/запрещенный список для управления доступом
- **Защита до инъекции заплат** — Санитизация против вредоносных шаблонов заплат
- **Шифрование AES-256-GCM** — Кридентали зашифрованы

</details>

<details>
<summary><b>🛑 6. "My provider went down and I lost my coding flow"</b></summary>

Провайдеры могут стать нестабильными, возвращать ошибки 5xx или выйти из строя
из-за кратковременной блокировки скорости. Если разработчик полагается на одного
провайдера, он разрывается. Без автоотключателей повторные запросы могут вызвать
сбой приложения

**Как OmniRoute решает проблему:**

- **Автоотключатель на модель** — Автооткрытие/закрытие с конфигурацией порога и
  задержки (Closed/Open/Half-Open), упраженном на модели для предотвращения
  шумового эффекта
- **ЭкспоненциальнойBackoff** — Прогрессивные задержки повторных запросов
- **Приемник за предотвращение конкуривущих Herd** Mutex + семафор защищает
  ожидание одновременного шторма повторных запросов
- **Серверное переключание по комбайну ** — Автоматическое переключение на
  резервный сервер
- **Кома автоавалактор с комбаином ** — Автожблает провайдеры в комбаине
- **Дашборд здоровья ** — Уptime, режимы автоматического отключения, блокировка

</details>

<details>
<summary><b>🔧 7. "Configuring each AI tool is tedious and repetitive"</b></summary>

Развейторы используют Cursor, Claude Code, Codex CLI, OpenClaw, Gemini CLI, Kilo
Code... Каждый инструмент требует отдельной конфигурации (конечной точки API,
ключа, модели). Перестановка конфигурации при переключении между провайдерами
моделями отнимает уйму времени.

**Как OmniRoute решает проблему:**

- **Панель инструментов CLI** — Задизайненный раздел с одной кнопкой для
  настройки для Claude Code, Codex CLI, OpenClaw, Kilo Code, Antigravity, Cline
- **Плагины GitHub Copilot** — Генерируют `чатЛВС.json` для VS Code с глобальным
  выбором моделей
- **Уživаемая настройка** — Руководство по 4 стадиам настройки для пользователей
- **Один интерфейс, все模型ы** — Определите `http://localhost:20128/v1` один раз,
  получить доступ к 67+ поставщиков

</details>

<details>
<summary><b>🔑 8. "Managing OAuth tokens from multiple providers is hell"</b></summary>

Claude Code, Codex, Gemini CLI, Copilot — все используют OAuth 2.0 с
экспирающими токенами. Разработчикам нужно повторно авторизоваться постоянно,
deal с `отсутствием секрета клиента`, `несовпадением redirect_uri`, и неудачей
на удаленных серверах. OAuth на LAN/VPS особенно проблематичен

**Как OmniRoute решает проблему:**

- **Автообновление токенов** — OAuth-туки обновляются в фоновом режиме до
  истечения срока
- **Встроенный OAuth 2.0 (PKCE)** — Автоматические потоки для Claude Code,
  Codex, Gemini CLI, Copilot, Kiro, Qwen, iFlow
- **Работа с множеством учетными данными OAuth** — Множественные аккаунты в
  провайдере методом JWT/ID токенов
- **Коррекция OAuth LAN/Remote** — Речивная IP-detection для `redirect_uri` +
  ручной способ URI режимов для удаленных серверов
- **OAuth за Nginx** — Использует ` window.location.origin` для совместимости
  отраженного прокси сервера
- **Руководство по Remote OAuth** — КРОК-руководство по Google Cloud учетной
  записи ВПС/Докерк

</details>

<details>
<summary><b>📊 9. "I don't know how much I'm spending or where"</b></summary>

Разработчики используют несколько платных провайдеров, но не имеют единого вид
на стоимость. Каждый провайдер имеет свой собственный балансный диспетчер, но
нет консолидированного показателя. Непредвиденные затраты могут стагнировать.

**Как OmniRoute решает проблему:**

- **Аналитика доходов** — Трекинг и управление бюджетом в провайдере по токенам
- **Бюджетные ограничения в каждой тюбр** — Уровни расхода за тротуя который
  приводит к автоматкуя переключение
- **Настройка цен модели** — Настраиваемые цены каждый-модели
- **Статистика использования API ключа** — Количество последний-задействованный
  временв штадт по ключу
- **Панель контроля аналитики** — Карты статистики, диаграмма использования
  модели, таблица провайдерам с успеховой скидки и задержки.

</details>

<details>
<summary><b>🐛 10. "I can't diagnose errors and problems in AI calls"</b></summary>

==WEBLATE_PART==\
Когда происходит неудачный вызов, разработчик не знает, почему это произошло:
слишком частые запросы, просроченный токен, неправильный формат или ошибки
провайдера. Разбросанные логи по разным терминалам без возможности наблюдения
делают отладку пробой-побой.

**Как OmniRoute решает проблему:**

- **Unified Logs Dashboard** — 4 вкладки: Логи запросов, логи прокси, журналы
  аудита, Консоль
- **Console Log Viewer** — Реактивное просмотрщик консольных дражжлв с цветовой
  кодировкой уровней, автоматической прокруткой, поиском и фильтром
- **SQLite Proxy Logs** — Пролонгированные логи, сохраняющиеся после
  перезагрузки сервера
- **Translator Playground** — 4 режима отладки: Плажарта (перевод формата),
  Чат-Тестер (пробный обход), Тест-Бенч (блочная отдача), Живая Мониторинг
  (реактивное следование)
- **Request Telemetry** — p50/p95/p99 замедление + Tracing X-Request-Id
- **File-Based Logging с Rotation** — Интерцептор Консоль, сохраняющий все логи
  в JSON формате с размерной подстановкой
- **System Info Report** — `npm run system-info` — генерация отчета о системе
  (Versiya Node, OmniRoute, OS, инструменты CLI, Docker/PM2). При отправке
  ошибок приложите этот файл для быстрой стадируюстициии

</details>

<details>
<summary><b>🏗️ 11. "Deploying and maintaining the gateway is complex"</b></summary>

Установка, настройка и поддержание работы АИ-прокси в различных средах
(локально, VPS, Docker, облаке) требует значительных усилий. Проблемы типа
закодированных путей, `EACCES` в каталогах, конкурирующие порты и
кроссплатформенные сборки добавляют трение.

**Как OmniRoute решает проблему:**

- **npm global install** — `npm install -g omniroute &amp;&amp; omniroute` —
  выполнено
- **Docker Multi-Platform** — nat. AMD64 + ARM64 (Apple Silicon, AWS Graviton,
  Raspberry Pi)
- **Docker Compose Profiles** — `base` (без CLI инструментов) и `cli` (с Claude
  Code, Codex, OpenClaw)
- **Electron Desktop App** — Нативная приложение для Windows/macOS/Linux с
  системным чашечкой, автоматической стартом, отключением
- **Split-Port Mode** — API и ДASHBOARD на отдельных портах для продвинутых
  сценариев (внутренний прокси, сетевое контейнеризовоние)
- **Cloud Sync** — синхронизация конфигурации на устройствах с помощью Воркеров
  Cloudflare
- **DB Backups** — Автоматическое резервное копирование, восстановление,
  экспортирование и импортирование всех настроек

</details>

<details>
<summary><b>🌍 12. "The interface is English-only and my team doesn't speak English"</b></summary>

Команды из стран с другими языками, особенно в Латинской Америке, Асии и Еуропе,
сталкиваются с английской-совокупной интерфейсами. Пограничные барьеры снижают
уровень приминенияя и увеличивают ошибки настроика.

**Как OmniRoute решает проблему:**

- **Панель управления i18n — 30 языков** — Все 500+ ключей переведены, включая
  арабский, болгарский, датский, немецкий, испанский, финский, французский,
  иврит, хинди, венгерский, индонезийский, итальянский, японский, корейский,
  малайский, нидерландский, норвежский, польский, португальский (PT/BR),
  румынский, русский, словацкий, шведский, тайский, украинский, вьетнамский,
  китайский, тайский, английский]
- **Поддержка RTL** — Правильная поддержка слева направо для арабского и иврита
- **Мультilingual READMEs** — 30 полных перевадов документации
- **Показатель языка** — Глобальный значек в хедере для реального времени
  переключения

</details>

<details>
<summary><b>🔄 13. "I need more than chat — I need embeddings, images, audio"</b></summary>

Программирование не только состоит в дополнении диалога. Разработчикам нужны
тоже генерировать изображения, транскрибировать аудио, создавать векторы для
RAG, перечеркивать документы, и модерировать контент.

**Как OmniRoute решает проблему:**

- **Векторные представления** — ` /v1/embeddings` с 6 провайдерами и 9+ моделями
- **Генерация картинок** — ` /v1 /images/поколений ` с 10 провайдерами и 20+
  моделями (OpenAI, xAI, Together, Fireworks, Nebius, Hyperbolic, NanoBanana,
  Antigravity, SD WebUI, ComfyUI)
- **Перевод текста в видео** — ` /v1/видео/генерации ` — ComfyUI (AnimateDiff,
  SVD) и SD WebUI
- **Перевод текста в музыку** — ` /v1/музыку/генерации ` — ComfyUI (Stable Audio
  Open, MusicGen)
- **Перевод аудио в текст** — ` /v1/аудио/переводов ` — Whisper + Nvidia NIM,
  HuggingFace, Qwen3
- **Голосовой синтез** — ` /v1/аудио/голоса ` — ElevenLabs, Nvidia NIM,
  HuggingFace, Coqui, Tortoise, Qwen3, ** Inworld **, ** Cartesia **, ** PlayHT
  ** . + существующих провайдеров
- **Фильтрация контента** — ` / v1/фильтрации ` — Контроль безопасности контента
- **Пересортировка документа** — ` /v1/пересортировка ` — Пересортировка
  документа по степени релевантности
- **API-ответов** — Полная поддержка ` /v1/ответов ` для Codex

</details>

<details>
<summary><b>🧪 14. "I have no way to test and compare quality across models"</b></summary>

Разработчикам хочется узнать, какая модель лучше всего подойдет для их проекта
по code, переводу, поиску, а но сравнивать вручную долго. Нет интегрированных
инструментов для оценки.

**Как OmniRoute решает проблему:**

- **Оценка МЛМ** — Золотое тестирование с 10 пред-налаштированными случаями,
  охватывающими приветствия, математические задачи, географию, code генерацию,
  json проверку, перевод, markdown, безопасное отторжение
- ** 4 стратегии соответствия** — ` точное ` содержит `, ` регекс `, `
  персональное ` (функция js )
- **Острова переводчиков. Тестовая рабочая область** — Блочное тестирование с
  множеством входных и ожидаемых выходов, сравнение провайдеров в хроме
- **Chat Tester** — Full round-trip with visual response rendering
- **Live Monitor** — Real-time stream of all requests flowing through the proxy

</details>

<details>
<summary><b>📈 15. "I need to scale without losing performance"</b></summary>

As request volume grows, without caching the same questions generate duplicate
costs. Without idempotency, duplicate requests waste processing. Per-provider
rate limits must be respected.

**Как OmniRoute решает проблему:**

- **Semantic Cache** — Two-tier cache (signature + semantic) reduces cost and
  latency
- **Request Idempotency** — 5s deduplication window for identical requests
- **Rate Limit Detection** — Per-provider RPM, min gap, and max concurrent
  tracking
- **Editable Rate Limits** — Configurable defaults in Settings → Resilience with
  persistence
- **API Key Validation Cache** — 3-tier cache for production performance
- **Health Dashboard with Telemetry** — p50/p95/p99 latency, cache stats, uptime

</details>

<details>
<summary><b>🤖 16. "I want to control model behavior globally"</b></summary>

Developers who want all responses in a specific language, with a specific tone,
or want to limit reasoning tokens. Configuring this in every tool/request is
impractical.

**Как OmniRoute решает проблему:**

- **System Prompt Injection** — Global prompt applied to all requests
- **Thinking Budget Validation** — Reasoning token allocation control per
  request (passthrough, auto, custom, adaptive)
- **6 Routing Strategies** — Global strategies that determine how requests are
  distributed
- **Wildcard Router** — `provider/*` patterns route dynamically to any provider
- **Combo Enable/Disable Toggle** — Toggle combos directly from the dashboard
- **Provider Toggle** — Enable/disable all connections for a provider with one
  click
- **Blocked Providers** — Exclude specific providers from `/v1/models` listing

</details>

<details>
<summary><b>🧰 17. "I need MCP tools as first-class product capabilities"</b></summary>

Many AI gateways expose MCP only as a hidden implementation detail. Teams need a
visible, manageable operation layer.

**Как OmniRoute решает проблему:**

- МКП отображается в навигации панели управления и вкладке протокола точки
  доступа
- Отдельная страница управления МКП с процессом, инструментами, областью
  видимости и аудитом
- Встроенная скорая поставка для `омниярута — мкп` и клиентского настройки

</details>

<details>
<summary><b>🧠 18. "I need A2A orchestration with sync + stream task paths"</b></summary>

Рабочие процессы агента требуют как прямых ответов, так и длительной
потоко-ориентированной исполнения с функцией контроля жизненного цикла

**Как OmniRoute решает проблему:**

- JSON-RPC API точки-ко-точки (`POST /a2a`) с `очередью/отправить` и
  `очередью/поток`
- Сжатый поток с терминальным состояниям распространением
- API životного цикла задач для `задачи/получить` и `задачи/отменить`

</details>

<details>
<summary><b>🛰️ 19. "I need real MCP process health, not guessed status"</b></summary>

Оперативные команды должны знать, жив МКП или нет, а не только доступность API

**Как OmniRoute решает проблему:**

- Файл heartbeat времени работы с PID, метками времени, транспорт, количество
  инструментов и режим области видимости
- API состояния МКП, объединяющая heartbeat + недавняя активность
- Коллекции статуса UI для процесс/uptime/freshess heartbeat

</details>

<details>
<summary><b>📋 20. "I need auditable MCP tool execution"</b></summary>

Когда инструменты поменяем конфигурацию или действуют на действия оповещения,
команды нужно иметь следы отследимость.

**Как OmniRoute решает проблему:**

- Логирование аудит SQLite для МКП, обслуживания инструментом
- Фильтры с помощью инструмента, успех/неудача, ключ оповещения, и pagination
- Таблица аудита панели управления + статистика API для автоматизации

</details>

<details>
<summary><b>🔐 21. "I need scoped MCP permissions per integration"</b></summary>

Различных клиентов должны иметь наименьшее привилегирование доступа к категориям
инструментов.

**Как OmniRoute решает проблему:**

- 9 крупных сфер управления доступом к контролируемым инструментам
- Управление видимостью и согласованием в интерфейсе управления MCP
- Безопасное базовое положение для эксплуатационных инструментов

</details>

<details>
<summary><b>⚙️ 22. "I need operational controls without redeploying"</b></summary>

Командам требуется быстрое изменение на лету во время инцидентов или событий по
стоимости.

**Как OmniRoute решает проблему:**

- Активация переключателя комбинации напрямую из диспетчера MCP
- Применение профилей устойчивости из готовых наборов политик
- Resetти state-автомата с одного и того же панели операций

</details>

<details>
<summary><b>🔄 23. "I need live A2A task lifecycle visibility and cancellation"</b></summary>

Без видимости по жизни, триггерные события-任务 становятся сложными для триговки.

**Как OmniRoute решает проблему:**

- Построение списка задач/фильтрация по статусу/навыку с пагинацией
- Детализация данных задач, событий и артефактов
- Пункт для отмены задачи и UI-акция с подтверждением отказа

</details>

<details>
<summary><b>🌊 24. "I need active stream metrics for A2A load"</b></summary>

Приливные потоки требуют оперативного вопролнения в реальном время с видимостью
concurrency и живых соединений.

**Как OmniRoute решает проблему:**

- Активные показатели счетчиков интегрированы в статус A2A
- Последняя метка времени задачи и счетчики по состоянию
- Диспетчерские визуальные панели A2A для реального времени мониторинга операций

</details>

<details>
<summary><b>🪪 25. "I need standard agent discovery for clients"</b></summary>

Внешним клиентам и орекстляторам нужно machine-readable данные-метаданные для
подстановки \
==WEBLATE_PART==

**Как OmniRoute решает проблему:**

- Карта агента открыта в `/well-known/agent.json`
- В hiểnчики управления отображаются способности и навыки пользователя
- API A2A статус содержит справочную информацию для автоматизации

</details>

<details>
<summary><b>🧭 26. "I need protocol discoverability in the product UX"</b></summary>

Если пользователи не могут обнаруживать протокол поверхности, снижается качество
принятия и поддержки.

**Как OmniRoute решает проблему:**

- Координированная ** страница конечных точек[endpoints], содержащая вкладки для
  прокси, MCP, A2A и API конечных точек.
- Влево inline статистики сервиса (Онлайн/Офлайн) MCP и A2A
- Ссылки в сводке на отдельные вкладки управления

</details>

<details>
<summary><b>🧪 27. "I need end-to-end protocol validation with real clients"</b></summary>

Проверочные тесты не достаточно для валидации совместимости протокола перед
выпуском.

**Как OmniRoute решает проблему:**

- Пленарный пакет с тестами, загружающий приложение и использующий реальный
  клиент транспорт MCP.
- Тесты клиента A2A для поиска, передачи, потоков, чтения и отмены потоков
  запросов
- Перекрестное сравнение утверждений от MCP аудита и задач A2A API.

</details>

<details>
<summary><b>📡 28. "I need unified observability across all interfaces"</b></summary>

Разделение функции наблюдения по протоколам создает зоны слепоте и увеличивает
скорость восстановления.

**Как OmniRoute решает проблему:**

- Единый рабочий стол для мониторинга, логов и аналитики в одном продукте.
- Здоровье и аудит + запрос на заявление на всех слоях OpenAI, MCP и A2A.
- Операционные API статуса и автоматизации

</details>

<details>
<summary><b>💼 29. "I need one runtime for proxy + tools + agent orchestration"</b></summary>

Выполнение многих отдельных сервисов приводит к увеличению операционных затрат и
способов сбоя.

**Как OmniRoute решает проблему:**

- Сервис прокси, MCP-сервер и A2A-сервер в один стек
- Общий доступ к базе данных, отказоустойчивость, хранение данных и мониторинг
- Целостная модель политики для всех поверхностей взаимодействия

</details>

<details>
<summary><b>🚀 30. "I need to ship agentic workflows without glue-code sprawl"</b></summary>

Командам становится хуже работать, когда им приходится стыковать множество
отдельных служб и скриптов.

**Как OmniRoute решает проблему:**

- Объединенная стратегия точки входа для клиентов и агентов
- Встроенные интерфейсы управления протоколами и проверка подгоночных путей
- Основания, производимые в production (безопасность, журнал,
  отказоустойчивость, резервное копирование)

</details>

### Примеры "планшетов" (Интегрированные случаи использования)

**Планшет A: Максимально использовать подписку + дешевый резерв

```txt
Комбо: "maximize-claude"
  1. cc/claude-opus-4-6
  2. glm/glm-4.7
  3. if/kimi-k2-thinking

Месячный затрат: $20 + малая затраты на резервное копирование
Итог: повышенная качество, близкое к нулю прерываний
```

**Планшет B: Некоштный набор для кодирования

```txt
Комбо: "free-forever"
  1. gc/gemini-3-flash
  2. if/kimi-k2-thinking
  3. qw/qwen3-coder-plus

Месячной стоимость: $0
Результат: стабильный бесплатный рабочий процесс кодирования
```

**Планшет C: 24/7 всегда включенная цепочка резервного подстраховки

```txt
Комбо: "always-on"
  1. cc/claude-opus-4-6
  2. cx/gpt-5.2-codex
  3. glm/glm-4.7
  4. minimax/MiniMax-M2.1
  5. if/kimi-k2-thinking

Результат: глубокая глубина резервного подстраховки для критических обстоятельств по умолчанию.
```

**Планшет D: Перчатка агент с MCP + A2A

```txt
1) Запустите транспорт MCP (`омнироут - mcp`) для инструментально-ориентированных операций
2) выполните задачи A2A с помощью `сEND сообщение` и `сEND поток сообщений`
3) наблюдение через /dashboard/endpoint (МCP и A2A вкладки)
4) Переключить службы с помощью онлайн-контроли для состояния
```

---

## – – – Играть бесплатно на ноль-конфигурации

> Установить AI-кодирование не более 15 минут в месяц за **$0/мес.**. Подключите
> эти бесплатные аккаунты и воспользуйтесь встроенным **комбо бесплатное стек**.

| Step | Действие                                           | Providers Unlocked                                                 |
| ---- | -------------------------------------------------- | ------------------------------------------------------------------ |
| 1    | Connect **Kiro** (AWS Builder ID OAuth)            | Claude Sonnet 4.5, Haiku 4.5 — **unlimited**                       |
| 2    | Connect **iFlow** (Google OAuth)                   | kimi-k2-thinking, qwen3-coder-plus, deepseek-r1... — **unlimited** |
| 3    | Connect **Qwen** (Device Code)                     | qwen3-coder-plus, qwen3-coder-flash... — **unlimited**             |
| 4    | Connect **Gemini CLI** (Google OAuth)              | gemini-3-flash, gemini-2.5-pro — **180K/mo free**                  |
| 5    | `/dashboard/combos` → **Free Stack ($0)** template | Round-robin all free providers automatically                       |

**Point any IDE/CLI to:** `http://localhost:20128/v1` · API Key: `any-string` ·
Done.

> **Optional extra coverage (also free):** Groq API key (30 RPM free), NVIDIA
> NIM (40 RPM free, 70+ models), Cerebras (1M tok/day), LongCat API key (50M
> tokens/day!), Cloudflare Workers AI (10K Neurons/day, 50+ models).

## Быстрый старт

### 1. Установите и запустите

```bash
npm install -g omniroute
omniroute
```

> **пнпм пользователи:** Запустите `пнпм approve-builds -g` после установки,
> чтобы.enable native build scripts, необходимые для `Better SQLite` и `
> @swc/core`:
> 
> ```bash
> пнпм install -g omniroute
> пнпм approve-builds -g   # Select all packages → approve
> omniroute
> ```

Быстрый запуск открывается в браузере по адресу `http://localhost:20128` и API
основной url находится по адресу `http://localhost:20128/v1`.

| Команда                 | Описание                                                                 |
| ----------------------- | ------------------------------------------------------------------------ |
| `omniroute`             | Запустить сервер ( `PORT=20128`, API и панель управления на одном порту) |
| `омniroute --port 3000` | Установить канонический порт для API в 3000                              |
| `омniroute --mcp`       | Запустить сервер МСП (транспорт stdio)                                   |
| `омniroute --no-open`   | Не запускать автоматически браузер                                       |
| `омniroute --помогить`  | Помощь                                                                   |

Набор дополнительных параметров для быстрой установки:

```bash
PORT=20128 DASHBOARD_PORT=20129 omniroute
# API:       http://localhost:20128/v1
# Dashboard: http://localhost:20129
```

### 1) Соедините провайдеров и создайте свой ключ API

1. Открите Дашборд → [Х17X]Провайдеры[Х27X] и подключите хотя бы один провайдер
   (OAuth или ключ API).
2. Открите Дашборд → [Х17X]Конечные точки[Х27X] и создайте ключ API.
3. (необязательно) Откройте Дашборд → [Х28X]Комбо[Х35X] и установите свой
   fallback-цепочку.

### 2) Поставьте в связь ваше инструментарие с OmniRoute.

```txt
URL основной страницы: http://localhost:20128/v1
Ключ API: [скопируйте с страницы Endpoint]
Модель:	if/kimi-k2-thinking (или любой префикс провайдера модели)
```

Поддерживает: Claude Code, Codex CLI, Gemini CLI, Cursor, Cline, OpenClaw,
OpenCode и SDK OpenAI-совместимые.

### 3) Включите и.validate протоколов (в2.0)

[Х0X]МКП (для инструментального взаимодействия):[Х35X]

```bash
omniroute --mcp
```

Затем подключите своё МКП-клаент через [Х34X]stdio[Х40X] и протестируйте
инструменты, такие как:

- [Х0X]omniroute_get_health[Х21X]
- [Х0X]omniroute_list_combos[Х22X]

[Х0X]А2А (для агент-агентных потоков):[Х37X]

```bash
curl http://localhost:20128/.well-known/agent.json
```

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"quickstart","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"Дайте мне краткий справочник квот."}]}}'
```

### 4) Валидация и проверка всего комплексно (рекомендуется)

```bash
npm run test:protocols:e2e
```

Этот комплект включает в себя проверку реальных клиентов МКП и А2А клиента
против работающего приложения.

### Альтернативное решение: выполнять из исходного кода.

```bash
cp .env.example .env
npm установить
PORT=20128 DASHBOARD_PORT=20129 NEXT_PUBLIC_BASE_URL=http://localhost:20129 npm run dev
```

---

## 🐳 Docker

OmniRoute доступно в качестве публичного образа Docker на [Docker
Hub](https://hub.docker.com/r/diegosouzapw/omniroute).

**Быстрый запуск:**

```bash
docker run -d \
  -e имя omniroute \
  --restart не остановить \
  -p 20128:20128 \
  -в omniroute-data:/апп/data \
  diegosouzapw/omniroute:последний
```

**С параметрами окружения:**

```bash
# Скопировать и отредактировать .env сначала
cp .env.example .env

docker run -d \
  -e имя omniroute \
  --restart не остановить \
  -е файла окружения .env \
  -p 20128:20128 \
  -в omniroute-data:/апп/данные \
  diegosouzapw/omniroute:последний
```

**Использование Docker Compose:**

```bash
# Основной профиль (без инструментов CLI)
docker.compose --profile base up -д

# Профиль CLI (Claude, Кодекс, OpenClaw встроенная)
docker.compose --profile cli up -d
```

| Изображение              | Тэг         | Размер | Описание                    |
| ------------------------ | ----------- | ------ | --------------------------- |
| `diegosouzapw/omniroute` | `последний` | ~250МБ | Последняя стабильная версия |
| `diegosouzapw/omniroute` | `1.0.3`     | ~250МБ | Текущая версия              |

---

## 🖥️ Desktop App — Offline & Always-On

> 🆕 **НОВОЕ!** OmniRoute теперь доступно как **native десктоп-приложение** под
> Windows, macOS и Linux.

Запускать OmniRoute можно как отдельное десктопное приложение — без командной
строки, браузера, интернета для местных моделей. Программа Electron включает в
себя:

- 🖥️ **Native Окно** — отдельное приложение с интеграцией в системную панель
- 🔄 **Авто-запуск** — запуск OmniRoute при входе в систему
- 🔔 **Нативные уведомления** — получение уведомлений о вытеснении квоты или
  проблемах провайдера
- ⚡ **Однократный установщик** — NSIS (Windows), DMG (macOS), AppImage (Linux)
- 🌐 **Режим Offline** — работает полностью в офлайн-режиме с вмонолитным
  сервером

### Быстрый старт

```bash
# Режим разработки
npm run electron:dev

# Построить для вашей платформы
npm run electron:build         # текущая платформа
npm run electron:build:win     # Windows (.exe)
npm run electron:build:mac     # macOS (.dmg) — x64 &amp; arm64
npm run electron:build:linux   # Linux (.AppImage)
```

### Панель системной области

Когда minimized, OmniRoute живет в системной области панели с быстрыми
действиями:

- Открыть панель управления
- Изменить порт сервера
- Выход из приложения

📖 Полное руководство: [`electron/README.md`](electron/README.md)

---

## 💰 Цены на взгляд

| Тариф           | Provider                      | Стоимость                                  | Сброс квоты                    | Лучшее для меня                                         |
| --------------- | ----------------------------- | ------------------------------------------ | ------------------------------ | ------------------------------------------------------- |
| **💳 ПОДПИСКА**  | Клод Код (Профессионал)       | $20/месяц                                  | 5ч + еженедельная              | Уже подписался                                          |
|                 | Codex (Плюс/Профессионал)     | $20-200/месяц                              | 5ч + еженедельная              | Пользователи OpenAI                                     |
|                 | Gemini CLI                    | **БЕСПЛАТНО**                              | 180К/месяц + 1К/день           | Для всех!                                               |
|                 | GitHub второй пилот           | $10-19/месяц                               | Ежемесячная                    | Пользователи GitHub                                     |
| **🔑 КЛЮЧ API**  | NVIDIA NIM                    | **БЕСПЛАТНО** (навсегда для разработчиков) | ~40 оборотов в минуту          | 70+ открытых моделей                                    |
|                 | Cerebras                      | **БЕСПЛАТНО** (1M ток/день)                | 60K TPM / 30 оборотов в минуту | Самая быстрая в мире                                    |
|                 | Groq                          | **БЕСПЛАТНО** (30 оборотов в минуту)       | 14.4K RPD                      | 超скорая Llama/Gemma                                     |
|                 | DeepSeek V3.2                 | $0.27/$1.10 за 1M                          | Нет                            | Лучшая цена/качество                                    |
|                 | xAI Grok-4 Fast               | **$0.20/$0.50 за 1M** 🆕                    | Нет                            | Быстрее всего + вызов инструментов, ультнизкая          |
|                 | xAI Grok-4 (стандарт)         | $0.20/$1.50 за 1M 🆕                        | Нет                            | Лидер разумения от xAI                                  |
|                 | Харви                         | Бесплатная пробная версия + платная        | Скорость ограничена            | Европейский ИИ                                          |
|                 | OpenRouter                    | Платная по использованию                   | Нет                            | 100+ аггрегированных моделей                            |
| **💰 ДЕШЕВОЙ**   | GLM-5 (через Z.AI) 🆕          | $0.5/1М                                    | По 10:00 каждый день           | 128К входных данных, самая последняя флагманская модель |
|                 | GLM-4.7                       | $0.6/1М                                    | По 10:00 каждый день           | Бюджетный резерв                                        |
|                 | MiniMax M2.5 🆕                | $0.3/1М входных данных                     | 5-часовой ролик                | Понимание + задачи с агентным поведением                |
|                 | MiniMax M2.1                  | ==WEBLATE_PART==\                          | 5-часовой ролик                | Самый дешёвый вариант                                   |
|                 | Kimi K2.5 (Lунный сбой API) 🆕 | Платная по использованию                   | Нет                            | Direктный доступ к API Lунный сбой                      |
|                 | Kimi K2                       | 9 $/мес фиксированная плата                | 10 млн токенов/мес             | Предсказуемый затратный                                 |
| **🆓 Бесплатно** | iFlow                         | **$0**                                     | LIMITLESS                      | Неограниченное количество моделей                       |
|                 | Qwen                          | **$0**                                     | LIMITLESS                      | Неограниченное количество моделей 4                     |
|                 | Kiro                          | **$0**                                     | LIMITLESS                      | Клод Сонет/Хайку (AWS Builder)                          |
|                 | Лонгкэт Флэш-Лайт 🆕           | ** $0** (50млн.токов/сутки 🔥)              | 1 RPS                          | Перегрузочная бесплатная квота на Земле                 |
|                 | Новинки Pollinations AI 🆕     | **$0** (без пароля)                        | 1 запрос/15с                   | GPT-5, Клод, DeepSeek, Ллама 4                          |
|                 | Cloudflare Workers AI 🆕       | **$0** (10K нейрон/день)                   | ~150 ответов/день              | 50+ модели, глобальный эдж                              |
|                 | Scaleway AI 🆕                 | **$0** (1М токенов общее)                  | Скорость ограничена            | EU/ГДПР, Qwen3 235B, Ллама 70B                          |

> 🆕 **Новые модели были добавлены (Март 2026):** Grok-4 Fast семейство по
> $0,20/$0,50/М (оценено в 1143мс – 30% быстрее, чем Gemini 2,5 Flash), GLM-5
> через Z.АЙ с 128К выход, MiniMax M2,5 рассуждения, DeepSeek V3,2 обновлённая
> цена, Kimi K2,5via Moonshot прямая API.

**💡 $0 Объединительный Стэк — Полный Бесплатный Объединитель:**

```
# 🆓 Ultimate Free Стэк 2026 — 11 Продавцов, $0 Вечно
Кирос (kr/)            → Клод Сонет/Хаику БЕЗ ГРАНИЦ
иФлоу (if/)            → кими-к2-мышление, qwen3-coder-plus, deepseek-r1 БЕЗ ГРАНИЦ
Длинный Кот Лайт (lc/)   → Длинный Кот-Flash-Лайт — 50М токенов/день 🔥
Популяции (пол/)       → ГПТ-5, Клод, DeepSeek, Ллама 4 — без пароля
Qwen (qw/)             → qwen3-coder-plus, qwen3-coder-flash, qwen3-coder-next БЕЗ ГРАНИЦ
Гемини (гемини/)      → Гемини 2,5 Flash — 1 500 запросов/день бесплатный API-ключ
Cloudflare AI (cf/)    → Ллама 70B, Гемма 3, Мистраль — 10К нейронов/день
Scaleway (scw/)        → Qwen3 235B, Ллама 70B — 1М бесплатных токенов (Евropa)
Грок (groq/)           → Ллама/Гемма сверхбыстрое — 14,4К запросов/день
НВИДИА НИМ (nvidia/)   → 70+ открытые модели — 40 РПМ навсегда
Серебрэс (cerebras/)   → Ллама/Qwen сверхбыстрый — 1М токенов/день
```

**Ноль стоимостей. Никогда не останавливается.** Configure это как один
OmniRoute комбо и все fallbacks начинаются автоматически — никакого ручного
переключения никогда.

---

---

## 🆓 Бесплатные модели — что вы на самом деле получаете

> Все модели ниже являются **100% бесплатными с нулевой картой защижения
> потребления**. OmniRoute автоматически сводит один из них, когда одна квота
> истекает — объедините все для неуязвимого $0 комбо.

### 🔵 МОДЕЛИ КЛУДА (через Киров — AWS Сборщик ID)

| Model              | Префикс | limit               | Ограничение скорости            |
| ------------------ | ------- | ------------------- | ------------------------------- |
| `claude-сонет-4.5` | `kr/`   | **Без ограничения** | Нет отчуждения ежедневной нормы |
| `claude-hаику-4.5` | `kr/`   | **Без ограничения** | Нет отчуждения ежедневной нормы |
| `claude-opus-4.6`  | `kr/`   | **Без ограничения** | С Latest Opus via Kiro          |

### 🟢 БЛОКИРИРОВАННЫЕ МОДЕЛИ (Бесплатный OAuth — Без карты платежей)

| Model                   | Префикс | limit               | Ограничение скорости |
| ----------------------- | ------- | ------------------- | -------------------- |
| `kimi-k2-мышление`      | `if/`   | **Без ограничения** | Нет задержки         |
| `qwen3-кодирующий плюс` | `if/`   | **Без ограничения** | Нет задержки         |
| `глубокий поиск-r1`     | `if/`   | **Без ограничения** | Нет задержки         |
| `минимакс-2.1`          | `if/`   | **Без ограничения** | Нет задержки         |
| `ками-кодер 2`          | `if/`   | **Без ограничения** | Нет задержки         |

### 🟡 РЕЖИМ QWEN (Код устройства)

| Model                    | Префикс | limit               | Ограничение скорости          |
| ------------------------ | ------- | ------------------- | ----------------------------- |
| `qwen3-кодирующий плюс`  | `qw/`   | **Без ограничения** | Нет задержки                  |
| `кодер flash Qwen3`      | `qw/`   | **Без ограничения** | Нет задержки                  |
| `кодер следующего Qwen3` | `qw/`   | **Без ограничения** | Нет задержки                  |
| `модель ВИЗИОН`          | `qw/`   | **Без ограничения** | Мультимодальный (изображения) |

### 🟣 КЛИЕНТ GEMINI (авторизация Google)

| Model                    | Префикс | limit                                          | Ограничение скорости   |
| ------------------------ | ------- | ---------------------------------------------- | ---------------------- |
| `Gemini-3-Flash-Preview` | `gc/`   | **180 Kb tokens v mesyatse/TДень** + 1 Kb/День | Ежемесячное обновление |
| `Gemini-2.5-Pro`         | `gc/`   | 180 Kb/Dol[Deli 180K/meshd]                    | Высокое качество       |

### ⚫ NVIDIA НИМ (Бесплатный API-ключ — build.nvidia.com)

| Тариф           | Дневной лимит             | Ограничение скорости | Примечания                                                  |
| --------------- | ------------------------- | -------------------- | ----------------------------------------------------------- |
| Бесплатно (Dev) | Нет ограничений на токены | **~40 RPM**          | 70+ модели; с февраля 2024 года внедряется нормально лимиты |

Популярные бесплатные модели: `moonshotai/kimi-k2.5` (Кими К2.5), `z-ai/glm4.7`
(GLM 4.7), `deepseek-ai/deepseek-v3.2` (DeepSeek V3.2),
`nvidia/llama-3.3-70b-instruct`, `deepseek/deepseek-r1`

### ⚪ CEREBRAS (Бесплатный API-ключ — inference.cerebras.ai)

| Тариф     | Дневной лимит       | Ограничение скорости           | Примечания                                                   |
| --------- | ------------------- | ------------------------------ | ------------------------------------------------------------ |
| Бесплатно | **1М токенов/день** | 60K TPM / 30 оборотов в минуту | Светлая самая быстрая инференс LLM; сбрасывается каждый день |

Доступно бесплатно: `llama-3.3-70b`, `llama-3.1-8b`,
`deepseek-r1-distill-llama-70b`

### 🔴 GROQ (Бесплатная API-ключ — console.groq.com)

| Тариф     | Дневной лимит      | Ограничение скорости          | Примечания                                           |
| --------- | ------------------ | ----------------------------- | ---------------------------------------------------- |
| Бесплатно | **14,4 ТП/ч[:X11X] | 30 запроса на модель в минуту | Без карты; 429 при достижении лимита, не начисляется |

Доступно бесплатно: `llama-3.3-70b-versatile`, `gemma2-9b-it`, `mixtral-8x7b`,
`whisper-large-v3`

### 🔴 LONGCAT AI (Бесплатная API-ключ — longcat.chat) 🆕

| Model                             | Префикс | Дневной бесплатный квота | Примечания                                |
| --------------------------------- | ------- | ------------------------ | ----------------------------------------- |
| `ДлинныйМач1-Кат-Flesh-Like`      | `lc/`   | **50М токенов** 💥        | Самое большое бесплатное квота когда-либо |
| `ДлинныйМач1-Кат-Флеш-Шат`        | `lc/`   | 500к токенов             | Мультицикловый чат                        |
| `ДлинныйМач1-Флеш-Надумочка`      | `lc/`   | 500к токенов             | Навыки рассуждения / CoT                  |
| `ДлинныйМач1-Флеш-Надумочка-2601` | `lc/`   | 500к токенов             | Версия января 2026 года                   |
| `ДлинныйМач1-Флеш-Омни-2603`      | `lc/`   | 500к токенов             | Мультирежим                               |

> Бесплатно в течение публичной бета-версии. Зарегистрируйтесь по электронной
> почте или телефону._RESET дневной 00:00 UTC.

### 🟢 POLLINATIONS AI (Нет ключа API) 🆕

| Model      | Префикс | Ограничение скорости | Поставщик За Которым |
| ---------- | ------- | -------------------- | -------------------- |
| `openai`   | `пол/`  | 1 запрос/15с         | GPT-5                |
| `claude`   | `пол/`  | 1 запрос/15с         | Anthropic Claude     |
| `гемини`   | `пол/`  | 1 запрос/15с         | Google Gemini        |
| `deepseek` | `пол/`  | 1 запрос/15с         | DeepSeek V3          |
| `лассы`    | `пол/`  | 1 запрос/15с         | Meta Llama 4 Scout   |
| `сентраль` | `пол/`  | 1 запрос/15с         | Mistral AI           |

> ✨ **Нулевое сопротивление:** Без регистрации, без ключа API. Добавьте
> Поставщика Pollinations, оставив поле ключа пустым, и оно начинает работать
> сразу.

### 🟠 СПРАБОТОВ ИНКАПЕРТРИВИСТОВ АЙ (Бесплатный ключ API — cloudflare.com) 🆕

| Тариф     | Дневной Нейрон | Навык использования                                 | Примечания                    |
| --------- | -------------- | --------------------------------------------------- | ----------------------------- |
| Бесплатно | [Х0Х]10,000**  | ~150 LLM resp / 500с пикселей аудио / 15K(embedded) | Глобальный конец, 50+ моделей |

Популярные бесплатные модели: `@cf/meta/llama-3.3-70б-направление`,
`@cf/google/gemma-3-12б-ит`, `@cf/openai/whisper-Large-v3-tурбо` (бесплатный
аудио!), `@cf/qwen/qwen2.5-coder-15b-направление`

> Требуется API-токен + ID аккаунта из
> [dash.cloudflare.com](https://dash.cloudflare.com). Сохраните ID аккаунта в
> настройках поставщика.

### 🟣 SCALEWAY AI (1M Бесплатные токены - scaleway.com) 🆕

| Тариф     | Бесплатная квота  | Расположение | Примечания                                          |
| --------- | ----------------- | ------------ | --------------------------------------------------- |
| Бесплатно | [Х0Х]1M токенов** | 🇫🇷 Париж, ЕС | Нет карты кредитной карты необходимы внутри лимитов |

Доступно бесплатно: `qwen3-235б-а22б-направление-2507` (Qwen3 235Б!),
`llama-3.1-70б-направление`, `mistral- Small-3.2-24b-направление-2506`,
`deepseek-v3-0324`

> ЕС/Правила о защите данных (GDPR) соответствует. Получите API-ключ на
> [console.scaleway.com](https://console.scaleway.com).

> [Х0Х]💡 Окончательная бесплатная стэковая модель (11 предоставитель, $ 0
> Окончательная):**
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

| Provider         | Free Credits           | Best Model                                   | Ограничение скорости         |
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

Затем в `/dashboard/media` → **Транскрипция** вкладке: загрузите любое аудио или
видеофайл → выберите точку завершения комбо → получите транскрипцию в
поддерживаемых форматах.

## 💡 Основные функции

OmniRoute v2.0 построен как операционная платформа, а не просто ретранслирующий
прокси.

### 🆕 Новая — вдохновлённые ClawRouter улучшения (.Mar 2026)

| Функция                                              | Что оно делает                                                                                                                             |
| ---------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| ⚡ **Grok-4 Fast Family**                             | Использование аи-моделей за $0,20/$0,50/М  — benchmark 1143мс (на 30% быстрее Gemini 2.5 Flash)                                            |
| 🧠 **GLM-5 через Z.AI**                               | Контекстный вывод объёмом 128К долларов, $0,5/1М  — самый свежий флагман от семейства GLM                                                  |
| 🔮 **MiniMax M2.5**                                   | Навыки рассуждения + агентные задачи за $0,30/1М  — значительное улучшение по сравнению с M2.1                                             |
| 🎯 **флаг вызова модельный инструмент**               | Свойства модели вызова: true/false` в реестре — AutoCombo пропускает модели, не способные вызывать инструменты                             |
| 🌍 **детекция языка целевой группы**                  | PT/ZH/ES/AR ключевые слова в AutoCombo подсчёте — улучшается выбор модели для неанглийского контента                                       |
| 📊 **Fallback в зависимости от метрики**              | В реальном времени p95 задержка из запросов live, комбинированная соитная подсчёт AutoCombo учитывает актуальные данные                    |
| 🔁 **отмена запроса**                                 | Дедуплицирование по содержанию-хешу базового окна — безопасная на уровня много-сервисов и предотвращает дополнительные оплаты за обработку |
| 🔌 **Подключаемый экземпляр стратегии маршрутизации** | Разширяемый интерфейс стратегии маршрутизации — добавляйте собственные логические правила для маршрутизации, yükно плагинами               |

### 🚀 Предыдущая версия v2.0.9+ — Игровая площадка, CLI, Fingerprints & ACP

| Функция                                                      | Что оно делает                                                                                                                                                                                                                                                                                     |
| ------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🎮 **ПлейGROUND модели**                                      | Страница Панель управления, предназначенная для тестирования любого модели напрямую — селекторы провайдером, моделью или конечной точкой, Monaco Editor, потокообработка, отмена и тайминга                                                                                                        |
| 🔏 **CLI подстановка скомитентных отпечатков**                | Подстановка порядка заголовков/телесных данных по провайдеру для совпадения с аутентификацией native CLI — перелистаете по порядку для каждого провайдера на Панели управления > Безопасность. **Мне сохраняется IP-протокола мой**                                                                |
| 🤝 **Руководство ACP (Агентский клиентский протокол)**        | Открытый аутентификатор агентов (Codex, Claude, Goose, Gemini CLI, OpenClaw + 9 других), процесс-привязка, `/api/acp/agents` конечная точка                                                                                                                                                        |
| 🤖 **Д dashboard агентов ACP**                                | Дебаг › Агенты страница панели управления — сетка из 14 агентов с статусом установки, версией, пользовательской сеткой для любой консольной утилиты. **Пользователь OpenCode** получает кнопку "Скачайте опенкоде.json", которая автоматически создает настраиваемый конфиг с доступными моделями. |
| 🔧 **Персональный маршрутизационный `apiFormat` Распознание** | Персональные модели с `apiFormat: "responses"` теперь корректно маршрутизируются на API-конечную точку translate                                                                                                                                                                                   |
| 🏢 **Изоляция рабочего места Codex**                          | Множество рабочих стоя Codex по электронной почте — сертифицированная OAuth корректно разделяет подключения по идентификатору рабочего места                                                                                                                                                       |
| 🔄 **Автономный обновленк Electron**                          | Десктопная программа проверяет обновления + аутономно-установке саму себе при перезагрузке                                                                                                                                                                                                         |

### 🤖 Операции агента и протокола (ver. 2,0).

| Функция                                       | Что оно делает                                                                                                 |
| --------------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| 🔧 **Сервер MCP (16 инструментов)**            | IDE/агентские инструменты через 3 транспорта: stdio, SSE (`/api/mcp/sse`), Streamable HTTP (`/api/mcp/stream`) |
| 🤝 **Сервер A2A (JSON-RPC + SSE)**             | Исполнение задач от агента к агенту с синхронными и поточными потоками                                         |
| 🧭 [Х2Х]Страница объединенных конечных точек** | Табличная страница управления конечными точками с вкладками Endpoint Proxy, MCP, A2A и API Endpoints           |
| 🎚️ [Х3Х]Кнопки включения/отключения услуг**   | Кнопки вкл/выкл для MCP и A2A с сохранением настроек (по умолчанию: ВКЛ)                                       |
| 🛰️ [Х3Х]Дзикость сервиса MCP в REAL-TIME**    | Реальный статус процесса (PID, uptime, возраст heartbeata, транспорт, режима scope)                            |
| 📋 [Х2Х]Журнал аудита MCP**                    | Фильтруемый журнал аудита с успехами/неудачами и ключевыми атрибутами                                          |
| 🔐 [Х2Х]Исполнение области MCP**               | 9 гранулярных прав доступа для контроля доступа к инструментам                                                 |
| 📡 [Х2Х]Поддержка жизненного цикла задач A2A** | Список/фильтрование задач, инспекция событий/артефактов, отмена выполняющихся задач                            |
| 📋 [Х2Х]Обеспечение карточки агента**          | `/.well-known/agent.json` для автоматического поиска клиента                                                   |
| 🧪 [Х2Х]Протокол Э2Э Тест-Харнесс[Х29Х]        | Валовая MCP SDK + клиент A2А потоки в [Х35Х]тестируемая:протоколы:э2э[Х54Х]                                    |
| ⚙️ [Х3Х]Системные Управляемые Параметры[Х25Х] | Переключатель комбо, применение профиля стойкости, сброс электрических защиты с одной панели управления        |

### 🧠 Маршрутизация и Интеллект

| Функция                                                   | Что оно делает                                                                               |
| --------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| 🎯 [Х2Х]Интеллектуальная четырехуровневая Перехватка[Х25Х] | Автоматическая маршрутизация: Подписка → Токен API → Дешевый → Бесплатный                    |
| 📊 [Х2Х]Онлайн-Отчетность по квотам[Х28Х]                  | Живые токены + сброс часов для каждого провайдера                                            |
| 🔄 [Х2Х]Автоматическая ПЕРЕВОД КЛАССА[Х22Х]                | Перевод OpenAI ↔ Claude ↔ Gemini ↔ Ответы со безопасной схемой преобразования                |
| 👥 Умножитель Поддержки Экзистенциальной Суммы             | Множество счетов каждого провайдера с интеллектуальным выбором                               |
| 🔄 [Х2Х]Авто Обновления Токена[Х22Х]                       | Токены OAUTH обновляются автоматически с повторным выполнением                               |
| 🎨 [Х2Х]Соедиения Изио[Х17Х]                               | 6 стратегий балансировки + контроль цепи фоллбэка                                            |
| 🌐 [Х2Х]Шаблонный Маршрутизатор[Х19Х]                      | `провайдер/*`динамическое маршрутизирование                                                  |
| 🧠 **Думая, бюджетное управление контролям**               | Передача, автомат, настраиваемый и адаптивный лимит рассуждений                              |
| 🔀 **Псевдонимы модели**                                   | Встроенная + настраиваемая функция назначения псевдонима и безопасность миграции             |
| ⚡ **Фоновое разрушение**                                  | Присваивать низкоприоритетные задачи модели дороже                                           |
| 🧪 **Задачно-авторазумная-smart-ориентация**               | Авто-подбор модели на основе типа содержания (кодирование/виждения/анализ/сводкаКодирования) |
| 💬 **Ввывожение в систему Prompt**                         | Глобальные управляющие параметры приложены последовательно                                   |
| 📄 **Совместимость API-ответов**                           | Полная `/v1/responses`совместимость с Kodex и продвинутыми агентскими потоками               |

### 🎵 APIs-мультиформатов

| Функция                         | Что оно делает                                                                                                                                                                               |
| ------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🖼️ **Генерация изображений**    | `/v1/images/generations`  с облачным и локальным backends                                                                                                                                    |
| 📐 **Завышения**                 | `/v1/embeddings` для поиска и pipelines РАГ                                                                                                                                                  |
| 🎤 **Аудио-Переводчик**          | `/v1/audio/transcriptions` — 7 провайдеров (Deepgram Nova 3, AssemblyAI, Groq Whisper, HuggingFace, ElevenLabs, OpenAI, Azure), автоматическая языковая распознавание, поддержка MP4/MP3/WAV |
| 🔊 **Текст к голосу**            | `/v1/audio/speech` — 10 провайдеров (ElevenLabs, OpenAI, Deepgram, Cartesia, PlayHT, HuggingFace, Nvidia NIM, Inworld, Coqui, Tortoise) с корректными ошибками сообщениями                   |
| 🎬 **Видео-Generate**            | `/v1/videos/generations` (ComfyUI + SD WebUI workflow)                                                                                                                                       |
| 🎵 **Музыка Generate**           | `/v1/music/generations` (ComfyUI workflow)                                                                                                                                                   |
| 🛡️ **Модерации**                | `/v1/moderations` проверки безопасности                                                                                                                                                      |
| 🔀 **Перекрестное ранжирование** | `/v1/rerank` для оценки актуальности                                                                                                                                                         |
| 🔍 **Веб-поиск** 🆕               | `/v1/search` — 5 провайдеров (Serper, Brave, Perplexity, Exa, Tavily), 6,500+ бесплатно в месяц, автоматический переадресация, кэш                                                           |

### 🛡️ Высокая производительность, Безопасность и Управление

| Функция                                                                   | Что оно делает                                                                         |
| ------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| 🔌 ** Расходники предназначены** для восстанавливаения связей между модели | Per-model trip/recover с порогом регулирования                                         |
| 🎯 **Модели под контролем конечной точки**                                 | Custom models declare supported endpoints + API format                                 |
| 🛡️ **Anti-Thundering Herd**                                               | Mutex + semaphore protections on retry/rate events                                     |
| 🧠 **Semantic + Signature Cache**                                          | Cost/latency reduction with two cache layers                                           |
| ⚡ **Request Idempotency**                                                 | Duplicate protection window                                                            |
| 🔒 **TLS Fingerprint Spoofing**                                            | Browser-like TLS fingerprint — **reduces bot detection and account flagging**          |
| 🔏 **CLI подстановка скомитентных отпечатков**                             | Matches native CLI request signatures — **reduces ban risk while preserving proxy IP** |
| 🌐 **IP Filtering**                                                        | Allowlist/blocklist control for exposed deployments                                    |
| 📊 **Editable Rate Limits**                                                | Configurable global/provider-level limits with persistence                             |
| 🔑 **API Key Management + Scoping**                                        | Secure key issuance/rotation and model/provider controls                               |
| 🛡️ **Protected `/models`**                                                | Optional auth gating and provider hiding for model catalog                             |

### 📊 Observability & Analytics

| Функция                                       | Что оно делает                                                       |
| --------------------------------------------- | -------------------------------------------------------------------- |
| 📝 **Запрос + Запись_PROXY_X27X]               | Полный лог запроса/ответа и proxy                                    |
| 📋 **Интегрированный Логовый Д.dashboard_X26X] | В один раздел: запросы, proxy, аудит и консольные логи               |
| 🔍 **Телеметрия Запросов_X21X]                 | п50/p95/p99 задержки и отслеживание запросов                         |
| 🏥 **Дашборд Здоровья_X20X]                    | Уptime, состояния Breakers, блокировки, статистика кэша              |
| 💰 **Отслеживание Стоимости_X17X]              | Управление бюджетом и видимостьricing модели по модели               |
| 📈 **Визуализация_Аналитики_X28X]              | Усилия по модели/предоставлению и тенденции просмотров               |
| 🧪 **Фреймворк_Оценки_X24X]                    | Тестирование золотого набора с настраиваемыми стратегиями совпадения |

### ☁️ Развертывание & Платформа

| Функция                                       | Что оно делает                                                            |
| --------------------------------------------- | ------------------------------------------------------------------------- |
| 🌐 **Развертывайтесь_Где_Зык_X19X]             | Локальный сервер, Виртуальный сервер, Docker,(Cloud) среда                |
| 💾 Синхронизация данных** в Cloud              | Синхронизация конфигурации с помощью работающего на Cloud воркера         |
| 🔄 Backup/Restore**                            | Экспорт/импорт и восстановление после катастрофы                          |
| 🧙 Вводных руководство "Welcome Wizard"**      | Наводящие на установку с помощью первой загрузки                          |
| 🔧 Панель инструментов для CLI                 | Однокликочный доступ к популярным инструментам программирования           |
| 🎮 **ПлейGROUND модели**                       | Тестирование любого провайдера/модели/конечной точки из панели управления |
| 🔏 Переключатель отпечатков пальцев для CLI ** | Соответствие отпечатков по-провайдеру в настройки > Безопасность          |
| 🌐 локализации интерфейса (30 языков)**        | Полная поддержка языка + документации, а также RTL настройки              |
| 🧹 Очистка всех моделей **                     | Один клик - очистка списка моделей в деталях провайдера                   |
| 📋 Шаблоны для отчетов **                      | С-standardized шаблоны GitHub для ошибок и функций                        |
| 📂 Настраиваемая директура данных**            | `Директория данных` - режим замены для местоположения хранения            |

### Глубокое погружение в funkciю

#### Практическая схема fallback с контролем затрат

```txt
Комбо: "мой стек"
  1. cc/claude-opus-4-6
  2. nvidia/llama-3.3-70b
  3. glm/glm-4.7
  4. if/kimi-k2-thinking
```

Когда квота, скорость или здоровье отказывают, OmniRoute автоматически переходит
к следующему кандидату без ручного переключения.

#### Управление протоколами, видимое и управляемое

- MCP + A2A являются открытыми в UI и доках (не скрытыми)
- API состояния протокола открывают живую операционную информацию (`/api/mcp/*`,
  `/api/a2a/*`)
- Дашборды включают действия для Операций В 2 (комбтоглы, сбросы брेकरов и
  отмены задач)

#### Панель переводчика и валидации

Панель переводчика включает:

- **Игровая площадь**: проверка преобразований
- **Тестер чата**: полный чек в чел-ответ
- **Базовая станция тестов**: проверки для одного хода
- **Онлайн-мониторинг**: реальное время просмотра пробега

Плюс валидация протокола с помощью реальных клиентов при `npm run
test:протоколов:e2e`.

> 📖 **[Справочник сервера MCP](open-sse/mcp-server/README.md)** — Руководство
> пользователя, конфигурации IDE, примеры клиентов
> 
> 📖 **[Справочник сервера A2A](src/lib/a2a/README.md)** — Поддерживаемые
> технологии, методы JSON-RPC, поточная передача и цикл жизни задач

## 🧪 Оценки (Оценочное)

OmniRoute включает в себя встроенный оценочный фремворк для проверки качестве
ответа LLM отнесения к золоту. Доступно через **Аналитики → Оценки** в панели
дашбордов.

### Встроенная золотая коллекция

Предзагруженная "омнирутина" Золотая коллекция содержит касейсы для:

- Приветствия, математика, география, генерация кода
- Надежность JSON-соответствия, перевода, генерация markdown
- Отказ от безопасности (вредный контент), счетчики, логика boolean

### Стратегии оценки

| Стратегия   | Описание                                              | Пример                               |
| ----------- | ----------------------------------------------------- | ------------------------------------ |
| `точно`     | Вывод должен совпадать точно                          | `"4"`                                |
| `содержит`  | Вывод должен содержать подстроку (без учета регистра) | `"Париж"`                            |
| `регулярка` | Вывод должен соответствовать регулярному шаблону      | `"1.*2.*3"`                          |
| `кUSTOM`    | Сохраняемая JS-функция вернула true/false.            | `(вывод) =&gt; вывод.лenght &gt; 10` |

---

## 📖 Руководство по подключению

### Настройка Протокола (MCP + A2A)

<details>
<summary><b>🧩 MCP Setup (Model Context Protocol)</b></summary>

Начать роботу MCP транспортом в режиме stdio:

```bash
omniroute --mcp
```

Рекомендуемый поток валидации:

1. Подключите клиент MCP через stdio.
2. Выполните `omniroute_get_health`.
3. Выполните `omniroute_list_combos`.
4. Откройте `/dashboard/mcp` для подтверждения сердцебиения, активности и
   аудита.

Полезные API для автоматизации:

- `GET /api/mcp/status`
- `GET /api/mcp/tools`
- `GET /api/mcp/audit`
- `GET /api/mcp/audit/stats`

</details>

<details>
<summary><b>🤝 A2A Setup (Agent2Agent)</b></summary>

Начать поиск агента:

```bash
curl http://localhost:20128/.well-known/agent.json
```

Отправить задание:

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"setup-a2a","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"Summarize quota status."}]}}'
```

Управление жизненным циклом:

- `GET /api/a2a/status`
- `GET /api/a2a/tasks`
- `GET /api/a2a/tasks/:id`
- `POST /api/a2a/tasks/:id/cancel`

Режим работы:

- `/dashboard/a2a` для наблюдения за заданиями/состояниями/потоками и нажатиями
  «запустить тест-драйв»

</details>

<details>
<summary><b>🧪 End-to-end protocol validation</b></summary>

Подтверждаем оба протокола с реальными клиентами:

```bash
npm run test:protocols:e2e
```

Это проверяет:

- Клиент MCP SDK: подключение, списки, вызов
- Открытие A2A: обнаружение, отправка, поток, получение, отмена
- Перекрестная проверка данных в аудитах MCP и управлениями заданиями A2A

</details>

<details>
<summary><b>💳 Subscription Providers</b></summary>

### Клод Код (Про/Макс)

```bash
Лента dashboard → Провайдеры → Подключение Клода Код → OAuth авторизация → Автообновление токена → Размещение метрик, отслеживаемых в течение 5 часов + недельных квот

Модели:
  cc/claude-opus-4-6
  cc/claude-sonnet-4-5-20250929
  cc/claude-haiku-4-5-20251001
```

**Профессиональный совет:** Используйте Опус для сложных задач, Соннет для
скорости. OmniRoute отслеживает квоты за модель!

### OpenAI Codex (Plus/Pro)

```bash
Лента dashboard → Провайдеры → Подключение Codex
→ OAuth авторизация (порт 1455)
→ 5-часовые + недели-рестарты

Модели:
  cx/gpt-5.2-codex
  cx/gpt-5.1-codex-max
```

#### Управление лимитами учетной записи Codex (5h + Неделя)

Каждая учетная запись Codex теперь имеет настраиваемые параметры политики в
`Ленте dashboard -&gt; Провайдеры`:

- `5 ч.` (ВКЛ/ВЫКЛ): применение политики по пороговому времени 5-часовой рамки.
- [Х0Х]Еженедельная[Х7Х] (ВКЛ/ВЫКЛ): принудить политику порогового значения окна
  для еженедельной политики.
- Поведение порога: когда активное окно достигает >=90% использования, этот
  аккаунт пропускается.
- Поведение развертывания: OmniRoute по умолчанию распределяет следующий
  доступный аккаунт Кодекса.
- Поведение сброса: по истечении указанного период времени `resetAt` аккаунт
  снова становится доступным автоматически.

Сценарии:

- [Х0Х]5h ВКЛ[Х6X] + [Х10Х]Еженедельная ВКЛ[Х20X]: аккаунт пропускается, когда
  либо окно достигает порога использования.
- [Х0Х]5h ВЫКЛ[Х7X] + [Х11Х]Еженедельная ВКЛ[Х21X]: только еженедельное
  использование может блокировать аккаунт.
- [Х0Х]5h ВКЛ[Х6X] + [Х10Х]Еженедельная ВЫКЛ[Х21X]: только 5-часовой
  использование может блокировать аккаунт.
- [Х0Х]resetAt[Х8X] passed: аккаунт возвращается в развертывание автоматически
  (без ручной рeregistrations).

### Gemini CLI (БЕСПЛАТНО 180К/месяц!)

```bash
Рабочий стол → Провайдеры → Подключить Gemini CLI
→ Google OAuth
→ 180К комплектаций/месяц + 1К/день

Модели:
  gc/gemini-3-flash-preview
  gc/gemini-2.5-pro
```

[Х0Х]Лучшая стоимость:[Х13X] Большие бесплатные тарифы! Используйте их перед
платными тарифами.

### GitHub второй пилот

```bash
Рабочий стол → Провайдеры → Подключить GitHub
→ OAuth через GitHub
→ Разовая проверка (1-е число месяца)

Модели:
  gh/gpt-5
  gh/claude-4.5-sonnet
  gh/gemini-3-pro
```

</details>

<details>
<summary><b>🔑 API Key Providers</b></summary>

### NVIDIA NIM (БЕСПЛАТНЫЙ разработчик для доступа — 70+ моделей)

1. Регистрация: [build.nvidia.com](https://build.nvidia.com)
2. Получить бесплатный API-ключ (включены 1000 баллов инференса)
3. Рабочий стол → Добавить Провайдера → NVIDIA NIM:
   - API-ключ: `nvapi-your-key`

[Х0Х]Модели:** `nvidia/llama-3.3-70b-instruct`, `nvidia/mistral-7b-instruct`, и
50+ еще.

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
3. Прибль → Добавить API-ключ:
   - Провайдер: `glm`
   - API-ключ: `your-key`

**Использовать:** `glm/glm-4.7`

**Рекомендация:** План цодинга предлагает 3× квоту по цене 1/7 от нормы! Сброс
квоты в 10:00 утра.

### MiniMax M2.1 (5ч сброса, $0,20/1 Мб)

1. Подписаться: [MiniMax](https://www.minimax.io/)
2. Get API key
3. Прибль → Добавить API-ключ

**Использовать:** `minimax/MiniMax-M2.1`

**Рекомендация:** Наиболее экономный вариант для длинных текстов (1 Мб токенов)!

### Kimi K2 ($9/месяц-flat)

1. Подписаться: [Moonshot AI](https://platform.moonshot.ai/)
2. Get API key
3. Прибль → Добавить API-ключ

**Использовать:** `kimi/kimi-latest`

**Рекомендация:** Fixed $9/месяц за 10 Мб токенов = $0,90/1 Мб эффективное
затраты!

</details>

<details>
<summary><b>🆓 FREE Providers (Emergency Backup)</b></summary>

### iFlow (5 БЕСПЛАТНЫХ моделей via OAuth)

```bash
Прибль → Подключить iFlow
→ вход в iFlow via OAuth
→ Бесконечный доступ

Модели:
  if/kimi-k2-thinking
  if/qwen3-coder-plus
  if/glm-4.7
  if/minimax-m2
  if/deepseek-r1
```

### Qwen (4 БЕСПЛАТНЫХ модели via Device Code)

```bash
Панель управления → Подключить Куена
→ Авторизация по коду устройства
→ Бессрочный доступ

Модели:
  кв/куен3-кодер-плюс
  кв/куен3-кодер-флеш
```

### Киро (ФРЕД)

```bash
Панель управления → Подключить Киро
→ ID AWS Builder или Google/GitHub
→ Бессрочный доступ

Модели:
  кр/клауд-соннет-4.5
  кр/клауд-хайку-4.5
```

</details>

<details>
<summary><b>🎨 Create Combos</b></summary>

### Пример 1: Выдвижение подписки → Дешевая резервная копия

```
Панель управления → КOMBOS → Создать Новый

Название: премиум-кодирование
Модели:
  1. cc/клауд-опус-4-6 (Подписка основная)
  2. glm/glm-4.7 (Дешевая резервная копия, $0.6/1М )
  3. минимакс/МиниМаксим- М2.1 ( Least Costly fallback, $0.20/1М )

Использование в CLI: премиум-кодирование
```

### Пример 2: Без средств (Zero Cost)

```
Название: бесплатный КOMBOS
Модели:
  1. gc/гемини-3-флаш-превью (180К бесплатно/мес  )
  2. если/кими-к2-думающий (бессрочный)
  3. кв/куен3-кодер-плюс (бессрочный)

Стоимость: $0 навсегда!
```

</details>

<details>
<summary><b>🔧 CLI Integration</b></summary>

### Курсор IDE

```
Настройки → Модели → Расширенные:
 /OpenAI API Base URL: http://localhost:20128/v1
  OpenAI API Key: [из OmniRoute панели управления]
  Модель: cc/клауд-опус-4-6
```

### Клод Код

Используйте страницу инструментов CLI Tools** в панели управления для одной
кнопочки конфигурации, либо редактируйте `~/.claude/settings.json` вручную.

### Кодекс CLI

```bash
export OPENAI_BASE_URL="http://localhost:20128"
export OPENAI_API_KEY="ваши-омнирут-ключ-api"

codex "ваш стимул"
```

### OpenClaw

**Вариант 1 — Панель управления (рекомендованное):**

```
Панель управления → Инструменты CLI → OpenClaw → Подключить Модель → Применить
```

**Вариант 2 — Руками:** Редактируйте `~/.openclaw/openclaw.json`:

```json
{
  "models": {
    "providers": {
      "омнирут": {
        "baseUrl": "http://127.0.0.1:20128/v1",
        "apiKey": "sk_омнирут",
        "api": "openai-completions"
      }
    }
  }
}
```

> **Примечание:** OpenClaw работает в локальной OmniRoute. Используйте
> `127.0.0.1` вместо `localhost`, чтобы избежать проблем с разрешением IPv6.

### Клайн / Продолжить / Ру-код

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

## Устранение неполадок

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

- Проверьте статистику использования в Панели управления → Расходы
- Переключить основной модель на GLM/MiniMax
- Использовать бесплатную версию (Gemini CLI, iFlow) для небезопасной работы

[Х0Х]Панель/ис-api порты неверны[Х31Х]

- [Х0Х]ПОРТ[Х5Х] - основной и по умолчанию канальный порт (и API-порт)
- [Х0Х]API_ПОРТ[Х9Х] преимущественно заменяет только OpenAI-совместимый
  API-ридер
- [Х0Х]ПОРТ_ДASHBOARD[Х15Х] заменяет только панель просмотра/ридер Next.js
- Установите [Х4Х]NEXT_PUBLIC_BASE_URL[Х25Х] для URL公共 обзор на вашем сервере
  (для входа OAuth)

[Х0Х]Ошибки синхронизации облачного окружения[Х19Х]

- Проверьте, чтобы [Х7Х]BASE_URL[Х16Х] указывал на ваш сервер
- Проверьте, чтобы [Х7Х]CLOUD_URL[Х17Х] указывал на Ваш облачный URL
- Подтверждение [Х5Х]NEXT_PUBLIC_*[Х19Х] значения парсить по сторонне с сервера

[Х0Х]Первый вход работать не будет[Х25Х]

- Проверьте [Х6Х]INITIAL_PASSWORD[Х23Х] в [Х28Х].env[Х33Х]
- Если не задано, то будет использован [Х31Х]123456[Х38Х]

[Х0Х]Нет логов запросов[Х17Х]

- Установите [Х4Х]ENABLE_REQUEST_LOGS=true[Х29Х] значение в [Х34Х].env[Х39Х]

[Х0Х]Проверка соединения показывает "Invalid" для OpenAI-совместимого
провайдера[Х65Х]

- Большинство провайдеров не имеют доступа к API '/models'
- OmniRoute v1.0.6+ включает в себя флаг-версию в чат-самоподвалениях.
- Навигация по базовому URL включает в себя `/v1` суффикс

### Сертификация OAuth на удаленном сервере

<a name="oauth-on-a-remote-server"></a> <a name="oauth-em-servidor-remoto"></a>

> **⚠️ Very important for users running OmniRoute on a VPS, Docker, or any
> remote server**

#### Почему Оauth / CLI Gemini Antigravity терпит фиаско на удаленных серверах?

Провайдеры **Antigravity** и **Gemini CLI** используют **Google OAuth 2.0**.
Google требует, чтобы в OAuth flow точно совпадал один из зарегистрированных URI
во время регистрации в консоли Google Cloud Console.

Правидентификаторы OAuth, включенные в OmniRoute, зарегистрированы **тольоко для
`localhost` only**. Когда вы используете OmniRoute на удаленном сервере
(например `https://omniroute.myserver.com`), Google запрещает авторизацию с:

```
Ошибкой 400: redirect_uri_mismatch
```

#### Решение: Configure вашу собственную Оauth-авторизацию

Вам необходимо создать собственный **OAuth 2.0 Client ID** в консоли Google
Cloud Console с URI своего сервера.

#### Шаг за шагом

**1. Откройте консоль Google Cloud**

Перейти в:
[https://console.cloud.google.com/apis/credentials](https://console.cloud.google.com/apis/credentials)

**2. Создать новый OAuth 2.0 Client ID**

- Нажмите **"+ Create Credentials"** → **"OAuth client ID"**
- Тип приложения: **"Web application"**
- Имя: что угодно (например `OmniRoute Remote`)

**3. добавить Авторизованные Redirect URIs**

В поле **"Authorized redirect URIs "**, добавьте:

```
https://your-server.com/callback
```

> Замените `your-server.com` на domain или IP своего сервера (включая порт в
> случае необходимости, например `http://45.33.32.156:20128/callback`).

**4. Сохраните и скопируйте учётные данные**

После создания, Google покажет **ID Клиента** и **Секретный ключ**.

**5. Установите переменные окружения**

В вашем `.env` (или переменных Docker):

```bash
# Для Antigravity:
ANTIGRAVITY_OAUTH_CLIENT_ID=your-client-id.apps.googleusercontent.com
ANTIGRAVITY_OAUTH_CLIENT_SECRET=GOCSPX-your-secret

# Для Gemini CLI:
GEMINI_OAUTH_CLIENT_ID=your-client-id.apps.googleusercontent.com
GEMINI_OAUTH_CLIENT_SECRET=GOCSPX-your-secret
GEMINI_CLI_OAUTH_CLIENT_SECRET=GOCSPX-your-secret
```

**6. Перезапустите OmniRoute**

```bash
# npm:
npm run dev

# Docker:
docker restart omniroute
```

**7. Снова попробуйте подключиться**

Дashboard → Provedory → Antigravity (или Gemini CLI) → OAuth

Google теперь корректно перенаправит на `https://your-server.com/callback`.

---

#### Порочный ход (без настройки пользовательских данных)

Если вы сейчас не хотите настраивать свои же учётные данные, вы можете всё равно
использовать **ручной поток авторизации**:

1. OmniRoute открывает URL авторизации Google
2. После авторизации Google пытается перенаправить на `localhost` (что приводит
   к ошибке на веб-сервере)
3. **Копируйте полный URL** из адресной строки вашего браузера (даже если
   страница не загружается)
4. Вставьте тот URL в показанный в OmniRoute модальный диалог
5. Нажмите **"Подключиться"**

> Это работает, поскольку код авторизации в URL является действительным, даже
> если страница перенаправления загрузилась.

---

<details>
<summary><b>🇧🇷 Versão em Português</b></summary>

#### Почему OAuth в Antigravity / Gemini CLI не работает на веб-серверах?

Провайдеры **Antigravity** и **Gemini CLI** используют **Google OAuth 2.0** для
аутентификации. Google требует, чтобы в URL авторизации был указан `URL
перенаправления` прецизионно[, который он зарегистрирован в Google Cloud Console
приложения.

креденты OAuth встроенные в OmniRoute зарегистрированы только для `localhost`
**. Когда вы acessas OmniRoute на удаленном сервере (например,
`https://omniroute.meuservidor.com`), [X26X]Google** отвергает аутентификацию с:

```
Ошибкой 400: redirect_uri_mismatch
```

#### Решение:Configure свои собственные креденты OAuth

Вам необходимо создать уникальный **Client ID OAuth 2.0** в Google Cloud Console
со URI вашего сервера.

#### Шаги:

**1. Адрес **Google Cloud Console**

Открыть:
[https://console.cloud.google.com/apis/credentials](https://console.cloud.google.com/apis/credentials)

**2. Создайте новый OAuth 2.0 Client ID**

- Нажмите на **"+" + Сreate Credentials** → **"OAuth client ID"**
- Тип приложения: **"Web application"**
- Имя: выберите любое имя (например, `OmniRoute Remote`)

**3. Добавить утвержденные Redirect URI

В поле **"Authorized redirect URIs"**, добавьте:

```
https://ваш-сервер.com/callback
```

> Замените `ваш-сервер.com` на домен или IP адрес вашего сервера (включая порт,
> если необходим, например, `http://45.33.32.156:20128/callback`).

**4. Сохраните и скопируйте креденты

После создания **Client ID** и **Client Secret** будут предоставлены.

**5. Configure переменные среды

В вашем `.env` (или в переменных среды Docker):

```bash
# Для Antigravity:
ANTIGRAVITY_OAUTH_CLIENT_ID=ваш-клиент-айди.apps.googleusercontent.com
ANTIGRAVITY_OAUTH_CLIENT_SECRET=GOCSPX-ваши-секрет
# Для Gemini CLI:
GEMINI_OAUTH_CLIENT_ID=ваш-клиент-айди.apps.googleusercontent.com
GEMINI_OAUTH_CLIENT_SECRET=GOCSPX-ваши-секрет
GEMINI_CLI_OAUTH_CLIENT_SECRET=GOCSPX-ваши-секрет
```

**6. Запустите OmniRoute заново**

```bash
# Если используем npm:
npm run dev

# Если используем Docker:
docker restart omniroute
```

**7. Повторите попытку подключения**

Панель управления → Поставщики → Antigravity (или Gemini CLI) → OAuth

Теперь Google правильно направит его на `https://ваш-сервер.com/callback` и
аутентификация начнётся.

---

#### Временное решение (без настройки собственных учетных данных)

Если не хотите создавать свои учетные данные сейчас, всё равно есть возможность
использовать веб-интерфейс **URL-манипулятор[getX93X]:

1. OmniRoute откроет URL-авторизации Google
2. После выдачи согласия, Google попытается направить на `localhost` (что не
   проходит в удалённом сервере)
3. **Скопируйте полную URL** из адресной строки вашего браузера (хотя страница
   может не загрузиться)
4. Введите эту URL в поле, появляющееся в модальном окне подключения OmniRoute
5. Нажмите **"Подключиться"**

> Это решение работает, поскольку код авторизации в URL является действительным,
> независимо от того, загружалось перенаправление или нет.

</details>

---

</details>

## 🛠️ Tech Stack

<details>
<summary><b>Click to expand tech stack details</b></summary>

- **Runtime**: Node.js 18–22 LTS (⚠️ Node.js 24+ не поддерживается** —
  `better-sqlite3` native binaries не совместимы)
- **Язык**: TypeScript 5.9 — **100% TypeScript** по всему `src/` и `open-sse/`
  (нет `any` в основных модулях с версии v2.0)
- **Фреймворк**: Next.js 16 + React 19 + Tailwind CSS 4
- **База данных**: LowDB (JSON) + SQLite (состояние домена + журналы прокси +
  аудит MCP + решения маршрутизации)
- **Редактируемые схемы**: Zod (инструмент MCP I/O валидациях, API-контракты)
- **Протоколы**: MCP (stdio/HTTP) + A2A v0.3 (JSON-RPC 2.0 + SSE)
- **Прямое стриминг[:12X]: Серверные события (SSE)
- **Авторизация[:36X]: OAuth 2.0 (PKCE) + JWT + API Keys + Управление доступом
  MCP
- **тестирования[:9X]: Node.js модуль для тестирования + Vitest (900+ тестов,
  включая единичные, интеграционные, E2E)
- ** CI/CD[:7X]: GitHub Actions (автоматическое публикация npm + Docker Hub на
  релиз)
- **Сайт**: [omniroute.online](https://omniroute.online)
- ** Package[:9X]:
  [npmjs.com/package/omniroute](https://www.npmjs.com/package/omniroute)
- **Docker[:8X]:
  [hub.docker.com/r/diegosouzapw/omniroute](https://hub.docker.com/r/diegosouzapw/omniroute)
- **Резилience[:12X]: Блокировки сетевого соединения, экспоненциальный сброс,
  защита от шторма, мимикрирование TLS, самоисцеление комбо

</details>

---

## Документация

| Документ                                                           | Описание                                                               |
| ------------------------------------------------------------------ | ---------------------------------------------------------------------- |
| [Руководство пользователя](docs/USER_GUIDE.md)                     | Поставщики, комбо, КЛИ, деплоймент                                     |
| [API Руководство](docs/API_REFERENCE.md)                           | Всі конечные точки с примерами                                         |
| [Провайдер MCP](open-sse/mcp-server/README.md)                     | 16 инструментов MCP, конфигурации IDE, клиенты из Python/TS/Go         |
| [Провайдер A2A](src/lib/a2a/README.md)                             | Протокол JSON-RPC 2.0, навыки, потоковый стриминг, управление задачами |
| [Мотор Auto-Combo](docs/auto-combo.md)                             | Оценка по 6 факторам, наборы пакетов, самонастоящаясь                  |
| [Тroubleshooting](docs/TROUBLESHOOTING.md)                         | Общие проблемы и решения                                               |
| [Архитектура](docs/ARCHITECTURE.md)                                | Архитектура системы и внутренности                                     |
| [Вклад в разработку](CONTRIBUTING.md)                              | Настройка и руководство по разработке                                  |
| [OpenAPI Спeцификация](docs/openapi.yaml)                          | Спeцификация OpenAPI 3.0                                               |
| [Политика безопасности](SECURITY.md)                               | Отчетность о уязвимостях и практики безопасности                       |
| [Развертывание на виртуальной машине](docs/VM_DEPLOYMENT_GUIDE.md) | Полный гайд: VM + nginx + Cloudflare                                   |
| [Галерея функций](docs/FEATURES.md)                                | Визуальный тур по dashboard с снимками экрана                          |
| [Печатная версия чека](docs/RELEASE_CHECKLIST.md)                  | Шаги проверки до релиза                                                |

---

## 🗺️ План действий

OmniRoute имеет **230+ функций)** запланировано на несколько этапов разработки.
Ниже перечислены основные направления:

| Категория                              | Планируемые функции | Акценты                                                                                                                                   |
| -------------------------------------- | ------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- |
| 🧠 **ROUTEING И ИНТЕЛЛЕКТ 🔄 **          | 25+                 | Расчет с наименьшей задержкой, маршрутизация на основе тегов, проверка квоты на этапе запрашивания, выбор счета P2C                       |
| 🔒 **Безопасность И Ракмемлемость[I24X] | 20+                 | Усиление защиты от SSRF, сокрытие учетных данных, лимитирующее количество запросов на каждый конечный пункт, ограничение ключа управления |
| 📊 **Наблюдаемость[I17X]                | 15+                 | Набор интеграций OpenTelemetry, мониторинг квоты в реальном времени, отслеживание затрат на каждый MODEL                                  |
| 🔄 **Интеграции Провайдер[I25X]         | 20+                 | Динамическая зарегистрированная модель, провайдер с задержкой, многоаккаунтный Codex, парсинг квоты Copilot                               |
| ⚡ **ВысотаPerformance[I15X]            | 15+                 | Блочная кэширующая стойкость, кэш запрашивания, кэш ответа, потоковая передача, передача пакета API                                       |
| 🌐 **Экосистема[I13X]                   | 10+                 | API WebSocket, hot-повторное обновление конфигурации, распределенная стоянка конфигурации, коммерческий режим                             |

### Скоро

- 🔗 **OpenCode Интеграция[I24X] — Нативная поддержка провайдера для IDE
  OpenCode-а по разработке AI
- 🔗 **TRAE Интеграция** — Полный поддержка TRAE AI разрабатываемых framework
- 📦 **Общаемся с API в наборами** — Асинхронное процессинга в наборах запросов
- 🎯 **Обратился по меткам маршрутизация** — Маршрутизация запросов по
  настраиваемым меткам и метаданных
- 💰 **Ловший ценовые стратегия** — Автоматически выберите дешевую доступную
  поставщика

> 📝 Полную спецификация доступна в [`docs/new-features/`](docs/new-features/)
> (217 подробную спецификация)

---

## 👥 Участники

[![Участники](https://contrib.rocks/image?repo=diegosouzapw/OmniRoute&max=100&columns=20&anon=1)](https://github.com/diegosouzapw/OmniRoute/graphs/contributors)

### Как Participation в этом Projekt

1. Fork репозиторий
2. Создать ваш бранч (`git checkout -b feature/amazing-feature`)
3. Сохранить ваши изменения (`git commit -m 'Add amazing feature'`)
4. Отправить изменения в бранч (`git push origin feature/amazing-feature`)
5. Открыть Pull Request

Пожалуйста, ознакомьтесь с [[CONTRIBUTING.md](CONTRIBUTING.md)] для подробной
Инструкции.

### Релизить новая версия

```bash
# Создать нового версию — npm publish происходит Автоматически
глава релизов создать v2.0.0 --title "v2.0.0" --generate-notes
```

---

## 📊 Написать истории звезд

## Звезда и время

## [![Звезда и время](https://starchart.cc/diegosouzapw/OmniRoute.svg?variant=adaptive)](https://starchart.cc/diegosouzapw/OmniRoute)

## 🙏 Признание

⭐️ Специальный спасибо ****(https://github.com/decolua/9router)[X36X] по
**[decolua](https://github.com/decolua)** — первоначальному проекту, оказавшему
вдохновение на этом ветвлении. OmniRoute построил на этом фантоме, расширив его
функциональность, добавив мультимодальные API и полное перекомпиляцию на
TypeScript.

⭐️ Специальный спасибо
**[CLIProxyAPI](https://github.com/router-for-me/CLIProxyAPI)** —
первоначальному имплементу на Go, который вдохновил JavaScript-порт.

---

## 📄 Лицензия

Лицензия MIT - см. [LICENSE](LICENSE) для подробной информации.

---

<div align="center">
  <sub>Built with ❤️ for developers who code 24/7</sub>
  <br/>
  <sub><a href="https://omniroute.online">omniroute.online</a></sub>
</div>
<!-- GitHub Discussions enabled for community Q&A -->
