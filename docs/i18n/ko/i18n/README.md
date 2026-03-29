# 🚀 OmniRoute — The Free AI Gateway

### 코드하는 것을 멈추지 마세요. 지능형 경로 설정을 위한 가볍고 저렴한 AI 모델에 대한 자동 fallback을 제공합니다.

_Your 통일된 API 프록시 - 하나의 종단점, 67+ 제공자, 0지움 시간. 현재 MCP & A2A 에이전트 오케스트레이션과 함께.

**채팅 완료 • 임베딩 시 • 이미지 생성 • 비디오 • 음악 • 오디오 • 리랭킹 • **웹 검색** • MCP 서버 • A2A 프로토콜 •
100% TypeScript**

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

🌐 **아vailable in:** 🇺🇸 영어 | 🇧🇷 브라질 포르투갈어 | 🇪🇸 스페인어 | 🇫🇷 프랑스어 | 🇮🇹 이탈리아어 | 🇷🇺
러시아어 | 🇨🇳 간체 중국어 | 🇩🇪 독일어 | 🇮🇳 힌디어 | 🇹🇭 태국어 | 🇺🇦 우크라이나어 | 🇸🇦 아랍어 | 🇯🇵 일본어 | 🇻🇳
베트남어 | 🇧🇬 불가리아어 | 🇩🇰 덴마크어 | 🇫🇮 핀란드어 | 🇮🇱 히브리어 | 🇭🇺匈牙利어 | 🇮🇩 인도네시아어 | 🇰🇷 한국어 | 🇲🇾
말레이어 | 🇳🇱 네덜란드어 | 🇳🇴 노르웨이어 | 🇵🇹 포르투갈어(포르투갈) | 🇷🇴 루마니아어 | 🇵🇱 폴란드어 | 🇸🇰 슬로바키아어 |
🇸🇪 스웨덴어 | 🇵🇭 필리핀어 | 🇨🇿 체코어

---

## 🆕 v3.0.0의 새로운 기능

> **v2.9.5에서 업그레이드하시나요?**? — 모든 변경 사항을 보기 위해 [full CHANGELOG]{1)에 가기 바랍니다.

