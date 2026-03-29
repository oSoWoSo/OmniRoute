# 🚀 OmniRoute — A Gateway AI Livre

### Nunca pare de codificar. Rotas inteligentes para **MODELOS DE IA gratuitos e de baixo custo** com fallback automático.

_Seu proxy de API universal — um endpoint, 67+ provedores, sem tempo de
inatividade. Agora com orquestração de agentes MCP & A2A._

**Conclusões de Chat • Incorporação • Geração de Imagens • Vídeo • Música •
Áudio • Reranking • **Busca na Web** • Servidor MCP • Protocolo A2A • 100%
TypeScript**

---

<div align="center">

[![versão
npm](https://img.shields.io/npm/v/omniroute?color=cb3837&logo=npm)](https://www.npmjs.com/package/omniroute)
[![baixados
npm](https://img.shields.io/npm/dm/omniroute?color=cb3837&logo=npm&label=npm%20downloads)](https://www.npmjs.com/package/omniroute)
[![Docker
Hub](https://img.shields.io/docker/v/diegosouzapw/omniroute?label=Docker%20Hub&logo=docker&color=2496ED)](https://hub.docker.com/r/diegosouzapw/omniroute)
[![Docker
Pulls](https://img.shields.io/docker/pulls/diegosouzapw/omniroute?logo=docker&color=2496ED&label=docker%20pulls)](https://hub.docker.com/r/diegosouzapw/omniroute)
[![Licença](https://img.shields.io/github/license/diegosouzapw/OmniRoute)](https://github.com/diegosouzapw/OmniRoute/blob/main/LICENSE)
[![Website](https://img.shields.io/badge/Website-omniroute.online-blue?logo=google-chrome&logoColor=white)](https://omniroute.online)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-Community-25D366?logo=whatsapp&logoColor=white)](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

[![Sitio Web](https://omniroute.online) • [![Início Rápido](#-quick-start) •
[![Características](#-key-features) • [![Documentação](#-documentation) •
[![Preços](#-pricing-at-a-glance) •
[![WhatsApp](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

</div>

🌐 **Disponível em:** 🇺🇸 [Inglês](README.md) | 🇧🇷 [Português
(Brasil)](docs/i18n/pt-BR/README.md) | 🇪🇸 [Espanhol](docs/i18n/es/README.md) |
🇫🇷 [Françês](docs/i18n/fr/README.md) | 🇮🇹 [Italiano](docs/i18n/it/README.md) |
🇷🇺 [Russo](docs/i18n/ru/README.md) | 🇨🇳 [Chinês
(Simplificado)](docs/i18n/zh-CN/README.md) | 🇩🇪 [Alemão](docs/i18n/de/README.md)
| 🇮🇳 [Hindi](docs/i18n/in/README.md) | 🇹🇭 [Tailandês](docs/i18n/th/README.md) |
🇺🇦 [Ucraniano](docs/i18n/uk-UA/README.md) | 🇸🇦 [Árabe](docs/i18n/ar/README.md) |
🇯🇵 [Japonês](docs/i18n/ja/README.md) | 🇻🇳 [Vietnamita](docs/i18n/vi/README.md) |
🇧🇬 [Búlgaro](docs/i18n/bg/README.md) | 🇩🇰 [Dinamarquês](docs/i18n/da/README.md)
| 🇫🇮 [Finlandês](docs/i18n/fi/README.md) | 🇮🇱 [Hebraico](docs/i18n/he/README.md)
| 🇭🇺 [Húngaro](docs/i18n/hu/README.md) | 🇮🇩 [Indonésio](docs/i18n/id/README.md)
| 🇰🇷 [Coreano](docs/i18n/ko/README.md) | 🇲🇾 [Malaio](docs/i18n/ms/README.md) |
🇳🇱 [Holandês](docs/i18n/nl/README.md) | 🇳🇴 [Norueguês](docs/i18n/no/README.md) |
🇵🇹 [Português (Portugal)](docs/i18n/pt/README.md) | 🇷🇴
[Romeno](docs/i18n/ro/README.md) | 🇵🇱 [Polonês](docs/i18n/pl/README.md) | 🇸🇰
[Slovaco](docs/i18n/sk/README.md) | 🇸🇪 [Sueco](docs/i18n/sv/README.md) | 🇵🇭
[Tagalo](docs/i18n/phi/README.md) | 🇨🇿 [Tcheco](docs/i18n/cs/README.md)

---

## 🆕 O que há de novo na v3.0.0

> **Está atualizando da v2.9.5?** — Veja o [CHANGELOG
> completo](CHANGELOG.md#300--2026-03-22-release-candidate--not-yet-merged-to-main)
> para todos os ajustes.

| Area                                | Mudança                                                                                                                                                                                                  |
| ----------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🔒 **Segurança CodeQL**              | Corrigidos 10+ alertas de CodeQL: polynomial-redos, injustiça aleatória, remediação de injúria de shell                                                                                                  |
| ✅ **Validação de Rotas**            | Todas as 176 rotas de API agora validadas com esquemas Zod + `validateBody()` — CI `check:route-validation:t06` passa                                                                                    |
| 🐛 **Vazamento de Tag do OmniModel** | Marquete interno `<omnimodel>` não vai vaziar para os clientes em respostas de fluxo SSE (#585)</omnimodel>                                                                                              |
| 🔑 **Chaves Registradas API**        | Facilita provisionamento de chaves de API por meio de `POST /api/v1/registered-keys` com quotação por provedor-conta, idempotência, armazenamento SHA-256 e relatório de problemas do GitHub facultativo |
| 🎨 **Ícones de Provedor**            | 130+ logotipos de provedores via `@lobehub/icons` (SVG) com fallback para PNG                                                                                                                            |
| 🔄 Atualizar Modelagem Automática**  | Agendador de 24h e botão de toggle de interface para sincronizar listas de modelos para provedores embutidos e personalizados compatíveis com OpenAI                                                     |
| 🌐 **OpenCode Zen/Go**               | Dois provedores novos de @kang-heewon via PR #530: plano gratuito + plano de assinatura via `OpencodeExecutor`                                                                                           |
| 🐛 **Gemini CLI OAuth**              | Exibir erro quando `GEMINI_OAUTH_CLIENT_SECRET` é ausente em Docker (antigo erro cripto de Google)                                                                                                       |
| 🐛 **OpenCode config**               | `saveOpenCodeConfig()` agora grava corretamente o TOML em `XDG_CONFIG_HOME`                                                                                                                              |
| 🐛 **Pinned model override**         | Se `body.model` está corretamente definido como `pinnedModel` na proteção da cache de contexto                                                                                                           |
| 🐛 **Codex/Claude loop**             | `tool_result` agora é convertido para texto para parar os loops infinitos                                                                                                                                |
| 🐛 **Login redirect**                | O login não congela mais após pular a configuração de senha                                                                                                                                              |
| 🐛 **Windows paths**                 | Caminhos MSYS2/Git-Bash (`/c/...`) sao normalizados automaticamente em `C:\...`                                                                                                                          |

---

## 🖼️ Dashboard Principal

<div align="center">
  <img src="./docs/screenshots/MainOmniRoute.png" alt="OmniRoute Dashboard" width="800"/>
</div>

---

## 📸 Antevisão do Dashboard

<details>
<summary><b>Click to see dashboard screenshots</b></summary>

| Página               | Tela de Captura                                       |
| -------------------- | ----------------------------------------------------- |
| **Fornecedores**     | ![Fornecedores](docs/screenshots/01-providers.png)    |
| **Combinações**      | ![Combinações](docs/screenshots/02-combos.png)        |
| **Análitica**        | ![Análitica](docs/screenshots/03-analytics.png)       |
| **Saúde**            | ![Saúde](docs/screenshots/04-health.png)              |
| **Tradutor**         | ![Tradutor](docs/screenshots/05-translator.png)       |
| **Configurações**    | ![Configurações](docs/screenshots/06-settings.png)    |
| **Ferramentas CLI**  | ![Ferramentas CLI](docs/screenshots/07-cli-tools.png) |
| **Registros de Uso** | ![Registros](docs/screenshots/08-usage.png)           |
| **Pontos de Fim**    | ![Pontos de Fim](docs/screenshots/09-endpoint.png)    |

</details>

---

### 🤖 Fornecedor de Inteligência Artificial Gratuito para seus agentes de codificação favoritos.

_Conecte qualquer IDE ou ferramenta CLI com potencial de inteligência artificial
através da OmniRoute — gateway de API gratuito para codagem infinita._

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

<sub>📡 Todas as agentes conectam-se por meio de
<code>http://localhost:20128/v1</code> ou
<code>http://cloud.omniroute.online/v1</code> — uma configuração, modelos
ilimitados e quota</sub>

---

## 🤔 Por que a OmniRoute?

**Pare de desperdiçar dinheiro e ter os limites restritos:**

- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  A quota de assinatura expira inutilizada a cada mês
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Os limites de taxa impedissem seu progresso de programação
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  APIs caras (US$ 20-50/mês por provedor)
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Mudanças manuais entre os provedores

**A OmniRoute resolve esse problema:**

- ✅ **Maximize suas assinaturas** - Rastreie quota, utilize todos antes do reset
- ✅ **Falha automática** - Assinatura → Chave API → Barata → Gratuita, zero
  tempo fora de linha
- ✅ **Multi-conta** - Arredonda-robin entre contas por provedor
- ✅ **Universal** - Funciona com Claude Code, Codex, Gemini CLI, Cursor, Cline,
  OpenClaw, qualquer ferramenta CLI

---

## 📧 Suporte

> 💬 **Acesse nossocomunidade!** [Grupo do
> WhatsApp](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t) -
> Obtenha ajuda, compartilhe dicas e fique atualizado

- **Site:** [omniroute.online](https://omniroute.online)
- **GitHub:**
  [github.com/diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute)
- **Issues:**
  [github.com/diegosouzapw/OmniRoute/issues](https://github.com/diegosouzapw/OmniRoute/issues)
- **WhatsApp:** [Grupo de
  Comunidade](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)
- **Colaboração:**: Veja [CONTRIBUTING.md](CONTRIBUTING.md), abra uma PR, ou
  escolha um `boa primeira abordagem`
- **Projeto Original**: [9rota do décimo](https://github.com/decolua/9router)

### 🐛 Relatar um Bug?

Ao abrir um problema, por favor execute o comando de informações do sistema e
anexe o arquivo gerado:

```bash
npm run system-info
```

Isso gera um `system-info.txt` com sua versão do Node.js, versão do OmniRoute,
detalhes do OS, ferramentas CLI instaladas (iflow, gemini, claude, codex,
antigravitde, droid, etc.), status do Docker/PM2, e pacotes do sistema — tudo
que precisamos para reproduzir sua issue rapidamente. Anexe o arquivo
diretamente ao seu problema do GitHub.

---

## Como Funciona

```
┌─────────────┐
│  Sua CLI   │  (Código Claude, Codex, CLI Gemini, OpenClaw, Cursor, Cline...)
│   Ferramenta│
└──────┬──────┘
       │ http://localhost:20128/v1
       ↓
┌─────────────────────────────────────────┐
│           OmniRoute (Rotador Inteligente)     │
│  • Tradução de formato (OpenAI → Claude) │
│  • Contagem de cotas + Embutidos + Imagens │
│  • Recarregamento de tokens automáticos │
└──────┬──────────────────────────────────┘
       │
       ├─→ [Nível 1: ASSINATURA] Código Claude, Codex, CLI Gemini
       │   ↓ cota exaurida
       ├─→ [Nível 2: CHAVE DA API] DeepSeek, Groq, xAI, Mistral, NVIDIA NIM, etc.
       │   ↓ limite de orçamento
       ├─→ [Nível 3: BARATO] GLM ($0,6/1M), MiniMax ($0,2/1M)
       │   ↓ limite de orçamento
       └─→ [Nível 4: GRÁTIS] iFlow, Qwen, Kiro (ilimitado)

Resultado: Nunca mais pare de codar, custo mínimo
```

---

## 🎯 O que o OmniRoute Resolve — 30 Problemas e Usos Reais de Dor

> **Todos os desenvolvedores que usam ferramentas de AI enfrentam esses
> problemas diariamente.** O OmniRoute foi construído para resolvê-los todos —
> desde excessos de custo até bloqueios regionais, desde fluxos OAuth quebrados
> até operações de protocolo e observabilidade empresarial.

<details>
<summary><b>💸 1. "I pay for an expensive subscription but still get interrupted by limits"</b></summary>

Os desenvolvedores pagam $20–200/mês por Claude Pro, Codex Pro ou GitHub
Copilot. Mesmo pagando, a cota tem uma limitação — 5h de uso, limites semanais,
ou limites de minuto. Meio da sessão de codificação, o fornecedor para de
responder e o desenvolvedor perde o fluxo e a produtividade.

**Como o OmniRoute resolve isso:**

- **Filtro de fallback inteligente de 4 níveis** — Se a cota de assinatura
  excede, redireciona automaticamente para Chave da API → Barato → Grátis sem
  intervenção manual
- **Contagem de cota em tempo real** — Exibe o consumo de tokens em tempo real
  com o recarregamento de contagem (5h, diário, semanal)
- **Suporte a múltiplos contas** — Múltiplas contas para cada fornecedor com
  switch automático — quando uma excede, alternativa para a próxima
- **Combinatórias personalizáveis** — Filtro de fallback personalizável com 6
  estratégias de equilíbrio (preenchimento primeiro, roda-roda, P2C, randômico,
  menos usado, otimizado por custo)
- **Quotas de Negócios do Codex** — Monitoramento de quotas para workspace de
  equipe diretamente no painel

</details>

<details>
<summary><b>🔌 2. "I need to use multiple providers but each has a different API"</b></summary>

O OpenAI utiliza uma forma, o Claude (Anthropic) outra, e o Gemini outra ainda.
Se um dev quiser testar modelos de diferentes provedores ou fallback entre eles,
precisam reconfigurar SDKs, mudar os endpoints, lidar com formatos
incompatíveis. Fornecedores personalizados (FriendLI, NIM) têm endpoints de
modelos não padrão.

**Como o OmniRoute resolve isso:**

- **Ponto de fusão único** — Um único `http://localhost:20128/v1` serve como
  proxy para todos os provenientes 67+
- **Tradução de formato** — Automática e transparente: OpenAI ↔ Claude ↔ Gemini
  ↔ API de Resposta
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

**Como o OmniRoute resolve isso:**

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

**Como o OmniRoute resolve isso:**

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
- **Estratégia de Otimização de Custo** — Estratégia de rotamento que escolhe
  automaticamente o provedor mais barato disponível

</details>

<details>
<summary><b>🔒 5. "I need to protect my AI gateway from unauthorized access"</b></summary>

Ao expor uma Gateway de Inteligência Artificial à rede (LAN, VPS, Docker),
qualquer pessoa com o endereço pode consumir os tokens/quotas do desenvolvedor.
Sem proteção, as APIs são vulneráveis ao mau-uso, injecção de prompt e abuso.

**Como o OmniRoute resolve isso:**

- **Gerenciamento de Chave API** — Geração, rotação e escopo por provedor com
  uma tela dedicada de `/painel/dashboard/api-manager`
- **Permissões a Nível de Modelo** — Restrinja as chaves API a modelos
  específicos (`openai/*`, padrões de wildcard), com opções de Permitir
  Todo/Restringir
- **Proteção de Endereço da API** — Exija uma chave para `/v1/models` e bloqueie
  provedores específicos da listagem
- **Guarda de Autenticação + Proteção CSRF** — Todas as rotas do painel
  protegidas com `comAuth` middleware + tokens CSRF
- **Limite de Taxa** — Limitação de taxa por IP com janelas configuráveis
- **Filtração de IP** — Permitir/Proibir para controle de acesso
- **Guarda contra Injeção de Prompt** — Sanitização contra padrões de prompt
  malicious
- **Criptografia AES-256-GCM** — Senhas criptografadas em repouso

</details>

<details>
<summary><b>🛑 6. "My provider went down and I lost my coding flow"</b></summary>

Os provedores de AI podem se tornar instáveis, retornar erros de 5xx ou bater em
limites de taxa temporários. Se um desenvolvedor depende de um único provedor,
eles são interrompidos. Sem circuit breakers, tentativas de retry repetidas
podem fazer o aplicativo explodir

**Como o OmniRoute resolve isso:**

- **Circuitos com Rombo a Nível de Modelo** — Abre/Fecha automaticamente com
  limiares e tempo de espera configuráveis (Fechado/Aberto/Medio-Aberto),
  escalonado por modelo para evitar blocos cascata
- **Atraso Exponencial** — Atrasos de repetição progressivos
- **Anti-Tráfego de Gado** — Proteção mutex + semáforo contra tempestades de
  retry concorrentes
- **Cadeias de Falha Combinadas** — Se o provedor primário falhar, automatizar o
  fallback através da cadeia sem intervenção
- **Combo Circuito com Rombo** — Desativa provedores falhos dentro de uma cadeia
  combinada
- **Painel de Status de Saúde** — Monitoramento de tempo de funcionamento,
  estados de circuit breaker, e bloqueios de cache, estatísticas de p50/p95/p99
  de latência

</details>

<details>
<summary><b>🔧 7. "Configuring each AI tool is tedious and repetitive"</b></summary>

Os desenvolvedores usam Cursor, Claude Code, Codex CLI, OpenClaw, Gemini CLI,
Kilo Code... Cada ferramenta precisa de configurações diferentes (endereço de
API, chave, modelo). Reconfigurar ao mudar provedores ou modelos é uma perda de
tempo.

**Como o OmniRoute resolve isso:**

- **CLI Ferramentas Painel** — Página dedicada apenas para o setup de um clique
  para Claude Code, Codex CLI, OpenClaw, Kilo Code, Antigravity, Cline
- **GitHub Copilot Configuração Gerador** — Gera `chatLanguageModels.json` para
  o VS Código com seleção de modelo em bloco
- **Mágico de Onboarding** — Setup guiado em 4 etapas para usuários iniciantes
- **Um ponto de acesso, todos os modelos** — Configure
  `http://localhost:20128/v1` uma vez, acesse 67+ provedores

</details>

<details>
<summary><b>🔑 8. "Managing OAuth tokens from multiple providers is hell"</b></summary>

Claude Code, Codex, Gemini CLI, Copilot — todos usam OAuth 2.0 com tokens
expiráveis. Os desenvolvedores precisam se re-autenticar constantemente, lidar
com `client_secret faltando`, `redirect_uri_mismatch` e falhas em servidores
remotos. OAuth no LAN/VPS é particularmente problemático

**Como o OmniRoute resolve isso:**

- **Atualização Automática de Token** — Tokens de OAuth atualizados em segundo
  plano antes da expiração
- **OAuth 2.0 (PKCE) Integrado** — Fluxo automático para Claude Code, Codex,
  Gemini CLI, Copilot, Kiro, Qwen, iFlow
- **OAuth Multi-conta** — Várias contas por provedor via JWT/ID token
  extrativismo
- **OAUTH LAN/Remoto Fix** — Detecção de endereço de rede privado para
  `redirect_uri` + modo de URL manual para servidores remotos
- **OAUTH Atrás do Nginx** — Usa `window.location.origin` para compatibilidade
  de proxy reverso
- **Guia de OAuth Remoto** — Guia passo a passo para credenciais do Cloud Google
  na VPS/Docker

</details>

<details>
<summary><b>📊 9. "I don't know how much I'm spending or where"</b></summary>

Os desenvolvedores usam múltiplos provedores pagos, mas não têm uma visão
unificada de despesas. Cada provedor tem seu próprio painel de gerenciamento de
faturamento, mas não há uma visão consolidada. Custos inesperados podem empilhar

**Como o OmniRoute resolve isso:**

- **Painel de Análise de Custos** — rastreamento de custo por token e
  gerenciamento de orçamento por provedor
- **Limite de Orçamento por Nível** — Teto de gasto por nível que desencadeia
  fallback automático
- **Configuração de Preços por Modelo** — Preços configuráveis por modelo
- **Estatísticas de Uso por Chave de API** — Contagem de requisição e ultima
  marca de tempo por chave
- **Painel de Análise** — Cartões de estatísticas, gráficos de uso de modelo,
  tabela de provedor com taxas de sucesso e latência

</details>

<details>
<summary><b>🐛 10. "I can't diagnose errors and problems in AI calls"</b></summary>

==WEBLATE_PART==\
Um erro de chamada pode não indicar se foi causado por limitação de taxa, token
expirado, formato errado ou algum erro do provedor. Sem observabilidade e
registradores fragmentados em diferentes terminais, a depuração é apenas um
processo de tentativa e erro.

**Como o OmniRoute resolve isso:**

- **Console Unified Logs** — 4 abas: Registros de Solicitações, Registros do
  Proxy, Registros de Auditoria, Console
- **Visualizador de Logs no Console** — Visualizador em tempo real com estilo de
  terminal, com cores codificadas, rolagem automática, busca, filtro
- **SQLite Registros do Proxy** — Registros persistentes que sobrevivem a
  reinicializações do servidor
- **Playground de Tradução** — 4 modos de depuração: Playground (tradução de
  formato), Chat Tester (retorno circular), Test Bench (lote), Live Monitor (em
  tempo real)
- **Telemetria de Solicitações** — latência p50/p95/p99 + X-Request-Id rastreio
- **Arquivos de Registro com Roção** — Interceptor de console capta tudo para
  arquivo de log JSON com rocação baseada em tamanho
- **Relatório de Informações do Sistema** — `npm run system-info` gera
  `system-info.txt` com seu ambiente completo (versão Node, OmniRoute, OS,
  ferramentas CLI, status Docker/PM2). Anexe para o relatório de casos para
  triagem instantânea.

</details>

<details>
<summary><b>🏗️ 11. "Deploying and maintaining the gateway is complex"</b></summary>

A instalação, configuração e manutenção de um proxy de IA em diferentes
ambientes (local, VPS, Docker, nuvem) pode ser sobrecarregadora. Problemas como
caminhos pré-definidos, `EACCES` em pastas, conflitos de porta e compilações
múltiplas em plataformas diferentes criam atrasos.

**Como o OmniRoute resolve isso:**

- **Instalação Global com npm** — `npm install -g omniroute &amp;&amp;
  omniroute` — concluído
- **Docker Múltipla Plataforma** — AMD64 + ARM64 nativa (Apple Silicon, AWS
  Graviton, Raspberry Pi)
- **Perfis de Docker Compose** — `base` (sem ferramentas CLI) e `cli` (com
  Claude Code, Codex, OpenClaw)
- **Aplicativo de Escritório com Electron** — Aplicativo nativo para
  Windows/macOS/Linux com área de notificação do sistema, auto-inicialização,
  modo off-line
- **Modo de Porta Dividida** — API e Console em portas separadas para cenários
  avançados (proxy reverso, networking de contêineres)
- **Sincronização da Nuvem** — Sincronização de configurações em diferentes
  dispositivos via Workers da Cloudflare
- **Backup de BD** — Backup automático, restauração, exportação e importação de
  todas as configurações

</details>

<details>
<summary><b>🌍 12. "The interface is English-only and my team doesn't speak English"</b></summary>

Equipes de países que não falam inglês, especialmente na América Latina, Ásia e
Europa, lutam com interfaces em inglês apenas. Barreiras de idioma reduzem a
adoção e aumentam os erros de configuração.

**Como o OmniRoute resolve isso:**

- **Painel de Controle i18n — 30 Idiomas** — Todas as 500+ chaves traduzidas
  incluindo Árabe, Búlgaro, Dinamarquês, Alemão, Espanhol, Finlandês, Francês,
  Hebraico, Hindi, Húngaro, Indonésio, Italiano, Japonês, Coreano, Malaio,
  Holandês, Norueguês, Polonês, Português (PT/BR), Romeno, Russo, Eslovaco,
  Sueco, Tailandês, Ucraniano, Vietnês, Chinês, Filipino, Inglês
- **Suporte a Leitura Direta** — Suporte à leitura direta para Árabe e Hebraico
- **READMEs em Múltiplas Idiomas** — 30 traduções completas de documentação
- ** Seleção de Idiomas** — Ícone de Globo no header para troca em tempo real

</details>

<details>
<summary><b>🔄 13. "I need more than chat — I need embeddings, images, audio"</b></summary>

A IA além de completamento de conversa, os devs precisam gerar imagens,
transcrever áudio, criar embeddings para RAG, reclassificar documentos, e
moderar conteúdo. Cada API tem um endpoint e um formato diferentes.

**Como o OmniRoute resolve isso:**

- **Embeddings** — `/v1/embeddings` com 6 provedores e 9+ modelos
- **Geração de Imagens** — `/v1/images/generations` com 10 provedores e 20+
  modelos (OpenAI, xAI, Together, Fireworks, Nebius, Hyperbolic, NanoBanana,
  Antigravity, SD WebUI, ComfyUI)
- **Texto para Vídeo** — `/v1/videos/generations` — ComfyUI (AnimateDiff, SVD) e
  SD WebUI
- **Texto para Música** — `/v1/music/generations` — ComfyUI (Stable Audio Open,
  MusicGen)
- **Transcrição de Áudio** — `/v1/audio/transcriptions` — Whisper + Nvidia NIM,
  HuggingFace, Qwen3
- **Voz em Texto** — `/v1/audio/speech` — ElevenLabs, Nvidia NIM, HuggingFace,
  Coqui, Tortoise, Qwen3, **Inworld**, **Cartesia**, **PlayHT**, + provedores
  existentes
- **Moderação** — `/v1/moderations` — Verificação de segurança de conteúdo
- **Reclasseificação** — `/v1/rerank` — Reclasseificação de relevância de
  documentos
- **API de Respostas** — Suporte completo para `/v1/responses` do Codex

</details>

<details>
<summary><b>🧪 14. "I have no way to test and compare quality across models"</b></summary>

Os desenvolvedores querem saber qual modelo é melhor para o caso de uso —
código, tradução, raciocínio — mas comparar manualmente é lento. Não existem
ferramentas de avaliação integradas.

**Como o OmniRoute resolve isso:**

- **Avaliações de LLM** — Testes em conjunto ouro com 10 casos pré-carregados
  cobrindo cumprimento de cumprimentos, matemática, geografia, geração de
  código, JSON de conformidade, tradução, markdown, recusa de segurança
- **Táticas de Correspondência** — `exato`, `contém`, `regex`, `personalizado`
  (função JavaScript)
- **Teste da Banco de Exemplos do Tradutor** — Testes em lote com múltiplas
  entradas e saídas esperadas, comparação de provedores cruzados
- **Alojamento de Testes do Bate-papo** — Rodada integral de ida e volta com
  renderização de resposta visual
- **Monitoramento em Tempo Real** — Fluxo em tempo real de todos os pedidos que
  passam pelo proxy

</details>

<details>
<summary><b>📈 15. "I need to scale without losing performance"</b></summary>

Quanto o volume de solicitações aumenta, sem a implementação de cache, as mesmas
perguntas geram custos duplicados. Sem idempotência, as solicitações duplicadas
desperdiçam processamento. É necessário respeitar os limites de taxa por
provedor.

**Como o OmniRoute resolve isso:**

- **Cache Semântico** — Cache em duas camadas (assinatura + semântico) reduz
  custo e latência
- **Idempotência de Solicitação** — Janela de 5s de deduplicação para
  solicitações idênticas
- **Detecção de Limites de Taxa** — Contagem de RPM por provedor, minimo de
  interjogo, e limite máximo de concorrentes a serem rastreados
- **Limites de Taxa Editáveis** — Configurações personalizáveis em Configurações
  → Resiliência com persistência
- **Cache de Validação de Chave de API** — Cache a três camadas para performance
  em produção
- **Painel de Controle de Saúde com Telemetria** — Latência p50/p95/p99,
  estatísticas de cache, e tempo de funcionamento

</details>

<details>
<summary><b>🤖 16. "I want to control model behavior globally"</b></summary>

Desenvolvedores que desejam todas as respostas em um determinado idioma, com um
determinado tom, ou queiram limitar tokens de razão. Configurar isso em todos os
instrumentos/solicitações é impraticável.

**Como o OmniRoute resolve isso:**

- **Injeção do Prompt do Sistema** — Prompt global aplicado a todas as
  solicitações
- **Validação do Ouro de Razão** — Controle de alocação de tokens de razão por
  solicitação (passe-through, automático, customizado, adaptativo)
- **6 Estratégias de Rotulação** — Estratégias globais que determinam como as
  solicitações são distribuídas
- **Roteador Wildecard** — `padrões de provedor/*` roteados dinamicamente para
  qualquer provedor
- **Habilitar/Desabilitar� Toggle Combinação** — Alternar as combinações
  diretamente do painel de controle
- **ToggleButton de Provedor** — Habilitar/desabilitar todas as conexões de um
  provedor com um clique
- **Provedores Bloqueados** — Excluir provedores específicos da lista de
  modelos/V1/v1/ `

</details>

<details>
<summary><b>🧰 17. "I need MCP tools as first-class product capabilities"</b></summary>

Muitos gateways de IA expõem MCP apenas como um detalhe de implementação oculto.
Equipes precisam de uma camada de operação visível e gerenciável.

**Como o OmniRoute resolve isso:**

- MCP aparece na navegação da tela inicial e na seção de protocolo do endpoint
- Página de gerenciamento dedicada de MCP com processos, ferramentas, escopos e
  auditoria
- Inicio rápido embutido para `omniroute --mcp`` e onboarding de clientes ```

</details>

<details>
<summary><b>🧠 18. "I need A2A orchestration with sync + stream task paths"</b></summary>

Fluxos de agentes precisam de respostas diretas e execução streamada com
controle de ciclo de vida.

**Como o OmniRoute resolve isso:**

- Pontencial de JSON-RPC (POST /a2a`) com `message/send`` e `message/stream``
- Streaming SSE com propagação de estado terminal
- APIs de ciclo de vida de tarefas para `tasks/get`` e `tasks/cancel``

</details>

<details>
<summary><b>🛰️ 19. "I need real MCP process health, not guessed status"</b></summary>

As equipes operacionais precisam saber se o MCP está vivo, e não apenas se a API
está acessível

**Como o OmniRoute resolve isso:**

- Arquivo de pulso de execução com PID, horários de tempo, transporte, número de
  ferramentas e modo de escopo
- API do status do MCP, combinando pulso de execução com atividade recente
- Cartões de status da interface para processos/uptime/atividade do pulso

</details>

<details>
<summary><b>📋 20. "I need auditable MCP tool execution"</b></summary>

Quando as ferramentas mutam a configuação ou ativam ações de operação, as
equipes precisam de rastreamento forense

**Como o OmniRoute resolve isso:**

- Log de auditoria baseado em SQLite para chamadas de ferramenta MCP
- Filtrar por ferramenta, sucesso/falha, chave API e paginação
- Tabela de auditoria da tela inicial + endpoints de estatísticas para automação

</details>

<details>
<summary><b>🔐 21. "I need scoped MCP permissions per integration"</b></summary>

Os clientes diferentes deveriam ter acesso de menos privilégios às categorias de
ferramentas.

**Como o OmniRoute resolve isso:**

- 9 Escopos de MCP granulares para acessar ferramentas controladas
- Implantação e visibilidade de escopo na interface da MCP de gerenciamento
- Fila de respaldo padrão para ferramental operacional

</details>

<details>
<summary><b>⚙️ 22. "I need operational controls without redeploying"</b></summary>

Os times precisam de mudanças rápidas durante incidentes ou eventos de custos

**Como o OmniRoute resolve isso:**

- Clique e ativa combo de atribuição diretamente na tela de dashboard da MCP
- Aplicar perfis de resiliência de packs de políticas pré-definidas
- Reinicie o estado de interrupção de corrente da mesma linha de panel de
  operações

</details>

<details>
<summary><b>🔄 23. "I need live A2A task lifecycle visibility and cancellation"</b></summary>

Sem visibilidade de ciclo de vida, incidentes de tarefa ficam difíceis de
triagem

**Como o OmniRoute resolve isso:**

- Listagem ou filtro de tarefas por estado/habilidades com paginação
- Ferramenta para exibição de metadados de tarefa, eventos e artefatos
- Endpoint de cancelamento e ação de UI de tarefa com confirmação

</details>

<details>
<summary><b>🌊 24. "I need active stream metrics for A2A load"</b></summary>

Fluxos de streaming requerem visão operacional da concorrência e conexões ativa

**Como o OmniRoute resolve isso:**

- Contadores de fludo ativo integrado ao status A2A
- Último timestamp de tarefa e contagem por estado
- Cartões da A2A para monitoramento de opération em tempo real

</details>

<details>
<summary><b>🪪 25. "I need standard agent discovery for clients"</b></summary>

Os clientes externos e orquestradores precisam de metadados lidos por máquina
para onboarding.

**Como o OmniRoute resolve isso:**

- Carteira de Agente exposta em `/.well-known/agent.json`
- Capacidades e habilidades exibidas no painel de gestão
- API do status A2A inclui metadados de descoberta para automação

</details>

<details>
<summary><b>🧭 26. "I need protocol discoverability in the product UX"</b></summary>

Se os usuários não conseguem descobrir superfícies de protocolo, a adotabilidade
e a qualidade de suporte caem.

**Como o OmniRoute resolve isso:**

- Página consolidada de **Pontos de Extremidade** com guias para Proxy, MCP, A2A
  e Pontos de Extremidade APIs
- Alternativas de status de serviço inline (Online/Offline) para MCP e A2A
- Links da versão geral para guias de gestão dedicados

</details>

<details>
<summary><b>🧪 27. "I need end-to-end protocol validation with real clients"</b></summary>

Testes de mockagem não são suficientes para validar compatibilidade de protocolo
antes da liberação.

**Como o OmniRoute resolve isso:**

- Suíte de teste E2E que inicializa a aplicação e utiliza o cliente de
  transporte de MCP SDK
- Testes do cliente A2A para descoberta, envio, fluxo de stream, e fluxos de
  obtenção e cancelamento
- Assertions cruzadas contra as APIs de auditoria de MCP e tarefas de A2A

</details>

<details>
<summary><b>📡 28. "I need unified observability across all interfaces"</b></summary>

A divisão da observabilidade por protocolo cria pontos cegos e aumenta o MTTR.

**Como o OmniRoute resolve isso:**

- Painéis unificados de log, análise e tela de controle em um único produto
- Telemetria de saúde, auditoria e solicitações do OpenAI, MCP e camadas A2A
- APIs operacionais para status e automação

</details>

<details>
<summary><b>💼 29. "I need one runtime for proxy + tools + agent orchestration"</b></summary>

Executar muitos serviços separados aumenta o custo operacional e modos de falha.

**Como o OmniRoute resolve isso:**

- Proxy compatível com Open AI, servidor MCP e servidor A2A em um único stack
- Autenticação compartilhada, resiliência, armazenamento de dados e
  observabilidade
- Modelo de política consistente em todos os superfícies de interação

</details>

<details>
<summary><b>🚀 30. "I need to ship agentic workflows without glue-code sprawl"</b></summary>

Equipes perdem velocidade quando montam serviços múltiplos ad-hoc e scripts

**Como o OmniRoute resolve isso:**

- Estratégia de ponto final unificada para clientes e agentes
- Interface de IU de gerenciamento de protocolo embutido e caminhos de
  validaçaom de fumaça
- Fundamentos prontos para produção (segurança, registro, resiliência, backup)

</details>

### Exemplos de Playbooks (Uso de Casos Integrais)

**Playbook A: Maximize assinatura paga + backup barato **

```txt
Combo: "maximize-claude"
  1. cc/claude-opus-4-6
  2. glm/glm-4.7
  3. if/kimi-k2-thinking

Custo mensal: $20 + pequeno backup gasto
Outcome: qualidade maior, interrupções quase zero
```

**Playbook B: Pilha de codificação zero-custo **

```txt
Combo: "gratuito-para-sempre"
  1. gc/gemini-3-flash
  2. if/kimi-k2-thinking
  3. qw/qwen3-coder-plus

Custo mensal: $0
Outcome: fluxo de codificação estável e gratuito
```

**Playbook C: Chain de fallback de falha durante 24/7 **

```txt
Combo: "sempre-ligado"
  1. cc/claude-opus-4-6
  2. cx/gpt-5.2-codex
  3. glm/glm-4.7
  4. minimax/MiniMax-M2.1
  5. if/kimi-k2-thinking

Outcome: profundidade de fallback profundo para trabalhos sob prazos críticos
```

**Playbook D: Operações de agente com MCP + A2A **

```txt
1) Inicie o transporte MCP (`omniroute --mcp`) para operações impulsionadas por ferramentas
2) Execute tarefas A2A via `enviar mensagem` e ` Fluxo de mensagem`
3) Observe via /dashboard/endpoint (tabs MCP e A2A)
4) Alternar serviços via controles de status inline
```

---

## 🆓 Inicie Gratuito — Zero Custo de Configuração

> Configure a programação de AI em minutos em **$0/mês**. Conecte esses contas
> gratuitas e use a combo de pilha embutida **livre stack**.

| Step | Ação                                               | Providers Unlocked                                                 |
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

## Início Rápido

### 1. Instale e execute

```bash
npm install -g omniroute
omniroute
```

> **pnpm users:** Executar `pnpm approve-builds -g` após a instalação para
> ativar os scripts de compilação nativa necessários pelo `better-sqlite3` e
> `@swc/core`:
> 
> ```bash
> pnpm install -g omniroute
> pnpm approve-builds -g   # Selecione todos os pacotes → aprovar
> omniroute
> ```

A dashboard abre em `http://localhost:20128` e a URL base da API é
`http://localhost:20128/v1`.

| Comando                 | Descrição                                                       |
| ----------------------- | --------------------------------------------------------------- |
| `omniroute`             | Iniciar servidor (`PORT=20128`, API e dashboard no mesmo porta) |
| `omniroute --port 3000` | Defina a porta canônica/AI para 3000                            |
| `omniroute --mcp`       | Iniciar servidor MCP (transporte estéreo)                       |
| `omniroute --no-open`   | NÃO Abrir navegador automaticamente                             |
| `omniroute --help`      | Mostrar ajuda                                                   |

Modo de porta opcional dividida:

```bash
PORT=20128 DASHBOARD_PORT=20129 omniroute
# API:       http://localhost:20128/v1
# Dashboard: http://localhost:20129
```

### 2) Conecte fornecedores e crie sua chave API

1. Abra o painel de controle → `Fornecedores` e conecte ao menos um fornecedor
   (OAuth ou chave API).
2. Abra o painel de controle → `Pontas` e crie uma chave API.
3. (Opcional) Abra o painel de controle → `Combos` e defina sua cadeia de
   fallback.

### 3) Pontua sua ferramenta de código para OmniRoute

```txt
URL-base: http://localhost:20128/v1
Chave API:  [copie a partir da página de Endpoint]
Modelo:    se/kimi-k2-pensamento (ou qualquer prefixo de fornecedor/modelo)
```

Funciona com Claude Code, Codex CLI, Gemini CLI, Cursor, Cline, OpenClaw,
OpenCode e SDKs compatíveis com OpenAI.

### 4) Ative e valide protocolos (v2.0)

**MCP (para operações de ferramenta):**

```bash
omniroute --mcp
```

Em seguida, conecte seu cliente de MCP sobre `stdio` e teste ferramentas como:

- `omniroute_get_health`
- `omniroute_list_combos`

**A2A (para fluxos entre agentes):**

```bash
curl http://localhost:20128/.well-known/agent.json
```

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"quickstart","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"Dê-me uma resumo curto de quota."}]}}'
```

### 5) Valide tudo de ponta a ponta (recomendado)

```bash
npm run test:protocolos:e2e
```

essa suite valida fluxos de cliente MCP e A2A reais contra uma aplicação em
execução.

### Alternativa: execute a partir da fonte.

```bash
cp .env.exemplo .env
npm install
PORT=20128 DASHBOARD_PORT=20129 NEXT_PUBLIC_BASE_URL=http://localhost:20129 npm run dev
```

---

## 🐳 Docker

A OmniRoute está disponível como imagem de Docker pública no [Docker
Hub](https://hub.docker.com/r/diegosouzapw/omniroute).

**Execução rápida:**

```bash
docker run -d \
  --name omniroute \
  --restart unless-stopped \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:latest
```

**Com arquivo de ambiente:**

```bash
# Copie e edite o arquivo .env primeiro
cp .env.exemplo .env

docker run -d \
  --name omniroute \
  --restart unless-stopped \
  --env-file .env \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:latest
```

**Usando O Docker Compose:**

```bash
# Perfil base (sem ferramentas CLI)
docker compose --profile base up -d

# Perfil CLI (Claude Code, Codex, OpenClaw embutido)
docker compose --profile cli up -d
```

| Imagem                   | Versão   | Tamanho | Descrição                 |
| ------------------------ | -------- | ------- | ------------------------- |
| `diegosouzapw/omniroute` | `latest` | ~250MB  | Última lançamento estável |
| `diegosouzapw/omniroute` | `1.0.3`  | ~250MB  | Versão atual              |

---

## 🖥️ Aplicativo de desktop — Offline & Always-On

> 🆕 **NOVO** OmniRoute está agora disponível como **aplicativo desktop nativo**
> para Windows, macOS e Linux.

Execute OmniRoute como aplicativo desktop standalone — nada de terminal,
navegador ou internet é necessário para modelos locais. O aplicativo baseado em
Electron inclui:

- 🖥️ **Janela Nativa** — Janela do aplicativo com integração ao painel de
  notificações do sistema
- 🔄 **Lançar Automático** — Inicie OmniRoute no login do sistema
- 🔔 **Notificações Nativas** — Receba alertas sobre esgotamento do limite de uso
  ou problemas dos provedores
- ⚡ **Instale Com Uma Só Clique** — NSIS (Windows), DMG (macOS), AppImage
  (Linux)
- 🌐 **Modo Offline** — Functiona totalmente offline com servidor embutido

### Início Rápido

```bash
# Modo de desenvolvimento
npm run electron:dev

# Construa para sua plataforma
npm run electron:build       # Plataforma atual
npm run electron:build:win   # Windows (.exe)
npm run electron:build:mac   # macOS (.dmg) — x64 &amp; arm64
npm run electron:build:linux # Linux (.AppImage)
```

### Painel de notificações

Quando minimizado, o OmniRoute vive no painel de notificações do sistema com
ações rápidas:

- Abrir Painel
- Alterar porta do servidor
- Sair do aplicativo

📖 Documentação completa: [`electron/README.md`](electron/README.md)

---

## Preços em Uma Visão Geral

| Nível              | Provedor                   | Custo                                           | Reiniciar da Quota      | Melhor para                                     |
| ------------------ | -------------------------- | ----------------------------------------------- | ----------------------- | ----------------------------------------------- |
| **💳 INSCRIÇÃO**    | Claude Código (Pro)        | $20/mês                                         | 5h + semanalmente       | Já inscrito                                     |
|                    | Codex (Plus/Pro)           | $20-200/mês                                     | 5h + semanalmente       | Usuários do OpenAI                              |
|                    | CLI do Gemini              | **GRATUITO**                                    | 180K/mês + 1K/dia       | Todos!                                          |
|                    | GitHub Copilot             | $10-19/mês                                      | Mensal                  | Usuários do GitHub                              |
| **🔑 CHAVE DA API** | NVIDIA NIM                 | **GRATUITO** (para desenvolvedores para sempre) | ~40 RPM                 | 70+ modelos abertos                             |
|                    | Cerebras                   | **GRATUITO** (1M tok/day)                       | 60K TPM / 30 RPM        | Mundo mais rápido                               |
|                    | Groq                       | **GRATUITO** (30 RPM)                           | 14,4K RPD               | Llama/Gemma ultra-rápido                        |
|                    | DeepSeek V3.2              | $0,27/$1,10 por 1M                              | Nenhum                  | Melhor preço/razão de qualidade                 |
|                    | xAI Grok-4 Ligeiro         | **$0,20/$0,50 por 1M** 🆕                        | Nenhum                  | Mais rápido + chamada de ferramenta, ultrabaixo |
|                    | xAI Grok-4 (padrão)        | $0,20/$1,50 por 1M 🆕                            | Nenhum                  | Lançamento razões marco da xAI                  |
|                    | Mistral                    | Teste gratuito + paga                           | limite de taxa atingido | AI europeu                                      |
|                    | OpenRouter                 | Pagamento por uso                               | Nenhum                  | 100+ modelos agrupados                          |
| **💰 BARATO**       | GLM-5 (via Z.AI) 🆕         | $0,50/1M                                        | Diário 10AM             | 128K de saída, modelo mais novo                 |
|                    | GLM-4,7                    | $0,60/1M                                        | Diário 10AM             | Controle orçamentário                           |
|                    | MiniMax M2,5 🆕             | $0,30/1M entrada                                | 5 horas de rodagem      | Tarefa de raciocínio + agente                   |
|                    | MiniMax M2,1               | $0,2/1000000                                    | 5 horas de rodagem      | Opção mais econômica                            |
|                    | Kimi K2.5 (Moonshot API) 🆕 | Pagamento por uso                               | Nenhum                  | Acesso direto à API Moonshot                    |
|                    | Kimi K2                    | $9/mês flat                                     | 10.000.000 tokens/mês   | Custo previsível                                |
| **🆓 ** GRÁTIS      | iFlow                      | **$0**                                          | Ilimitado               | 5 modelos ilimitados                            |
|                    | Qwen                       | **$0**                                          | Ilimitado               | 4 modelos ilimitados                            |
|                    | Kiro                       | **$0**                                          | Ilimitado               | Claude Sonnet/Haiku (AWS Builder)               |
|                    | LongCat Flash-Lite 🆕       | **$0** (50.000.000 tok/day 🔥)                   | 1 RPS                   | Maior quota gratuita na Terra                   |
|                    | Polinizações AI 🆕          | **$0** (nenhuma chave necessária)               | 1 req/15s               | GPT-5, Claude, DeepSeek, Llama 4                |
|                    | Cloudflare Workers AI 🆕    | **$0** (10K Neuron/dia)                         | ~150 resp/ dia          | 50+ modelos, pontos de extremidade global       |
|                    | Scaleway AI 🆕              | **$0** (1 M total de tokens)                    | limite de taxa atingido | UE/ RGPD, Qwen3 235B, Llama 70B                 |

> 🆕 **Nove modelos adicionados (mar. 2026):** Grok-4 Fast familia em
> $0,20/$0,50/M (medido em 1143ms — 30% mais rápido do que o Gemini 2,5 Flash),
> GLM-5 via Z.AI com 128K de saída, MiniMax M2,5 de raciocínio, DeepSeek V3,2 de
> preço atualizado, Kimi K2,5 via Moonshot API direta.

** 💡 Combo Pilha sem cobrança — O Setup Total Gratuito:**

```
# ![](🆓 Pilha Totalmente Gratuita 2026 — 11 Provedores, $0 Forever)
Kiro (kr/)             → Claude Sonnet/Haiku SEM LIMITES
iFlow (if/)            → kimi-k2-pensamento, qwen3-coder_plus, deepseek-r1 SEM LIMITES
LongCat Lite (lc/)     → LongCat-Flash-Lite — 50M tokens/ dia 🔥
Polinizações (pol/)    → GPT-5, Claude, DeepSeek, Llama 4 — sem chave necessária
Qwen (qw/)             → qwen3-coder_plus, qwen3-coder_flash, qwen3-coder_next SEM LIMITES
Gemini (gemini/)       → Gemini 2,5 Flash — 1,500 req/dia de chave API gratuita
Cloudflare AI (cf/)    → Llama 70B, Gemma 3, Mistral — 10K Neuron/ dia
Scaleway (scw/)        → Qwen3 235B, Llama 70B — 1M tokens gratuitos (eu)
Groq (groq/)           → Llama/Gemma ultra-rápido — 14,4K req/ dia
NVIDIA NIM (nvidia/)   → 70+ modelos abertos — 40 RPM forever
Cerebras (cerebras/)   → Llama/Qwen mais rápido do mundo — 1M tok/dia
```

**Sem custo algum. Nunca para de codificar.** Configure essa como uma combo
OmniRoute e todas as falhas acontecem automaticamente — não é necessário
manualmente mudar a configuração nunca.

---

---

## 🆓 Modelos livres — O que você realmente recebe

> Todos os modelos abaixo são **100% gratos sem necessidade de cartão de
> crédito**. OmniRoute auto-routes entre eles quando uma quota esgote —
> combine-os todos para uma combo inquebrável de $0.

### 🔵 MÓDELOS CLAUDE (via Kiro — ID do construtor do AWS)

| Modelo              | Prefixo | Limite        | Limite de Taxa                  |
| ------------------- | ------- | ------------- | ------------------------------- |
| `claude-sonnet-4.5` | `kr/`   | **Ilimitado** | Sem informação de limite diário |
| `claude-haiku-4.5`  | `kr/`   | **Ilimitado** | Sem informação de limite diário |
| `claude-opus-4.6`   | `kr/`   | **Ilimitado** | Último Opus via Kiro            |

### 🟢 MODELOS DE FLUXO DE IFLOW (Oauth Gratuito - Sem Cartão de Crédito)

| Modelo                | Prefixo | Limite        | Limite de Taxa      |
| --------------------- | ------- | ------------- | ------------------- |
| `kimi-k2-pensando`    | `if/`   | **Ilimitado** | Sem limite relatado |
| `qwen3-coder-plus`    | `if/`   | **Ilimitado** | Sem limite relatado |
| Pesquisa Profunda-r1` | `if/`   | **Ilimitado** | Sem limite relatado |
| Minimáximo-m2.1`      | `if/`   | **Ilimitado** | Sem limite relatado |
| Kimi-k2`              | `if/`   | **Ilimitado** | Sem limite relatado |

### 🟡 MODELOS QWEN (Código de Autenticação do Dispositivo)

| Modelo                           | Prefixo | Limite        | Limite de Taxa       |
| -------------------------------- | ------- | ------------- | -------------------- |
| `qwen3-coder-plus`               | `qw/`   | **Ilimitado** | Sem limite relatado  |
| `qwen3-Flash do Código do Coder` | `qw/`   | **Ilimitado** | Sem limite relatado  |
| `qwen3-Next do Coder`            | `qw/`   | **Ilimitado** | Sem limite relatado  |
| `modelo de visão`                | `qw/`   | **Ilimitado** | Multimodal (imagens) |

### 🟣 CLI GÊMNI (Google OAuth)

| Modelo             | Prefixo | Limite                                  | Limite de Taxa    |
| ------------------ | ------- | --------------------------------------- | ----------------- |
| `gemini-3-preview` | `gc/`   | **180K tokens por mês** + 1K/dia        | Reset mensal      |
| `gemini-2.5-pro`   | `gc/`   | 180K/token por mês (pool compartilhado) | De Alta Qualidade |

### ⚫ NVIDIA NIM (Chave de API gratuita — build.nvidia.com)

| Nível                  | Limite Diário       | Limite de Taxa | Notas                                                                          |
| ---------------------- | ------------------- | -------------- | ------------------------------------------------------------------------------ |
| Grátis (Desenvolvedor) | Sem limite de token | **~40 RPM**    | 70+ modelos; mudança para limites puramente de taxa a partir da metade de 2025 |

Modelos gratuitos populares: `moonshotai/kimi-k2.5` (Kimi K2.5), `z-ai/glm4.7`
(GLM 4.7), `deepseek-ai/deepseek-v3.2` (DeepSeek V3.2),
`nvidia/llama-3.3-70b-instruct`, `deepseek/deepseek-r1`

### ⚪ BRUSH  (Chave de API gratuita — inference.cerebras.ai)

| Nível | Limite Diário     | Limite de Taxa   | Notas                                                     |
| ----- | ----------------- | ---------------- | --------------------------------------------------------- |
| Free  | **1M tokens/day** | 60K TPM / 30 RPM | Inferência LLM mais rápida do mundo; reinicia diariamente |

Disponível gratuitamente: `llama-3.3-70b`, `llama-3.1-8b`,
`deepseek-r1-distill-llama-70b`

### 🔴 GROQ (Chave de API gratuita — console.groq.com)

| Nível | Limite Diário | Limite de Taxa    | Notas                                               |
| ----- | ------------- | ----------------- | --------------------------------------------------- |
| Free  | **14.4K RPD** | 30 RPM por modelo | Sem cartão de crédito; 429 na limite, não é cobrado |

Disponível gratuitamente: `llama-3.3-70b-versatile`, `gemma2-9b-it`,
`mixtral-8x7b`, `whisper-large-v3`

### 🔴 LONGCAT AI (Chave de API gratuita — longcat.chat) 🆕

| Modelo                        | Prefixo | Diário Gratuito Quota | Notas                         |
| ----------------------------- | ------- | --------------------- | ----------------------------- |
| `LongCat-Flash-Lite`          | `lc/`   | **50M tokens** 💥      | Maior quota gratuita já vista |
| `LongCat-Flash-Chat`          | `lc/`   | 500K tokens           | Conversa de múltiplas voltas  |
| `LongCat-Flash-Thinking`      | `lc/`   | 500K tokens           | Raciocínio / CoT              |
| `LongCat-Flash-Thinking-2601` | `lc/`   | 500K tokens           | Versão de janeiro de 2026     |
| `LongCat-Flash-Omni-2603`     | `lc/`   | 500K tokens           | Multimodal                    |

> 100% gratuito enquanto em beta pública. Cadastre-se no
> [longcat.chat](https://longcat.chat) com email ou telefone. Recarregue
> diariamente às 00:00 UTC.

### 🟢 POLINIZAÇÕES AI (Nenhum conjunto de chaves não é necessário) 🆕

| Modelo     | Prefixo | Limite de Taxa | Fornecedor por Trás |
| ---------- | ------- | -------------- | ------------------- |
| `openai`   | `pol/`  | 1 req/15s      | GPT-5               |
| `claude`   | `pol/`  | 1 req/15s      | Anthropic Claude    |
| `gemini`   | `pol/`  | 1 req/15s      | Google Gemini       |
| `deepseek` | `pol/`  | 1 req/15s      | DeepSeek V3         |
| `llama`    | `pol/`  | 1 req/15s      | Meta Llama 4 Scout  |
| `mistral`  | `pol/`  | 1 req/15s      | Mistral AI          |

> ✨ **Sem atrito: Zero:** Não há cadastramento, sem API. Adicione o provedor
> Pollinations com um campo de chave em branco e isso funciona imediatamente.

### 🟠 CLOUDFLARE WORKERS AI (Chave de API gratuita — cloudflare.com) 🆕

| Nível | Neurônios Diários | Uso Equivalente                                 | Notas                             |
| ----- | ----------------- | ----------------------------------------------- | --------------------------------- |
| Free  | **10.000**        | ~150 LLM por servidor / 500s áudio / 15K embeds | Tela de borda global, 50+ modelos |

Modelos populares gratuitos: `@cf/meta/llama-3.3-70b-instruct`,
`@cf/google/gemma-3-12b-it`, `@cf/openai/whisper-large-v3-turbo` (áudio
gratuito!), `@cf/qwen/qwen2.5-coder-15b-instruct`

> Requer API Token + ID de conta de
> [dash.cloudflare.com](https://dash.cloudflare.com). Armazene o ID da conta em
> configurações do provedor.

### 🟣 SCALEWAY AI (1M Tokens gratuitos — scaleway.com) 🆕

| Nível | Cota gratuita | Localização  | Notas                                                    |
| ----- | ------------- | ------------ | -------------------------------------------------------- |
| Free  | **1M tokens** | 🇫🇷 Paris, EU | Nenhum cartão de crédito é necessário dentro dos limites |

Disponível gratuitamente: `qwen3-235b-a22b-instruct-2507` (Qwen3 235B!),
`llama-3.1-70b-instruct`, `mistral-pequeno-3.2-24b-instruct-2506`,
`deepseek-v3-0324`

> Cumprindo o EU/GDPR. Obtenha a chave API em
> [console.scaleway.com](https://console.scaleway.com).

> ** 💡 A Estaketa Free Mais Útil (11 Provedores, $0 Sempre): **
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

| Provedor         | Free Credits           | Best Model                                   | Limite de Taxa               |
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

Agora em `/painel/midia` → **Transcrição** de tela: carregue qualquer arquivo de
áudio ou vídeo → selecione seu endpoint de combo → obtenha a transcrição nos
formatos suportados.

## Características-chave

O OmniRoute v2.0 foi construído como uma plataforma operacional, e não apenas em
um proxy de relé.

### 🆕 Novo - Melhorias Inspiradas no Router-Claw (Mar 2026)

| Característica                         | O que ela faz                                                                                                                         |
| -------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| ⚡ **Família Grok-4 Fast**              | Modelos de inteligência artificial por $0,20/$0,50/M — benchmarkados em 1143ms (30% mais rápido do que o Gemini 2.5 Flash)            |
| 🧠 **GLM-5 via Z.AI**                   | Contexto de saída de 128K, $0,5/1M — a nova bandeira da família GLM                                                                   |
| 🔮 **MiniMax M2,5**                     | Tarefas de raciocínio + agente por $0,30/1M — uma ampla atualização em relação ao M2.1                                                |
| 🎯 **Bandeira de Chamada de Modelo**    | `Chamada de modelo por [X2X]modelo por modelo[X30X]: verdadeiro/falso` no registro — AutoCombo ignora modelos não capazes de chamadas |
| 🌍 **Detecção de Intenção Multilíngue** | Palavras-chave no AutoCombo com PT/ZH/ES/AR — seleção melhor de modelos para conteúdo não em inglês                                   |
| 📊 **Falhas Conduzidas por Benchmark**  | Latência real p95 de pedidos ao vivo alimenta a pontuação do combo — o AutoCombo aprende a partir de dados reais                      |
| 🔁 **Deduplication de Solicitação**     | Janela de dedup hash do conteúdo — a salva seguramente contra cobranças duplicadas                                                    |
| 🔌 **Roteador Estratégia Plugável**     | Interface de estratégia de roteamento extensível `RoteadorStrategy` — adicione lógica de roteamento personalizada como plugins        |

### 🚀 Anterior v2.0.9+ — Playground, CLI Dedos & ACP

| Característica                                        | O que ela faz                                                                                                                                                                                                                                                                                                          |
| ----------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🎮 **Lembrança de Modelo Playground**                  | Página de painel para testar qualquer modelo diretamente — seletores de provedor/modelo/retorno, Editor Monaco, streaming, abortar, tempo                                                                                                                                                                              |
| 🔏 **CLI Fingerprint de Correspondência**              | Ordem de cabeçalho/corpo por provedor para corresponder à assinatura nativa da CLI — habilite por provedor em Configurações > Segurança. **O seu IP de proxy é preservado**                                                                                                                                            |
| 🤝 **Suporte ao ACP (Protocolo de Agente de Cliente)** | Descoberta da agente CLI (Códex, Claude, Goose, Gemíno CLI, OpenClaw + 9 mais), lançador de processo, `/api/acp/agentes` ponto de extremidade                                                                                                                                                                          |
| 🤖 **Lançador do Dashboard de Agentes ACP**            | Página de depuração › Agentes — mosaico de 14 agentes com status de instalação, versão, formulário de agente personalizado para qualquer ferramenta de CLI. **Usuários do OpenCode** obtêm um botão "Baixar opencode.json" que gera automaticamente uma configuração pronta para uso com todos os modelos disponíveis. |
| 🔧 **Rotagem Personalizada `apiFormat` do Modelo**     | Modelos personalizados com `apiFormat: "respostas"` agora rodam corretamente para o Tradutor de API de Respostas                                                                                                                                                                                                       |
| 🏢 **Isolamento do Trabalho de Código**                | Múltiplos trabalhos de Códex por e-mail — OAuth separa corretamente as conexões por ID de trabalho                                                                                                                                                                                                                     |
| 🔄 **Atualização por Eletrônica Automática**           | Aplicativo de desktop verifica atualizações + auto-instala ao reiniciar                                                                                                                                                                                                                                                |

### 🤖 Operações de Agente & Protocolo (v2.0)

| Característica                        | O que ela faz                                                                                                                |
| ------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| 🔧 **MCP Server (16 tools)**           | IDE/agent tools via 3 transports: stdio, SSE (`/api/mcp/sse`), Streamable HTTP (`/api/mcp/stream`)                           |
| 🤝 **A2A Server (JSON-RPC + SSE)**     | Agent-to-agent task execution with sync and streaming flows                                                                  |
| 🧭 **Consolidated Endpoints Page**     | Tabbed management page with Endpoint Proxy, MCP, A2A, and API Endpoints tabs                                                 |
| 🎚️ **Service Enable/Disable Toggles** | ON/OFF switches for MCP and A2A with settings persistence (default: OFF)                                                     |
| 🛰️ **MCP Runtime Heartbeat**          | Real process status (pid, uptime, heartbeat age, transport, scope mode)                                                      |
| 📋 **MCP Audit Trail**                 | Filterable audit logs with success/failure and key attribution                                                               |
| 🔐 **MCP Scope Enforcement**           | 9 granular scope permissions for controlled tool access                                                                      |
| 📡 **A2A Task Lifecycle Management**   | List/filter tasks, inspect events/artifacts, cancel running tasks                                                            |
| 📋 **Agent Card Discovery**            | `/.well-known/agent.json` for client auto-discovery                                                                          |
| 🧪 **Protocolo de Teste E2E em Lab**   | Recurso MCP SDK + client fluxo A2A em `test:protocols:e2e`                                                                   |
| ⚙️ **Controle Operacional**           | Comando de seleção, aplicação de perfis de resistência e reset de interruptores com base em uma única superfície de controle |

### 🧠 Roteamento & Inteligência

| Característica                                           | O que ela faz                                                                       |
| -------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| 🎯 **Fallback Inteligente 4 Camadas**                     | Rotas automáticas: Inscrição → Chave de API → Mais Barato → Grátis                  |
| 📊 **Monitoramento em Tempo Real de Quotas**              | Contagem de token ao vivo + contagem de prorrogação de prazo por provedor           |
| 🔄 **Tradução de Formatação**                             | OpenAI ↔ Claude ↔ Gemini ↔ Converções com conversões para schema seguras            |
| 👥 **Suporte a Multi-Funções**                            | Várias contas por provedor com seleção inteligente                                  |
| 🔄 **Atualização Automática de Token**                    | Tokens OAuth se atualizam automaticamente com reenvio                               |
| 🎨 **Combinatórias Personalizadas**                       | 6 estratégias de equilíbrio + controle da cadeia de fallback                        |
| 🌐 **Roteador de Selos de Bem Vindo**                     | `fornecedor*/` roteamento dinâmico                                                  |
| 💭 **Ajustes de Orçamento do **                           | Rota de passagem, automático, personalizado e limites de razão adaptativos          |
| 🔀 **Aliasamentos de Modelos**                            | Aliasamento de modelo embutido + personalizado e segurança de migração              |
| ⚡ **Degradabilidade de Fundo**                           | Roteie as tarefas de fundo de baixa prioridade para modelos mais econômicos         |
| 🧪 **Abordagem Inteligente de Encaminhamento Tarefa[x28X] | Autoseleccione o modelo pelo tipo do conteúdo (codificação/cognição/procura/resumo) |
| 💬 **Injeção de Prompt do Sistema**                       | Controles de comportamento globais aplicados consistentemente                       |
| 📄 **Compatibilidade da API de Respostas**                | Suporte completo ao `/v1/respostas` para Codex e fluxos agênticos avançados         |

### 🎵 APIs Multi-Modais

| Característica              | O que ela faz                                                                                                                                                                     |
| --------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🖼️ **Geração de Imagens**   | `/v1/images/generations` com backends de nuvem e local                                                                                                                            |
| 📐 **Ajustes de Embeddings** | `/v1/embeddings` para tubulações de busca e RAG                                                                                                                                   |
| 🎤 **Audio Transcrição**     | `/v1/audio/transcrições` — 7 provedores (Deepgram Nova 3, AssemblyAI, Groq Whisper, HuggingFace, ElevenLabs, OpenAI, Azure), detecção de idioma automática, suporte a MP4/MP3/WAV |
| 🔊 **Text-to-Speech**        | `/v1/audio/fala` — 10 provedores (ElevenLabs, OpenAI, Deepgram, Cartesia, PlayHT, HuggingFace, Nvidia NIM, Inworld, Coqui, Tortoise) com correções de erros corretas              |
| 🎬 **Geração de Vídeo**      | `/v1/videos/generações` (ComfyUI + GUI Web do SD workflows)                                                                                                                       |
| 🎵 **Geração de Música**     | `/v1/música/generações` (fluxos de trabalho do ComfyUI)                                                                                                                           |
| 🛡️ **Moderações**           | `/v1/moderções` controles de segurança                                                                                                                                            |
| 🔀 **Reranking**             | `/v1/reclassificar` para pontuação de relevância                                                                                                                                  |
| 🔍 **Pesquisa na Web** 🆕     | `/v1/busca` — 5 provedores (Serper, Brave, Perplexity, Exa, Tavily), 6.500+ gratuito/mês, falha-suficiente automática, cache                                                      |

### 🛡️ Resiliência, Segurança & Governança

| Característica                           | O que ela faz                                                                          |
| ---------------------------------------- | -------------------------------------------------------------------------------------- |
| 🔌 **Circuitos de quebra**                | Recuperação/tríplice comum por faixa de controle                                       |
| 🎯 **Modelos cientes do final**           | Custom models declare supported endpoints + API format                                 |
| 🛡️ **Anti-Thundering Herd**              | Mutex + semaphore protections on retry/rate events                                     |
| 🧠 **Semantic + Signature Cache**         | Cost/latency reduction with two cache layers                                           |
| ⚡ **Request Idempotency**                | Duplicate protection window                                                            |
| 🔒 **TLS Fingerprint Spoofing**           | Browser-like TLS fingerprint — **reduces bot detection and account flagging**          |
| 🔏 **CLI Fingerprint de Correspondência** | Matches native CLI request signatures — **reduces ban risk while preserving proxy IP** |
| 🌐 **IP Filtering**                       | Allowlist/blocklist control for exposed deployments                                    |
| 📊 **Editable Rate Limits**               | Configurable global/provider-level limits with persistence                             |
| 🔑 **API Key Management + Scoping**       | Secure key issuance/rotation and model/provider controls                               |
| 🛡️ **Protected `/models`**               | Optional auth gating and provider hiding for model catalog                             |

### 📊 Observability & Analytics

| Característica                              | O que ela faz                                                               |
| ------------------------------------------- | --------------------------------------------------------------------------- |
| 📝 Solicite + Registo Proxie**               | Registo completo de requisição/resposta e registo de proxy                  |
| 📋 Painel de Dados de Registros Unificados** | Visualização de requisições, proxy, auditoria e console em uma única página |
| 🔍 **Análise de Requisições**                | Latência e rastreamento de requisições (p50/p95/p99)                        |
| 🏥 Painel de Status de Saúde**               | Uptime, estados de quebra, ocorrências de bloqueio, estatísticas de cache   |
| 💰 Seguimento de Despesas**                  | Controle de orçamento e visibilidade de preços por modelo                   |
| 📈 Visualização de Dados de Análise**        | Insights de uso de modelo/provedor e visualização de tendências             |
| 🧪 **Estrutura de Avaliação**                | Uso do conjunto-gold com estratégias de alinhamento configuráveis           |

### ☁️ Implantação e Plataforma

| Característica                         | O que ela faz                                                                          |
| -------------------------------------- | -------------------------------------------------------------------------------------- |
| 🌐 **Implanta Em Qualquer Lugar**       | Localhost, VPS, Docker, Ambientes do Nuvem                                             |
| 💾 **Sincronização de nuvem**           | Sincronização de configuração por meio de trabalhador de nuvem                         |
| 🔄 **Backup/Restore**                   | Fluxos de exportação/importação e recuperação de desastres                             |
| 🧙 **Máquina Onboarding**               | Configuração orientada por usário da instância                                         |
| 🔧 **Painel de console CLI**            | Configuração em um clique para ferramentas de programação populares                    |
| 🎮 **Lembrança de Modelo Playground**   | Testar qualquer provedor/modelo/ponto final do dashboard                               |
| 🔏 **Alternar impressão digital CLI**   | Compatilhamento de impressão digital de provedor por meio de Configurações > Segurança |
| 🌐 **i18n (30 idiomas)**                | Suporte completo a idiomas do dashboard + docs, com cobertura RTL                      |
| 🧹 **Limpar todos modelos**             | Limpar em um clique a lista de modelos na detalhe do provedor                          |
| 📋 **Modelos de_issues**                | Modelos padrão de GitHub para bugs e recursos                                          |
| 📂 **Diretório de dados personalizado** | [Diretório de dados`]DATA_DIR` para sobrescrita de localização de armazenamento        |

### Profundidade de Recursos

#### Fallback inteligente com controle de custo prático

```txt
Combo: "minha-pilha-de-codificação"
  1. cc/claude-opus-4-6
  2. nvidia/llama-3.3-70b
  3. glm/glm-4.7
  4. if/kimi-k2-thinking
```

Quando a quota, a tarifa ou a saúde falham, o OmniRoute muda automaticamente
para o próximo candidato sem necessidade de interrupção manual.

#### Gerenciamento de protocolos visível e operável

- MCP + A2A são descobertos na interface e nos documentos (não são ocultados)
- APIs de status de protocolo expõem dados operacionais ao vivo (`/api/mcp/*`,
  `/api/a2a/*`)
- Painéis de controle incluem ações para o dia 2 (combinar alternativas,
  reiniciar os quebradores, cancelar tarefas)

#### Fluente de Tradução + validação

A área de Tradução inclui:

- **Brincadeira**: verificações de transformação com pedido
- **Testador de Chat**: rota de pedido/desresposta completa
- **Bancada de Testes**: casos múltiplos em uma execução
- **Monitor em Tempo Real**: visualização de tráfego em tempo real

Adiciona a validação de protocolos com clientes reais via `npm run Test:
protocolos:e2e`.

> 📖 **[README Servidor MCP](open-sse/mcp-server/README.md)** — Referência de
> ferramenta, configurações do IDE e exemplos de clientes
> 
> 📖 **[README Servidor A2A](src/lib/a2a/README.md)** — Habilidades, métodos
> JSON-RPC, streaming e gerenciamento de tarefas

## 🧪 Avaliações (Evals)

O OmniRoute inclui um conjunto de ferramentas de avaliação para testar a
qualidade da resposta do LLM contra um conjunto de ouro. Acesse-o via
**Analytics → Evals** no dashboard.

### Conjunto Golden pré-carregado

O pre-armazenado "OmniRoute Golden Set" conterá casos de teste para:

- Bem-vindas, matemática, geografia, geração de código
- Conformidade JSON, tradução, geração de markdown
- Recusa de segurança (conteúdo prejudicial), contagem, lógica booleana

### Estratégias de Avaliação

| Estratégia          | Descrição                                                | Exemplo                              |
| ------------------- | -------------------------------------------------------- | ------------------------------------ |
| `exat`              | O saída deve coincidir exatamente                        | `"4"`                                |
| `conti`             | O saída deve conter substring (case-insensitive)         | `"Paris"`                            |
| `expressão regular` | A saída deve coincidir com o padrão de expressão regular | `"1.*2.*3"`                          |
| `personalizado`     | Função JS personalizada retorna true/false               | `(saída) =&gt; saída.length &gt; 10` |

---

## 📖 Guia de Configuração

### Configuração de Protocolo (MCP + A2A)

<details>
<summary><b>🧩 MCP Setup (Model Context Protocol)</b></summary>

Inicie o transporte do MCP em modo estádio:

```bash
omniroute --mcp
```

Fluxo de validação recomendado:

1. Conecte seu cliente de MCP por stdio.
2. Execute `omniroute_get_health`.
3. Execute `omniroute_list_combos`.
4. Acesse `/ Painel de Controle /mcp` para confirmar heartbeat, atividade e
   auditoria.

APIs úteis para automação:

- `GET /api/mcp/status`
- `GET /api/mcp/tools`
- `GET /api/mcp/audit`
- `GET /api/mcp/audit/stats`

</details>

<details>
<summary><b>🤝 A2A Setup (Agent2Agent)</b></summary>

Descubra o agente:

```bash
curl http://localhost:20128/.well-known/agent.json
```

Envie uma tarefa:

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"setup-a2a","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"Resumo do status de quota."}]}}'
```

Gerencie a vida ciclo:

- `GET /api/a2a/status`
- `GET /api/a2a/tarefas`
- `GET /api/a2a/tarefas/:id`
- `POST /api/a2a/tarefas/:id/cancelar`

Interface de Estado Operacional:

- `/painel de controle/a2a` para observabilidade e ações de fumaça de
  tarefa/estado/fluxo

</details>

<details>
<summary><b>🧪 End-to-end protocol validation</b></summary>

Verifique tanto os protocolos quanto clientes reais:

```bash
npm run test:protocolos:e2e
```

Isso verifica:

- Cliente do MCP conecte/liste/chame
- Descubra A2A e envie/mantenha em fluxo/cancele
- Recupere dados em audit MCP e API de gestão de tarefas A2A

</details>

<details>
<summary><b>💳 Subscription Providers</b></summary>

### Claude Code (Pro/Max)

```bash
Painel → Fornecedores → Conecte Claude Code
→ Login de OAuth → Recarregamento automático de token
→ Contagem de quota de 5 horas e semanas

Modelos:
  cc/claude-ópus-4-6
  cc/claude-soneto-4-5-20250929
  cc/claude-haikai-4-5-20251001
```

**Dica Pro**: Use Ópus para tarefas complexas, Soneto para velocidade. OmniRoute
acompanha a quota por modelo!

### OpenAI Codex (Plus/Pro)

```bash
Painel → Fornecedores → Conecte Codex
→ Login de OAuth (porta 1455)
→ Resetação semanal e de 5 horas

Modelos:
  cx/gpt-5.2-codex
  cx/gpt-5.1-codex-max
```

#### Gerenciamento de Limites do Conta do Codex (5h + Semanal)

Agora cada conta do Codex tem opções de política nos `Painel → Fornecedores`:

- `5h` (LIGADO/DISPOSIÇÃO): force o limite de janela de 5 horas\
  ==WEBLATE_PART==
- `Semanal` (LIGADO/DISPONÍVEL): impor aplicar a política de janela de prazo
  semanal.
- Comportamento do limiar: quando uma janela habilitada atinge >=90% de uso, o
  respectivo conta é pulada.
- Comportamento de rotação: o OmniRoute redireciona para a próxima conta do
  Codex elegível automaticamente.
- Comportamento de reset: quando passa o tempo de `resetAt` definido pelo
  provedor, a conta torna-se elegível novamente automaticamente.

Cenários:

- `5h LIGADO` + `Semanal LIGADO`: a conta é pulada quando qualquer janela atinge
  o limiar.
- `5h DESLIGADO` + `Semanal LIGADO`: apenas o uso semanal pode bloquear a conta.
- `5h LIGADO` + `Semanal DESLIGADO`: apenas o uso de 5 horass pode bloquear a
  conta.
- `resetAt` passou: a conta reingressa na rotação automaticamente (não há
  necessidade de reativação manual).

### CLI de Gemini (GRÁTIS 180K/mês!)

```bash
Painel → Provedores → Conectar CLI de Gemini
→ Google OAuth
→ 180K conclusões/mês + 1K/dia

Modelos:
  gc/gemini-3-preview
  gc/gemini-2.5-pro
```

**Melhor Valor:** Tirão de gratuído! Use antes dos níveis paga.

### GitHub Copilot

```bash
Painel → Provedores → Conectar GitHub
→ OAuth via GitHub
→ Reinicialização mensal (1º dia do mês)

Modelos:
  gh/gpt-5
  gh/claude-4.5-sonnet
  gh/gemini-3-pro
```

</details>

<details>
<summary><b>🔑 API Key Providers</b></summary>

### NVIDIA NIM (ACESSO DE DVLPR GRÁTIS — 70+ modelos)

1. Cadastre-se: [build.nvidia.com](https://build.nvidia.com)
2. Obtenha a chave de API gratuita (1000 créditos de inferência incluídos)
3. Painel → Adicionar Provedor → NVIDIA NIM:
   - Chave de API: `nvapi-suasa-chave`

**Modelos:** `nvidia/llama-3.3-70b-instruct`, `nvidia/mistral-7b-instruct` e
mais 50+\
\
Observações:\
- As strings em inglês foram preservadas.\
- O uso de "Semanal" ao invés de "Semanal" segue a sugestão de mantener a
terminologia consistente.\
- A substituição de "Completions" por "conclusões" também seguiu a sugestão de
manter a terminologia consistente.

**Dica Prática:** API compatível com OpenAI — funciona seamless com a tradução
do formato da OmniRoute!

### DeepSeek

1. Cadastre-se: [platform.deepseek.com](https://platform.deepseek.com)
2. Obtenha a chave API
3. Painel → Adicionar Fornecedor → DeepSeek

**Modelos:** `deepseek/deepseek-chat`, `deepseek/deepseek-coder`

### Groq (Disponível na Camada Gratuito!)

1. Cadastre-se: [console.groq.com](https://console.groq.com)
2. Obtenha a chave API (incluída na camada gratuita)
3. Painel → Adicionar Fornecedor → Groq

**Modelos:** `groq/llama-3.3-70b`, `groq/mixtral-8x7b`

**Dica Prática:** Inferência ultra-rápida — melhor para codificação em tempo
real!

### OpenRouter (100+ Modelos)

1. Cadastre-se: [openrouter.ai](https://openrouter.ai)
2. Obtenha a chave API
3. Painel → Adicionar Fornecedor → OpenRouter

**Modelos:** Acesse 100+ modelos de todos os principais provedores por meio de
uma única chave API.

</details>

<details>
<summary><b>💰 Cheap Providers (Backup)</b></summary>

### GLM-4.7 (Reseta diário, $0.6/1M)

1. Cadastre-se: [Zhipu AI](https://open.bigmodel.cn/)
2. Obtenha a chave API do Plano de Código
3. Painel de Controle → Adicionar Chave API:
   - Fornecedor: `glm`
   - Chave API: `suachave`

**Use:** `glm/glm-4.7`

**Dica Pro:** O Plano de Código oferece 3× quota por 1/7 do custo! Reinicialize
diariamente às 10:00 AM.

### MiniMax M2.1 (reset a cada 5h, $0,20/1M)

1. Matricule-se: [MiniMax](https://www.minimax.io/)
2. Obtenha a chave API
3. Painel de Controle → Adicionar Chave API

**Use:** `minimax/MiniMax-M2.1`

**Dica Pro:** Opção mais barata para contexto longo (1M tokens)!

### Kimi K2 ($9/mês fixo)

1. Se subscreva: [Moonshot AI](https://platform.moonshot.ai/)
2. Obtenha a chave API
3. Painel de Controle → Adicionar Chave API

**Use:** `kimi/kimi-latest`

**Dica Pro:** Cobrança fixa de $9/mês por 10M tokens = $0,90/1M de custo
efetivo!

</details>

<details>
<summary><b>🆓 FREE Providers (Emergency Backup)</b></summary>

### iFlow (5 modelos gratuitos via OAuth)

```bash
Painel de Controle → Conectar iFlow
→ iFlow OAuth login
→ Uso ilimitado

Modelos:
  if/kimi-k2-thinking
  if/qwen3-coder-plus
  if/glm-4.7
  if/minimax-m2
  if/deepseek-r1
```

### Qwen (4 modelos grátis via Código de Dispositivo)

```bash
Dashboard → Conectar Qwen
→ Autorização de código do dispositivo
→ Uso ilimitado

Modelos:
  qw/qwen3-coder-plus
  qw/qwen3-coder-flash
```

### Kiro (Claude FREE)

```bash
Dashboard → Conectar Kiro
→ AWS Builder ID ou Google/GitHub
→ Uso ilimitado

Modelos:
  kr/claude-sonnet-4.5
  kr/claude-haiku-4.5
```

</details>

<details>
<summary><b>🎨 Create Combos</b></summary>

### Exemplo 1: Maximize Subscription → Cópia de Segurança Barata

```
Dashboard → Combos → Criar Novo

Nome: desempenho-de-código
Modelos:
  1. cc/claude-opus-4-6 (Princial de assinatura)
  2. glm/glm-4.7 (Cópia de segurança barata, $0,6/1M)
  3. minimax/MiniMax-M2.1 (Fallback mais barato, $0,20/1M)

Use em CLI: desempenho-de-código
```

### Exemplo 2: Livre-Sozinho (Sem Custo)

```
Nome: free-combo
Modelos:
  1. gc/gemini-3-flash-preview (180K livre/mês)
  2. if/kimi-k2-thinking (ilimitado)
  3. qw/qwen3-coder-plus (ilimitado)

Custo: $0 para sempre!
```

</details>

<details>
<summary><b>🔧 CLI Integration</b></summary>

### Cursor IDE

```
Configurações → Models → Avançado:
  URL base da API do OpenAI: http://localhost:20128/v1
  Chave da API do OpenAI: [da interface do usuário do OmniRoute]
  Modelo: cc/claude-opus-4-6
```

### Claude Code

Usar a página de ferramentas CLI no painel de controle para uma configuração em
um clique, ou editar [~/.claude/settings.json] MANUALMENTE.

### Codex CLI

```bash
export OPENAI_BASE_URL="http://localhost:20128"
export OPENAI_API_KEY="sua-omniroute-api-key"

codex "sua prompt"
```

### OpenClaw

[Opção 1 — Painel de Controle (recomendado ):

```
Painel de Controle → Ferramentas CLI → OpenClaw → Selecionar Modelo → Aplicar
```

[Opção 2 — Manual:[Editar [~/.openclaw/openclaw.json]:

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

> [Nota: Abra um terminal para começar com OpenClaw. Utilize 127.0.0.1 em vez de
> localhost para evitar problemas de resolução de endereços IPv6.

### Cline / Continuar / RooCode

```
Configurações → Configuração da API:
  Fornece do provider: OpenAI Compatible
  URL Base: http://localhost:20128/v1
  Chave da API: [a partir da dashboard do OmniRoute]
  Modelo: if/kimi-k2-pensamento
```

### OpenCode

**Etapa 1:** Adicione o OmniRoute como provedor personalizado:

```bash
opencode
/connect
# Selecione "Outro" → Insira ID: "omniroute" → Insira a chave da API do OmniRoute
```

**Etapa 2:** Crie/edit `archivo de configuracao opencode.json` em sua raiz do
projeto:

```json
{
  "$schema": "https://opencode.ai/config.json",
  "provider": {
    "omniroute": {
      "npm": "@ai-sdk/openai-compatible",
      "nome": "OmniRoute",
      "options": {
        "baseURL": "http://localhost:20128/v1"
      },
      "models": {
        "cc/claude-sonnet-4-20250514": { "nome": "Claude Sonnet 4" },
        "gg/gemini-2.5-pro": { "nome": "Gemini 2.5 Pro" },
        "if/kimi-k2-pensamento": { "nome": "Kimi K2 (Gratuito)" }
      }
    }
  }
}
```

**Etapa 3:** Selecione o modelo no OpenCode:

```bash
/models
# Selecione qualquer modelo do OmniRoute da lista
```

> **Dica:** Adicione qualquer modelo disponível em seu endpoint OmniRoute
> `/v1/models` à seção `models`. Use o formato `provider/model-id` do seu
> dashboard do OmniRoute.

</details>

---

## Solução de Problemas

<details>
<summary><b>Click to expand troubleshooting guide</b></summary>

**"O modelo de linguagem não forneceu mensagens"**

- O quota do provedor foi esgotado → Verifique o rastreador de quota da
  dashboard
- solução: use fallback combinado ou mude para tier mais barato

**Limitação de taxa**

- Quota da assinatura excedida → Fallback para GLM/MiniMax
- Adicione combo: `cc/claude-opus-4-6 → glm/glm-4.7 → if/kimi-k2-pensamento`

**"Token OAuth expirou"**

- Atualizado automaticamente pelo OmniRoute
- Se os problemas persistirem: Dashboard → Provedor → Reconectar

**Custos altos**

- Consultar estatísticas de uso no Painel → Custos
- Mudar modelo principal para GLM/MiniMax
- Usar faixa gratuita (Gemini CLI, iFlow) para tarefas não críticas

**Painel/Dashboard/API ports estão errados**

- `PORT` é o portal de base canônico (e porta de API por padrão)
- `API_PORT` sobrescreve apenas ouvinte de API compatível com OpenAI
- `DASHBOARD_PORT` sobrescreve apenas ouvinte do painel/Next.js
- Defina `NEXT_PUBLIC_BASE_URL` para sua URL públic de dashboard/public (para
  callbacks de OAuth)

**Erros de sincronização da nuvem**

- Verifique se `BASE_URL` está apontando para sua instância em execução
- Verifique se `CLOUD_URL` está apontando para seu endpoint de nuvem esperado
- Mantenha `NEXT_PUBLIC_*` valores alinhados com valores do lado do servidor

**Primeiro login não está funcionando**

- Verifique `INITIAL_PASSWORD` em `.env`
- Se não estiver configurado, o senha padrão é `123456`

**Ainda não há logs de requisições**

- Defina `ENABLE_REQUEST_LOGS=true` em `.env`

**O teste de conexão mostra "Inválido" para provedores compatíveis com OpenAI**

- Muitos provedores não expõem o `/models` endpoint
- A versão do OmniRoute 1.0.6+ inclui uma validação por meio de completos de
  chat
- Insira o URL base com o sufixo `/v1`

### Autenticação OAuth em um Servidor Remoto

<a name="oauth-on-a-remote-server"></a> <a name="oauth-em-servidor-remoto"></a>

> **⚠️ Importante para usuários que executam o OmniRoute em um VPS, Docker ou
> qualquer servidor remoto**

#### Por que a autenticação OAuth da / Antigravity / CLI CLI Gemini falha em servidores remotos?

O **Antigravity** e o **Gemini CLI** provider usam o **OAuth 2.0 Google**. O
Google exige que o `redirect_uri` no fluxo de autenticação precise ser
exatamente igual a uma das URIs registradas em prévias em console do aplicativo
da Google Cloud.

As credenciais OAuth embutidas no OmniRoute são registradas ** somente para
`localhost` **. Quando você acessa o OmniRoute em um servidor remoto (por
exemplo, ` https://omniroute.myserver.com `), Google rejeita a autenticação com:

```
Erro 400: redirect_uri_mismatch
```

#### Solução: Configure suas próprias credenciais OAuth

Você precisa criar um **ID de cliente OAuth 2.0 ** no console do Google Cloud
com o URI do seu servidor.

#### Passo a passo

**1. Abra o Console do Google Cloud **

Vá para:
[https://console.cloud.google.com/apis/credentials](https://console.cloud.google.com/apis/credentials)

**2. Crie um novo ID de cliente OAuth 2.0 **

- Clique em **"+ Criar credenciais"** → **"ID do cliente OAuth"**
- Tipo de aplicação: **"Aplicativo web"**
- Nome: qualquer coisa que você goste (por exemplo, ` OmniRoute Remoto `)

**3. Adicione URIs de redirecionamento autorizadas **

Na **"URIs de redirecionamento autorizadas"** clique em adicionar:

```
https://seu-servidor.com/callback
```

> Substitua `seu-servidor.com` pelo domínio ou IP do seu servidor (inclua o
> porta se necessário, por exemplo, `http://45.33.32.156:20128/callback`).

**4. Salve e copie as credenciais**

Após criar, o Google exibirá o **ID do cliente** e o **segredo do cliente**.

**5. Defina variáveis de ambiente**

Em seu `.env` (ou variáveis de ambiente do Docker):

```bash
# Para Antigravity:
ANTIGRAVITY_OAUTH_CLIENT_ID=seu-cliente-id.apps.googleusercontent.com
ANTIGRAVITY_OAUTH_CLIENT_SECRET=GOCSPX-seu-senha
# Para Gemini CLI:
GEMINI_OAUTH_CLIENT_ID=seu-cliente-id.apps.googleusercontent.com
GEMINI_OAUTH_CLIENT_SECRET=GOCSPX-seu-senha
GEMINI_CLI_OAUTH_CLIENT_SECRET=GOCSPX-seu-senha
```

**6. Reinicie a OmniRoute**

```bash
# npm:
npm run dev

# Docker:
docker restart omniroute
```

**7. Tente conectar novamente**

Painel de controle → Provedores → Antigravity (ou Gemini CLI) → OAuth

Agora o Google redirecionará corretamente para
`https://seu-server.com/callback`.

---

#### Trabalho temporário (sem credenciais personalizadas)

Se você não quiser configurar suas próprias credenciais agora, ainda pode usar o
**fluxo de URL manual**:

1. A OmniRoute abre a URL de autorização do Google
2. Após autorizar, o Google tenta redirecionar para `localhost` (que falha no
   servidor remoto)
3. **Copeie a URL completa** do endereço de sua barra de endereços do navegador
   (mesmo se a página não carregar)
4. Coloque essa URL na caixa mostrada no modal de conexão da OmniRoute
5. Clique em **"Conectar"**

> Isso funciona porque o código de autorização na URL é válido,
> independentemente de a página de redirecionamento carregar.

---

<details>
<summary><b>🇧🇷 Versão em Português</b></summary>

#### Por que o OAuth do Antigravity / Gemini CLI falha em servidores remotos?

Os provedores **Antigravity** e **Gemini CLI** usam **OAuth 2.0 do Google** para
autenticação. O Google exige que a `URI de redirecionamento` usada no fluxo
OAuth seja **exatamente** uma das URIs pré-cadastradas no Google Cloud Console
do aplicativo.

As credenciais OAuth embutidas no OmniRoute estão cadastradas **apenas para
`localhost`**. Quando você acessa o OmniRoute em um servidor remoto (ex:
`https://omniroute.meuservidor.com`), o Google rejeita a autenticação com:

```
Erro 400: redirect_uri_mismatch
```

#### Solução: Configure suas próprias credenciais OAuth

Você precisa criar um **OAuth 2.0 Client ID** no Google Cloud Console com a URI
do seu servidor.

#### Passo a passo

**1. Acesse o Google Cloud Console**

Abra:
[https://console.cloud.google.com/apis/credentials](https://console.cloud.google.com/apis/credentials)

**2. Crie um novo OAuth 2.0 Client ID**

- Clique em **"+ Criar credenciais"** → **"OAuth client ID"**
- Tipo de aplicativo: **"Aplicação web"**
- Nome: escolha qualquer nome (ex: `OmniRoute Remoto`)

**3. Adicione as URLs de redirecionamento autorizadas**

No campo **"URLs de redirecionamento autorizadas"**, adicione:

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

**6. Reinicie o OmniRoute**

```bash
# Se usando npm:
npm run dev

# Se usando Docker:
docker restart omniroute
```

**7. Tente conectar novamente**

Painel → Fornecedores → Antigravidade (ou CLI do Gemini) → OAuth

Agora o Google redirecionará corretamente para
`https://seu-servidor.com/callback` e a autenticação funcionará.

---

#### Workaround temporário (sem configurar credenciais próprias)

Se não quiser criar credenciais próprias agora, ainda é possível usar o fluxo
**manual de URL**:

1. O OmniRoute abrirá a URL de autorização do Google
2. Após você autorizar, o Google tentará redirecionar para `localhost` (que
   falha no servidor remoto)
3. **Copie a URL completa** da barra de endereço do seu navegador (mesmo que a
   página não carregar)
4. Cole essa URL no campo que aparece no modal de conexão do OmniRoute
5. Clique em **"Conectar"**

> Este workaround funciona porque o código de autorização na URL é válido,
> independentemente do redirecionamento ter carregado ou não.

</details>

---

</details>

## 🛠️ Stack Técnico

<details>
<summary><b>Click to expand tech stack details</b></summary>

- **Runtime**: Node.js 18-22 LTS (⚠️ Node.js 24+ não é **suportado** — `binários
  nativos de melhor-biblioteca-sqlite3[] são incompatíveis)
- **Idioma**: TypeScript 5.9 — **100% de TypeScript** ao longo de `src/` e
  `open-sse/` (zero `any` em módulos de kernel desde a v2.0)
- **Framework**: Next.js 16 + React 19 + Tailwind CSS 4
- **Banco de dados**: LowDB (JSON) + SQLite (estado do domínio + registros do
  proxy + auditorias do MCP + decisões de roteamento)
- **Especificadores de esquema**: Zod (tool de validação de I/O do MCP,
  contratos de API)
- **Protocolos**: MCP (stdio/HTTP) + A2A v0.3 (JSON-RPC 2.0 + SSE)
- **Streaming**: Transmissão: Evensts Servidor-Side (ESS)
- **Auth**: Autenticação: OAuth 2.0 (PKCE) + JWT + Chaves de API + Autorização
  do Escopo do MCP
- **Testing**: Testes Node.js + Vitest (900+) testes, incluindo unidades,
  integração e E2E
- **CI/CD**: GitHub Actions (publicação automática do npm + Docker Hub no
  lançamento)
- **Site:** [omniroute.online](https://omniroute.online)
- **Package**:
  [npmjs.com/package/omniroute](https://www.npmjs.com/package/omniroute)
- **Docker**:
  [hub.docker.com/r/diegosouzapw/omniroute](https://hub.docker.com/r/diegosouzapw/omniroute)
- **Resilience**: Circuito de interrupção, atrasos exponenciais, anti-choque de
  manada, forjamento de TLS, auto-combo de auto-cura

</details>

---

## Documentação

| Documenta                                              | Descrição                                                                  |
| ------------------------------------------------------ | -------------------------------------------------------------------------- |
| [Guia do Usuário](docs/USER_GUIDE.md)                  | Provedores, combinações, integração CLI, implantação                       |
| [Referência da API](docs/API_REFERENCE.md)             | Todos os pontos de extremidade com exemplos                                |
| [MCP Server](open-sse/mcp-server/README.md)            | 16 ferramentas de MCP, configurações do IDE, clientes do Python/TS/Go      |
| [A2A Server](src/lib/a2a/README.md)                    | Protocolo JSON-RPC 2.0, habilidades, transmissão, gerenciamento de tarefas |
| [Motor do Auto-Combo](docs/auto-combo.md)              | Classificação por 6 fatores, pacotes de modo, auto-conjunto                |
| [Troubleshooting](docs/TROUBLESHOOTING.md)             | Problemas comuns e soluções                                                |
| [Arquitetura](docs/ARCHITECTURE.md)                    | Arquitetura do sistema e internos                                          |
| [Contribuindo](CONTRIBUTING.md)                        | Configuração de desenvolvimento e diretrizes                               |
| [OpenAPI Spec](docs/openapi.yaml)                      | Especificação da abertura da API 3.0                                       |
| [Política de Segurança](SECURITY.md)                   | Relatório de vulnerabilidade e práticas de segurança                       |
| [Despacho VM](docs/VM_DEPLOYMENT_GUIDE.md)             | Guia completo: VM + nginx + Cloudflare setup                               |
| [Galpão de recursos](docs/FEATURES.md)                 | Turismo de dashboard visual com capturas de tela                           |
| [Verificação de lançamento](docs/RELEASE_CHECKLIST.md) | Passos de validação pré-lançamento                                         |

---

## 🗺️ Plano de ação

OmniRoute tem **210+ recursos planejados** em várias fases desenvolvimentistas.
Aqui estão as principais áreas:

| Categoria                        | Funcionalidades Planejadas | Destaque                                                                                                                             |
| -------------------------------- | -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| 🧠  ** Rotas & Inteligência**     | 25+                        | Rotas com baixa latência, rotas com base em tag, verificação de quota antes, seleção de conta P2C                                    |
| 🔒 ** Segurança & Compliance**    | 20+                        | Reforço contra SSRF, ocultação de credenciais, limite de taxa por ponto final, escopo de chave de gerenciamento                      |
| 📊 ** Observabilidade**           | 15+                        | Integração com OpenTelemetry, monitoramento de quota em tempo real, rastreio de custo por modelo                                     |
| 🔄 ** Integrações de Fornecedor** | 20+                        | Cadastro dinâmico de modelo, embotecimento de cooldown do provedor, quota de múltiplas contas do Codex, extração de quota do Copilot |
| ⚡ ** Performance**               | 15+                        | Camada de cache dupla, cache de solicitação, cache de resposta, keepalive de streaming, batches de API                               |
| 🌐 ** Ecosistema**                | 10+                        | API WebSocket, recarga de configuração quente, armazenamento de configuração distribuído, modo comercial                             |

### Em Breve

- 🔗 ** Integração OpenCode** — Suporte nativo do provedor para o IDE de
  codificação de código aberto AI
- 🔗 **INTEGRAÇÃO TRAE** — Suporte completo para o framework de desenvolvimento
  da IA TRAE
- 📦 **API em Lote** — Processamento em lote assíncrono para solicitações em
  massa
- 🎯 **Roteamento com Base em Marcação** — Roteie solicitações com base em marcas
  e metadados personalizados
- 💰 [X2X)Estratégia de Custo mais Baixo** — Selecione automáticamente o provedor
  mais barato disponível

> 📝 Especificações de recursos disponíveis em
> [`docs/novaes-especificações/`](docs/new-features/) (217 especificações
> detalhadas)

---

## 👥 Contribuintes

[![Contribuintes](https://contrib.rocks/image?repo=diegosouzapw/OmniRoute&max=100&columns=20&anon=1)](https://github.com/diegosouzapw/OmniRoute/graphs/contributors)

### Como Contribuir

1. Fork o repositório
2. Crie seu branch de recursos (`git checkout -b recursos/lindo recurso`)
3. Comите alterações (`git commit -m 'Adicione recurso lindo'`)
4. Empurre para o branch (`git push origin recursos/lindo recurso`)
5. Abra uma Solicitação de Pull

Consulte [CONTRIBUTING.md](CONTRIBUTING.md) para diretrizes detalhadas

### Liberação de Uma Nova Versão

```bash
# Crie uma liberação — o npm publish acontece automaticamente
gh release create v2.0.0 --title "v2.0.0" --generate-notes
```

---

## 📊 Histórico de Estrelas

## Estrelas por tempo

## [![Estrelas por tempo](https://starchart.cc/diegosouzapw/OmniRoute.svg?variant=adaptive)](https://starchart.cc/diegosouzapw/OmniRoute)

## 🙏 Agradecimentos

Agradecimentos especiais a
**[CLIProxyAPI](https://github.com/decolua/9router)[X36X] — a implementação
original em Go que inspirou essa versão em JavaScript.

Agradecimentos especiais a
**[X0X](https://github.com/router-for-me/CLIProxyAPI)[X32X] por
[X38X][decolua]{2}[X52X] — o projeto original que inspirou essa bifurcação. O
OmniRoute Constrói-se sobre essa excelente base, com características adicionais,
APIs multimodais e uma reescrita completa em TypeScript.

---

## 📄 Licença

Licença MIT — consulte [LICENSE](LICENSE) para obter detalhes.

---

<div align="center">
  <sub>Built with ❤️ for developers who code 24/7</sub>
  <br/>
  <sub><a href="https://omniroute.online">omniroute.online</a></sub>
</div>
<!-- GitHub Discussions enabled for community Q&A -->
