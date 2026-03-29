# 🚀 OmniRoute — AI Brána Zdarma

### Nikdy nepřestávejte kódovat. Inteligentní směrování k **ZDARMA a nízkonákladovým AI modelům** s automatickým přepnutím.

_Váš univerzální API proxy — jeden endpoint, 67+ poskytovatelů, žádné výpadky.
Nyní s **MCP & A2A** orchestrací agentů._

**Dokončování Chatu • Vkládání • Generování Obrázků • Video • Hudba • Audio •
Přeřazování • **Hledání na Webu** • MCP Server • A2A Protokol • 100%
TypeScript**

---

<div align="center">

[![verze
npm](https://img.shields.io/npm/v/omniroute?color=cb3837&logo=npm)](https://www.npmjs.com/package/omniroute)
[![npm
stahování](https://img.shields.io/npm/dm/omniroute?color=cb3837&logo=npm&label=npm%20downloads)](https://www.npmjs.com/package/omniroute)
[![Docker
Hub](https://img.shields.io/docker/v/diegosouzapw/omniroute?label=Docker%20Hub&logo=docker&color=2496ED)](https://hub.docker.com/r/diegosouzapw/omniroute)
[![Docker
Pulls](https://img.shields.io/docker/pulls/diegosouzapw/omniroute?logo=docker&color=2496ED&label=docker%20pulls)](https://hub.docker.com/r/diegosouzapw/omniroute)
[![Licence](https://img.shields.io/github/license/diegosouzapw/OmniRoute)](https://github.com/diegosouzapw/OmniRoute/blob/main/LICENSE)
[![Web](https://img.shields.io/badge/Website-omniroute.online-blue?logo=google-chrome&logoColor=white)](https://omniroute.online)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-Community-25D366?logo=whatsapp&logoColor=white)]{14]

[🌐 Web](https://omniroute.online) • [🚀 Rychlý start](#-quick-start) • [💡
Funkce](#-key-features) • [📖 Dokumentace](#-documentation) • [💰
Ceník](#-pricing-at-a-glance) • [💬
WhatsApp](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

</div>

🌐 **K dispozici v:** 🇺🇸 [English](README.md) | 🇧🇷 [Português
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

## Nedávná poznámka: Zásady limitů pro účty Codex

> **Upgradujete z v2.9.5?** — Prohlédněte si [plný
> CHANGELOG](CHANGELOG.md#300--2026-03-22-release-candidate--not-yet-merged-to-main)
> pro všechny změny.

| Oblast                                        | Změnit                                                                                                                                                                                                |
| --------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🔒 **KódQL bezpečnost**                        | Fixováno 10+ upozornění CodeQL: eliminace polynomických smyček vracejících se zpět, neshromažďování náhodných čísel, odstranění injections shell                                                      |
| ✅ **Ověření trasy**                           | Všech 176 API cest bylo ověřeno pomocí schémat Zod + `ověřitTělo()` — CI `zkontroluje:trasy-očkované:t06` prošel                                                                                      |
| 🐛 **Proťukání oznámení odbavovacího modelu**  | Vnitřní `` značky již neproudí k lidem pomocí SSE toků vstupů/úloh (#585)                                                                                                                             |
| 🔑 **Registrované klíče API**                  | Automatizované zřízení API klíčů prostřednictvím `POST /api/v1/registrované-klíčy` s přiřazený poskytovatelem/účtem_quota užití, jedinečnost, vágnost 256 SHA, a volitelné zápisem do GitHub problému |
| 🎨 **Ikony poskytovatelů**                     | 130+ ikony poskytovatelů prostřednictvím `@lobehub/icons` (SVG) s fallbackem v PNG → řetězu                                                                                                           |
| 🔄 **Synchronizace modelu automatizace**       | 24hodinový plánovač a ruční tlačítko UI pro synchronizaci seznamů modelů pro vstavené a uživatelsky naformátované provizoriálně zpřístupněné                                                          |
| 🌐 **OpenCode Zen/Go**                         | Dvě nové poskytovatele z @kang-heewon skrze PR #530: zdarma + tarifováno prostřednictvím `OpencodeExecutor`                                                                                           |
| 🐛 **Ověřování CLI OAuth pro Gemini**          | Rozsahově k dispozici chybové zpravování, když `GEMINI_OAUTH_CLIENT_SECRET` chybí v Docker (původně kryptické chybové zpravování Google)                                                              |
| 🐛 **Konfigurace OpenCode**                    | `Uložit konfiguraci OpenCode()` nyní správně zapisuje TOML do `XDG_CONFIG_HOME`                                                                                                                       |
| 🐛 **Odstraňování přednastavených modelů=X25X] | `Nastavení modelu těla` bylo správně nastaveno k předem zařazenému `předemNastaveným modelu` na ochranu kontextu-klauzule                                                                             |
| 🐛 **Cyklický/odpovídající Codex/Claude**      | `Nástroj výsledků` bloky nyní konvertovány do textu pro zastavení nekonečných cyklů                                                                                                                   |
| 🐛 **Přihlášení redirekt**                     | Přihlášení už nezdržuje po přeskočení nastavení hesla                                                                                                                                                 |
| 🐛 **Windows cesty**                           | MSYS2/Git-Bash cesty (`/c/...`) normalizovány na `C:\...` automaticky                                                                                                                                 |

---

## 🖼️ Hlavní Panel

<div align="center">
  <img src="./docs/screenshots/MainOmniRoute.png" alt="OmniRoute Dashboard" width="800"/>
</div>

---

## 📸 Předěl Panelu

<details>
<summary><b>Click to see dashboard screenshots</b></summary>

| Stránka                        | Sken                                                             |
| ------------------------------ | ---------------------------------------------------------------- |
| **Dobrovolníci**               | ![Dobrovolníci](docs/screenshots/01-providers.png)               |
| **Kombinace**                  | ![Kombinace](docs/screenshots/02-combos.png)                     |
| **Analytika**                  | ![Analytika](docs/screenshots/03-analytics.png)                  |
| **Zdravotní stav**             | ![Zdravotní stav](docs/screenshots/04-health.png)                |
| **Přeložitel**                 | ![Přeložitel](docs/screenshots/05-translator.png)                |
| **Parametry**                  | ![Nastavení](docs/screenshots/06-settings.png)                   |
| **Nástroje na příkazové řádě** | ![Nástroje na příkazové řádě](docs/screenshots/07-cli-tools.png) |
| **Přihlášení/Xeje Logs**       | ![Použití](docs/screenshots/08-usage.png)                        |
| **Koncové body/Xeje            | ![Koncové body](docs/screenshots/09-endpoint.png)                |

</details>

---

### 🤖 Bezpplatný AI poskytnout vámi oblíbenými agentům kódování

_Pojďte kdekoli s AI-pojitými IDE nebo nástroji na příkazové řádě OmniRoute –
bezplatný brána API pro nekonečné kódování._

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

<sub>📡 Všechny agenti připojují se přes <code>http://localhost:20128/v1</code>
nebo <code>http://cloud.omniroute.online/v1</code> – jedna konfigurace,
nekonečné modely a kvota</sub>

---

## 🤔 Proč OmniRoute?

**Zdržujete peníze a dosahujete limitech:**

- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Závazek na paušál mizí nevyužitý ve druhém měsíci
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Limity omezují další kódování
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Drahé APIS (20-50 měsíčně za vybraného poskytovatele)
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Průběžné přepínání mezi poskytovateli

**OmniRoute vyřeší tento problém:**

- ✅ **Maximální použitá paušála** - Připravenost na kvótu, použití každé hodnoty
  před resetem
- ✅ **Automatické pádnutí** - Paušál -> klíč API -> levá -> bezplatná, nikoli s
  přestávkami
- ✅ **Zapojení více účtů** - Omezování účtů kolem jednoho poskytovatele mezi
  sebou
- ✅ **Univerzální ** - Pracuje se sloučením CLAUDE CODE, CODEX, GEMINI CLI,
  CURSOR, CLINE, OPENCLAW, jakékoli nástroj CLI

---

## 📧 Podpora

> 💬 **Přidejte se do naší komunity!** Chat na WhatsApp [WhatsApp
> Group](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t) - Získejte
> pomoc, sdílejte tipy a zůstaňte v obraze.

- **Webová stránka**: [omniroute.online](https://omniroute.online)
- **GitHub**:
  [github.com/diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute)
- **Issues**:
  [github.com/diegosouzapw/OmniRoute/issues](https://github.com/diegosouzapw/OmniRoute/issues)
- **WhatsApp**: [Komunitní
  skupina](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)
- **O přispívání**: Zkontrolujte [CONTRIBUTING.md](CONTRIBUTING.md), otevřete
  pull request nebo si vyberte `dobrý první úkol`
- **Originální projekt**: [9router od
  decolua](https://github.com/decolua/9router)

### 🐛 Zpracování chyby?

Při otevírání nové Issue, prosím spusťte system-info příkaz a připojte
generovaný soubor:

```bash
npm run system-info
```

To generuje soubor `system-info.txt` s Vaší verzí Node.js, verzí OmniRoute, OS
podrobnostmi, nainstalovanými nástroji CLI (iflow, gemini, claude, codex,
antigravity, droid, atd.), stáním Docker/PM2, systémem balíků — vše potřebné k
zopakování Vaší chyby rychle. Připojte soubor přímo k vaší otevřené-issue na
GitHubu.

---

## Jak to funguje

```
┌─────────────┐
│    Vaše CLI   │  (Claude Code, Codex, Gemini CLI, OpenClaw, Cursor, Cline...)
│  Klient      │
└──────┬──────┘
       │ http://localhost:20128/v1
       ↓
┌─────────────────────────────────────────┐
│          OmniRoute (Smarter Router)        │
│ •  Přeformátování překladů (OpenAI ↔ Claude) │
│ •  Obsluha kvót + Embeddings + Obrázky  │
│ •  Automatické obnovování tokenů       │
└──────┬──────────────────────────────────┘
       │
       ├─→ [Tier 1: PŘESENSTVÍ] Claude Code, Codex, Gemini CLI
       │   ↓ kvota vyčerpána
       ├─→ [Tier 2: Klíč API] DeepSeek, Groq, xAI, Mistral, NVIDIA NIM, atd.
       │   ↓ limit rozpočet
       ├─→ [Tier 3: ÚSPORA] GLM (0,6/1M), miniMax (0,2/1M)
       │   ↓ limit rozpočet
       └─→ [Tier 4: BEZPLATNÉ] iFlow, Qwen, Kiro (neomezené)

Výsledky: nikdy se nezastavujte, minimální náklady
```

---

## 🎯 Jak OmniRoute řeší problémy - 30 reálných problémů a uživatelských případů

> **Každý vývojář, který používá nástroje AI, čelí těchto problémům denně.**
> OmniRoute byl postaven, aby je vyřešil všechny — od nákladů překročení po
> regionální blokování, od porušených OAuth toků po protokolové operace a
> podnikovou sledovací schopnosti.

<details>
<summary><b>💸 1. "I pay for an expensive subscription but still get interrupted by limits"</b></summary>

Vývojáři platí 20-200 Kč/ měsíc za CLAUDE PRO, CODEX PRO nebo GitHub Copilot. I
když platí, kvota má strop — 5h používání, týdenní limity nebo minutologické
limity. Uprostřed kódovacího řetězu poskytovatel přestane reagovat a developer
ztratí proud a produktivitu.

**Jak OmniRoute to řeší:**

- **Smarter 4-Tier Fallback ** - Pokud se vyčerpá předplatné kvota, automaticky
  přesměruje na klíč API → Cheap → Free s nulovou manuální intervencí
- **Reálný časový sled quaot ** - Ukazuje spotřebování tokenů v reálném čase s
  countdownem resetování (5h, každý den, každý týden)
- **Podpora více účtů** - více účtů pro provider s automatickým rotací — když
  jeden vyčerpá, přepne ke druhé\
  ==WEBLATE_PART==
- **Úživatelsky definovatelné kombinace** — Kusovní sklady s 6 strategiemi
  rovnováhy (první naplnění, kolečkové kolo, p2c, náhodné, nejméně používané,
  optimalizace nákladů)
- **Rozsahy_quota Business Codex** — Monitoring pracovních prostoru
  Business/Team přímo na panelu

</details>

<details>
<summary><b>🔌 2. "I need to use multiple providers but each has a different API"</b></summary>

OpenAI používá jednu formát, Claude (Anthropic) jiný, Gemini další. Pokud
vývojář chce ověřit modely z různých dodavatelů nebo přepínat mezi nimi, musí
změní SDKs, úpravy bodů zakočení, zvláštňování nekonzistentních forem. Custom
dodavatelé (FriendLI, NIM) mají nekonzistentní body zakočení modelů.

**Jak OmniRoute to řeší:**

- **Součást proxy[18X] — Jedná se o jeden[32X]http://localhost:20128/v1[58X],
  který slouží jako proxy pro více než 67+ poskytovatelů
- **Rozsahy Překlad Formátu** — Automatický a transparentní: OpenAI ↔ Claude ↔
  Gemini ↔ Zodpovědnost API
- **Ochrana proti mícháním odpovědí** — Odstraňování nekonzistentních polí
  (`x_groq`, `usage_breakdown`, `service_tier`), které porušují OpenAI SDK
  v1.83+
- **Normalizace roli** — Převod uživatelů `developer` → `system` pro ne- OpenAI
  dodavatele; `system` → `user` pro GLM/ERNIE
- **Výběr značky “Think”[22X] — Extrahování `<think>` bloků z modelů, jako je
  DeepSeek R1 do standardizovaných `obsahu racionálního myšlení/X118X</think>
- **Strukturovaný formát pro Gemini** — Převod `json_schema` na
  `responseMimeType`/`responseSchema` automatická konverze
- **`stream` default nastaveni na `false`[30X] — Lze v souladu s OpenAI
  specifikací, eliminuje neočekávanou SSE v Python/Rust/Go SDKs

</details>

<details>
<summary><b>🌐 3. "My AI provider blocks my region/country"</b></summary>

Poskytovatelé, jako je OpenAI/Codex, zablokovávají přístup z určitých
geografických oblastí. Uživatelé dostávají chyby, jako je
`unsupported_country_region_territory`, během procesu OAuth a API připojení. To
je obzvláště obtížné pro vývojáře z rozvojových zemí.

**Jak OmniRoute to řeší:**

- **3 úrovní config proxy[22X] — Konfigurujeme proxy na 3 úrovních: globální
  (všichni provozovatelé), pro jednoho provozovatele (jen jeden provozovatel), a
  pro jednotlivé připojení/klíče
- **Proxy Badges s barevnou kódou** — Visuální indikátory: 🟢 globální proxy, 🟡
  proxy provider, 🔵 spojení s proxy, vždy zobrazuje IP
- **Nastavení tokenu OAuth přes proxy** — Krok OAuth také prochází provyrou,
  vyřeší `unsupported_country_region_territory`
- **Testy připojení pomocí proxy** — Testuje připojení s konfigurovaným proxy
  (žádné více přímé obcházení)
- **Podpora SOCKS5** — Plná podpora SOCKS5 proxy pro routed routing
- **Falešný otisk TLS** — Browser-like TLS otisk via `wreq-js` k obejití detekce
  botů
- **Přepisování otisku CLI oken** — Rotací hlaviček a těla zpráv k odpovídání
  původním nativní CLI binary kódům, významně snižuje riziko zablokování účtu.
  Proxy IP je zachována - máte i obávaný **stealth[a203X] a síle IP mazníku.

</details>

<details>
<summary><b>🆓 4. "I want to use AI for coding but I have no money"</b></summary>

Všichni nemohou platit 20-200$/měsíc za AI předplatné. Studenti, vývojáři z
rozvojových zemí, kutilové a freelanceři potřebují přístup ke kvalitním modelům
zdarma.

**Jak OmniRoute to řeší:**

- **Bezplatní Rozponěvatelé** — Nativní podpora 100% bezplatných poskytovatelů:
  iFlow (5 neomezených modelů přes OAuth: kimi-k2-přemýšlení, qwen3-kódér-plus,
  deepseek-r1, minimax-m2, kimi-k2), Qwen (4 neomezené modely: qwen3-kódér-plus,
  qwen3-kódér-skok, qwen3-kódér-našlápnutí, vizní-model), Kiro (Claude + AWS
  Stavitel ID pro bezplatné) , Gemini CLI (180K tokens/ měsíc bezplatné)
- **Ollama Cloud** — Cloud-hostovaný Ollama modely na `api.ollama.com` s volným
  „lehkým používáním“ úrovni; používaj `ollamacloud/<model>`
  prefiksování</model>
- **Neomezené kombinace bezplatné** — Poklepajte `gc/gemini-3-skok →
  if/kimi-k2-přemýšlení → qw/qwen3-kódér-plus` = 0 Kč/měsíc s nulovým dočasím
  čekání
- **NVIDIA NIM Bezplatné připojení** — ~40 RPM rozvoje-křižovanky zdarma pro 70+
  modelů na build.nvidia.com (přecházíte z kreditů na čisté limity
- **Strategie optimalizace nákladů** — Routing strategie, která automaticky volí
  nejlevnější dostupného poskytovatele

</details>

<details>
<summary><b>🔒 5. "I need to protect my AI gateway from unauthorized access"</b></summary>

Při zpřístupnění AI brány v síti (LAN, VPS, Docker) může kdokoli, kdo zná její
adresu, čerpat tokeny nebo kvótu vývojáře. Bez ochrany jsou API náchylná ke
zneužití, vkládání příkazů a neoprávněnému přístupu.

**Jak OmniRoute to řeší:**

- **Správa API klíč** — Generování obrázků rotace a vymezení rozsahu podle
  poskytovatele s odlišenou `/nástěnka/správa-API[k112X] stránkou
- **Omezení model-prostup** — Omezení API klíč pro specifické modely
  (`openai/*`, šablonové vzory), s Allow All/Restrict přepínač
- **Chránění API koncového bodu** — Požadováno klíče k `/v1/models` a
  zablokování specifických poskytovatelů z obsahu seznamu
- **Chránění pro přihlášení + CSRF ochrana** — Všichni dashboard trasy chráněni
  `s přihlašením` middleware + CSRF tokens
- **Omezení rychlosti** — Omezení rychlosti pro přístup
- **Filtry IP adres** — Omlouvání / blokádaci podle přístupu omezení
- **Ochrana proti injekčním útokům na požadavky** — Ochrana proti nebezpečným
  vzorům žádostí přípravy
- **AES-256-GCM šifrování** — Připevnění údajů v klid

</details>

<details>
<summary><b>🛑 6. "My provider went down and I lost my coding flow"</b></summary>

Poskytovatelé AI se mohou zmást, vrátí 5xx chyby nebo zhoršit dočasná omezení
rychlosti. Pokud se vývojář spoléhá na jediného poskytovatele, jsou vypracovaní.
Bez obvodů vyhozený se smyčkovým způsobem často strhávají aplikaci.

**Jak OmniRoute to řeší:**

- **Automatický obvod pro každý model** — Otvírá/uzavírá s konfigurovatelnými
  zásadami a chlazením (Zastrčeno/Otevřeno/Hálováno), omezený jen modely, aby se
  předešlo zasažení
- **Exponenciální odložení** — Pokročilé odložené pokuty
- **Prémiové ochrana před hromadným zatížením ** — Mutex + semaforická ochrana
  proti hromadnému oživení
- **Combo fallback řetězcích** — Pokud primární poskytovatel selže, automaticky
  přechází do řetězce s žádným zásahem.
- **Kombinovaný systém ochrany proti přetrženinu** — Automaticky vypnutý špatné
  poskytovatele uvnitř kombinovaného řetězce
- **Dashboard zdraví** — Monitoring běžnosti úsporu času, stav ochrany proti
  přetrženinu, uzamčení, statistiky cache, odezva p50/p95/p99

</details>

<details>
<summary><b>🔧 7. "Configuring each AI tool is tedious and repetitive"</b></summary>

Vývojáři používají kurzor, Claude Code, Code Codex, OpenClaw, Gemini CLI, Kilo
Code... Každý nástroj vyžaduje jiný konfigurační soubor (koncová bod API,
klíčidlo, model). Rekonfiguraci při přechodu na jiné poskytovatele nebo modely
považujeme za neproduktivní práci

**Jak OmniRoute to řeší:**

- **Dashboard nástrojů CLI** — Speciální stránka s jednou kliknou konfigurací
  pro Claude Code, Codex CLI, OpenClaw, Kilo Code, Antigravity, Cline
- **Generátor konfigurace GitHub Copilot** — Generuje `chatLanguageModels.json`
  pro VS Code s hromadnou výběrem modelů
- **Úvodní průvodce** — Uvědomění se 4 kroku pro první uživatele
- **Jeden koncový bod a všechny modely** — Konfigurace
  `http://localhost:20128/v1` jednou, přístup k 67+ poskytovatelům

</details>

<details>
<summary><b>🔑 8. "Managing OAuth tokens from multiple providers is hell"</b></summary>

Claude Code, Codex, Gemini CLI, Copilot — vše používá OAuth 2.0 s expirujícími
tokeny. Vývojářům musí trvale obnovovat přihlášení, řešit `missing
client_secret`, `redirect_uri_mismatch`, selhání na vzdálených serverech a
zpracovávání tokenů přes LAN/VPS je zvlášť obtížné.

**Jak OmniRoute to řeší:**

- **Automatická aktualizace tokenů/X20X] — Tokeny OAuth aktualizovány na pozadí
  před vypršením
- **Nakonfigurovaný 2.0 OAuth (PKCE) ** — Automatický tok pro Claude Code,
  Codex, Gemini CLI, Copilot, Kiro, Qwen, iFlow
- **Multi-Account OAuth** — Vytvoři více účtů pro jednoho poskytovatele
  prostřednictvím tokenu JWT/ID
- **Rozhoduje OAuth LAN/Remote Fix** — Rozpoznání privátních IP adres pro
  `redirect_uri` a ruční režim pro vzdálené servery
- **Nastavení OAuth za nginx** — Použije `window.location.origin` pro zpětnou
  kompatibilitu proxy
- **Průvodce OAuth pro vzdálené servery** — Rozběhová instrukce pro služby
  Google Cloud na VPS/Docker

</details>

<details>
<summary><b>📊 9. "I don't know how much I'm spending or where"</b></summary>

Vývojáři používají více placených poskytovatelů bez sjednoceného přehledu o
výdajích. Každý poskytovatel má svůj vlastní panel fakturace, ale není-li
vytvořeno sjednocené pohledu, může se hromadit nečekaný výkyv nákladů

**Jak OmniRoute to řeší:**

- **Dashboard analýzy nákladů** — Monitoring nákladů za tokeny a správa rozpočtu
  pro každého poskytovatele
- **Omezení rozpočtu na úrovni schváleného stupně** — Limity výdajů na úrovni
  stupně, který spouští automatické navrstvení
- **Nastavení ceny pro model[]
- **Používání statistik na klíč API** — Počet požadavků a poslední použité
  timestamp pro klíč
- **Hlavní_deska_analýzy** — Statistické karty, diagram modelu užití a tabulka
  poskytovatelů s úspěchy a zpožděním

</details>

<details>
<summary><b>🐛 10. "I can't diagnose errors and problems in AI calls"</b></summary>

Bez observability se vývojář nedovídá, zda selhal požadavek z důvodu omezení
rychlosti, vypršení časového limitu, špatné formáty nebo chyby poskytovatele.
Skladba logů napříč různými terminály bez observability vede pouze k
trial-and-error.

**Jak OmniRoute to řeší:**

- **Sloučené_logs_desky** — 4 lištičky: Žádané_logs, Proxy_logs, Audit_logs,
  Console
- **Prohlížeče_konzolové_logs** — Reálný časový prohlížeč stylu terminálu s
  barvem kódu, auto-scroll, vyhledávání a filtrování
- **SQLite_proxy Logs** — Trvalé pozastavené záznamy, které vydrží restart
  serveru
- **Nástupiště_prekladatele** — 4 režimy prošetření: Nástupiště(provedení
  prekladu), Tester_chat (obrázokovú cestu), Testovacia_plocha (sada),
  Živá_monitory (živé času)
- **Žádané_diagnostické_indikátory** — p50/p95/p99 zpoždění + sledování requestu
  "X-Request-Id"
- **Souborová_logging_s_podobou_rotace** — Konzolový stínřetřiš s kapacitní
  rotací, který uchovává vše do souboru JSON
- **Zpráva_o_systemu** — `npm run system-info` vygeneruje soubor
  `system-info.txt` se vaším úplným prostředím (verze Node, verze OmniRoute, OS,
  vývojářské nástroje, Docker/PM2 status). Připojte k němu, pokud chcete
  okamžité vymezování problémů.

</details>

<details>
<summary><b>🏗️ 11. "Deploying and maintaining the gateway is complex"</b></summary>

Instalace, konfigurace a údržba AI proxy ve verschiedenen prostředích (lokál,
VPS/Docker, cloudu) je časově náročná. Problémy jako předdefinovaná cesty,
`EACCES` na adresáře, konfondence portů a cross-platform budovy vytvářejí odpor.

**Jak OmniRoute to řeší:**

- **globální_npm_instalace** — `npm install -g omniroute &amp;&amp; omniroute` —
  hotovo
- **Docker_mnohostatovací** — AMD64 + ARM64 native (Apple Silicon, AWS Graviton,
  Raspberry Pi)
- **Docker_Kompozice_profilů** — `základ` (bez konzolového nástroje) a
  `konzol[X60X) (s Claude Code, Codex, OpenClaw)
- **Programové rozhraní Desktopu_Electron** — Nativní aplikace pro
  Windows/macOS/Linux se spuštěním systému tray, offline režimem
- **Rozdělený_režim_sekund** — API a Dashboard na oddělených portů pro pokročilé
  scénáře (inverzní proxy, kontejnerní síť)
- **Hromadný_sync s cloudem** — Synchronizace nastavení mezi zdroji s využitím
  Cloudflare Workers
- **DB Zálohování** — Automatická záloha, obnovení, export a import všech
  nastaví

</details>

<details>
<summary><b>🌍 12. "The interface is English-only and my team doesn't speak English"</b></summary>

Týmy ve zemí, kde se málo mluví anglicky, zvláště v Latinské Americe, Asii a
Evropě, se potýkají se složitým anglickým účtem. Bariéry jazykových úrovní
snižují adoption a zvyšují počet chyb při nastavení

**Jak OmniRoute to řeší:**

- **Rozhraní Přenosy — — Celých 500+ klíčů přeloženo včetně arabštiny,
  bulharštiny, dánštiny, němčiny, španělštiny, finštiny, francouzštiny,
  hebrejštiny, hindštiny, chorvatštiny, indonéštiny, italštiny, japonštiny,
  korejštiny, malajštiny, nizozemštiny, norské, polštiny, portugalštiny (PT/BR),
  rumunštiny, ruštiny, slovenské, švédštiny, thajštiny, ukrajinsky,
  vietnamštiny, čínštiny, filipinštiny a angličtiny
- **Podpora zobrazení zleva** — Podpora práva doleva pro arabštinu a hebrejštinu
- **Multi-Lanaguage READMEs** — 30 kompletní dokumentace překlady
- **Výběr jazyků** — Zeměpisný symbol v záhlaví pro reálné přepnutí

</details>

<details>
<summary><b>🔄 13. "I need more than chat — I need embeddings, images, audio"</b></summary>

AI není jen chatový dokončení. Programátoři potřebují generarět obrázky,
transkribovat audia, vytvářet vypočitatelnost pro RAG, přehodnocovat dokumenty a
moderovat obsah. Každý poskytovatel má jiný koncový bod a formát

**Jak OmniRoute to řeší:**

- **Vypočtatelnost** — `/v1/embeddings` se 6 poskytovateli a 9+ modely
- **Generování obrázků** — `/v1/images/generations` s 10 poskytovateli a 20+
  modely (OpenAI, xAI, Together, Fireworks, Nebius, Hyperbolic, NanoBanana,
  Antigravity, SD WebUI, ComfyUI)
- **Text-to-Video** — `/v1/videos/generations` — ComfyUI (AnimateDiff, SVD) a SD
  WebUI
- **Text-to-Music** — `/v1/music/generations` — ComfyUI (Stable Audio Open,
  MusicGen)
- **Transkripce Audio** — `/v1/audio/transcriptions` — Whisper + Nvidia NIM,
  HuggingFace, Qwen3
- **Text-to-Speech** — `/v1/audio/speech` — ElevenLabs, Nvidia NIM, HuggingFace,
  Coqui, Tortoise, Qwen3, **Inworld**, **Cartesia**, **PlayHT**, + stávající
  poskytovatelé
- **Vykonávání moderací** — `/v1/moderations` — Kontrola bezpečí obsahu
- **Posuzování dokumentu** — `/v1/rerank` — Dokumenty
- **API odpovědí** — Plná `/v1/responses` podpora kódu

</details>

<details>
<summary><b>🧪 14. "I have no way to test and compare quality across models"</b></summary>

Programátoři chtějí lépe vědět, který model je vhodný pro jejich použití –
kódové překlady, argumenty – ale porovnávání manuální je pomalé. Neexistují
integrované eval nástroje.

**Jak OmniRoute to řeší:**

- **Vyhodnocení LLM ** — Zlatá sada testování s 10 přednastavenými podmínkami
  pokrývající pozdravy, matematiku, geografii, generování kódu, kontrolu JSON,
  překlad, markdown a odmítnutí bezpečnosti
- **4 strategie pro určení shody ** — `výrazná `, `obsahuje `, `rozšířené `,
  `custom ` (funkce v JS)
- **Testovací plocha překladatele ** — Testování v sadách s více vstupními daty
  a očekávanými výsledky, srovnání různých poskytovatelů služeb
- **Tester čeťe ** — Páteřní cesta s vizuální zobrazení odpovědí
- **Živý monitor ** — Aktuální tok všech požadavků tekoucích skrz proxy

</details>

<details>
<summary><b>📈 15. "I need to scale without losing performance"</b></summary>

S narůstající objemem požadavků, bez použití cache stejné otázky znovu potřebují
stejný náklad. Bez idempotence duplicitní požadavky zneužívají zpracování. Musí
být dodržena konečná sazba pro každého poskytovatele.

**Jak OmniRoute to řeší:**

- **Semantická cache ** — Dvoulodní cache (signatura + semantics) snižuje náklad
  a latenci
- **Idempotence požadavku ** — 5s okénko odstranění duplicity pro stejné
  požadavky
- **Detekce sazby ** — Sazba za poskytovatele RPM, minimální odstup a maximální
  současné sledování
- **Upravitelné limitace sazby ** — Nastavení výchozích hodnot v Nastavení →
  Bezpečenosti s trvalej uchováním
- **Validace klíč API Cache ** — 3-třídová cache ke zlepšení výkonnosti v
  produkci
- **Statistika zdravotního pásma s telemetrickou ** — P50 / p95 / p99 latence,
  cache, dostupnost

</details>

<details>
<summary><b>🤖 16. "I want to control model behavior globally"</b></summary>

Vývojáři, kteří chtějí mít všechny odpovědi v určité jazyce, s konkrétní tonací,
nebo chtějí omezit tokeny dedukce. Nastavením tohoto v každém nástroji/požadunci
je prakticky nemožné.

**Jak OmniRoute to řeší:**

- **Injektace vstupní podkladové promt ** — Globální promt aplikováno na všechny
  požadavky
- **Overlimitní rozpočtová validace ** — Kontrola tokenů rozpoznání na
  požiadantom (prodloužení, automatické, specifikace, adaptivní)
- **6 strategií pro směrování požadavků ** — Globální strategie určující, jak
  požadavky jsou distribuované
- **Divné směrovače ** — `poskytovatel/*` vzory směrují dynamicky k jakémukoliv
  poskytovateli
- **Vypnutí/ovládání kombinací ** — Přepínání kombinačních nabídek přímo z
  dashboardu
- **Dostupnost poskytovače — Zapneme/zapne všechna připojení pro poskytovatele
  jedním klepem na tlačítko
- **Zablokované poskytovatele** — Izolovat konkrétní poskytovatele ze seznamu
  `/v1/models`

</details>

<details>
<summary><b>🧰 17. "I need MCP tools as first-class product capabilities"</b></summary>

Mnoho AI brán vystavuje MCP jako skrytou implementační detail. Na to potřebují
vidět viditelnou a manažerství operaci vrstvu.

**Jak OmniRoute to řeší:**

- MCP je viditelná v navigaci dashboard a sekci koncové úloha - tab
- Samostatný stránka -MCP pro správu s proces, nástroje, rozsah a audit
- Postavený rychle spustit pro `omnirout – mcp` a onboardingu klienta

</details>

<details>
<summary><b>🧠 18. "I need A2A orchestration with sync + stream task paths"</b></summary>

Agenty potřebovaly obou přímé odpovědi a dlouhé připojení řízení s životnostem
kontrol

**Jak OmniRoute to řeší:**

- A2A JSON-RPC koncový bod (`POST /a2a`) s `odeslal/X54X message a `stream/X75X
  message
- SSE odeslaného s terminálním stavu šíření
- Třídy životní API pro `tasks /get` a `tasks/cancel`

</details>

<details>
<summary><b>🛰️ 19. "I need real MCP process health, not guessed status"</b></summary>

Operační týmy potřebují vědět, zda MCP je skutečně aktivní, ne pouze zda je přes
API dostupný

**Jak OmniRoute to řeší:**

- Synchronizovaný soubor – srdce s PIDDATATIMESTAMPTRANSPORT tool_COUNTSOPROPODU
- API stavu MCP kombinující srdce + nedávné aktivity
- Karty UI stavu pro proces/průběh/ Srdcovky/freschness

</details>

<details>
<summary><b>📋 20. "I need auditable MCP tool execution"</b></summary>

Kdykoli nástroje mutovat konfiguraci nebo aktivovat akcí op -Témy potřebují
forenzní stopy.

**Jak OmniRoute to řeší:**

- SquLite zastoupený audit logování pro MCP nástroje kóduvali
- Filtery podle nástroje, úspěšnosti/neúspěšnosti, API klíče a stránkování
- Tabulková stránka auditu + koncové body s statistikami pro automatizaci

</details>

<details>
<summary><b>🔐 21. "I need scoped MCP permissions per integration"</b></summary>

Odmítnout přístup různé klienty má co nejnižší právo na kategorie nástroje.

**Jak OmniRoute to řeší:**

- 9 zhruba rozložitá obor pro omezený přístup nástroje
- Zajištění a viditelnost ve správě MCP
- Bezpečné výchozí nastavení pro nástroje pro provozování

</details>

<details>
<summary><b>⚙️ 22. "I need operational controls without redeploying"</b></summary>

Týmy potřebují rychlá změna běhu za incident nebo náklady.

**Jak OmniRoute to řeší:**

- Aktivace kombinace přepínače přímo z tabulky obsluhy MCP
- Pokyny pro odolnost podle předem definovaných balíčků politik
- Resetování stavu obvodu pro bránici přímo z stejné úpravy panelu

</details>

<details>
<summary><b>🔄 23. "I need live A2A task lifecycle visibility and cancellation"</b></summary>

Bez vizibility v cyklu života úloha s výzkumnou obtížnost triáže.

**Jak OmniRoute to řeší:**

- Zobrazení úloh, filtrování podle stavu/nákladu se stránkováním
- Drill-down na úlohová metadata, události a artefakty
- Účelové koncové body a tlačítko pro zrušení úlohy s potvrzením

</details>

<details>
<summary><b>🌊 24. "I need active stream metrics for A2A load"</b></summary>

Průběžné výkony vyžadují operativní přehled o běhu a živých spojeních.

**Jak OmniRoute to řeší:**

- Aktivních proudů počítá včlenění do A2A statusu.
- Poslední dílčinnost timestamp apočty podle stavu
- Dashboard A2A k reálnému monitorování provozu

</details>

<details>
<summary><b>🪪 25. "I need standard agent discovery for clients"</b></summary>

Externí klienti a orchestrátory potřebují strojově čitelnou metadata pro
naboarding.

**Jak OmniRoute to řeší:**

- Nakartička agenta je dostupná na adrese `/.well-known/agent.json`
- Schopnosti a dovednosti jsou ukázány v nastavení Správní obrazovka
- API A2A zahrnuje metadata objevování pro automatizaci

</details>

<details>
<summary><b>🧭 26. "I need protocol discoverability in the product UX"</b></summary>

Pokud uživatelé nemohou objevit povrchy protokolu, klesá adoptace a kvalita
podpory.

**Jak OmniRoute to řeší:**

- Konsolidovaný stránka s ** Úkonu** se spustí s kartami pro Proxy, MCP, A2A a
  API Endpoints.
- Inline přepínače stavu služeb (online/offline) pro MCP a A2A
- Odkazy na přehled do specializované taby Správní

</details>

<details>
<summary><b>🧪 27. "I need end-to-end protocol validation with real clients"</b></summary>

Mock testy nestačí k ověřování kompatibility protokolu před vydáním.

**Jak OmniRoute to řeší:**

- Krokový testování aplikaci a používá reálné MCP SDK klient transport
- Testy A2A klient pro objevování, odeslání, prouž, získat a zrušit tok
- Krokový kontrola proti MCP audit a A2A tasky API

</details>

<details>
<summary><b>📡 28. "I need unified observability across all interfaces"</b></summary>

Rozdělení pozorování podle protokolu vytváří slepé místo a delší MTTR.

**Jak OmniRoute to řeší:**

- Unifikované dashbordy/logs/analytics v jednom produktu.
- Health + audit + request telemetry přes OpenAI, MCP a vrstvu A2A
- Operativní API pro stav a automatizaci

</details>

<details>
<summary><b>💼 29. "I need one runtime for proxy + tools + agent orchestration"</b></summary>

Spoustění mnoha oddělených služeb zvyšuje operativní náklady a režimy selhání.

**Jak OmniRoute to řeší:**

- Proxy kompatibilní s OpenAI, server MCP a server A2A v jedné válcovně
- Sdílená autentizace, odolnost, úložiště údajů a sledování
- Konzistentní model politiky na všech interakčních površích

</details>

<details>
<summary><b>🚀 30. "I need to ship agentic workflows without glue-code sprawl"</b></summary>

Squady ztrácejí rychlost při kladení více ad-hoc služeb a skriptů.

**Jak OmniRoute to řeší:**

- Unifikovaný koncept zakázky pro klienty a agenty
- Nastavené protokoly pro řízení UI a cesty záblesků (smoke validation)
- Běžně dostupné základy pro produkční prostředí (bezpečnost, protokolování,
  odolnost, záloha)

</details>

### Příklady Playbooku (Integrované případy použití)

**Playbook A: Maximalizace placeného zakázky + levné zálohy**

```txt
Kombinace: "maximalizovat-claude"
  1. cc/claude-opus-4-6
  2. glm/glm-4.7
  3. if/kimi-k2-thinking

Výdajy za měsíc: $20 + malé plnění zálohy
Výsledek: vyšší kvalita, near-zero přerušení
```

**Playbook B: Nulová náklady pro kódovací stavebnicí**

```txt
Kombinace: "zdravý na věčnost"
  1. gc/gemini-3-flash
  2. if/kimi-k2-thinking
  3. qw/qwen3-kódér plus

Výdajy za měsíc: $0
Výsledek: stálá volní kódovací workflow
```

**Playbook C: Obnovení 24/7 fallbacková řetězec**

```txt
Kombinace: "always-on"
  1. cc/claude-opus-4-6
  2. cx/gpt-5.2-codex
  3. glm/glm-4.7
  4. minimax/MiniMax-M2.1
  5. if/kimi-k2-thinking

Výsledek: hluboký fallbackový základem pro deadline-critical workloads
```

**Playbook D: Agent ops s MCP + A2A**

```txt
1) Spustit přepravní dopravu MCP (`omniroute --mcp`) pro nástrojové operace
2) Spustit A2A úkoly prostřednictvím `zpráva/send` a `zpráva/stream`
3) Nátežte pomocí /dashboard/endpoint (MCP a A2A záložky)
4) Rozbalit služby prostřednictvím inline status kontrol
```

---

## ŇDÁK Má start zdarma — Nula Cena Konfigurace

> Nastavte AI kódováníwithin několika minut za **$0/měsíc**. Připojte tyto
> bezplatné účty a využijte vnořené **Základní Nástrojem zdarma** kombinaci.

| Krok | Akce                                                        | Dodavatelé rozluštěné                                                |
| ---- | ----------------------------------------------------------- | -------------------------------------------------------------------- |
| 1    | Připojte **Kiro** (AWS Stavbu ID OAuth)                     | Claude Sonnet 4.5, Haiku 4.5 — **neomezeno**                         |
| 2    | Připojte **iFlow** (Google OAuth)                           | kimi-k2-kvalifikoval, qwen3-kód plus, deepseek-r1... — **neomezeno** |
| 3    | Připojte **Qwen** (Uživatelský kód)                         | qwen3-kód plus, qwen3-kód flash... — **neomezeno**                   |
| 4    | Připojte **Gemini CLI** (Google OAuth)                      | gemini-3-flash, gemini-2.5-pro — **180K/mo zdarma**                  |
| 5    | `/dashboard/typy/X18X] → **Základní Nástroj (0 $)** šablona | Automaticně okrouhlí všechny volné poskytovatele                     |

**Uveďte kterou IDE/CLI používáte:** `http://localhost:20128/v1` · API Key:
`jakýkoliv-string` · Hotovo.

> **Volitelná další pokrytí (také zdarma):** Groq API klíč (30 RPM zdarma),
> NVIDIA NIM (40 RPM zdarma, 70+ modelů), Cerebras (1 000 000 tokenů/den),
> LongCat API klíč (50 000 000 tokenů/den!), Cloudflare Workers AI (10 000
> neuronů/den, 50+ modelů).

## Rychlý start

### 1. Instalace a spuštění

```bash
npm install -g omniroute
omniroute
```

> **pnpm uživatelé:** Spusťte `pnpm approve-builds -g` po instalaci, aby se
> povolovaly nativní skripty budování požadované `better-sqlite3` a `@swc/core`:
> 
> ```bash
> pnpm install -g omniroute
> pnpm approve-builds -g   # Vyberte vše → schválení
> omniroute
> ```

Okno rozhraní se otevře na `http://localhost:20128` a URL API je
`http://localhost:20128/v1`.

| Povel                   | Popis                                                          |
| ----------------------- | -------------------------------------------------------------- |
| `omniroute`             | Spusťte server (`PORT=20128`, na stejném portu API a rozhraní) |
| `omniroute --port 3000` | Nastavte kanonicní port pro API na 3000                        |
| `omniroute --mcp`       | Spusťte server MCP (transport na standardní vstup/výstup)      |
| `omniroute --no-open`   | Nepřehledejte prohlížeč automaticky                            |
| `omniroute --help`      | Zobrazte nápovědu                                              |

Nástupní režim rozsoček:

```bash
PORT=20128 DASHBOARD_PORT=20129 omniroute
# API:       http://localhost:20128/v1
# Přehledová plocha:  http://localhost:20129
```

### 2) Připojení poskytovatelů a vytváření API klíče

1. Otevřít Přehledovou plochu → `Poskytovatelé` a připojte alespoň jeden
   poskytovatel (OAuth nebo API klíč).
2. Otevřít Přehledovou plochu → `Úchyty` a vytvořte API klíč.
3. (Optionální) Otevřít Přehledovou plochu → `Kombinace` a nastavte váš zadní
   řetězec.

### 3) Nasměrujte váš vývojový nástroj na OmniRoute

```txt
základní adresa:  http://localhost:20128/v1
API Key:  [kopírujte z Úchyty stránky]
Model:    if/kimi-k2-thinking (nebo jakékoli prefix poskytovatele/modelu)
```

Funguje se s Claude Code, Codex CLI, Gemini CLI, Cursor, Cline, OpenClaw,
OpenCode a SDKmi kompatibilními s OpenAI.

### 4) Aktivujte a ověřte protokoly (v2.0)

**MCP (pro operační nástroje):**

```bash
omniroute --mcp
```

Pokud potom připojte svůj klient MCP přes `stdio` a ověřte nástroje jako:

- `omniroute_get_health`
- `omniroute_list_combos`

**A2A (pro agenty k agenty workflow):**

```bash
curl http://localhost:20128/.well-known/agent.json
```

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"quickstart","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"Give me a short quota summary."}]}}'
```

### 5) Ověřte vše konce ke konce (doporučeno)

```bash
npm run test:protocols:e2e
```

Tato-suite ověřuje skutečné MCP a A2A klientské toky proti běžící aplikaci.

### Alternativa: spustit ze zdrojů

```bash
cp .env.example .env
npm install
PORT=20128 DASHBOARD_PORT=20129 NEXT_PUBLIC_BASE_URL=http://localhost:20129 npm run dev
```

---

## 🐳 Docker

OmniRoute je k dispozici jako veřejný Docker image na [Docker
Hub](https://hub.docker.com/r/diegosouzapw/omniroute).

**Rychlá spuštění:**

```bash
docker run -d \
  --name omniroute \
  --restart unless-stopped \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:latest
```

**Se souborem nastavení:**

```bash
# Kopírování a editace .env první
cp .env.example .env

docker run -d \
  --name omniroute \
  --restart unless-stopped \
  --env-file .env \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:latest
```

**Použití Docker Compose:**

```bash
# Základ profil ( bez nástrojů klientské části)
docker compose --profile base up -d

# Profil CLI (Claude Code, Codex, OpenClaw zabudovaný)
docker compose --profile cli up -d
```

| Obrázky                  | Značka       | Velikost | Popis                   |
| ------------------------ | ------------ | -------- | ----------------------- |
| `diegosouzapw/omniroute` | `nejnovější` | ~250MB   | Poslední stabilní verze |
| `diegosouzapw/omniroute` | `1.0.3`      | ~250MB   | Aktuální verze          |

---

## 🖥️ Desktopová aplikace — Offline & Always-On

> 🆕 **NOWÝ!** OmniRoute je nyní k dispozici jako **nativní desktopová aplikace**
> pro Windows, macOS a Linux.

Spusťte OmniRoute jako státni desktopovou aplikaci — bez terminálu, bez
prohlížeče, bez internetu vyžadovaného pro lokální modely. Electronová aplikace
zahrnuje:

- 🖥️ **Nativní okno** — Vyhrazené okno aplikace s integrací systému panelky
  systému
- 🔄 **Auto-Zahájení** — Spustit OmniRoute při přihlášení systému
- 🔔 **Nativní upozornění** — Získat upozornění pro vyčerpání limitu nebo
  problémy s poskytovatelem služeb
- ⚡ **Tlačítko pro rychlý start** — NSIS (Windows), DMG (macOS), AppImage
  (Linux)
- 🌐 **Módní režim** — Pracuje zcela offline s zabaleným serverem

### Rychlý start

```bash
# Rozvojový režim
npm run electron:dev

# Postavte si aplikaci pro své platformy
npm run electron:build       # Současná platforma
npm run electron:build:win   # Windows (.exe)
npm run electron:build:mac   # macOS (.dmg) — x64 a arm64
npm run electron:build:linux # Linux (.AppImage)
```

### Systémový panel

Po zmenšení OmniRoute žije v vašem systémem panelu s rychlými akcemi:

- Otevřít nástěnku
- Změnit serverový port
- Konec aplikace

📖 Plná dokumentace: [`electron/README.md`](electron/README.md)

---

## 💰 Ceník najdete zde

| Sať             | Poskytovatel               | Náklady                                         | Převrat Resetování     | Nejlepší pro                                  |
| --------------- | -------------------------- | ----------------------------------------------- | ---------------------- | --------------------------------------------- |
| **💳 PŘÍSPĚVEK** | Claude Code (Pro)          | $20/mo                                          | Ochotě + týdně         | Žádost už jste možná                          |
|                 | Codex (Plus/Pro)           | $20-200/mo                                      | Ochotě + týdně         | Použivatelé OpenAI                            |
|                 | Gemini CLI                 | **ZDARMA**                                      | 180K/mo + 1K/den       | Kdokoli!                                      |
|                 | GitHub Copilot             | $10-19/mo                                       | Příměr                 | Použivatelé GitHubu                           |
| **🔑 API KLÍČ**  | NVIDIA NIM                 | **BESPLATNÝ** (vždy zdarma)                     | ~40 RPM                | 70+ otevřených modelů                         |
|                 | Cerebras                   | **BESPLATNÝ** (1M tokenů/den)                   | 60 000 TPM / 30 RPM    | Nejrychlejší na světě                         |
|                 | Groq                       | **BESPLATNÝ** (30 RPM)                          | 14,4 tis. RPD          | Ultra-rychlá Llama/Gemma                      |
|                 | DeepSeek V3.2              | $0,27/$1,10 za 1M                               | Žádný                  | Nejsnadnější poměr cena/výkon                 |
|                 | xAI Grok-4 Fast            | **$0,20/$0,50 za 1M**  🆕                        | Žádný                  | Nejrychlejší + volání nástrojů, ultra nízká   |
|                 | xAI Grok-4 (standard)      | 0,20$/1,50 USD za 1M 🆕                          | Žádný                  | Důvodem je vlajkové modelu ze společnosti xAI |
|                 | Mistral                    | Krátka bezplatná zkušební verze a placená verze | Omezeno                | Evropský AI                                   |
|                 | OpenRouter                 | Placené používání na základě požadavků          | Žádný                  | Sběr 100+ modelů                              |
| **💰 **          | GLM-5 (pomocí Z.AI) 🆕      | 0,5/1M$                                         | 10h denně              | Nová vlajková značka 128K výstupu             |
|                 | GLM-4.7                    | 0,6/1M$                                         | 10h denně              | Rozpočet při náhradní operační síle           |
|                 | MiniMax M2.5 🆕             | 0,3/1M vstupy                                   | 5hodinové rozpracování | Racionalizace + agenty                        |
|                 | MiniMax M2.1               | 0,02$/1M                                        | 5hodinové rozpracování | Nejnižší varianta                             |
|                 | Kimi K2.5 (Moonshot API) 🆕 | Placené používání na základě požadavků          | Žádný                  | Prím Herní API přístup                        |
|                 | Kimi K2                    | 9$ za měsíc                                     | 10M vět za měsíc       | Předpřítomné náklady                          |
| **🆓 ZAČÍNEjte** | iFlow                      | **$0**                                          | Neomezený              | 5 modelů neomezeno                            |
|                 | Qwen                       | **$0**                                          | Neomezený              | 4 modelů neomezeno                            |
|                 | Kiro                       | **$0**                                          | Neomezený              | Claude Sonnet/Haiku (AWS Builder)             |
|                 | LongCat Flash-Lite 🆕       | **$0** (50M tok/day  🔥)                         | 1 RPS                  | Největší zdarma kvóta na Zemi                 |
|                 | Pollinations AI  🆕         | **$0** (nestačí klíč)                           | 1 req/15s              | GPT-5, Claude, DeepSeek, Llama 4              |
|                 | Cloudflare Workers AI  🆕   | **$0** (10K Neuronů/day)                        | ~150 odpovědí/den      | 50+ modelů, globální okraj                    |
|                 | Scaleway AI  🆕             | **$0** (1M tokens celkem)                       | Omezeno                | EU/GDPR, Qwen3 235B, Llama 70B                |

> 🆕 **Nové modely přidány (březen 2026):** Grok-4 Fast rodina za $0,20/$0,50/M
> (měřeno na 1143ms – 30 % rychlejší než Gemini 2,5 Flash), GLM-5
> prostřednictvím Z.AI s 128K výstupy, MiniMax M2,5 úvah, DeepSeek V3,2
> aktualizované ceny, Kimi K2,5 prostřednictvím Moonshot přímý API.

**💡 $0 Combo Styl – Kompletní zdarma nastavení:**

```
# 🆓 Definitivní Ultimate Free Stack 2026 — 11 poskytovatelů, $0 navždy
Kiro (kr/)             → Claude Sonnet/Haiku NEOMEZENÝ
iFlow (if/)            → kimi-k2-přemýšlení, qwen3-kódér-plus, deepseek-r1 NEOMEZENÝ
LongCat Lite (lc/)     → LongCat-Flash-Lite — 50M tokens/day  🔥
Pollinations (pol/)    → GPT-5, Claude, DeepSeek, Llama 4 — není potřeba klíč
Qwen (qw/)             → qwen3-kódér-plus, qwen3-kódér-Flash, qwen3-kódér-Next NEOMEZENÝ
Gemini (gemini/)       → Gemini 2,5 Flash — 1 500 req/day zdarma klíč API
Cloudflare AI (cf/)    → Llama 70B, Gemma 3, Mistral — 10K Neuronů/day
Scaleway (scw/)        → Qwen3 235B, Llama 70B — 1M zdarma tokens (EU)
Groq (groq/)           → Llama/Gemma ultra-rychlé — 14,4K req/day
NVIDIA NIM (nvidia/)   → 70+ otevřené modely — 40 RPM navždy
Cerebras (cerebras/)   → Llama/Qwen svět-fast — 1M tok/day
```

**Nulová úhrada. Nikdy neukončí kódování.** Konfigurujte tento jako jeden
OmniRoute kombo a všechny fallbacky probíhají automaticky — žádné ruční
přepínání nikdy.

---

---

## 🆓 Volné modely — Co se vlastně můžete očekávat

> Všechny níže uvedené modely jsou **100% zdarma s nulovou nutností kreditní
> karty**. OmniRoute automaticky směruje mezi nimi, když se jedna úloha vyčerpá
> — kombinujte je všechny pro nevýpravný $0 kombo.

### 🔵 MODELY CLAUDE (prostřednictvím Kiro — AWS Stavitel ID)

| Model                | Předpona | Limit          | Limit rychlosti        |
| -------------------- | -------- | -------------- | ---------------------- |
| `Claudiův sonet 4.5` | `kr/`    | **Bez limitu** | Žádná denní kapacita   |
| `Claudiův haiku 4.5` | `kr/`    | **Bez limitu** | Žádná denní kapacita   |
| `Claudiův opus 4.6`  | `kr/`    | **Bez limitu** | Poslední Opus via Kiro |

### 🟢 NÁSTROPNI MODELY (Free OAuth — Nezaplacení kreditní karty)

| Model                 | Předpona | Limit          | Limit rychlosti  |
| --------------------- | -------- | -------------- | ---------------- |
| `Kimi-k2-neschopnost` | `if/`    | **Bez limitu** | Žádný hlášen cíl |
| `qwen3-kódér-plus`    | `if/`    | **Bez limitu** | Žádný hlášen cíl |
| `hluboko-hledače-r1`  | `if/`    | **Bez limitu** | Žádný hlášen cíl |
| `minimax-m2.1`        | `if/`    | **Bez limitu** | Žádný hlášen cíl |
| `kimi-k2`             | `if/`    | **Bez limitu** | Žádný hlášen cíl |

### 🟡 MOÐELOVÉ QWEN (Zařízení Code Autentizace)

| Model               | Předpona | Limit          | Limit rychlosti     |
| ------------------- | -------- | -------------- | ------------------- |
| `qwen3-kódér-plus`  | `qw/`    | **Bez limitu** | Žádný hlášen cíl    |
| `qwen3-kódér-flash` | `qw/`    | **Bez limitu** | Žádný hlášen cíl    |
| `qwen3-kódér-next`  | `qw/`    | **Bez limitu** | Žádný hlášen cíl    |
| `vizionářský model` | `qw/`    | **Bez limitu** | Multimoda (obrázky) |

### 🟣 GEMINI CLI (Google OAuth)

| Model                      | Předpona | Limit                            | Limit rychlosti |
| -------------------------- | -------- | -------------------------------- | --------------- |
| `Gemini-3 - flash preview` | `GC/`    | **180K tokenů/měsíc** + 1K/den   | Měsíční reset   |
| `Gemini-2.5 pro`           | `GC/`    | 180K tokenů/měsíc (sdílený pool) | Vysoce kvalitní |

### ⚫ NVIDIA NIM ( FREE API klíč — build.nvidia.com )

| Sať               | Denní limit          | Limit rychlosti | Poznámky                                                          |
| ----------------- | -------------------- | --------------- | ----------------------------------------------------------------- |
| Free ( Rozvojář ) | Bez tokenové hranice | **~40 RPM**     | 70+ modelů; přechod na čistá omezování rychlosti koncem roku 2025 |

Populární zdarma modely: `moonshotai/kimi-k2.5` (Kimi K2.5), `z-ai/glm4.7` (GLM
4.7), `deepseek-ai/deepseek-v3.2` (DeepSeek V3.2),
`nvidia/llama-3.3-70b-instruct`, `deepseek/deepseek-r1`

### ⚪ CEREBRAS ( FREE API klíč — inference.cerebras.ai )

| Sať    | Denní limit       | Limit rychlosti     | Poznámky                                                   |
| ------ | ----------------- | ------------------- | ---------------------------------------------------------- |
| Zdarma | **1M tokenů/den** | 60 000 TPM / 30 RPM | Světově nejrychlejší inference LLM; každý den se restarted |

K dispozici zdarma: `llama-3.3-70b`, `llama-3.1-8b`,
`deepseek-r1-distill-llama-70b`

### 🔴 GROQ (Volná API klíc — console.groq.com)

| Sať    | Denní limit   | Limit rychlosti | Poznámky                                               |
| ------ | ------------- | --------------- | ------------------------------------------------------ |
| Zdarma | **14,4K RPD** | 30 RPM na model | Žádné kreditní karty; 429 na limit, zásobuje se zdarma |

K dispozici zdarma: `llama-3.3-70b-versatile`, `gemma2-9b-it`, `mixtral-8x7b`,
`whisper-large-v3`

### 🔴 LONGCAT AI (Volná API klíc — longcat.chat) 🆕

| Model                         | Předpona | Denní zadarmo    | Poznámky                      |
| ----------------------------- | -------- | ---------------- | ----------------------------- |
| `LongCat-Flash-Lite`          | `lc/`    | **50M tokenů** 💥 | Největší zadarmo ve své cestě |
| `LongCat-Flash-Chat`          | `lc/`    | 500 tisíc tokenů | Multi-turn rozhovor           |
| `LongCat-Flash-Thinking`      | `lc/`    | 500 tisíc tokenů | Rozhodování / CoT             |
| `LongCat-Flash-Thinking-2601` | `lc/`    | 500 tisíc tokenů | Verze z ledna 2026            |
| `LongCat-Flash-Omni-2603`     | `lc/`    | 500 tisíc tokenů | Multimodální                  |

> 100% zadarmo, pokud je v veřejném beta. Zaregistrujte se na
> [longcat.chat](https://longcat.chat) pomocí emailu nebo telefonu. Periodicky
> se obnoví každý den o 00:00 UTC.

### 🟢 POLINACE AL (Bez požadavku na API klíč) 🆕

| Model              | Předpona         | Limit rychlosti | Dodavatel Za Zázrukou      |
| ------------------ | ---------------- | --------------- | -------------------------- |
| `openai`           | Dodavatel `pol/` | 1 req/15s       | GPT-5                      |
| `claude`           | Dodavatel `pol/` | 1 req/15s       | Dodavatel Claude Anthropic |
| Dodavatel `gemini` | Dodavatel `pol/` | 1 req/15s       | Google Gemini              |
| `deepseek`         | Dodavatel `pol/` | 1 req/15s       | DeepSeek V3                |
| Dodavatel `llama`  | Dodavatel `pol/` | 1 req/15s       | Skout Meta Llama 4         |
| `mistral`          | Dodavatel `pol/` | 1 req/15s       | Dodavatel Mistral AI       |

> ✨ **Nulová odporu:** Beznásobková registrace, žádné API klíče. Přidejte
> poskytovatele Pollinations s prázdným polím klíč a funguje ihned.

### 🟠 CLOUDFLARE WORKERS AI (Free API Key — cloudflare.com) 🆕

| Sať    | Každodenní Neurony | Ekvivalentní použití                    | Poznámky                   |
| ------ | ------------------ | --------------------------------------- | -------------------------- |
| Zdarma | **10,000**         | ~150 LLM resp / 500s audio / 15K embeds | Globální okraj, 50+ modelů |

Populární zdarma modely: `@cf/meta/llama-3.3-70b-instruct`,
`@cf/google/gemma-3-12b-it`, `@cf/openai/whisper-large-v3-turbo` (audio
zdarma!), `@cf/qwen/qwen2.5-coder-15b-instruct`

> Potřebuje API Token + ID účtu z
> [dash.cloudflare.com](https://dash.cloudflare.com). Uložte ID účtu do
> nastaveníprověřovacích údajů.

### 🟣 SCALEWAY AI (1M free tokens — scaleway.com) 🆕

| Sať    | Bezplatný limit | Místo        | Poznámky                                      |
| ------ | --------------- | ------------ | --------------------------------------------- |
| Zdarma | **1M tokenů**   | 🇫🇷 Paříž, EU | Přístup k kreditní kartě není nutný do limitů |

Dostupno za cenu 0 korun: `qwen3-235b-a22b-instruct-2507` (Qwen3 235B!),
`llama-3.1-70b-instruct`, `mistral-small-3.2-24b-instruct-2506`,
`deepseek-v3-0324`

> EU/GDPR slučitelné. Získejte API klíč na
> [console.scaleway.com](https://console.scaleway.com).

> ** 💡 Nejlepší Zadarmo Stack (11 poskytovatelů, 0$ bezkoncově): **
> 
> ```
> Kiro (kr/)             → Claude Sonnet/Haiku BEZPLATNÉ
> iFlow (if/)            → kimi-k2-zamyslený, qwen3-řemeslníkplus, deepseek-1 UNLIMITED
> LongCat Lite (lc/)     → LongCat-Flash Lite — 50 milionů tokenů/den 
> Pollinations (pol/)    → GPT-5, Claude, DeepSeek, Llama 4 — žádný klíč potřebný
> Qwen (qw/)             → qwen3-řemeslníkovy modely UNLIMITED
> Gemini (gemini/)       → Gemini 2.5 Flash — 1,5 tisíc žádostí/den zdarma
> Cloudflare AI (cf/)    → 50+ modelů — 10 tisíc neuronů/den
> Scaleway (scw/)        → Qwen3 235B, Llama 70B — 1 milión zdarma (EU)
> Groq (groq/)           → Llama/Gemma — 14,4 tisíce žádostí/den ultra-rychlé
> NVIDIA NIM (nvidia/)   → 70+ volně dostupné modely — 40 RPM věčně
> Cerebras (cerebras/)   → Llama/Qwen světo-fastest — 1 milión toků/den
> ```

## 🎙️ Zadarmo kombinovaný přepis

> Přepisujte jakékoliv audio/video zdarma za **0$ ** — Deepgram vede s 200$
> zdarma, AssemblyAI 50$ fallback, Groq Whisper jako neomezený nouzový záloha.

| Poskytovatel     | Zadarmo kredit                    | Nejlepší Model                               | Limit rychlosti                    |
| ---------------- | --------------------------------- | -------------------------------------------- | ---------------------------------- |
| 🟢 **Deepgram**   | **200$ zdarma ** (registrovat se) | `nova-3` — nejlepší přesnost, 30+ jazyků     | Žádné limity RPM na zadarmo kredit |
| 🔵 **AssemblyAI** | **50$ zdarma ** (registrovat se)  | `universal-3-pro` — kapitoly, sentiment, PII | Žádné limity RPM na zadarmo kredit |
| 🔴 **Groq**       | **Zdarma věčně **                 | `whisper-large-v3` — OpenAI Whisper          | 30 RPM (omezený limitem)           |

**Doporučená kombinace v `/dashboard/combos`:**

```
Strategy: Priorita
```

Tězká transkripce\
==WEBLATE_part==\
Potom ve `/dashboard/media` → **Transkripce** okení: zkuste přiložit qualquer
zvukový nebo video soubor → vyberte své kombinovanou endpoint → získejte
transkripci ve formátech podporovaných.

## 💡 Význačné funkce

OmniRoute v2.0 je postaven jako operační platforma, nejen jako proxy relay.

### 🆕 Nová — Inspirované Vylepšení ClawRouter (Mar 2026)

| Funkce                                             | Co to dělá                                                                                                |
| -------------------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| ⚡ **Grok-4 Rychlá Rodina**                         | xAI modely za $0.20/$0.50/M — benchmarkovaný 1143ms (30% rychlejší než Gemini 2.5 Flash)                  |
| 🧠 **GLM-5 prostřednictvím Z.AI**                   | 128K výstupní kontext, $0.5/1M — nejnovější vlajková loď z rodiny GLM                                     |
| 🔮 **MiniMax M2.5**                                 | Důvodování + agentivní úkoly za $0.30/1M — zásadní upgrade od M2.1                                        |
| 🎯 **Dodatečný model každý z modelu**               | Jeden z `Dostupný model: pravda/pseudo` v registru — AutoKombinace prochází přes ne-více schopnými modely |
| 🌍 **Multilizující detekce záměru**                 | PT/ZH/ES/AR klíčová slova v skórování AutoKombinace — lepší výběr modelů pro obsah nerozumné angličtiny.  |
| 📊 **Benchmark-driven fallbacky**                   | Skutečný p95 latence z živých požadavků krátká skórování — AutoKombinace naučil se z reálnými daty.       |
| 🔁 **Odstranění duplicitních požadavků**            | Vyhledávací okno na základě obsahu — multiagentově bezpečné, zabrání duplicitním nárocím                  |
| 🔌 Strategii routování **Pluggable RouterStrategy** | Rozšiřitelný ` Routovací strategie ` interface — přidej zákaznickou logiku routování jako doplňky         |

### 🚀 Předchozí v2.0.9+ — Playground, CLI Fingerprints & ACP

| Funkce                                         | Co to dělá                                                                                                                                                                                                                                                                                                |
| ---------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🎮 Hrací plocha **Model Playground**            | Přístupová stránka ke testování jakéhokoli modelu přímo — poskytovatel/model/poUNUSED konektory, Monaco Editor, streamování, zrušení, časování                                                                                                                                                            |
| 🔏 **Fingerprinty CLI **                        | Nastavení pořadí hlaviček a těla na úrovni poskytovatele pro shodu s původní CLI podpisem — přepínač pro změnu v nastaveních > Bezpečnost. **Vaše proxy IP je uchováváno**                                                                                                                                |
| 🤝 **Podpora ACP (Agent Client Protocol) **     | Odhalení agentů CLI (Codex, Claude, Goose, Gemini CLI, OpenClaw + 9 dalších), spawner processů, `/api/acp/agents` bod koncový                                                                                                                                                                             |
| 🤖 Tiskárna ACP Agentů **ACP Agents Dashboard** | Podrobnostiagentů › stránka se schránkou z 14 agentů se stavem instalace, verzí, přizpůsobeným formulářem pro kteroukoli nástroj CLI. ** OpenCode ** uživatelé dostanou tlačítko "Stáhnout opencode.json", které automaticky generuje hotovo použitelné konfigurační soubor s veškerými dostupnými modely |
| 🔧 **Pozicování modelů s customou `apiFormat`** | Modely s `apiFormat: "responses"` jsou nyní správně směrovány k překladateli API odpovědí                                                                                                                                                                                                                 |
| 🏢 **Odebírání prostory Codex Workspace **      | Nastavení více pracovních prostorů Codexu na základě emailu — OAuth odděluje připojení po pracovních ID                                                                                                                                                                                                   |
| 🔄 **Automatizace obnovení Electronu **         | Zákaznický klient kontroluje aktualizace + automaticky instaluje při restartu                                                                                                                                                                                                                             |

### 🤖 Agent a protokoly operace (v2.0)

| Funkce                                      | Co to dělá                                                                                                            |
| ------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| 🔧 **Server MCP (16 nástruh)**               | Přiřazování nástrojů IDE/agentů pomocí 3 prostředků: stdio, SSE (`/api/mcp/sse`), Streamable HTTP (`/api/mcp/stream`) |
| 🤝 **A2A Server (JSON-RPC + SSE)**           | Provádění úkolů mezi agenty v synchronních a streamovacích tokích                                                     |
| 🧭 **Stránka zjednodušenýchpunktů **         | Stránka se sekčním řízením včetně panelů Proxyschop, MCP, A2A a API Endpoints                                         |
| 🎚️ **Rozdvojitelné přepínače stavu služeb** | Spínače ve tvaru ON/OFF pro MCP a A2A s trvalými Nastaveními (výchozí stav: OFF)                                      |
| 🛰️ **Heartbeat běhu MCP v reálném čase**    | Járočného procesního stavu (pid, uptime, Heartbeat Age, transport, Scope Mode)                                        |
| 📋 **Audit Trail MCP**                       | Filrovatelný protokol uskutečněných událostí s úspěšným/failovacím provedením a podrobnou specifikací                 |
| 🔐 **Implementace vymezení rozsahu MCP**     | 9 konkrétních oprávnění pro omezení přístupu nástrojů                                                                 |
| 📡 **Životní cyklus úkolů A2A**              | Výpis/filtr úkolů včetně inspekcí probíhajících událostí a artefaktů s možností zrušení úkolů běhu                    |
| 📋 **Agent Card Discovery**                  | /X0X /.well-known/agent.json X24X/ pro agentovo auto-nalezení                                                         |
| 🧪 X2X Protokolová E2E Test Harness X29X     | Skutečný SDK MCP + A2A klienta v X35X test:protokoly:e2e X54X                                                         |
| ⚙️ X3X Operační Kontrola X25X               | Sčítadlo přepínače, aplikujte profil odolnosti, restartujte zásobovače z jedné ovládací plochy                        |

### 🧠 Náhodné & Inteligence

| Funkce                                    | Co to dělá                                                                             |
| ----------------------------------------- | -------------------------------------------------------------------------------------- |
| 🎯 X2X Smarter Fallback 4-Trio X25X        | Automatické: Přihlášení → Klientský klíč → Levná → Zdarma                              |
| 📊 X2X Monitoring Spotřeby v Čase X28X     | Živý tok tokenů + Restartovací odpočet na poskytovatele                                |
| 🔄 X2X Formátování Překlad X22X            | OpenAI ⇒ Claude ⇒ Gemini ⇒ Odpovědi s bezpečností schématu                             |
| 👥 X2X Podpora Více Účtů X25X              | Mnohonásobná účtující poskytovatelích se inteligentním výběrem                         |
| 🔄 X2X Automatické Obnovení Tokenu X22X    | Ověřený token OAuth Automaticképřenos opětovný pokus                                   |
| 🎨 X2X Kombinace Nápravy X17X              | 6 zrovnovážených strategií + Řízení řetězcefallback                                    |
| 🌐 **Wildkartový Router**                  | `dostupitel/.*` dynamické rozlišení cest                                               |
| 🧠 **Rozpočet Myslete Kontroly**           | Přesnost, automatické, zásadně a přizpůsobivé limitace rozlišení                       |
| 🔀 **Modelové Aliasy**                     | Vlastní + přizpůsobivané modelové aliasování a migrace na bezpečné stránky             |
| ⚡ **Background Degradace**                | Routujte zpočátku pozadí zadužených úloh na levnější modely                            |
| 🧪 **Svědomé Průmyslová chytrá Routování** | Automatické vybírání modelu podle obsahu typu (kódování/vision/analysis/summarization) |
| 💬 **Systémová Promptové Přisuje**         | Globální řízení chování aplikované vždy konzistentně                                   |
| 📄 **Odpovídaní API Kompatibilita**        | Plná `/v1/responses` podpora pro Codex a pokročilé agente workflowy                    |

### 🎵 Multi-Modalové API

| Funkce                                      | Co to dělá                                                                                                                                                                                   |
| ------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🖼️ **Obrazy Generace**                      | `/v1/images/generations` s cloudu a lokálními backendy                                                                                                                                       |
| 📐 **Vnořené Vektory**                       | [v1/embeddings`] pro vyhledávání a toků RAG                                                                                                                                                  |
| 🎤 Poslech transkripce**                     | [v1/audio/transcriptions`] — 7 poskytovatelů (Deepgram Nova 3, AssemblyAI, Groq Whisper, HuggingFace, ElevenLabs, OpenAI, Azure), automatické detekování jazyka, podpora formátů MP4/MP3/WAV |
| 🔊 **Text-to-Speech**                        | [v1/audio/speech`] — 10 poskytovatelů (ElevenLabs, OpenAI, Deepgram, Cartesia, PlayHT, HuggingFace, Nvidia NIM, Inworld, Coqui, Tortoise) s správnými chybami                                |
| 🎬 **Generování videa**                      | [v1/videos/generations`] (ComfyUI + SD WebUI workflowy)                                                                                                                                      |
| 🎵 **Generování hudby**                      | [v1/music/generations`] (ComfyUI workflowy)                                                                                                                                                  |
| 🛡️ **Ochrana proti nevhodnému содержимому** | [v1/moderations`] zajištění bezpečnosti                                                                                                                                                      |
| 🔀 **Přeposlech**                            | [v1/rerank`] pro skóre relevance                                                                                                                                                             |
| 🔍 **Vyhledávání** 🆕                         | [v1/search`] — 5 poskytovatelů (Serper, Brave, Perplexity, Exa, Tavily), 6 500+ zdarma měsíčně, automatické failover, cache                                                                  |

### 🛡️ Odolnost, zabezpečení & správa

| Funkce                                      | Co to dělá                                                                                                                               |
| ------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| 🔌 **Circuit Breakers**                      | Per-model trika / obnovení se kontrolou prahů                                                                                            |
| 🎯 **Cílový modelovy Endpoint-Aware Models** | Požadavky na modely prohlášují podporovaná rozhraní API + formát API                                                                     |
| 🛡️ **Anti-zástruhový Herd**                 | Synchronization mutex + semafor protokolů na případy opakovaného chybového nebo rychlostního chování                                     |
| 🧠 **Semantic + Signátura Cache**            | Snížení nákladů a latence s použitím dvou vrstev cache                                                                                   |
| ⚡ **Jednotlivost žádosti**                  | Okno ochrany duplikátů                                                                                                                   |
| 🔒 **Narušení TLS Fingerpriintingu**         | Browser-like TLS fingerprint – **zvýšená ochrana proti detekci botů a zobrazení upozornění**                                             |
| 🔏 **Fingerprinty CLI **                     | Souhlasí s jedinečnými signaturami příchozích požadavků od native CLI – **snížena riziko zablokování zatímco se udrží IP proxy serveru** |
| 🌐 **Filtrace IP**                           | Ovládání dovolených/blokovacích seznamů pro vystavené nasazení                                                                           |
| 📊 **Editovatelná rychlostní limity**        | Koncesionalní globální/výkonové limity s persistencí                                                                                     |
| 🔑 **Úschova API klíčů + oborové omezení**   | Bezpečné vystavení/obnovování klíčů a ovládání modelů/zdůraznění poskytovatelů                                                           |
| 🛡️ **Ochrana `/models`**                    | Volitelná autentizace pro zatavění a skrývání poskytovatelů pro model catalog                                                            |

### 📊 monitorování & analýzy

| Funkce                           | Co to dělá                                                            |
| -------------------------------- | --------------------------------------------------------------------- |
| 📝 **Žádost + proxy Logging**     | Plná žádaná/získaná data a proxy logging                              |
| 📋 **Unifikovaný Logs Dashboard** | Zobrazení požadavků/proxy, auditů a konzoly na jedné stránce          |
| 🔍 **Žádostová Telemetrie**       | Dodržování latencí (p50/p95/p99) a sledování požadavků                |
| 🏥 **Zdravotní Dashboard**        | Dostupnost, stav breakeru, vyřazení, paměťové statistiky              |
| 💰 **Sledování nákladů**          | Rozpočet a kontrola cen za jednotlivé modely                          |
| 📈 **Výše Analýtika Visualizace** | Uživatelská data a trendy pro jednotlivé modely/providery             |
| 🧪 **Evaluation Framework**       | Testování na základě zlacených souborů s možností nastavení strategií |

### ☁️ nasazení & platforma

| Funkce                                          | Co to dělá                                                             |
| ----------------------------------------------- | ---------------------------------------------------------------------- |
| 🌐 **Nakdy nasadit kdekoliv**                    | Místní server, VPS, Docker, cloudové prostředí                         |
| 💾 **Synchronizace s cloudy**                    | Synchronizace nastavení prostřednictvím cloudu                         |
| 🔄 **Náhled/Obnovení**                           | Export/import a k dispozici obnova po selhání                          |
| 🧙 **Úvodní průvodce**                           | Průvodce prvními kroky při spouštění                                   |
| 🔧 **Rozhraní pro nástroje na rozhraní příkazů** | Jednorázová instalace pro oblíbené vyvinávací nástroje                 |
| 🎮 Hrací plocha **Model Playground**             | Testujte jakýkoli poskytovatelmodel/ koncový bod z rozhraní            |
| 🔏 **Zavřete prstenec pro rozhraní příkazu**     | Souření fingerprint konkrétních poskytovatelů v nastavení > Bezpečnost |
| 🌐 **Mezinárodní lokalizace (30 jazyků)**        | Kompletní podporapodporuje dokumenty s podporou RTL textu              |
| 🧹 **Clear All Models**                          | Jednorázové smazání seznamu modelů v podrobnostech poskytovatele       |
| 📋 **Šablony problému**                          | Standardizované šablony GitHub pro chyby a funkce                      |
| 📂 **Vybrat složitkové adresáře**                | [Přepiš Data Directory] nastavení pro adresář uschování                |

### Detail o funkci

#### Inteligentní náhrada funkčností se zvláštní kontrolou nákladů

```txt
Combino: "můj-kódovací-plocha"
  1. cc/claude-opus-4-6
  2. nvidia/llama-3.3-70b
  3. glm/glm-4.7
  4. if/kimi-k2-thinking
```

Při selhání kvoty, sazby nebo zdraví automaticky přistupuje OmniRoute k dalším
kandidátům bez nutnosti ručního přepínání.

#### Správa protokolu, která je viditelná a ovladatelná

- MCP + A2A jsou v UI a dokumentacích sdělovatelné (ne skrývané)
- API protokolu exposing žijící provozní data (`/api/mcp/*`, `/api/a2a/*`)
- Konzoly zahrnují akce na day-2 operacích (svícení kombinace, reset brány,
  zrušení úkolu)

#### Překladatel + validation workflow

Oblast Překladatele zahrnuje:

- **Playground**: zajištění kontrol transformace
- **Chat Tester**: kompletní kolo vyžádání/odpovědi
- **Test Bench**: více případů ve jednoho spuštění
- **Live Monitor**: reálný pohled na provoz

Velký protokol validation s reálnými klienty prostřednictvím `npm run
test:protocols:e2e`.

> 📖 **[Dokumentace MCP Server](open-sse/mcp-server/README.md)** — Návod k
> použití, IDE konfigurace a příklady klientů
> 
> 📖 **[Dokumentace A2A Server](src/lib/a2a/README.md)** — Dovednosti, JSON-RPC
> metody, streamování a životní cyklus úloh

## 🧪 Evaluace (Evals)

OmniRoute obsahuje vlastní rámec pro hodnocení kvality LLM odpovědí vzhledem k
zlaté sadě. Najdete jej ** Analytika → Hodnocení ** na nástěnce.

### Zahrnutá Golden Set

Připojena a přednastavená "OmniRoute Golden Set" obsahuje test pro:

- Rozhodnutí, matematika, geografie, generace kódu
- Kompatibilita ve formátu JSON, překlad, generování markdownee
- Odmítnutí zajištění bezpečnosti (škodlivý obsah),početování, Logika Boolean

### Strategie hodnocení

| Strategie           | Popis                                                             | Příklad                               |
| ------------------- | ----------------------------------------------------------------- | ------------------------------------- |
| `exaktní`           | Výstup se musí shodit přesně                                      | `"4"`                                 |
| `obsahuje`          | Výstup se musí obsahovat podřetězec (nezámění se velikost písmen) | `"Paříž"`                             |
| `souborové soubory` | Výstup se musí shodit s pravidlem souborového souboru             | `"1.*2.*3"`                           |
| `základní`          | Základní funkce JavaScript vrátí true/false                       | `(výstup) =&gt; výstup.délka &gt; 10` |

---

## 📖 Nápověda k nastavení

### Nastavení protokol (MCP + A2A)

<details>
<summary><b>🧩 MCP Setup (Model Context Protocol)</b></summary>

Nastartujte transport MCP v režimu stdio:

```bash
omniroute --mcp
```

Doporučený tok ověřování:

1. Spojit svého klienta MCP přes stdio.
2. Spustit omniroute_get_health`.
3. Spustit omniroute_list_combos`.
4. Otevřít `/dashboard/mcp`, aby se zobrazil puls, aktivita a audit.

Použitelné API pro automatizaci:

- `GET /api/mcp/status`
- `GET /api/mcp/tools`
- `GET /api/mcp/audit`
- `GET /api/mcp/audit/stats`

</details>

<details>
<summary><b>🤝 A2A Setup (Agent2Agent)</b></summary>

Objevte एजेंta:

```bash
curl http://localhost:20128/.well-known/agent.json
```

Poslat úloha:

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'obsah-type: aplikace/json' \
  -d '{"jsonrpc":"2.0","id":"setup-a2a","method":"message/send","params":{"skill":"quota-management","přenosy":[{"role":"user","content":"Zkrátka stavu kvóty."}]}}'
```

Řešení života:

- `GET /api/a2a/status`
- `GET /api/a2a/tasks`
- `GET /api/a2a/tasks/:id`
- `POSDLE /api/a2a/tasks/:id/stornovat`

Operační UI:

- `/dashboard/a2a` pro sledování úloh/zálohy/televize a zápasy z hasic.

</details>

<details>
<summary><b>🧪 End-to-end protocol validation</b></summary>

Overte oba protokoly s reálnými klienty:

```bash
npm run test:protocols:e2e
```

Provoře:

- Klient pro SDK MCP připojit/seznámit zavolat
- Nalezení na A2A zaslání/tokovací/získat/rušení
- Křížové vyhodnocení dat v MCP auditu a režimu Správa úkolu A2A API

</details>

<details>
<summary><b>💳 Subscription Providers</b></summary>

### Claude Code (Pro/Max)

```bash
Panel -&gt; Dodavatelé -&gt; Připojit Claude Code
-&gt; Přihlášení pomocí OAuth -&gt; Automatická obnovení tokenu
-&gt; sledování kvóty po 5 hodinách + týdnu

Modely:
  cc/claude-opus-4-6
  cc/claude-sonnet-4-5-20250929
  cc/claude-haiku-4-5-20251001
```

**Pro Tips**: Na složitá úkoly použijte Opus, pro rychlost Sonnet. OmniRoute
sleduje kvóty pro každé modely!

### OpenAI Codex (Plus/Pro)

```bash
Panel -&gt; Dodavatelé -&gt; Připojit Codex
-&gt; Přihlášení pomocí OAuth (port 1455)
-&gt; kvóta pro 5 hodin + týdenní reset

Modely:
  cx/gpt-5.2-codex
  cx/gpt-5.1-codex-max
```

#### Správa limitů účtů Codexu (5h + Týdenní

Na každé účtě Codexu nyní platí přepínačy zásad v sekci `Panel -&gt;
Dodavatelé`:

- `5 hodiny` (VLOŽITI/ODMIŤITI): Použít prahy pro 5 hodinovou zásadu.
- `Týden` (VLOŽITI/ODMIŤITI): Použít prahy pro týdenní zásadu.
- Chování pro prahy: když se dosáhne pověření okna >= 90% využití, account je
  přehlédnut.
- Chování pro rotaci: OmniRoute směruje na následující způsobilý účet Codexu
  automaticky.
- Resetování chování: když dojde k příchodu času pro resetování, account stane
  způsobilým opětovně automaticky.

Scénáře:

- `5 hodin VLOŽITI` + `Týdenní VLOŽITI`: účet je přehlédnut, když se dosáhne
  prahů pro některou z zásad.
- `5 hodin ODMÍTITI` + `Týdenní VLOŽITI`: pouze týdenní využití může zablokovat
  účet.
- `5 hodin VLOŽITI` + `Týdenní ODMÍTNUTI`: pouze pětihodinový usage může
  zablokovat účet.
- `Reset v ` proběhlo: účet automaticky obnovuje rotaci (žádná manuální povolení
  není nutná).

### Gemini CLI (ZDE 180K/month!)

```bash
Přístupová panel → Dodavatelé → Připojit Gemini CLI
→ Google OAuth
→ 180K úspěšných vyhodnocení za měsíc + 1K za den

Modely:
  gc/gemini-3-flash-preview
  gc/gemini-2.5-pro
```

**Nejlepší hodnota:** Obrovský zdarma smluvní! Použijte prosím tuto před placené
smlouvy.

### GitHub Copilot

```bash
Přístupová panel → Dodavatelé → Připojit GitHub
→ OAuth prostřednictvím GitHub
→ Pravidelné resetování (1. den měsíce)

Modely:
  gh/gpt-5
  gh/claude-4.5-sonnet
  gh/gemini-3-pro
```

</details>

<details>
<summary><b>🔑 API Key Providers</b></summary>

### NVIDIA NIM (ZDE vývojářský přístup zdarma –> 70+ modelů)

1. Zaregistrujte se: [build.nvidia.com](https://build.nvidia.com)
2. Získat API klíč zdarma (zahrnující 1000 inference creditů)
3. Přístupová panel → Přidat dodavatele → NVIDIA NIM:
   - API klíč: `nvapi-vašské-kliče`

**Modely:** `nvidia/llama-3.3-70b-instruct`, `nvidia/mistral-7b-instruct` a
další 50+ modelů

**Tip pro pokročilé:** Otevřený API společnosti OpenAI – funguje bezproblémově
se službou OmniRoute pro překlad formátu!

### DeepSeek

1. Zaregistrujte se: [platform.deepseek.com](https://platform.deepseek.com)
2. Získat API klíč
3. Přístupová panel → Přidat dodavatele → DeepSeek

**Modely:** `deepseek/deepseek-chat`, `deepseek/deepseek-coder`

### Groq (Dostupné zdarma smluvní!)

1. Zaregistrujte se: [console.groq.com](https://console.groq.com)
2. Získat API klíč (přidružený k zdarma smluvní)
3. Přístupová panel → Přidat dodavatele → Groq

**Modely: ** `groq/llama-3.3-70b`, `groq/mixtral-8x7b`

**Pro tip:** Ultra-fast inference — ideal for real-time coding!

### OpenRouter (100+ Models)

1. Zaregistrovat: [openrouter.ai](https://openrouter.ai)
2. Získat API klíč
3. Nabídka → Přidat poskytovatele → OpenRouter

**Modely:** Přístup k 100+ modelům z největších zdrojů prostřednictvím jediného
API klíče.

</details>

<details>
<summary><b>💰 Cheap Providers (Backup)</b></summary>

### GLM-4.7 (daily reset, 0,06 $/1M)

1. Zaregistrovat: [Zhipu AI](https://open.bigmodel.cn/)
2. Převzít API klíč z plánu Coding
3. Nabídka → Přidat API klíč:
   - Poskytovatel: `glm`
   - API klíč: `vaš-klíč`

**Použít:** `glm/glm-4.7`

**Pro tip:** Plán Coding nabízí 3× kvótu za 1/7 ceny! Reset daily 10:00 AM.

### MiniMax M2.1 (5h reset, 0,20 $/1M)

1. Zaregistrovat: [MiniMax](https://www.minimax.io/)
2. Získat API klíč
3. Dashboard → Přidat API klíč

**Použít:** `minimax/MiniMax-M2.1`

**Pro tip:** Nejlevnější nabídka pro dlouhý kontext (1M tokenů)!

### Kimi K2 (9 $/měsíc plochý)

1. Přihlásit: [Moonshot AI](https://platform.moonshot.ai/)
2. Získat API klíč
3. Dashboard → Přidat API klíč

**Použij:** `kimi/kimi-latest`

**Pro tip:** Měsíční platba 9 $ za 10 milionů tokenů = efektivní cena 0,90 $/1
milion!

</details>

<details>
<summary><b>🆓 FREE Providers (Emergency Backup)</b></summary>

### iFlow (5 přístupů zdarma prostřednictvím OAuth)

```bash
Ovládací panel → Připojení iFlow
→ Přihlášení k OAuth iFlow
→ Neomezené užití

Modely:
  if/kimi-k2-thinking
  if/qwen3-coder-plus
  if/glm-4.7
  if/minimax-m2
  if/deepseek-r1
```

### Qwen (4 přístupů zdarma prostřednictvím zátěže zařízení)

```bash
Ovládací panel → Připojení Qwen
→ Autorizace prostřednictvím kódu zařízení
→ Neomezené užití

Modely:
  qw/qwen3-coder-plus
  qw/qwen3-coder-flash
```

### Kiro (CLAUDE ZDARMA)

```bash
Ovládací panel → Připojení Kiro
→ AWS ID stavebního klapky nebo Googlu/GitHub
→ Neomezené užití

Modely:
  kr/claude-sonnet-4.5
  kr/claude-haiku-4.5
```

</details>

<details>
<summary><b>🎨 Create Combos</b></summary>

### Příklad 1: Maximální předplatné → Třetí strana

```
Ovládací panel → Kombinace → Nová kombinace

Název: premium-coding
Modely:
  1. cc/claude-opus-4-6 (Předplatné primární)
  2. glm/glm-4.7 (Třetí strana levnou, 0,60 $/1 milion)
  3. minimax/MiniMax-M2.1 (Drahá záloha, 0,20 $/1 milion)

Spolehlivost:
 premium-coding
```

### Příklad 2: Bezplatná kombinace (Nulová cena)

```
Název: free-combo
Modely:
  1. gc/gemini-3-flash-preview (180K měsíčně zdarma)
  2. if/kimi-k2-thinking (limitless)
  3. qw/qwen3-coder-plus (limitless)

Český finanční: 0 $ neskončí!
```

</details>

<details>
<summary><b>🔧 CLI Integration</b></summary>

### Cursor IDE

```
Nastavení → Modely → Pokročilé:
  Báze OpenAI API: http://localhost:20128/v1
  API klíč OpenAI: [z OmniRoute ovládacího panelu]
  Model: cc/claude-opus-4-6
```

### Claude Code

Použijte stránku **Nástroje CLI ** v ovládacím panelu pro jedno kliknutí, nebo
editujte `~/.claude/settings.json ` ručně.

### Codex CLI

```bash
export OPENAI_BASE_URL="http://localhost:20128"
export OPENAI_API_KEY="tvoj-omniroute-klíč API"

codex "Tvůj prompt"
```

### OpenClaw

**Volba 1 — Ovládací panel (doporučeno):**

```
Dashboard → nástroje CLI → OpenClaw → Vyberte model → Použij
```

**Volba 2 — Manuál:** Upravit soubor `~/.openclaw/openclaw.json`:

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

> **Poznámka:** OpenClaw funguje pouze s místním OmniRoute. Použijte
> ``127.0.0.1`` namísto ``localhost`` pro vyhnout se problémům při resoluci
> IPv6.

### Cline / Pokračovat / RooCode

```
Nastavení → Konfigurace API:
  Základ: OpenAI Kompatibilní
  Adresa URL: http://localhost:20128/v1
  API klíč: [ze OmniRoute rozhraní]
  Model: if/kimi-k2-thinking
```

### OpenCode

**Krok 1:** Přidat OmniRoute jako zákazníka sestaveny:

```bash
opencode
/connect
# Zvolte „Ostatní“ → Zadejte ID: „omniroute“ → Zadejte svůj klíč OmniRoute
```

**Krok 2:** Vytvořit/sdílet soubor ``opencode.json`` ve kořenovém adresáři
projektu:

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

**Krok 3:** Vyberte model v OpenCode:

```bash
/models
# Vyberte jakýkoli model OmniRoute ze seznamu
```

> **Tip:** Přidat jakýkoli model dostupný v rámci svého OmniRoute `/v1/models`
> pointu do sekce `models`. Použijte formát `zákazník/modelový ID` ze svého
> rozhraní OmniRoute.

</details>

---

## Odstraňování problémů

<details>
<summary><b>Click to expand troubleshooting guide</b></summary>

**„Models neposkytl žádné zprávy“**

- Limit množství provider → Zkontrolujte ukazatel kvóty dashboard
- Réseň: Použít kombinaci náhrad nebo přepojit se na levnější tarif

Kvantifikace připojení **

- Připojení odebráno → Použijte GLM/MiniMax.
- Přidat kombinaci: `cc/claude-opus-4-6 → glm/glm-4.7 → if/kimi-k2-začínající`

**Tokén OAuth vypršel**

- Auto-refreshed od OmniRoute
- Pokud se problémy přetrvávají: Ovládací panel → Provider → Pokytahovout

**Vysoké náklady**

- Zkontrolujte statistiky využití na Ovládacím panelu → Náklady
- Odvést primární model na GLM/MiniMax
- Použijte volné tary (Gemini CLI, iFlow) pro nekritické úkoly

**Ovládací panel/API porty jsou špatené**

- `PORT` je kánonický základní port (a port API výchozí)
- `API_PORT` přepne pouze otevřený API vyslědce kompatibilní s OpenAI
- `DASHBOARD_PORT` přepne pouze ovládací/Next.js vyslědce
- Nastavte `NEXT_PUBLIC_BASE_URL` na vaší ovládací/veřejné adresu URL (pro
  ověřování OAuth)

**Chyby synchronizace v cloudu**

- Ověřte, zda `BASE_URL` ukazuje na spuštěný okamžek
- Ověřte také, zda `CLOUD_URL` ukazuje na očekávaný koncový bod v cloudu
- Zachovejte `NEXT_PUBLIC_*` hodnoty v souladu s hodnotami na straně serveru

**První přihlášení nefunguje**

- Zkontrolujte `INITIAL_PASSWORD` v [.env]`
- Pokud není nastaveno, použije se fallback heslo `123456`

**Žádné záznamy o požadavcích**

- Set `POZVOLI Request Logy=true` v `.env`

**Prověrka připojení zobrazuje "Neplatný" ** pro poskytovatele kompatibilní s
OpenAI

- Mnoho poskytovatelů neexponuje `/models` bod ukončení
- OmniRoute v1.0.6+ zahrnuje pádové validaci prostřednictvím chatových dokončení
- Zajistěte, aby základová URL zahrnovala `/v1` příponu

### 🔐 Ověřování OAuth na vzdáleném Serveru

<a name="oauth-on-a-remote-server"></a> <a name="oauth-em-servidor-remoto"></a>

> **⚠️ Důležné pro uživatele spustující OmniRoute na VPS, Docker nebo
> kterémkolivzdáleném serveru**

#### Proč Selhání Antigravity / Gemini CLI OAuth na vzdálených serverech?

Poskytovatelé **Antigravity** a **Gemini CLI** používají **ověřování Google
OAuth 2.0**. Google vyžaduje, aby `redirect_uri` v toku ověřování přesně
souhlasil s jedním z registrovaných URI v aplikace console Google Cloud.

OAuth přihlašovací údaje přednastavené v OmniRoute jsou registrovány **jen na
`localhost`**. Jakmile se pokusíte o přístup k OmniRoute na vzdáleném serveru
(například `https://omniroute.mujserver.com`), Google odmítne ověření s chybou:

```
Chyba 400: nekonzistence redirect_uri
```

#### Řešení: Nastavte si vlastní přihlašovací údaje pro OAuth

Potřebujete vytvořit vlastní **OAuth 2.0 klienta ID** v Google Cloud Console se
URI svého serveru.

#### Krok za krokem

**1. Přihlaste se do Google Cloud Console**

Přejděte na:
[https://console.cloud.google.com/apis/credentials](https://console.cloud.google.com/apis/credentials)

**2. Vytvořte nový OAuth 2.0 klienta ID**

- Klikněte na **+ Vytvořit ověření"**→ **OAuth klienta ID"**
- Typ aplikace: **"Web aplikace"**
- Název: cokoliv vám bude líbit (např. `OmniRoute Remote`)

**3. Přidáno povolených Redirect URI**

V poli **Povoleny redirect URI**, přidejte:

```
https://vaš-server.com/callback
```

> Změňjte `https://vaš-server.com` na název nebo IP adresu vášho serveru (pokud
> potřebujete přidat port, používejte například
> `http://45.33.32.156:20128/callback`).

**4. Uložte a zkopírujte kredentials**

Po vytvoření zobrazí Google **ID klienta** a **tajný klient**.

**5. Nastavte prostředí proměnné**

V `.env` (nebo v proměnných containteru Docker):

```bash
# Pro Antigravity:
ANTIGRAVITY_OAUTH_CLIENT_ID=vaš-client-id.apps.googleusercontent.com
ANTIGRAVITY_OAUTH_CLIENT_SECRET=GOCSPX-vaš-secret

# Pro Gemini CLI:
GEMINI_OAUTH_CLIENT_ID=vaš-client-id.apps.googleusercontent.com
GEMINI_OAUTH_CLIENT_SECRET=GOCSPX-vaš-secret
GEMINI_CLI_OAUTH_CLIENT_SECRET=GOCSPX-vaš-secret
```

**6. Restartujte OmniRoute**

```bash
# npm:
npm run dev

# Docker:
docker restart omniroute
```

**7. Zkuste se znovu připojit**

Nástěnka → Poskytovatelé → Antigravity (nebo Gemini CLI) → OAuth

Google teď správně předá na `https://vaš-server.com/callback`.

---

#### Dočasná oprava (bez vlastní identifikace uživatele)

Pokud nechcete nastavovat vlastní přihlašovací údaje hned teď, můžete stále
použít **ruční odkaz na tok OAuth**:

1. OmniRoute otevře adresu Google s odběrem
2. Po autorizaci se Google snaží vrátit k `localhost` (což však selže nazdávaném
   serveru)
3. **Zkopírujte plnou adresní čáru** z odkazu ve vašem prohlížeči (i v případě,
   že stránka se nezabije)
4. Vložte tu adresní čáru do pole v okně při připojování k OmniRoute
5. Klikněte na **"Spojení"**

> Funkce běží porque kód autentizace v URL zůstává platný bez ohledu na to, zda
> se stránka s přesměrováním načte.

---

<details>
<summary><b>🇧🇷 Versão em Português</b></summary>

#### Proč selže OAuth Antigravity / Gemini CLI na vzdálených serverech?

Dodavatelé **Antigravity** a **Gemini CLI** používají **Google OAuth 2.0** pro
ověřování. Google vyžaduje, aby URL přesměrování `redirect_uri`, které je
použito v o autorizačním toku OAuth, **exaktě** odpovídal jednou z předem
registrovaných URI v Google Cloud Console aplikace.

OAuth pověření zabudovaná v OmniRoute jsou zaregistrována **vždy pouze pro
`localhost`**. Když se pokúšíte získat přístup k OmniRoute na vzdáleném serveru
(například `https://omniroute.meuservidor.com`), Google odmítne ověřenou
ověřování s touto zprávou:

```
Chyba 400: nekonzistence redirect_uri
```

#### Řešení: Konfigurovat vlastní pověření OAuth

Musíte vytvořit **OAuth 2.0 Client ID** v Google Cloud Console s URI svého
serveru.

#### Krok po kroku

**1. Přístup k Google Cloud Console**

Otevřete:
[https://console.cloud.google.com/apis/credentials](https://console.cloud.google.com/apis/credentials)

**2. Přidat nový OAuth 2.0 Client ID**

- Klikněte na **"+ Create Credentials"** → **"OAuth client ID"**
- Typ aplikace: **"Web application"**
- Název: vyberte kterýkoli název (například `OmniRoute Remote`)

**3. Přidat povolené Přesměrování URI

Do pole **"Authorized redirect URIs"**, zaškrtněte:

```
https://seu-servidor.com/callback
```

> Zaměňte `seu-servidor.com` se svým doménou nebo IP adresa serveru (zahrnující
> číslo portu pokud je vyžadováno, například
> `http://45.33.32.156:20128/callback`)

**4. Uložit a zkopírovat pověření

Po vytvoření bude Google přinutě zobrazit **Klient ID** a **Klient Secret**.

**5. Konfigurace môištění

Váš `.env` soubor (nebo prostředí aplikací Docker):

```bash
ANTIGRAVITY_OAUTH_CLIENT_ID=vaš-služební ID klienta.apps.googleusercontent.com
ANTIGRAVITY_OAUTH_CLIENT_SECRET=GOCSPX-vaše-zakázané tajemství

GEMINI_OAUTH_CLIENT_ID=vaš-služební ID klienta.apps.googleusercontent.com
GEMINI_OAUTH_CLIENT_SECRET=GOCSPX-vaše-zakázané tajemství
GEMINI_CLI_OAUTH_CLIENT_SECRET=GOCSPX-vaše-zakázané tajemství
```

**6. Restartujte OmniChannel **

```bash
# V případě použití npm:
npm run dev

# V případě použití Docker:
docker restart omniroute
```

**7. Pokuste se připojit znovu**

Nástěnka → Dodavatelé → Antigravity (nebo Gemini CLI) → OAuth

Google teď bude řádně připojovat uživatelů na
`https://vaše-servářní.com/callback` a autentizace by měla fungovat.

---

#### Dočasný rozjezd (bez vlastní konfigurace ověřování)

Pokud nechtěte vytvořit své vlastní pověření nyní, ještě stále můžete použít
**ruční instrukce URL**:

1. Omniroute otevře adresu Google ke schválení
2. Po vašem schválení Google pokusí připojovat zpět uživatelů na `localhost` (co
   způsobí selhání na vzdáleném serveru)
3. **Zkopírujte adresu URL plnou na adresní řádku vašeho prohlížeče (stejným
   způsobem, i když stránka nebude načtena)
4. Zadejte takovou adresu do pole, které se objeví v modalovém dialogu spojení
   Omniroutem
5. Klikněte na **"Připojit"**

> Tento trik funguje proto, že kód žádosti o souhlas v adrese URL by měl platit
> samy o sobě, nezávisle na úspěchu připojení.

</details>

---

</details>

## 🛠️ Budova technologie

<details>
<summary><b>Click to expand tech stack details</b></summary>

- **Runtime**: Node.js 18–22 LTS (⚠️ Node.js 24+ nelze **podporovat** — nativní
  binární kód pro knihovnu better-sqlite3 nefunguje)
- **Jazyk**: TypeScript 5.9 — **100% TypeScript** napříč `src/` a `open-sse/`
  (žádné `any` v rámci jádra modulů od verze 2.0)
- **Framewokr**: Next.js 16 + React 19 + Tailwind CSS 4
- **Báze údajů**: LowDB (JSON) + SQLite (stavy domény + proxy logy + MCP audit +
  rozhodnutí trasy)
- **Schema**: Zod (vlastní nástroje MCP I/O validace, API smlouvy)
- **Pravidla komunikace**: MCP (stdio/HTTP) + A2A v0.3 (JSON-RPC 2.0 + SSE)
- **Proučování**: Server-Sent Events (SSE)
- **Autentizace**: OAuth 2.0 (PKCE) + JWT + API klíče + MCP skopení autentizace
- **Testování**: Node.js test runner + Vitest (900+ testů včetně jednotkových,
  integrací, E2E)
- **CI/CD**: GitHub Actions (auto npm publikovat + Docker Hub na relace)
- **Webová stránka**: [omniroute.online](https://omniroute.online)
- **Balíček**:
  [npmjs.com/package/omniroute](https://www.npmjs.com/package/omniroute)
- **Docker**:
  [hub.docker.com/r/diegosouzapw/omniroute](https://hub.docker.com/r/diegosouzapw/omniroute)
- **Odolnost**: Circuity brány, exponentiální úprava zpět, proti-záhadě
  shromáždění, únik z TLS, samo-zlepšení sebe-záchrany

</details>

---

## Dokumentace

| Dokument                                             | Popis                                                           |
| ---------------------------------------------------- | --------------------------------------------------------------- |
| [Ruční průvodce](docs/USER_GUIDE.md)                 | Dodavatelé, komba, integrační příkazový řádek, nasazení         |
| [Referenční API](docs/API_REFERENCE.md)              | Všichni příchozí s příklady názvů                               |
| [MCP Server](open-sse/mcp-server/README.md)          | 16 nástrojů MCP, IDE konfigurace, klienti Python/TS/Go          |
| [A2A Server](src/lib/a2a/README.md)                  | JSON-RPC 2.0 protokol, schopnosti, streamování, zásahy v řízení |
| [Auto-Kombinační Motor](docs/auto-combo.md)          | Šest-faktorové skórování, módní balíčky, samozáchranářství      |
| [Návod na řešení chyby](docs/TROUBLESHOOTING.md)     | Obvyklé problémy a jejich řešení                                |
| [Architektura](docs/ARCHITECTURE.md)                 | Systémová architektura a interní mechanismy                     |
| [Pravidla přispívání](CONTRIBUTING.md)               | Nastavení vývojářů a praktické návod                            |
| [Specifikace OpenAPI](docs/openapi.yaml)             | Specifikace OpenAPI 3.0                                         |
| [Záklona pro bezpečnost](SECURITY.md)                | Zpracování bezpečnostních incidentů a praktiky zabezpečení      |
| [Rozložení VM](docs/VM_DEPLOYMENT_GUIDE.md)          | Kompletní návod k rozložení VM + nginx + Cloudflare             |
| [Galerie funkcí](docs/FEATURES.md)                   | Přehledná vizuální ukázka rozhraní s obrázky                    |
| [Kontrolní seznam vydání](docs/RELEASE_CHECKLIST.md) | Kroky před úplným vydání                                        |

---

## 🗺️ Plán podniku

OmniRoute nyní počítá s **210+ funkcemi naplánovanými pro ** na více fázi
vývoje. Zde jsou klíčové směry:

| Kategorie                    | Plánované funkce | Highlighty                                                                                                |
| ---------------------------- | ---------------- | --------------------------------------------------------------------------------------------------------- |
| ️💡 **Routing & inteligence** | 25+              | Nejnízší-latentní routing, tag-based routing, úvodní ověřování kvót, výběr účtů P2C                       |
| 🔒 **Bezpečnost & soulad**    | 20+              | Hardening SSRF, skrývání přihlašovacích údajů, omezení rychlosti na koncovém bodu, rozsahové klíče správy |
| 📊 **Náhodnost**              | 15+              | Integrace OpenTelemetry, reálné monitorování kvót, sledování nákladů podle modelu                         |
| 🔄 **Integrace dodavatelů**   | 20+              | Dynamická registry modelů, cooldowny dodavatelů, multiaccount Codex, parsovat kvóty Copilotu              |
| ⚡ **Výkonnost**              | 15+              | Dvouúrovňový cache, cache prompts, cache odezvy, aktivace trvalé komunikace, batch API                    |
| 🌐 **Ecosystem**              | 10+              | WebSocket API, horké zátOPY konfigurace, distribuovaný úložiště konfigurace, komerční režim               |

### Již brzy

- 🔗 **Integrace OpenCode** — Příchozí podporu pro IDE kódování OpenCode AI
- 🔗 **Integrace TRAE** — Kompletní podpora kódovací framework AI TRAE
- 📦 **Batch API** — Asynchronní zpracování balíčku požadavků
- 🎯 **Tag-Based Routing** — Routed požadavky na základě zadaných štítků a
  metadata
- 💰 **Nízkonákladová strategie** — Automaticky si vyberte nejnižší dostupnou
  dodavatele

> 📝 Plné specifikace dostupné v
> [`dokumenty/neuvodny-vysvetlivka/`](docs/new-features/) (217 podrobných
> specifikací)

---

## 👥 Spisovatelé

[![Spisovatelé](https://contrib.rocks/image?repo=diegosouzapw/OmniRoute&max=100&columns=20&anon=1)](https://github.com/diegosouzapw/OmniRoute/graphs/contributors)

### Jak se zapojit do přispívání

1. Pochopte si repository
2. Vytvořte si kmenovou větüven ( `git checkout -b feature/amazing-feature` )
3. Zapsat své změny ( `git commit -m 'Pridejte si vynikající funkcionalitu'` )
4. Push vámi odvodilé změny ( `git push origin feature/amazing-feature` )
5. Otevřete pull vyžádání

Prohlédněte si [[CONTRIBUTING.md](CONTRIBUTING.md)] pro podrobný návod.

### Nové verzi verze

```bash
# Vytvořte si verzi — okamžité publikování
gh release create v2.0.0 --title "v2.0.0" --generate-notes
```

---

## 📊 Histories hvězdiček

## Chytráci hvězdiček

## [![Chytráci hvězdiček](https://starchart.cc/diegosouzapw/OmniRoute.svg?variant=adaptive)](https://starchart.cc/diegosouzapw/OmniRoute)

## 🙏 Děkujeme

Velmi děkuji **[9router](https://github.com/decolua/9router)** by
**[decolua](https://github.com/decolua)** — projekt, který byl zdrojem inspirace
pro tento větev. OmniRoute staví na založení této zázračné podoby s přidáním
nových funkce, multimodálními API a kompletní překladem TypeScript.

Děkuji vám ** [CLIProxyAPI](https://github.com/router-for-me/CLIProxyAPI)** —
originální Go, který založil tento JavaScriptový překlad.

---

## 📄 Licencě

Licence MIT - podrobnosti najdete v souboru [LICENSE](LICENSE).

---

<div align="center">
  <sub>Built with ❤️ for developers who code 24/7</sub>
  <br/>
  <sub><a href="https://omniroute.online">omniroute.online</a></sub>
</div>
<!-- GitHub Discussions enabled for community Q&A -->