| section                   | section                                                                                                             |
| ------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| 🔒 **CodeQL Security**     | 10+ CodeQL 경고 사항을 수선했습니다: polynomial-redos, 불안전한 난수 발생, shell-injection 치료                                          |
| ✅ **Route Validation**    | 모두 176 API 경로가 Zod 스키마와 함께 확인되며 `validateBody()`로 신속 한 CI `check:route-validation:t06`가 통과했습니다                      |
| 🐛 **omniModel Tag Leak**  | 내부 `<omnimodel>` 태그가 세션 스트리밍 응답에 client로 전달되어 더 이상 발생하지 않습니다 (#585)</omnimodel>                                     |
| 🔑 **Registered Keys API** | API 키를 자동으로 준비하십시오. 각 제공자의 계정 별 할당량 및 중복 시 이중성, SHA-256 스토리지, 옵션 GitHub 이슈 보고 및 `POST /api/v1/registered-keys`를 통해. |
| 🎨 **Provider Icons**      | 130+` 제공 로고 via `lobehub/icons[X123X] (SVG) with PNG → 일반 대체 체인                                                     |
| 🔄 **모델 자동同步**             | 24시간 스케쥴러와 수동 UI 토글을 이용해 내장형 및 Custom OpenAI 호환 제공자들에 대한 모델 목록을 동기화합니다.                                             |
| 🌐 **오픈코드 지움/고**           | @kang-heewon 의 PR #530에서 제공하는 두 개의 новых 제공자는 무료 계층과 구독 계층이 있으며 `오픈코드 실행자`를 매개변수로 제공합니다.                            |
| 🐛 **가마비 CLI OAuth**       | `GEMINI_OAUTH_CLIENT_SECRET` 가 отсутств할 때 Docker 에서 구체적인 Google 오류가 아닌 동작 가능한 오류를 표시합니다.                           |
| 🐛 **오픈코드 구성**             | `saveOpenCodeConfig()` 는 이제 `XDG_CONFIG_HOME` 에 TOML 을 정확히 기록합니다.                                                   |
| 🐛 **고정 모델 오버라이드**         | `body.model` 은 이제 `고정된 모델`의 값을 [X52X]context-cache 보호[X64X] 에서 설정합니다.                                               |
| 🐛 **코데/클라우드 로프**          | `tool_result` 블록은 이제 text 로 변환되어 불한 증류를 중단합니다.                                                                      |
| 🐛 **로그인 재지정**             | 로그인은 이제 패스워드 설정을 빠르게 뛰어넘는 경우 동결되지 않습니다.                                                                             |
| 🐛 **윈도우 경로**              | MSYS2/기본-Bash 경로 (`/c/...`)는 이제 automatically `C:\...`로 정규화됩니다.                                                     |

---

## 🖼️ 메인 대시보드

<div align="center">
  <img src="./docs/screenshots/MainOmniRoute.png" alt="OmniRoute Dashboard" width="800"/>
</div>

---

## 📸 대시보드 미리 보기

<details>
<summary><b>Click to see dashboard screenshots</b></summary>

| 페이지                     | 스크린샷                                           |
| ----------------------- | ---------------------------------------------- |
| [ X0X ] 제공 업체 [ X11X ]  | ![ 제공 업체 ](docs/screenshots/01-providers.png)  |
| [ X0X ] 조합 [ X8X ]      | ![ 조합 ](docs/screenshots/02-combos.png)        |
| [ X0X ] 분석 [ X11X ]     | ![ 분석 ](docs/screenshots/03-analytics.png)     |
| [ X0X ] 건강 [ X8X ]      | ![ 건강 ](docs/screenshots/04-health.png)        |
| [ X0X ] 번역 기사 [ X12X ]  | ![ 번역 기사 ](docs/screenshots/05-translator.png) |
| [ X0X ] 설정 [ X10X ]     | ![ 설정 ](docs/screenshots/06-settings.png)      |
| [ X0X ] CLI 도구 [ X11X ] | ![ CLI 도구 ](docs/screenshots/07-cli-tools.png) |
| [ X0X ] 사용 로그 [ X12X ]  | ![ 사용 ](docs/screenshots/08-usage.png)         |
| [ X0X ] 엔드 포인트 [ X11X ] | ![ 엔드 포인트 ](docs/screenshots/09-endpoint.png)  |

</details>

---

### 🤖 코드가好き한 에이전트들의 좋아하는 무료 인공지능 제공 업체

_AI-파워드 IDE 또는 CLI 툴을 연결하세요 - _무제한 코딩을 위한 무료 API 게이트웨이인 OmniRoute

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

<sub>📡 모든 에이전트는 <code>http://localhost:20128/v1</code> 또는
<code>http://cloud.omniroute.online/v1</code> — 하나의 구성, 무제한 모형 및 자원에 연결</sub>

---

## 🤔 OmniRoute는 何인가?

**금액을 낭비하고 제한을 맞을 필요가 없습니다:**

- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  월별로 자원은 남은 날까지 사용되지 않는다
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  제한된 비율로 작성을 중단합니다
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  실패한 API 프로바이더들 ($20-50/월에 달하는 비용)
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  모든 제공자 사이를 수동으로 스위칭

**OmniRoute는 이 문제를 해결합니다:**

- ✅ **할당량 tối대화** - 자원의 트랙킹, 리셋之前 모든 것을 사용하세요
- ✅ **자동으로 대체** - 구독 → API 키 → 저렴한 경우 → 무료, 영구 중단없이
- ✅ **멀티-계정** - 프로바이더마다 계정들의 중복을 round-robin으로 대체
- ✅ **형식에 의한** - CLUDE-Code, OpenClaw, Cursor, CLI 도구 등 모든 CLI 툴을 대응합니다

---

## 📧 사용자의 도움요청

> 💬 **여러분의 커뮤니티로 연결해 주세요!** [화상 메세지
> GROUP](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t) — 도움, 팁 공유
> 및 최신 업데이트를 받아보세요

- **공식사이트**: [omniroute.online](https://omniroute.online)
- **GitHub**:
  [github.com/diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute)
- **Issue**:
  [github.com/diegosouzapw/OmniRoute/issues](https://github.com/diegosouzapw/OmniRoute/issues)
- **화면의 지원**: [Community
  Group](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)
- **구성**: [CONTRIBUTING.md](CONTRIBUTING.md), PR 생성 또는 `좋은 첫 번째 이슈` 만들기
- **원래 프로젝트**: [9router by decolua](https://github.com/decolua/9router)

### 🐛 버그 신고하는 건가요?

이슈를 엽니다. 이 때, 시스템 정보(command) 명령을 연달아 실행하여 생성된 파일을 첨부합니다.

```bash
npm run system-info
```

제네레이트된 `system-info.txt`에는 Node.js 버전, OmniRoute 버전, OS 정보, 설치한 CLI 도구 (iflow,
gemini, claude, codex, antigravity, droid 등), Docker/PM2 상태, 시스템 패키지 및 기타 정보가
포함되어 있습니다. 이 정보를 통해 문제를 재생하고 다시 reproduce 할 수 있도록 GH 이슈에 직접 파일을 첨부합니다.

---

## 작동 방식

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
       ├─→ [Tier 1: 구독] Claude Code, Codex, Gemini CLI
       │   ↓ 수치 초과
       ├─→ [Tier 2: API KEY] DeepSeek, Groq, xAI, Mistral, NVIDIA NIM, etc.
       │   ↓ 지출 한도
       ├─→ [Tier 3: 저렴] GLM ($0.6/1M), MiniMax ($0.2/1M)
       │   ↓ 지출 한도
       └─→ [Tier 4: 무료] iFlow, Qwen, Kiro (무제한)

결과: 끊임없이 코딩해야 하며 비용 적발
```

---

## 🎯 OmniRoute가 çözüm하는 30 가지 실존하는 문제와 사용 사례

> ** 모든 개발자가 AI TOOL을 사용하는 사람들에게 문제가 일어나지만. ** OmniRoute는 해결책을 만드는데 사용되었습니다 — 비용
> 초과, 지역 차단, 패킷 도청, 메타 데이터 및 기업 도구 시야에서 나와옴

<details>
<summary><b>💸 1. "I pay for an expensive subscription but still get interrupted by limits"</b></summary>

개발자는 Claude Pro, Codex Pro 또는 GitHub Copilot를 위해 $20-$200의 월정액을 지불합니다. 결제 후에도
할당량(Limit)은 마주하게되며 정기적인 패킷 초과, 자원 초과, 요금 초과 한도 등을 마주하게되며 프로세스 중단, 중단, 개발자 흐름이
사라지게되기까지

**OmniRoute는 이를 어떻게 해결할까요?

- **지능형 4-Tier 후크 ** — 가용한 할당량 내에서 문제가 발생하면 자동으로 API KEY →Cheap → Free 경로에 빠르게
  전환 가능합니다
- **실시간 할당량 추적 ** — 사용된 토큰을 실시간으로 감시할 수 있으며(Reset 재발생) 리셋 카운트(5, 일간리셋, 주간 리셋)
- **Multi-Account 지원 ** — 다양한 계정을 지원하며 1개 account가 상향된지 바로 다음 account로 auto
  switch
- **Custom 합쳐지는 것 ** — 사용자 지정 fallback Chain을 지원하며 6가지의 균형 이룰 수 있는 스탠다드
  (fill-first, round-robin, P2C, random, least-used, cost-optimized)
- **Codex Business 할당량 ** — Business/Team의 workspace quota를 제공하며 직접 dashboard에서
  monitoring

</details>

<details>
<summary><b>🔌 2. "I need to use multiple providers but each has a different API"</b></summary>

OpenAI는 한 종류의 포맷을 사용합니다. Claude 또한 다른 형식으로 사용됩니다. Gemini도. 개발자만이 여러 종류의 패킷을 하나에
합쳐야만 합니다. Custom Provider도 그들의 전역을 재조망 해야만 합니다. 비중을 일으키는 것으로 인해 비율이 매우 미미합니다.

**OmniRoute는 이를 어떻게 해결할까요?

- **Unified endpoint ** — 단 하나의 `http://localhost:20128/v1`가 모든 67+ Providers
- **포맷 번역 ** — 자동으로 수행됩니다; OpenAI ↔ Claude ↔ Gemini ↔ Responses API
- **Response Sanitization** — 필드가 비 표준 항목인 경우 (`x_groq`, `usage_breakdown`,
  `service_tier`) OpenAI SDK v1.83+에서 제거
- **Role Normalization** — OpenAI 공급자 이외의 경우 `개발자` را `시스템`으로, GLM/ERNIE 에서는
  `시스템`을 `사용자`로 변환 함
- **Think Tag Extraction** — 모델에 적용되는 `&lt;think&gt;` 블록을 표준화 된 `의사 결정 내용`으로 추출
  함
- **Structured Output for Gemini** — `json_schema`를 ` 응답 유형`/` 응답 스키마`로 자동 변환 함
- **`stream`이 기본적으로 `false`임** — OpenAI 스펙을 일치 시KEN하며, Python/Rust/Go SDK에서 예상하지
  못한 SSE를 피 함

</details>

<details>
<summary><b>🌐 3. "My AI provider blocks my region/country"</b></summary>

인증과 API 접속시 특정 지리 지역에서 액세스를 차단하는 공급자가 있으며, 특히 개발자들은 사용자들은 개발국 출신일 때 이러한 오류를
경험합니다.

**OmniRoute는 이를 어떻게 해결할까요?

- **3-Level Proxy Config** — 전역, 공급자, 연결 키 수준의 구성 가능한 프록시
- **Color-Coded Proxy Badges** — 시각적으로 나타내는 프록시 : 🟢 전역 프록시, 🟡 공급자 프록시, 🔵 연결 프록시
  (IP 표시 항상)
- OAuth 흐름도 프록시를 통한 인증 토큰 교환** — 인증 토큰 교환도 프록시를 통하게 함으로써 `지원되지 않는 국가/지역 분지` 문제를
  해결함
- **Connection Tests via Proxy** — 연결 테스트도 프록시를 사용 함 (다시 직접 연결 하지 않음)
- **SOCKS5 지원** — 전송 라우팅을 위한 완전한 SOCKS5 프록시 지원
- **TLS 디지털 인상 오염** — `wreq-js`를 사용하여 보트 감지를 피하여 웹 브라우저와 같이 TLS 디지털 인상
- **🔏 CLI FingerPrint 매칭** — 원본 CLI 바이너스 시그니처에 맞추어 헤더 및 몸체 필드를 재 배치하여 계정 플래그 짚을
  피하고 아이피를 은닉하여 동시에 스틸스하고 아이피 홀딩을 함

</details>

<details>
<summary><b>🆓 4. "I want to use AI for coding but I have no money"</b></summary>

모든 사람들이 $20-$200/월에 AI 구독을 소비할 수 는 없습니다. emerginc countries의 개발자 및 초보 개발자, 헛병아 기
및 Freelancer들은 우수한 모델에 대해 0달러의 액세스를 필요로 하며, 그들의 수요를 충족시킵니다

**OmniRoute는 이를 어떻게 해결할까요?

- **무료 종류 공급자 built-in** — 자급자급의 자립 공급자 native 지원으로 : iFlow (OAuth로 5 models 무
  한정 액세스: kimi-k2-thinking, qwen3-coder-plus, deepseek-r1, minimax-m2, kimi-k2),
  Qwen (4 models 무 한정 액셀 : qwen3-coder-plus, qwen3-coder-flash,
  qwen3-coder-next, vision-model. Kiro (Claude + AWS 빌더 ID 는 무료), Gemini CLI
  (180K 토큰/월 무 한정 액셀)
- **Ollama 클라우드** — ` api.ollama.com` 의 클라우드 기반 ollama 모델 (free "Light usage"
  tier를 가짐 ): ollamacloud/
- **무료 Only combos** — 구성을 연결합니다. gc/gemini-3-flash → if/kimi-k2-thinking →
  qw/qwen3-coder-plus` = $0/month (zero downtime)
- **NVIDIA NIM이 무료 액셀** — ~40RPM 개발자가永久 무료 액셀을 가지기 위해 7+ 모델에 접근 할 수 있게 함
  (transitioning from credits to pure rate limits)
- **Cost Optimized Strategy** — Routing strategy that automatically chooses the
  cheapest available provider

</details>

<details>
<summary><b>🔒 5. "I need to protect my AI gateway from unauthorized access"</b></summary>

When exposing an AI gateway to the network (LAN, VPS, Docker), anyone with the
address can consume the developer's tokens/quota. Without protection, APIs are
vulnerable to misuse, prompt injection, and abuse.

**OmniRoute는 이를 어떻게 해결할까요?

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

**OmniRoute는 이를 어떻게 해결할까요?

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

**OmniRoute는 이를 어떻게 해결할까요?

- **CLI 툴 디스플레이** — Claude Code, Codex CLI, OpenClaw, Kilo Code, Antigravity,
  Cline 대 한 일 클릭 설정을 위한 전용 페이지
- **GitHub Copilot 설정 생성기** — `채팅 언어 모델 JSON`을 VS Code에 bulk 모델 선택과 함께 생성
- **온보딩 마법사** — 첫 번째 사용자의 경우 4 단계 설정을 위한 인도 된 대화
- **일つの 엔드 포인트, 모든 모델** — `http://localhost:20128/v1`을 한번 설정하면, 67+ 제공자를 접근 하실 수
  있습니다

</details>

<details>
<summary><b>🔑 8. "Managing OAuth tokens from multiple providers is hell"</b></summary>

Claude Code, Codex, Gemini CLI, Copilot — 모두 OAuth 2.0 이용 인가 토큰을 사용하며, 발급 기간이
흘러가기 전에 발급 받으셔야 합니다. 개발자들은 항상 재 발급을 사용 하셔야 하며, `클라이언트 시크릿이 누락 될 때`, `리다이렉트 URI를
불일치 할 때`,와 원격서버의 실패를 해결 하시려면 OAuth LAN/ VPS는 특히 문제가 많습니다.

**OmniRoute는 이를 어떻게 해결할까요?

- **자동 Token 갱신** — OAuth 토큰이 만료하기 전에 배경에서 갱신
- **OAuth 2.0 (PKCE) Built-in** — 자동 워크 플로우로 Claude Code, Codex, Gemini CLI,
  Copilot, Kiro, Qwen, iFlow 지원
- **다중 계정 OAuth** — 제공자의 경우 JWT/ID 토큰 추출을 통해 구분 된 계정
- **OAuthLAN/Remote Fix** — `리다이렉트 URI`에_PRIVATE IP 감지로 + 원격 서버를 위해 수동 URL 모드
- **OAuth 뒤 nginx** — 리버스 프록시 호환성에 대하여 `창 닫기. 원본`사용
- **원격 OAuth 가이드** — VPS/Docker를 대하여 Google Cloud credential Step-by-step 구성

</details>

<details>
<summary><b>📊 9. "I don't know how much I'm spending or where"</b></summary>

개발자들이 다중 비용을 결제 하지만 유니폼한 지출 통계 화면을 가지고 계거나 안됩니다 각 제공자가 자신의 이익의 지수를 가지고 있지만 안됩니다
합계되는 지출 화면을 보는 경우 예상되지 않은 비용이 쌓이 고 있습니다

**OmniRoute는 이를 어떻게 해결할까요?

- **비용 통계 디스플레이** — 제공자별 단일 토큰 비용 추적 및 예산 관리
- **각 계층당 예산 한도** — 지출 한계가 자동으로 내리 기 트리거하는 예산 한도
- **모델당 가성구성** — 설정가능한 요금별 모델 비용
- **API Key 당 사용 통계** — 키당 요청 카운트 및 마지막으로 사용한 시간
- **분석 통계 화면** — 통계 카드를 모용했 는 모형사용 그래프, 제공자의 표에 대한 성공률과 지연 시간

</details>

<details>
<summary><b>🐛 10. "I can't diagnose errors and problems in AI calls"</b></summary>

When a call fails, the dev doesn't know if it was a rate limit, expired token,
wrong format, or provider error. Fragmented logs across different terminals.
Without observability, debugging is trial-and-error.

**OmniRoute는 이를 어떻게 해결할까요?

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

**OmniRoute는 이를 어떻게 해결할까요?

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

**OmniRoute는 이를 어떻게 해결할까요?

- **대시보드 국제화 — 30개 언어** — 모두 500개 이상의 키의 번역, včetně 아랍어, 불가리아어, 덴마크어, 독일어, 스페인어,
  핀란드어, 프랑스어, 히브리어, 힌디어, 헝가리어, 인도네시아어, 이탈리아어, 일본어, 한국어, 말레이어, 네덜란드어, 노르웨이어,
  폴란드어, 포르투갈어, 루마니아어, 러시아어, 스위스어, 스웨덴어, 태국어, 우크라이나어, 베트남어, 중국어, 필리핀어, 영어
- **문장 지원** — 아랍어와 히브리어에 대한 우 прави쓰-왼쪽 지원
- **다국어 README** — 30개의 완전한 문서 번역
- **언어 선택기** —.header에 실시간 전환을위한 글로벌 동그란 icon

</details>

<details>
<summary><b>🔄 13. "I need more than chat — I need embeddings, images, audio"</b></summary>

AI는 단순한 채팅 완료 외에도 개발자가 이미지 생성, 오디오 녹음, RAG에 대해 임베딩, 문서 재 랭크, 콘텐츠 모니터링을 할 수 있습니다.
각 API는 다른 끝점과 형식이 있습니다.

**OmniRoute는 이를 어떻게 해결할까요?

- ** 임베딩** — `/v1/embeddings`와 함께 6개의 공급자 및 9+ 모형
- **이미지 생성** — `/v1/images/generations`와 함께 10개의 공급자 및 20+ 모형 (OpenAI, xAI,
  Together, Fireworks, Nebius, Hyperbolic, NanoBanana, Antigravity, SD WebUI,
  ComfyUI)
- **텍스트-비디오** — `/v1/videos/generations` — ComfyUI (AnimateDiff, SVD)와 SD WebUI
- **텍스트-음악** — `/v1/music/generations` — ComfyUI (Stable Audio Open, MusicGen)
- ** 오디오 사전 처리** — `/v1/audio/transcriptions` — Whisper + Nvidia NIM,
  HuggingFace, Qwen3
- **텍스트-음성** — `/v1/audio/speech` — ElevenLabs, Nvidia NIM, HuggingFace, Coqui,
  Tortoise, Qwen3, **Inworld**, **Cartesia**, **PlayHT**, + 기존 공급자
- ** 모니터링** — `/v1/moderations` — 콘텐츠 안전 체크
- ** 리랜킹** — `/v1/rerank` — 문서 관련성 리랜킹
- **응답 API** — Codex의 모든 `/v1/responses` 지원

</details>

<details>
<summary><b>🧪 14. "I have no way to test and compare quality across models"</b></summary>

개발자는 코드, 번역, 추론에 각 용도에 가장 적합한 모델을 알고 싶어합니다만, 수동으로 비교하려면 매우 시간이 걸립니다. 통합 정의 기기는
존재하지 않습니다.

**OmniRoute는 이를 어떻게 해결할까요?

- ** LLM 평가** — 10개의 프리 로드 케이스가 담갔던 인사, 산술 연산, 지리학, 코드 생성, JSON 준수, 번역, 마크다운, 안전
  거부의 골덴 셋 테스트
- ** 4가지 일치 전략** — `exact`, `contains`, `regex`, `custom` (JS 함수)
- ** 번역기 플레이그라운드 테스트 테이블** — 다중 입력과 예상 옴아의 배치 테스트, 제공업체間의 리한 비교
- **채팅 테스터** — 완전한 라운트 트립과 시각적 응답 렌더링
- **라이브 모니터** — 모든请求에 대한 리얼 타임 스트림

</details>

<details>
<summary><b>📈 15. "I need to scale without losing performance"</b></summary>

요청 부하가 증가할수록, 캐싱되지 않은 동일한문제는 중복 비용을 발생시킨다. 중복 요청은 처리를 낭비한다. 제공자별 속도 제한 사항은 반드시
준수되어야한다.

**OmniRoute는 이를 어떻게 해결할까요?

- **명령어 캐시** — 서명 + 명령어 캐시 (두 계층)를 비용과 지연도를 줄인다
- **중복 요청 제어** — 동일한 요청에 대한 5초 지연 기간
- **속도 제한 감지** — 제공자별 RPM, 최소 간격, 최대 동시 프로세스 추적
- ** 편집 가능한 속도 제한** — 설정 → 강건성에 영구 저장가능 한 기본값
- ** API 키 검증 캐시** — 프로덕션 내 성능 최적화
- **health 데시포드 화면에 텔레미터리** — p50/p95/p99 지연, 캐시 통계, 경과 시간

</details>

<details>
<summary><b>🤖 16. "I want to control model behavior globally"</b></summary>

개발자가 모든 응답에 대한 특정 언어, 특정 톤, 또는 사유 토큰 제한을 설정하고 싶다면, 다른 도구/요청에 적용하는 것은 부담된다.

**OmniRoute는 이를 어떻게 해결할까요?

- **시스템 프롬프트 주입** — 모든 요청에 글로벌로 적용되는 프롬프트
- **사유 예산 검증** — 요청별 사유 토큰 할당 제어
- **6 경로 전략** — 요청 분배에 관련된 전역 전략
- ** 와일드 카드 라우터** — 제공자/* 패턴에서 요청을 동적인 제공자에 라우팅
- **콤보 ENABLE/DISABLE 토글** — 도슈보드에서 콤보를 직접 활성화/비활성화로 설정합니다.
- **제공자 토글** — 제공자 하나를 클릭하면 모든 연결을 활성화하거나 비활성화할 수 있습니다
- **차단된 제공자** — 주소 /v1/models/X67X/_listing에서 특정 제공자를 포함하고 싶지 않습니다

</details>

<details>
<summary><b>🧰 17. "I need MCP tools as first-class product capabilities"</b></summary>

많은 AI 게이트웨이는 MCP를 최소한의 구현 디테일로 노출한다. 팀이 보이지 않는 경고 층에서 제어가 가능한 visible, 관리 가능한 운영
층이 필요합니다.

**OmniRoute는 이를 어떻게 해결할까요?

- 대시보드 내비게이션과 엔드포인트 프로토콜 탭에서 MCP가 나타납니다.
- 스COPE, 툴, 프로세스, ауд트와 같은 데디케이드 MCP 관리 페이지
- 인 omniroute --mcp와 클라이언트 onboard링을 위한 내장 quick-start `에 관해

</details>

<details>
<summary><b>🧠 18. "I need A2A orchestration with sync + stream task paths"</b></summary>

에이전트 워크플로는 직접 응답과 Lifecycle 관리가 가능한 롱 런닝 스트리밍 스타임이 필요합니다.

**OmniRoute는 이를 어떻게 해결할까요?

- A2A JSON-RPC 엔드포인트 (`POST /a2a`)는 [X41X와 [X60X가 있습니다.
- SSE 스트리밍은 종단 상태 전파와 함께 사용됩니다.
- 작업 라이프 사이클 API는 `tasks/get`> 와 `tasks/cancel`>이 있습니다.

</details>

<details>
<summary><b>🛰️ 19. "I need real MCP process health, not guessed status"</b></summary>

운영 팀은 MCP가 실제로 살아 있는지, API만 도달할 수 있는건지 나누어 알고 싶습니다.

**OmniRoute는 이를 어떻게 해결할까요?

- 종료 시간, PID, 스코프 모드, 도구 세트, 통신 모드와 같은 런타임 하트 비트 파일
- MCP 상태 API는 하트 비트 + 최근 활동 combining
- 프로세스/업타임/하트 비트 청순도와 같은 UI 상태 카드

</details>

<details>
<summary><b>📋 20. "I need auditable MCP tool execution"</b></summary>

도구 config 또는 OPs 작업을 트리거할 때 팀은 법학적 추적 가능성이 필요합니다.

**OmniRoute는 이를 어떻게 해결할까요?

- SQLight 백드업으로 audit 로깅을 위하여 MCP tool calls
- 도구, 성공/실패, API 키, 페이저와 같은 필터링이 필요합니다.
- 자동화용 대시보드 AUDIT 테이블 + 스태츠 엔드 포인트

</details>

<details>
<summary><b>🔐 21. "I need scoped MCP permissions per integration"</b></summary>

클라이언트는 최소 특권 접근을 할 수 있는 도구 카테고리\
```

**OmniRoute는 이를 어떻게 해결할까요?

- 9 가지 조정된 도구 액세스를 위한 세세한 MCP 스코프
- MCP 관리 UI 내에서 스코프 강제 및 가시성
- 운영 도구링에 대한 safe 기본 의식

</details>

<details>
<summary><b>⚙️ 22. "I need operational controls without redeploying"</b></summary>

비상사태나 비용 이벤트 시 인시던트 또는 빠른 런타임 설정이 필요합니다.

**OmniRoute는 이를 어떻게 해결할까요?

- MCP داش보드에서 스위치 콤보 활성화
- 정의済み 정책 패키스에서 탄력성 프로파일 적용
- 같은 작업 조정 패널에서 순서 브레이커 상태 복원

</details>

<details>
<summary><b>🔄 23. "I need live A2A task lifecycle visibility and cancellation"</b></summary>

타スク 인시던트가 잘못_triage되어 지적이 어려울 경우 생기는 lifecycles 가시성이 없습니다.

**OmniRoute는 이를 어떻게 해결할까요?

- 태스크목록/필터링을 바탕에 한 pagination
- 원천에 한된 태스크 메타데이터,이벤트 및 원본에 대한_drill down
- 예약 태스크 취소 엔드포인트 및 UI 액션에 대한 확인

</details>

<details>
<summary><b>🌊 24. "I need active stream metrics for A2A load"</b></summary>

스트리밍 워크플로가 동시執행 및 실시간 연결에 대해 작업 효율성의 관점이 필요합니다.

**OmniRoute는 이를 어떻게 해결할까요?

- A2A 상태내에 유효한 스트림 카운터 통합
- 최상태의 태스크 티스트임스탬프 및 한 상태당 개수
- 실시간 오픈 모니터링을 위한 A2A داش보드 카드

</details>

<details>
<summary><b>🪪 25. "I need standard agent discovery for clients"</b></summary>

온보딩에 필요했던 머신-readable 메타데이터를 클라이언트 및 유도차를 필요합니다.

**OmniRoute는 이를 어떻게 해결할까요?

- एज런트 카드 `/.well-known/agent.json` 노출
- 관리 UI에서 보여지는 능력과 강점
- A2A статус API는 자동화에 사용되는 탐지 메타데이터를 포함합니다.

</details>

<details>
<summary><b>🧭 26. "I need protocol discoverability in the product UX"</b></summary>

사용자들이 프로토콜 표면을 탐지하지 못하는 경우, 수용 및 지원 품질이 저하됩니다.

**OmniRoute는 이를 어떻게 해결할까요?

- 결합된 **엔드포인트** 페이지에 탭으로 Proxy, MCP, A2A, API Endpoints가 있습니다.
- MCP와 A2A의 온라인/오프라인 상태를 표시하는 인라인 서비스 статус 스위치
- 개요에 해당하는 관리 탭으로의 링크

</details>

<details>
<summary><b>🧪 27. "I need end-to-end protocol validation with real clients"</b></summary>

Mock 테스트만으로는 프로토콜 호환성을 시험해볼 수 없습니다.

**OmniRoute는 이를 어떻게 해결할까요?

- 앱을 부팅하고 MCP SDK 클라이언트 전송을 사용하는 단위 테스트
- A2A 클라이언트 테스트: send, stream, get, cancel 플로우
- MCP 감사 및 A2A 작업 시 API와의 보충적 검증 확인

</details>

<details>
<summary><b>📡 28. "I need unified observability across all interfaces"</b></summary>

프로토콜에 따라 보이지 않는 장소와 큰 MTTR를 발생시키는 조립 관찰

**OmniRoute는 이를 어떻게 해결할까요?

- 하나의 제품에서 유니파이드 다쉬보드/로그/분석도구
- OpenAI, MCP, A2A 계층에 걸쳐 성능 + 감사 + 수요 수신 추적
- 상태와 자동화에 대한 운영 API

</details>

<details>
<summary><b>💼 29. "I need one runtime for proxy + tools + agent orchestration"</b></summary>

여러 별도의 서비스를 실행하는 경우 운영 비용과 장애 모드가 증가합니다.

**OmniRoute는 이를 어떻게 해결할까요?

- OpenAI-compatible proxy, MCP 서버, 및 A2A 서버는 한 개의 스택
- 공유 인증, 내결함성, 데이터 저장소, 및 관찰可能性
- 모든 상호 작용 표면에서 일관된 정책 모델

</details>

<details>
<summary><b>🚀 30. "I need to ship agentic workflows without glue-code sprawl"</b></summary>

팀이 여러 아등바등한 서비스 및 스크립트를 연결하는 작업이 지속될 때 velocity를 잃습니다

**OmniRoute는 이를 어떻게 해결할까요?

- 클라이언트와 에이전트에 대한 통합 엔드포인트 전략
- 내장된 프로토콜 관리 UI와 스픈 인증 경로
- 보안, 로깅, 내결함성, 백업을 포함한 생산 준비 태스트베이스

</details>

### 인터그레이티드 사용 사례 예시(Playbooks)

**Playbook A: 최대 결제 서브스크립션 + 낮은 백업 비용**

```txt
콤보: "maximize-claude"
 1. cc/claude-opus-4-6
 2. glm/glm-4.7
 3. if/kimi-k2-thinking

월간 비용: $20 + 낮은 백업 비용
결과: 더 높은 품질, 고유의 중단
```

**Playbook B: 무료 코딩 스택**

```txt
콤보: "free-forever"
 1. gc/gemini-3-flash
 2. if/kimi-k2-thinking
 3. qw/qwen3-coder-plus

월간 비용: $0
결과: 안정적인 무료 코딩 워크플로우
```

**Playbook C: 24/7 정상작동용 백업 체인**

```txt
콤보: "always-on"
 1. cc/claude-opus-4-6
 2. cx/gpt-5.2-codex
 3. glm/glm-4.7
 4. minimax/MiniMax-M2.1
 5. if/kimi-k2-thinking

결과: 기한 엄수한 작업 부하에 대한 깊은 백업 깊이
```

**Playbook D: 에이전트 작동 + MCP + A2A**

```txt
1) MCP 전송 시작 (`omniroute --mcp`) tool-driven 작동을 위하여
2) A2A tasks Run via `message/send` 및 `message/stream`
3) MCP 및 A2A 탭을 포함한 /dashboard/endpoint (MCP와 A2A)를 통해서 관찰
4) Inline 상태 제어를 통하여 서비스切りをToggle
```

---

## 🆓 무료로 시작 — zero configuration 비용을 지불하지 않습니다

> **$0/month**에 대해 AI 코딩을 분속시간 내에 설정하고, 무료 계정을 연결하고 내장된 **Free Stack** 콤보를
> 사용하세요.

| -step | 액션                                      | 제공사 해제                                                       |
| ----- | --------------------------------------- | ------------------------------------------------------------ |
| 1     | Connect **Kiro** (AWS Builder ID OAuth) | 클라우드 소ネット 4.5, 하이쿠 4.5 — **무제한**                             |
| 2     | Connect **iFlow** (Google OAuth)        | kimi-k2-thinking, qwen3-coder-plus, deepseek-r1... — **무제한** |
| 3     | Connect **Qwen** (Device Code)          | qwen3-coder-plus, qwen3-coder-flash... — **무제한**             |
| 4     | Connect **Gemini CLI** (Google OAuth)   | gemini-3-flash, gemini-2.5-pro — **180K/mo 무료**              |
| 5     | `/대시보드/컴보` → **무료 스택 ($0)** 템플릿         | 자동으로 모든 무료 제공사를 순환합니다                                        |

**IDE/CLI를 ** `http://localhost:20128/v1`로 지시하세요: · API Key: `어떤 문자열` · 완료.

> **선택적인 초과 커버리지 (또한 무료): ** Groq API 키 (30 RPM 무료), NVIDIA NIM (40 RPM 무료, 70+
> 모델), Cerebras (1M tok/day), LongCat API 키 (50M tokens/day!), Cloudflare
> Workers AI (10K 뉴런/day, 50+ 모델).

## 빠른 시작

### 1. 설치 및 실행

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

### 2) 공급자와 연결하여 API 키를 생성하세요

1. Open Dashboard → 공급자` 연결` 최소 하나의 공급자 (OAuth 또는 API 키)를 연결하세요.
2. Open Dashboard → 엔드포인트[X35X] 창에서 API 키를 생성하세요.
3. (전용) Open Dashboard → 대체 체인`을 설정할 경우

### 3) 개발 도구를 OmniRoute로 설정하세요

```txt
서버 URL: http://localhost:20128/v1
API 키:  엔드포인트에서 복사
모델:    if/kimi-k2-thinking (또는 공급자/ 모델 접두사)
```

Claude Code, Codex CLI, Gemini CLI, Cursor, Cline, OpenClaw, OpenCode, OpenAI 호환
가능 애플리케이션 SDK와 호환합니다.

### 4) 프로토콜을 활성화 및 Validate (v2.0)

**MCP (도구에 의해 구동되는 작업):**

```bash
omniroute --mcp
```

그런 다음 MCP 클라이언트를 `stdio`를 통해 연결하고 TOOL을 테스트하세요:

- `omniroute_get_health`
- `omniroute_list_combos`

**A2A (사용자 간 워크플로의 대리인):**

```bash
curl http://localhost:20128/.well-known/agent.json
```

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"quickstart","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"내용 요약을 주세요."}]}}'
```

### 5) 모든 게 끝까지 테스트하길 권장합니다

```bash
npm run test:protocols:e2e
```

이 스위트는実行중인 앱에 대한 실제 MCP 및 A2A client flow를 검증합니다.

### Alternate는 소스 코드를 실행합니다.

```bash
cp .env.example .env
npm install
PORT=20128 DASHBOARD_PORT=20129 NEXT_PUBLIC_BASE_URL=http://localhost:20129 npm run dev
```

---

## 🐳 Docker

오면닉루트는 [Docker Hub](https://hub.docker.com/r/diegosouzapw/omniroute)에 공개 Docker
이미지로 이용할 수 있습니다.

**빠른 구동:**

```bash
docker run -d \
  --name omniroute \
  --restart unless-stopped \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:latest
```

**환경 파일 사용:**

```bash
#.env 예시 파일 복사 후 편집 먼저
cp .env.example .env

docker run -d \
  --name omniroute \
  --restart unless-stopped \
  --env-file .env \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:latest
```

**Docker Compose 사용:**

```bash
# 기본 프로파일 (클라이언트 도구 없음)
docker compose --profile base up -d

# CLI 프로파일 (Claude Code, Codex, OpenClaw 기본)
docker compose --profile cli up -d
```

| 이미지                      | 태그      | 크기     | Description |
| ------------------------ | ------- | ------ | ----------- |
| `diegosouzapw/omniroute` | `최신`    | ~250MB | 최신 안정 버전    |
| `diegosouzapw/omniroute` | `1.0.3` | ~250MB | 현재 버전       |

---

## 🖥️ 데스크톱 앱 — 오프라인 & 항시 동작

> 🆕 **NEW!** OmniRoute is now available as a **native desktop application** for
> Windows, macOS, and Linux.

Run OmniRoute as a standalone desktop app — no terminal, no browser, no internet
required for local models. The Electron-based app includes:

- 🖥️ **Native Window** — Dedicated app window with system tray integration
- 🔄 **Auto-Start** — Launch OmniRoute on system login
- 🔔 **Native Notifications** — Get alerts for quota exhaustion or provider
  issues
- ⚡ **One-Click Install** — NSIS (Windows), DMG (macOS), AppImage (Linux)
- 🌐 **Offline Mode** — Works fully offline with bundled server

### 빠른 시작

```bash
# Development mode
npm run electron:dev

# Build for your platform
npm run electron:build         # Current platform
npm run electron:build:win     # Windows (.exe)
npm run electron:build:mac     # macOS (.dmg) — x64 & arm64
npm run electron:build:linux   # Linux (.AppImage)
```

### System Tray

When minimized, OmniRoute lives in your system tray with quick actions:

- 대시보드 열기
- Change server port
- Quit application

📖 Full documentation: [`electron/README.md`](electron/README.md)

---

## 💰 Pricing at a Glance

| Tier               | Provider                   | Cost                     | Quota Reset      | Best For                          |
| ------------------ | -------------------------- | ------------------------ | ---------------- | --------------------------------- |
| **💳 SUBSCRIPTION** | Claude Code (Pro)          | $20/mo                   | 5h + weekly      | Already subscribed                |
|                    | Codex (Plus/Pro)           | $20-200/mo               | 5h + weekly      | OpenAI users                      |
|                    | Gemini CLI                 | **FREE**                 | 180K/mo + 1K/day | Everyone!                         |
|                    | GitHub 코파일럿                | $10-19/mo                | Monthly          | GitHub users                      |
| **🔑 API KEY**      | NVIDIA NIM                 | **FREE** (dev forever)   | ~40 RPM          | 70+ open models                   |
|                    | Cerebras                   | **FREE** (1M tok/day)    | 60K TPM / 30 RPM | World's fastest                   |
|                    | Groq                       | **FREE** (30 RPM)        | 14.4K RPD        | Ultra-fast Llama/Gemma            |
|                    | DeepSeek V3.2              | $0.27/$1.10 per 1M       | 없음               | Best price/quality reasoning      |
|                    | xAI Grok-4 Fast            | **$0.20/$0.50 per 1M** 🆕 | 없음               | Fastest + tool calling, ultralow  |
|                    | xAI Grok-4 (standard)      | $0.20/$1.50 per 1M 🆕     | 없음               | Reasoning flagship from xAI       |
|                    | 미스트랄                       | 免費試用 + 收費                | 요금 제한            | 歐洲 AI                             |
|                    | OpenRouter                 | 按需付費                     | 없음               | 100+ 模型叢集                         |
| **💰 便宜**           | GLM-5 (通過 Z.AI) 🆕          | 每 100萬個 $0.5             | 每天 10 點鐘         | 128k 輸出，最新冠軍                      |
|                    | GLM-4.7                    | 每 100萬個 $0.6             | 每天 10 點鐘         | 預算備份                              |
|                    | MiniMax M2.5 🆕             | 每 100萬個輸入 $0.3           | 5 小時移動           | 推理 + 式任務                          |
|                    | MiniMax M2.1               | $0.2/1M                  | 5 小時移動           | 가장 저렴한 옵션                         |
|                    | Kimi K2.5 (Moonshot API) 🆕 | 按需付費                     | 없음               | moonshot API 직접 접근                |
|                    | Kimi K2                    | 기본 요금 $9/월               | 월 10만 개 토큰       | 예측할 수 있는 비용                       |
| **🆓 무료**           | iFlow                      | **$0**                   | 무제한              | 5 모델 무제한                          |
|                    | Qwen                       | **$0**                   | 무제한              | 4 모델 무제한                          |
|                    | Kiro                       | **$0**                   | 무제한              | Claude Sonnet/Haiku (AWS Builder) |
|                    | LongCat Flash-Lite 🆕       | **$0** (50M tok/day 🔥)   | 1초당 1개 요청        | 자연어 중대 한정량                        |
|                    | Pollinations AI 🆕          | **$0** (no key needed)   | 1 req/15s        | GPT-5, Claude, DeepSeek, Llama 4  |
|                    | Cloudflare Workers AI 🆕    | **$0** (10K Neurons/day) | ~150 resp/day    | 50+ models, global edge           |
|                    | Scaleway AI 🆕              | **$0** (1M tokens total) | 요금 제한            | EU/GDPR, Qwen3 235B, Llama 70B    |

> 🆕 **뉴 모델이 추가되었습니다 (2026년 3월). ** Grok-4 Fast 가족 ($0.20/$0.50/M - 1143ms -
> Gemini 2.5 Flash보다 30% 빠르다), GLM-5 (Z.AI를 통해 128K 출력), MiniMax M2.5 reasoning,
> DeepSeek V3.2 가격 업데이트, Kimi K2.5 (Moonshot 직접 API를 통해)

**💡 $0 콤보 스택 — 완전한免费 설정: **

```
# 🆓 2026년 최고의 무료 스택 - 11개 제공자, $0.forever
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

**$0 never stops coding.** 하나의 OmniRoute 콤보로 구성하면 모든 폴백이 자동으로 일어나 — 매뉴얼 스틱 스위칭이
필요하지 않습니다.

---

---

## 🆓 무료 모델 — 실제로 받을 수 있는 것

> 아래의 모든 모델은 **100% 무료이며$0의 크레디트 카드가 필요** 합니다. OmniRoute는 한 계정의 할당량이 마감될 때마다
> 사용자의 계정을 자동으로 라우팅합니다 — 한 쌓기를 모두 조합하면 절대 무제한의 $0 콤보가됩니다.

### 🔵 CLAUDE 모델(시로 -- AWS 빌더 ID를 통해)

| Model               | 접두사   | limit         | 비율 제한                 |
| ------------------- | ----- | ------------- | --------------------- |
| `claude-sonnet-4.5` | `kr/` | **Unlimited** | No reported daily cap |
| `claude-haiku-4.5`  | `kr/` | **Unlimited** | No reported daily cap |
| `claude-opus-4.6`   | `kr/` | **Unlimited** | Latest Opus via Kiro  |

### 🟢 IFLOW MODELS (Free OAuth — No Credit Card)

| Model              | 접두사   | limit         | 비율 제한           |
| ------------------ | ----- | ------------- | --------------- |
| `kimi-k2-thinking` | `if/` | **Unlimited** | No reported cap |
| `qwen3-coder-plus` | `if/` | **Unlimited** | No reported cap |
| `깊이 탐색-r1`         | `if/` | **Unlimited** | No reported cap |
| `최소최대자-m2.1`       | `if/` | **Unlimited** | No reported cap |
| `키미-k2`            | `if/` | **Unlimited** | No reported cap |

### 🟡 QWEN 모델 (디바이스 코드 인증)

| Model               | 접두사   | limit         | 비율 제한           |
| ------------------- | ----- | ------------- | --------------- |
| `qwen3-coder-plus`  | `qw/` | **Unlimited** | No reported cap |
| `qwen3-coder-flash` | `qw/` | **Unlimited** | No reported cap |
| `qwen3-coder-next`  | `qw/` | **Unlimited** | No reported cap |
| `VISION 모델`         | `qw/` | **Unlimited** | 멀티 모달 (이미지)     |

### 🟣 지니미 클리 (구글 OATH)

| Model                   | 접두사  | limit                | 비율 제한 |
| ----------------------- | ---- | -------------------- | ----- |
| gemini-3-flash-preview` | gc/` | **180K 토큰/월** + 1K/일 | 월간 리셋 |
| gemini-2.5 프로`          | gc/` | 180K/month (공유 풀로부터) | 고 品질  |

### ⚫ NVIDIA NIM (미료 API-key — build.nvidia.com)

| Tier     | 일일 한도    | 비율 제한       | 메모                                 |
| -------- | -------- | ----------- | ---------------------------------- |
| 무료 (Dev) | 토큰 제한 없음 | **~40 RPM** | 70+ 모델; 2025년 중반 pure rate 제한으로 전환 |

가장 인기 있는 무료 모델: `moonshotai/kimi-k2.5` (Kimi K2.5), `z-ai/glm4.7` (GLM 4.7),
`deepseek-ai/deepseek-v3.2` (DeepSeek V3.2), `nvidia/llama-3.3-70b-instruct`,
`deepseek/deepseek-r1`

### ⚪ CEREBRAS (미료 API-key — inference.cerebras.ai)

| Tier | 일일 한도       | 비율 제한            | 메모                       |
| ---- | ----------- | ---------------- | ------------------------ |
| 무료   | **1M 토큰/일** | 60K TPM / 30 RPM | 세계에서 가장 빠른 LLM 추론; 일일 리셋 |

유료로 이용 가능: `llama-3.3-70b`, `llama-3.1-8b`, `deepseek-r1-distill-llama-70b`

### 🔴 GROQ (무료 API 키 — console.groq.com)

| Tier | 일일 한도         | 비율 제한     | 메모                               |
| ---- | ------------- | --------- | -------------------------------- |
| 무료   | **14.4K RPD** | 1 모델당 30초 | 신용카드로 billed되지 않음; 한도 초과시 429 오류 |

유료로 이용 가능: `llama-3.3-70b-versatile`, `gemma2-9b-it`, `mixtral-8x7b`,
`whisper-large-v3`

### 🔴 LONGCAT AI (무료 API 키 — longcat.chat) 🆕

| Model                         | 접두사   | 일일 무료 할부         | 메모                     |
| ----------------------------- | ----- | ---------------- | ---------------------- |
| `LongCat-Flash-Lite`          | `lc/` | **50M tokens** 💥 | 자세히 보는-largest free 할부 |
| `LongCat-Flash-Chat`          | `lc/` | 500K tokens      | 멀티턴 채팅                 |
| `LongCat-Flash-Thinking`      | `lc/` | 500K tokens      | 이유/CoT                 |
| `LongCat-Flash-Thinking-2601` | `lc/` | 500K tokens      | 2026년 1월 버전            |
| `LongCat-Flash-Omni-2603`     | `lc/` | 500K tokens      | 멀티 모드                  |

> 퍼블릭 베타期间 100% 무료입니다. 이메일이나 전화로 [longcat.chat](https://longcat.chat) 에 가입하세요.
> 매일 00:00 UTC에서 리셋됩니다.

### 🟢 POLLINATIONS AI (API 키 없이) 🆕

| Model      | 접두사    | 비율 제한     | 서비스 제공자 뒤에         |
| ---------- | ------ | --------- | ------------------ |
| `openai`   | `pol/` | 1 req/15s | GPT-5              |
| `claude`   | `pol/` | 1 req/15s | Anthropic Claude   |
| `gemini`   | `pol/` | 1 req/15s | Google Gemini      |
| `deepseek` | `pol/` | 1 req/15s | DeepSeek V3        |
| `llama`    | `pol/` | 1 req/15s | Meta Llama 4 Scout |
| `mistral`  | `pol/` | 1 req/15s | Mistral AI         |

> ✨ **적응 없는 중립력:** 회원가입도 안했구, API 키도 없는데 Pollinations provider에 공백키로 넣으면 바로
> 작동합니다.

### 🟠 클라우드 플레어 워커스 AI (무료 API 키 - cloudflare.com) 🆕

| Tier | 일일 뉴런    | equivaleint usage                          | 메모             |
| ---- | -------- | ------------------------------------------ | -------------- |
| 무료   | [10,000] | ~150 LLM resp / 500s audio / 15,000 embeds | 글로벌 엣지, 50+ 모델 |

인기있는 무료 모델: [@cf/meta/llama-3.3-70b-instruct] , [@cf/google/gemma-3-12b-it] ,
[@cf/openai/whisper-large-v3-turbo](무료 오디오!),
[@cf/qwen/qwen2.5-coder-15b-instruct]

> API 토큰 및 계정 ID가 필요하며 [dash.cloudflare.com](https://dash.cloudflare.com)에서
> 얻으십시오. 계정 ID는 제공자 설정에 저장해 주십시오.

### 🟣 SCALEWAY AI (1M 무료 토큰 — scaleway.com) 🆕

| Tier | 무료 할당량      | 위치        | 메모                             |
| ---- | ----------- | --------- | ------------------------------ |
| 무료   | [1M tokens] | 🇫🇷 파리, EU | 한도를 넘어서지 않는 한信用 카드가 필요하지 않습니다. |

무료로 khả 쓰는 것?: [@qwen3-235b-a22b-instruct-2507](Qwen3 235B!) ,
[@llama-3.1-70b-instruct] , [@mistral-small-3.2-24b-instruct-2506] ,
[@deepseek-v3-0324]

> EU/GDPR 동의. API 키는 [console.scaleway.com](https://console.scaleway.com)에서
> 받으십시오.

> ** 📈 최상의 무료 스택(11 개 제공자, 영원히 무료): [ ]
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

| Provider         | Free Credits           | Best Model                                   | 비율 제한                        |
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
| 🔌 **이플러그 ability RouterStrategy**   | 확장 가능한 `RouterStrategy`インタ페이스 — 플러그인으로 커스텀 라우팅 로직을 추가하십시오                                   |

### 🚀 이전 v2.0.9+ — 플레이그라운드, CLI 지문 & ACP

| Feature                              | What It Does                                                                                            |
| ------------------------------------ | ------------------------------------------------------------------------------------------------------- |
| 🎮 **Model 플레이그라운드**                  | 모델을 직접 테스트하는 데 사용되는 디래쉬보드 페이지 — 제공자/모델/엔드포인트 선택기에, Monaco 편집기, 스트리밍, 중단, 타임킹                            |
| 🔏 **CLI 지문 매칭**                      | 제공업체 별 헤더/바디 정렬을 통해 원본 CLI 서명과 매칭하십시오 — 세팅 > 보안에서 제공업체 별 toggle를 사용하십시오. **Your proxy IP is preserved** |
| 🤝 **ACP 지원 (Agent Client Protocol)** | CLI 에이전트 검색 (Codex, Claude, Goose, Gemini CLI, OpenClaw + 9 more), 프로세스 스퍼너, `/api/acp/agents` 엔드포인트    |
| 🤖 **ACP 에이전트 디스플레이**                 | 디버그 > 에이전트 페이지 — 14개의 에이전트 그리드에 설치 상태, 버전, 커스텀 에이전트 설정 옵션 (아마CLI TOOL 임)                                |
| 🔧 **Custom 모델 `apiFormat` 라우팅**      | Custom 모들들 에서 `apiFormat: "responses"`가 올바르게 Responses API Translator 쪽으로 라우팅 됩니다                       |
| 🏢 **Codex 워크스페이스 격리**                | 이메일 당 복수의 코덱스 워크스페이스 — OAuth는 연결 ID를 사용하여 연결을 분리합니다                                                     |
| 🔄 **Electron 자동 업데이트**               | 데สก탑 앱은 업데이트를 확인 + 새로운 데스크탑 세션시 업데이트 자동 설치합니다                                                           |

### 🤖 에이전트 및 프로토콜 작업 (v2.0)

| Feature                               | What It Does                                                                                       |
| ------------------------------------- | -------------------------------------------------------------------------------------------------- |
| 🔧 **MCP Server (16 tools)**           | IDE/agent tools via 3 transports: stdio, SSE (`/api/mcp/sse`), Streamable HTTP (`/api/mcp/stream`) |
| 🤝 **A2A Server (JSON-RPC + SSE)**     | Agent-to-agent task execution with sync and streaming flows                                        |
| 🧭 **Consolidated Endpoints Page**     | Tabbed management page with Endpoint Proxy, MCP, A2A, and API Endpoints tabs                       |
| 🎚️ **Service Enable/Disable Toggles** | ON/OFF switches for MCP and A2A with settings persistence (default: OFF)                           |
| 🛰️ **MCP Runtime Heartbeat**          | Real process status (pid, uptime, heartbeat age, transport, scope mode)                            |
| 📋 **MCP Audit Trail**                 | Filterable audit logs with success/failure and key attribution                                     |
| 🔐 **MCP Scope Enforcement**           | 9 granular scope permissions for controlled tool access                                            |
| 📡 **A2A Task Lifecycle Management**   | List/filter tasks, inspect events/artifacts, cancel running tasks                                  |
| 📋 **Agent Card Discovery**            | `/.well-known/agent.json` for client auto-discovery                                                |
| 🧪 프로토콜 E2E 테스트 하네스**%s                | 실제 MCP SDK + A2A 클라이언트 순차 흐름 in `test:protocols:e2e`                                               |
| ⚙️ **운영 조작기**                         | 스위치 조합, apply 내결함성 프로파일, 복원 전자 차단 기기                                                               |

### 🧠 라우팅 및 지능

| Feature                   | What It Does                                             |
| ------------------------- | -------------------------------------------------------- |
| 🎯 **스마트 4-Tier Fallback** | 자동 라우팅: 구독 → API 키 → 저비용 → 무료                            |
| 📊 **실시간 할당량 추적**          | 라이브 토큰 수 + 리셋 회차 카운트 per 제공자                             |
| 🔄 **형식 번역**               | OpenAI ↔ Claude ↔ Gemini ↔ 형식 안정 전환                      |
| 👥 **다중 계정 지원**            | 여러 계정 per 제공자와 지능적 선택                                    |
| 🔄 **자동 토큰 갱신**            | OAuth 토큰이 자동으로 갱신되며.retry                                |
| 🎨 **사용자 정의 조합**           | 6 밸런싱 전략 + 실패 회피 통제기                                     |
| 🌐 ** 와일드카드 라우터**          | `제공자/*`  동적 네비게이션                                        |
| 🧠 ** бюдж̣트를 위한 생각**      | 자동, 수동, 및 적응 가능한 합리화 제한                                  |
| 🔀 ** 모델 이름**              | 내장 및 사용자 지정 모델 이름 및 마이그레이션 안전 기능                         |
| ⚡ ** 배경 감퇴**              | 낙관적 배경 작업을 저렴한 모델로 라우팅                                   |
| 🧪 ** 작업에 대한 지혜로운 라우팅**    | 내용 종류 (코딩/시각/분석/요약)에 따라 모델이 자동적으로 선택                     |
| 💬 ** 시스템 지시**             | 원則적 지침을 일관되게 적용                                          |
| 📄 ** 응답 API 호환**          | Codex와 고급 고정 작태 워크플로에 대해 /v1/responses` 지원을 전부 받을 수 있습니다 |

### 🎵 다중 모달 API

| Feature            | What It Does                                                                                                                                                               |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🖼️ ** 이미지 생성**     | `/v1/images/generations`에 대한 클라우드 및 로컬 백엔드를 지원                                                                                                                             |
| 📐 ** 임베딩**         | `/v1/embeddings`에 대한 검색 및 RAG 파이프 라인 지원                                                                                                                                    |
| 🎤 **음성록전cription** | `/v1/audio/transcriptions` — 7 providers (Deepgram Nova 3, AssemblyAI, Groq Whisper, HuggingFace, ElevenLabs, OpenAI, Azure), auto-language detection, MP4/MP3/WAV support |
| 🔊 **음성인식**         | `/v1/audio/speech` — 10 providers (ElevenLabs, OpenAI, Deepgram, Cartesia, PlayHT, HuggingFace, Nvidia NIM, Inworld, Coqui, Tortoise) with correct error messages          |
| 🎬 **비디오 생성**       | `/v1/videos/generations` (ComfyUI + SD WebUI workflows)                                                                                                                    |
| 🎵 **음악 생성**        | `/v1/music/generations` (ComfyUI workflows)                                                                                                                                |
| 🛡️ **성과안전관리**      | `/v1/moderations` safety checks                                                                                                                                            |
| 🔀 **재순위 조정**       | `/v1/rerank` for relevance scoring                                                                                                                                         |
| 🔍 **인터넷 검색** 🆕     | `/v1/search` — 5 providers (Serper, Brave, Perplexity, Exa, Tavily), 6,500+ free/month, auto-failover, cache                                                               |

### 🛡️ 재시도, 안정성 및 관리

| Feature                            | What It Does                                                                           |
| ---------------------------------- | -------------------------------------------------------------------------------------- |
| 🔌 **회로부수**                         | Per-model trip/recover with threshold controls                                         |
| 🎯 **모델-호출형 모델**                    | Custom models declare supported endpoints + API format                                 |
| 🛡️ **Anti-Thundering Herd**        | Mutex + semaphore protections on retry/rate events                                     |
| 🧠 **Semantic + Signature Cache**   | Cost/latency reduction with two cache layers                                           |
| ⚡ **Request Idempotency**          | Duplicate protection window                                                            |
| 🔒 **TLS Fingerprint Spoofing**     | Browser-like TLS fingerprint — **reduces bot detection and account flagging**          |
| 🔏 **CLI 지문 매칭**                    | Matches native CLI request signatures — **reduces ban risk while preserving proxy IP** |
| 🌐 **IP Filtering**                 | Allowlist/blocklist control for exposed deployments                                    |
| 📊 **Editable Rate Limits**         | Configurable global/provider-level limits with persistence                             |
| 🔑 **API Key Management + Scoping** | Secure key issuance/rotation and model/provider controls                               |
| 🛡️ **Protected `/models`**         | Optional auth gating and provider hiding for model catalog                             |

### 📊 Observability & Analytics

| Feature            | What It Does                              |
| ------------------ | ----------------------------------------- |
| 📝 **요청 + 프록시 로깅**  | 전체 요청/응답 및 프록시 로깅                         |
| 📋 **통합 로그 데스크톱**   | 요청, 프록시, 감사, 콘솔_VIEW을 가진 하나의 화면           |
| 🔍 **요청 이론판**       | p50/p95/p99 지연 시간 및 요청 추적                 |
| 🏥 **보건 데스크톱**      | 업타임, 브레이커 상태, 차단, 캐시 통계                   |
| 💰 **비용 추적**        | 예산 제어 및 모델당 가격 görün이ml 표시                |
| 📈 **분석 시각화**       | 모델/제공 업usage 및 트렌드 뷰                      |
| 🧪 **평가 Framework** | 골덴 세트 테스트_에 동한Match_STRATEGY configurable |

### ☁️ 배포 및 플랫폼

| Feature             | What It Does                 |
| ------------------- | ---------------------------- |
| 🌐 **어디서든 배포**       | 로컬 서버, VPS, Docker, 구름 서버 환경 |
| 💾 **구름 동기화**        | 구름 워커를 통해 환경 구성 동기화          |
| 🔄 **백업/복원**         | 데이터 수출/수입 및 재해 복구 과정         |
| 🧙 **온보딩 마법사**       | 첫 실행시 가이드드 설정                |
| 🔧 **CLI 툴 대시보드**    | 주류 프로그래밍 툴 쉽게 구축             |
| 🎮 **Model 플레이그라운드** | 테스트: 제공자/모델/엔드 포인트 대시보드로     |
| 🔏 **CLI 지문 토글**     | 설정 > 보안에서 제공자별 지문 일치 지원      |
| 🌐 **국제화 (30 언어)**   | 전체 대시보드 + 문서 국문 지원 및 RTL 적용  |
| 🧹 **모델 모두 삭제**      | 사용자 제공자 세부 사항에서 모델 목록 삭제     |
| 📋 **이슈 템플릿**        | 기 nhu GitHub 템플릿 (버그 및 기능)   |
| 📂 **커스텀 데이터 디렉토리**  | `데이터 디렉토리` 저장 장소를 오버라이드하는    |

### 기능 깊이 분석

#### 스마트 리커버리와 용량 제어

```txt
콤보 : "내 코딩 스택"
  1. cc/claude-opus-4-6
  2. nvidia/llama-3.3-70b
  3. glm/glm-4.7
  4. if/kimi-k2-thinking
```

할당량, 비율 또는 건강에 대한 실패 시, OmniRoute는 자동으로 다음 후보에게 이동하여 수동 전환 없이 작동합니다.

#### 연결 관리가 표시되고 작동되는 프로토콜 관리

- MCP + A2A는 UI 및 문서에서 숨김되지 않습니다.
- 프로토콜 상태 API는 생鲜 운영 데이터 (`/api/mcp/*`, `/api/a2a/*`)를 노출합니다.
- 대시보드에는 일 2 차 운영에 대한 작업 (콤비 토글, 브레이커 리셋,task 취소) 포함됩니다.

#### 번역기 및 validation 워크플로

번역기 영역에는 다음이 포함됩니다.

- **플레야그라운드**: 요청 변형 확인
- **채팅 테스트**: 전사적 요청/응답 라운드 트립
- **테스트 벤치**: 한_RUN에 여러 가지 사례
- **라이브 모니터**: 실시간 트래픽 뷰

더욱한 프로토콜 validation은 `npm run 프로토콜-e2e test:`를 통한 유가한 클라이언트를 통해 수행됩니다.

> 📖 **[MCP 서버 레드메인](open-sse/mcp-server/README.md)** - 도구 레퍼런스, IDE 환경 설정, 클라이언트
> 예제
> 
> 📖 **[A2A 서버 레드메인](src/lib/a2a/README.md)** - 능력, JSON-RPC 메소드, 스트리밍, 태스크 라이프
> 사이클

## 🧪 평가(Evals)

omiRoute에는 골든 세트보다 LLM 응답 품질을 테스트하는 평가 프레임워크가 내장되어 있습니다. 대시보드에서 **의
Evals(X135X)를 통하여 액세스할 수 있습니다.

### Built-in Golden Set

이것은 빌트인으로 제공되는 "OmniRoute Golden Set"입니다.\
이 Golden Set 내에는 다음 유형의 테스트 케이스가 제공됩니다.

- 인사말, 수학, 지리학, 코드 생성
- JSON 형식의 일관성, 번역, 마크다운 생성
- 사해로운 콘텐츠 탐지, 카운팅, 불리언 논리

### 평가 전략

| 전략         | Description                      | 예                            |
| ---------- | -------------------------------- | ---------------------------- |
| `exact`    | 부분과 일치해야 합니다.                    | `"4"`                        |
| `contains` | 부분 문자열 (대/소문자 구분X)               | `"Paris"`                    |
| `regex`    | 정규표현식과 일치해야 합니다.                 | `"1.*2.*3"`                  |
| `custom`   | 사용자 정의 함수가 true/false를 반환해야 합니다. | `(도출) =&gt; 도출의 길이가 10보다 크다` |

---

## 📖 안내 가이드

### 프로토콜 설정 (MCP + A2A)

<details>
<summary><b>🧩 MCP Setup (Model Context Protocol)</b></summary>

stdio 모드에서 MCP 전송을 시작하세요:

```bash
omniroute --mcp
```

권장하는 유효성 검사 흐름:

1. stdio로 MCP 클라이언트를 연결하세요.
2. `omniroute_get_health` 함수를 수행해 보세요.
3. `omniroute_list_combos` 함수를 수행해 보세요.
4. `/dashboard/mcp`를 열어 heartbeat, activity 및 audit 확인을 해보세요.

자동화에 유용한 API:

- `GET /api/mcp/status`
- `GET /api/mcp/tools`
- `GET /api/mcp/audit`
- `GET /api/mcp/audit/stats`

</details>

<details>
<summary><b>🤝 A2A Setup (Agent2Agent)</b></summary>

agens 정보를 발견하세요:

```bash
curl http://localhost:20128/.well-known/agent.json
```

과제를 전송하세요:

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"setup-a2a","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"구매량 상태를 요약해 보세요."}]}}'
```

수명 주기를 관리하세요:

- `GET /api/a2a/상태`
- `GET /api/a2a/작업`
- `GET /api/a2a/작업/:id`
- `POST /api/a2a/작업/:id/취소`

운용 UI:

- `/대시보드/a2a` 작업/상태/스트림 관찰 및 스モ크 액션

</details>

<details>
<summary><b>🧪 End-to-end protocol validation</b></summary>

실제 클라이언트와 두 프로토콜 모두 유효성 검사:

```bash
npm run test:protocols:e2e
```

이는 확인합니다:

- MCP SDK 클라이언트 접속/목록/통화
- A2A 탐지/전송/스트림/이상 취소
- MCP审核 및 A2A 작업 관리 API에서 데이터 상관 관계 확인:

</details>

<details>
<summary><b>💳 Subscription Providers</b></summary>

### 클루드 코드 (프로/맥스)

```bash
대시보드 → 공급자 → 클루드 코드 연결 → OAuth 로그인 → 토큰 자동刷新 → 5시간 + 주간 할당량 추적

모델:
 cc/클루드-오플-4-6
 cc/클루드-슨нет-4-5-20250929
 cc/클루드-하이쿠-4-5-20251001
```

**프로 팁:** 복잡한 작업에 오플을, 속도에 소넷을 사용하십시오! OmniRoute는 할당량을 모델별로 추적합니다!

### 오픈 AI 코덱스 (플러스/프로)

```bash
대시보드 → 공급자 → 코덱스 연결 → OAuth 로그인 (포트 1455) → 5시간 + 주간 리셋

모델:
 cx/GPT-5.2 코덱스
 cx/GPT-5.1 코덱스 맥스
```

#### 코덱스 계정 제한 관리 (5시간 + 주간 리셋)

코덱스 계정 각 계정에는 정책 스와이تش가 Dashboard -> Providers 의 `에서 있습니다:`

- `5시간` (켜기/끄기): 5시간 시간 창계정 정책 강제 설정.\
  ==WEBLATE_PART==
- `주간` (ON/OFF): 주간窗口 임계값 정책 강제입니다.
- 임계값 повед음: 사용률 >= 90%를 reached 할 때, 계정은 skipped 됩니다.
- ROTATION behavior: OmniRoute 다음 할당 가능한 Codex 계정으로 무조건 라우팅됩니다.
- 리셋 behavior: 공급자 `리셋At` 시간 passage에 따라 계정은 다시 할당 가능합니다.

Scenario:

- `5 시간 ON` + `주간 ON`: account가 threshold를 reached 할때 둘중 하나가 계정을 skip합니다.
- `5 시간 OFF` + `주간 ON`: 주간 사용량만 계정을 block할 수 있습니다.
- `5 시간 ON` + `주간 OFF`: 5 시간 사용량만 계정을 block할 수 있습니다.
- `리셋At` already passage: account가 재로 rotation에 무조건 등록됩니다 (수동 재허용 불필요).

### Gemini CLI (FREE 180K/month!)

```bash
Dashboard → Providers → Connect Gemini CLI
→ Google OAuth
→ 180K completions/month + 1K/day

Models:
  gc/gemini-3-flash-preview
  gc/gemini-2.5-pro
```

**가장 높은 가치: ** 무료 티어가 엄청나규습니다. 이 무료 티어를 사용하기 전에 유료 티어를 사용하세요.

### GitHub 코파일럿

```bash
Dashboard → Providers → Connect GitHub
→ OAuth via GitHub
→ 매월 리셋 (월 1일)

Models:
  gh/gpt-5
  gh/claude-4.5-sonnet
  gh/gemini-3-pro
```

</details>

<details>
<summary><b>🔑 API Key Providers</b></summary>

### NVIDIA NIM (FREE 개발자 접근 권한 — 70+ 모델)

1. 회원 가입: [build.nvidia.com](https://build.nvidia.com)
2. 무료 API key 얻기 (인ферен스 크레딧 1000개 포함)
3. Dashboard → Provider 추가 → NVIDIA NIM:
   - API Key: `nvapi-your-key`

**모델:** `nvidia/llama-3.3-70b-instruct`, `nvidia/mistral-7b-instruct`, 50+) 더 많은
모델이 있습니다.

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
3. 대시보드 → API 키 추가:
   - 제공자: `glm`
   - API 키: `your-key`

**사용:** `glm/glm-4.7`

**프로 팁:** 코딩 플랜은 3배의 선물비용과 7배의 비용입니다. 일일 10:00 AM에 리셋합니다.

### MiniMax M2.1 (5시간 리셋, $0.20/1M)

1. 회원 가입: [MiniMax](https://www.minimax.io/)
2. Get API key
3. 대시보드 → API 키 추가

**사용:** `minimax/MiniMax-M2.1`

**프로 팁:** 장기 컨텍스트 (1M 토큰) için 가장 저렴한 옵션입니다!

### Kimi K2 ($9/월 flat)

1. 구독: [Moonshot AI](https://platform.moonshot.ai/)
2. Get API key
3. 대시보드 → API 키 추가

**사용:** `kimi/kimi-latest`

**프로 팁:** 10M 토큰당 $9/월 fixed = $0.90/1M 효과적인 비용입니다!

</details>

<details>
<summary><b>🆓 FREE Providers (Emergency Backup)</b></summary>

### iFlow (OAuth를 통해 5 FREE 모델)

```bash
대시보드 → iFlow 연결
→ iFlow OAuth 로그인
→ 무제한 사용

모델:
  if/kimi-k2-thinking
  if/qwen3-coder-plus
  if/glm-4.7
  if/minimax-m2
  if/deepseek-r1
```

### Qwen (디바이스 코드를 통해 4 FREE 모델)

```bash
Dashboard → Connect Qwen
→ Device code authorization
→ Unlimited usage

Models:
  qw/qwen3-coder-plus
  qw/qwen3-coder-flash
```

### Kiro (Claude FREE)

```bash
Dashboard → Connect Kiro
→ AWS Builder ID or Google/GitHub
→ Unlimited usage

Models:
  kr/claude-sonnet-4.5
  kr/claude-haiku-4.5
```

</details>

<details>
<summary><b>🎨 Create Combos</b></summary>

### Example 1: Maximize Subscription → Cheap Backup

```
Dashboard → Combos → Create New

Name: premium-coding
Models:
  1. cc/claude-opus-4-6 (Subscription primary)
  2. glm/glm-4.7 (Cheap backup, $0.6/1M)
  3. minimax/MiniMax-M2.1 (Cheapest fallback, $0.20/1M)

Use in CLI: premium-coding
```

### Example 2: Free-Only (Zero Cost)

```
Name: free-combo
Models:
  1. gc/gemini-3-flash-preview (180K free/month)
  2. if/kimi-k2-thinking (unlimited)
  3. qw/qwen3-coder-plus (unlimited)

Cost: $0 forever!
```

</details>

<details>
<summary><b>🔧 CLI Integration</b></summary>

### 커서 IDE

```
Settings → Models → Advanced:
  OpenAI API Base URL: http://localhost:20128/v1
  OpenAI API Key: [from OmniRoute dashboard]
  Model: cc/claude-opus-4-6
```

### 클로드 코드

Use the **CLI Tools** page in the dashboard for one-click configuration, or edit
`~/.claude/settings.json` manually.

### Codex CLI

```bash
export OPENAI_BASE_URL="http://localhost:20128"
export OPENAI_API_KEY="your-omniroute-api-key"

codex "your prompt"
```

### OpenClaw

**Option 1 — Dashboard (recommended):**

```
Dashboard → CLI Tools → OpenClaw → Select Model → Apply
```

**Option 2 — Manual:** Edit `~/.openclaw/openclaw.json`:

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

> **Note:** OpenClaw only works with local OmniRoute. Use `127.0.0.1` instead of
> `localhost` to avoid IPv6 resolution issues.

### Cline / Continue / RooCode

```
설정 → API 구성:
  제공자: OpenAI 호환
  기본 URL: http://localhost:20128/v1
  API 키: [OmniRoute 대시보드에서]
  모델: if/kimi-k2-thinking
```

### OpenCode

**단계 1:** OmniRoute을 사용자 정의 제공자로 添加:

```bash
opencode
/connect
# "다른 것" → ID: "omniroute" → OmniRoute API 키 입력
```

**단계 2:** 프로젝트 루트에서 다음 `opencode.json`을 생성/수정:

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

**단계 3:** OpenCode에서 모델을 선택:

```bash
/models
# OmniRoute 모델 목록에서任意 모델 선택
```

> **팁:** OmniRoute `/v1/models` 엔드포인트에서 이용 가능한 모델을 모델 `models` 섹션에 추가 할 수 있습니다.
> OmniRoute 대시보드에서 이용 가능한 provider/model-id` 형식을 사용하세요.

</details>

---

## 문제 해결

<details>
<summary><b>Click to expand troubleshooting guide</b></summary>

**"기호 언어 모델이 메시지를 제공하지 못하였습니다.""**

- 제공자 대수소를 사용량超過 → 대시보드 추적기에서 확인
- 해결지: 콤보 지연 전환 또는 저렴한 티어로 전환

**률 제한**

- 지불 대수소가소적 → GLM/MiniMax로 전환
- 콤보 추가: `cc/claude-opus-4-6 → glm/glm-4.7 → if/kimi-k2-thinking`

**OAuth 인증서가 만료되었습니다."**

- 자동으로 OmniRoute이 업데이트
- 위치 해결 지속 : 대시보드 → 제공자 → Reconnect

**고성능 비용**

- Check usage stats in Dashboard → Costs
- Switch primary model to GLM/MiniMax
- Use free tier (Gemini CLI, iFlow) for non-critical tasks

**Dashboard/API ports are wrong**

- `PORT` is the canonical base port (and API port by default)
- `API_PORT` overrides only OpenAI-compatible API listener
- `DASHBOARD_PORT` overrides only dashboard/Next.js listener
- Set `NEXT_PUBLIC_BASE_URL` to your dashboard/public URL (for OAuth callbacks)

**Cloud sync errors**

- Verify `BASE_URL` points to your running instance
- Verify `CLOUD_URL` points to your expected cloud endpoint
- Keep `NEXT_PUBLIC_*` values aligned with server-side values

**First login not working**

- Check `INITIAL_PASSWORD` in `.env`
- If unset, fallback password is `123456`

**No request logs**

- Set `ENABLE_REQUEST_LOGS=true` in `.env`

**Connection test shows "Invalid" for OpenAI-compatible providers**

- Many providers don't expose a `/models` endpoint
- OmniRoute v1.0.6+ includes fallback validation via chat completions
- 기본 URL에는 `/v1` 접미사 포함되어야 합니다.

### 🔒 외부 서버에서 OAuth

<a name="oauth-on-a-remote-server"></a> <a name="oauth-em-servidor-remoto"></a>

> **⚠️ VPS, Docker 또는 원격 서버에서 OmniRoute 작동하는 사용자[481]에는 매우 중요[81X]

#### Antigravity / Gemini CLI OAuth가 원격 서버에서 실패하는 이유는 무엇인가?

**Antigravity** 및 **Gemini CLI** providor은 **Google OAuth 2.0**을 제공하고 있으며
Google은 OAuth 흐름에서 `redirect_uri`이 app의 Google Cloud Console에서 pre-등록된 URI와 정확히
일치해야 한다고합니다.

OmniRoute에서 제공하는 OAuth 인증서는 **'localhost'에만 등록[80X]되어 있습니다. 원격 서버에 접속하는 경우(예:
`https://omniroute.myserver.com`) Google은 인증을 거부하며 다음과 같이 메시지를 전달합니다:

```
오류 400: redirect_uri_mismatch
```

#### 해결 방안: OAuth 자격 증명을 구성하십시오

_own OAuth 자격 증명을 구성해야 합니다._

#### Google 클라우드-console에서 자체 OAuth 2.0 클라이트 ID를 만들어야 합니다.

단계별

[X0X]1. Google 클라우드-console에 접속[30X]

https://console.cloud.google.com/apis/credentials로 가십시오.

- [X0X]2. 새로운 OAuth 2.0 클라이트 ID를 만들하십시오
- [+]Create Credentials → OAuth 클라이트 ID 클릭하십시오
- 애플리케이션 유형 : [X18X]'웹 애플리케이션':[37X]

이름 : 원하는 이름(예: [X30X]OmniRoute 원격[47X]) \
==WEBLATE_PART ==\
**3. 권한된 리다이렉트 URI를 추가하십시오

"권한된 리다이렉트 URI" 字段에 URL을 입력하십시오:

```
https://your-server.com/callback
```

> `your-server.com`을 원격서버의 도메인이나 IP로 대체하십시오(포트 포함, 예:
> `http://45.33.32.156:20128/callback`)

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
오류 400: redirect_uri_mismatch
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

**6. OmniRoute을 재시작**

```bash
# npm을 사용하는 경우:
npm run dev

# Docker를 사용하는 경우:
docker restart omniroute
```

**7. 다시 연결하면**

대시보드 → 제공자 → Antigravity (또는 Gemini CLI) → OAuth

이제 Google은 올바르게 `https://seu-servidor.com/callback`로 리다이렉트해 줄
것이며-authentication은 작동할 것입니다.

---

#### 시초 (만들어지지 않은 특정 자바스크립트)

만들어지지 않은 자바스크립트 자격 증명을 만들지 않을 경우 여전히 플로우 **URL의 수동 처리자**를 사용할 수 있습니다:

1. Omniroute은 Google의 인증 허가 URL을 열겠습니다.
2. 당신이 허가 한 후 Google은 리다이렉트하려고 할 것으며 `로컬호스트` (전용 서버에서 실패)로 리다이렉트하려고 합니다.
3. **브라우저 주소 창에서 전체 URL 복사**합니다
4. 이 URL을 Omniroute의 연결 모달에서 나타나는 필드에 붙여붙혀 주세요
5. [x0X]"연결합니다"**버튼 클릭

> 이 수동은 작동한다는 이유입니다. URL의 인증 코드는 리다이렉트가 로드되는지 여부와 상관없이 유효합니다.

</details>

---

</details>

## 🛠️ 기술 스택

<details>
<summary><b>Click to expand tech stack details</b></summary>

- ***런타임**: Node.js 18–22 LTS (⚠️ Node.js 24+은 **지원되지 않습니다** — `보다 좋은 SQLite`
  Bản 기계 번역이 체계적으로 충돌합니다)
- ***\
  주문어: 타이\
  타입: 스타트\
  (X7X)): X10 타입\
  **: TYPESCRIPT 9.5—— 98% TYPESCRIPT** src/` 및 [X64X] open-sse/` (0 이하는 Zero
  core module ` since ` v2.0)
- *** 프레임 워크**: Next.js 16 + React 19 + Tailwind CSS 4
- ***\
  다이 내스: 데이터 베이스\
  **: 데이터 베이스\
  (X1X)) LowDB (JSON) + SQLite (영역 상태 + 프록시 로그 + MCP 상태 + 순서관련
- *** 스키마**: Zod (MCP 툴 입/출력 유효성 검사, API 조약)
- *** 프로토콜**: MCP (stdio/HTTP) + A2A v0.3 (JSON-RPC 2.0 + SSE)
- **스스트리밍**: 서버 전송 이벤트 (SSE)
- **관리자**: OAuth 2.0 (PKCE) + JWT + API 키 + MCP 구독 범위 인증
- **테이스트[T9X]: Node.js 테스트 러너 + Vitest (단위 테스트, 통합 테스트, E2E 테스트 900개 이상)
- **CI/CD**: GitHub Actions (자동 npm 발표 + Docker Hub 빌드 및 배포)
- **공식사이트**: [omniroute.online](https://omniroute.online)
- **팩크지지[P9X]:
  [npmjs.com/package/omniroute](https://www.npmjs.com/package/omniroute)
- **도커**:
  [hub.docker.com/r/diegosouzapw/omniroute](https://hub.docker.com/r/diegosouzapw/omniroute)
- **재해력**: 제이브레이커, 지수적 보복, 반파� herd 예방, tls 패드딩 스, 자체 치료

</details>

---

## 문서

| 문서 작성                                          | Description                                    |
| ---------------------------------------------- | ---------------------------------------------- |
| [사용자 가이드](docs/USER_GUIDE.md)                  | 제공자 도움말, CLI 통합, 배포                            |
| [API 참조](docs/API_REFERENCE.md)                | 모든 엔드포인트 설명                                    |
| [MCP 서버](open-sse/mcp-server/README.md)        | 16 MCP 도구, IDE config, 파이선/TS/Go 클라이언트         |
| [A2A 서버](src/lib/a2a/README.md)                | JSON-RPC 2.0 프로토콜, 스킬, 스트리밍, 태스크 매니지           |
| [Auto-Combo 엔진](docs/auto-combo.md)            | 6-factor scoring, mode packs, self-healing     |
| [Troubleshooting](docs/TROUBLESHOOTING.md)     | Common problems and solutions                  |
| [Architecture](docs/ARCHITECTURE.md)           | System architecture and internals              |
| [Contributing](CONTRIBUTING.md)                | Development setup and guidelines               |
| [OpenAPI Spec](docs/openapi.yaml)              | OpenAPI 3.0 specification                      |
| [Security Policy](SECURITY.md)                 | Vulnerability reporting and security practices |
| [VM Deployment](docs/VM_DEPLOYMENT_GUIDE.md)   | Complete guide: VM + nginx + Cloudflare setup  |
| [Features Gallery](docs/FEATURES.md)           | Visual dashboard tour with screenshots         |
| [Release Checklist](docs/RELEASE_CHECKLIST.md) | Pre-release validation steps                   |

---

## 🗺️ Roadmap

OmniRoute has **210+ features planned** across multiple development phases. Here
are the key areas:

| Category                     | 예정된 기능 | Highlights                                                                             |
| ---------------------------- | ------ | -------------------------------------------------------------------------------------- |
| 🧠 **Routing & Intelligence** | 25+    | Lowest-latency routing, tag-based routing, quota preflight, P2C account selection      |
| 🔒 **Security & Compliance**  | 20+    | SSRF hardening, credential cloaking, rate-limit per endpoint, management key scoping   |
| 📊 **Observability**          | 15+    | OpenTelemetry integration, real-time quota monitoring, cost tracking per model         |
| 🔄 **Provider Integrations**  | 20+    | Dynamic model registry, provider cooldowns, multi-account Codex, Copilot quota parsing |
| ⚡ **Performance**            | 15+    | Dual cache layer, prompt cache, response cache, streaming keepalive, batch API         |
| 🌐 **Ecosystem**              | 10+    | WebSocket API, config hot-reload, distributed config store, commercial mode            |

### 곧 출시

- 🔗 **OpenCode Integration** — Native provider support for the OpenCode AI
  coding IDE
- 🔗 **AI 통합** — TRAE AI 개발 프레임워크에 대한 FULL 지원
- 📦 **버전트API** — bulk 요청에 대해 대기열 처리
- 🎯 **태그기반 라우팅** — 커스텀 태그 및 메타데이터에 따라 요청 라우팅
- 💰 **가장 저렴한 전략** — 저렴한 제공업체 중에서 자동으로 선택

> 📝 모든 특징에 대한 상세된 명세서는 [`docs/new-features/`](docs/new-features/)(217 개의 이름난 명세)
> 에서 찾을 수 있습니다.

---

## 👥 공조자

[![Contributors](https://contrib.rocks/image?repo=diegosouzapw/OmniRoute&max=100&columns=20&anon=1)](https://github.com/diegosouzapw/OmniRoute/graphs/contributors)

### 기여하는 방법

1. 레파지토리 Fork
2. 기능 브랜치 생성 (`git checkout -b feature/amazing-feature`)
3. 변경 사항을 커밋 (`git commit -m 'Add amazing feature'`)
4. 브랜치에 푸시 (`git push origin feature/amazing-feature`)
5. 풀 리퀘스트 열기

자세한 지침은 [CONTRIBUTING.md](CONTRIBUTING.md)를 참고하시길 바랍니다.

### 새 버전 릴리즈

```bash
# 릴리즈 생성 — npm publish가 무조건 자동화
gh release create v2.0.0 --title "v2.0.0" --generate-notes
```

---

## 📊 스타 ιστο리

## 시간에 따른 스태거져

## [![Stargazers over time](https://starchart.cc/diegosouzapw/OmniRoute.svg?variant=adaptive)](https://starchart.cc/diegosouzapw/OmniRoute)

## 🙏 감사합니다

감사의 마음을 담아 **[CLIProxyAPI](https://github.com/decolua/9router)[X36X] 에게 고마움을
느낍니다. — 본 프로젝트를 구현하는데 영감을 주신 원래 Go 구현체입니다. OmniRoute는 그에 더하여 추가 기능, 다중 모드 API 및
TypeScript로 다시 작성되는 가운데 그 놀라운 토대를 확장합니다.

감사의 마음을 담아 **[9router](https://github.com/router-for-me/CLIProxyAPI)[X32X] 에게
고마움을 느낍니다. — 본 프로젝트를 구현하는데 영감을 주신 원래 프로젝트입니다. OmniRoute는 그에 더하여 추가 기능, 다중 모드
API, 그리고 전체 TypeScript 다시 작성으로 그 놀라운 토대를 확장합니다.

---

## 📄 라이선스

MIT 라이선스 — 자세한 사항은 [LICENSE](LICENSE)를 확인하시겨 주십시오.

---

<div align="center">
  <sub>Built with ❤️ for developers who code 24/7</sub>
  <br/>
  <sub><a href="https://omniroute.online">omniroute.online</a></sub>
</div>
<!-- GitHub Discussions enabled for community Q&A -->
