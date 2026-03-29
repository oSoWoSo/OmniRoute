# 🚀 OmniRoute — Der kostenlose AI-Gateway

### Nie aufhören, zu coden. intelligentes Routing für **KOSTENLOSRAGEN & kostenlose AI-Modelle** mit automatischer Fallback-Vorschrift.

_Ihr universeller API-Proxy — ein Endpoint, 67+ Anbieter, null Ausfallzeiten.
Jetzt mit** MCP & A2A ** Agenten-Orchestrierung._

**Chat-Erweiterungen • Embeddings • Bildgenerierung auf Anforderung • Video •
Musik • Audio • UMWERTEN • **Suche im Web** • MCP-Server • A2A-Protokoll • 100%
TypeScript**

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
[![Lizenz](https://img.shields.io/github/license/diegosouzapw/OmniRoute)](https://github.com/diegosouzapw/OmniRoute/blob/main/LICENSE)
[![Website](https://img.shields.io/badge/Website-omniroute.online-blue?logo=google-chrome&logoColor=white)](https://omniroute.online)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-Community-25D366?logo=whatsapp&logoColor=white)](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

[🌐 Website](https://omniroute.online) • [🚀 Schnelle Anfertigung](#-quick-start)
• [💡 Merkmalen](#-key-features) • [📖 Dokumentation](#-documentation) • [💰
Preise](#-pricing-at-a-glance) • [💬
WhatsApp](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

</div>

🌐 **Verfügbar auf:** 🇺🇸 [Englisch](README.md) | 🇧🇷 [Portugiesisch
(Brasilien)](docs/i18n/pt-BR/README.md) | 🇪🇸 [Español](docs/i18n/es/README.md) |
🇫🇷 [Français](docs/i18n/fr/README.md) | 🇮🇹 [Italien](docs/i18n/it/README.md) |
🇷🇺 [Русский](docs/i18n/ru/README.md) | 🇨🇳 [中文 (简体)](docs/i18n/zh-CN/README.md) |
🇩🇪 [Deutsch](docs/i18n/de/README.md) | 🇮🇳 [हिन्दी](docs/i18n/in/README.md) | 🇹🇭
[ไทย](docs/i18n/th/README.md) | 🇺🇦 [Українська](docs/i18n/uk-UA/README.md) | 🇸🇦
[العربية](docs/i18n/ar/README.md) | 🇯🇵 [日本語](docs/i18n/ja/README.md) | 🇻🇳 [Tiếng
Việt](docs/i18n/vi/README.md) | 🇧🇬 [Български](docs/i18n/bg/README.md) | 🇩🇰
[Dansk](docs/i18n/da/README.md) | 🇫🇮 [Suomi](docs/i18n/fi/README.md) | 🇮🇱
[עברית](docs/i18n/he/README.md) | 🇭🇺 [Magyar](docs/i18n/hu/README.md) | 🇮🇩
[Bahasa Indonesia](docs/i18n/id/README.md) | 🇰🇷 [한국어](docs/i18n/ko/README.md) |
🇲🇾 [Bahasa Melayu](docs/i18n/ms/README.md) | 🇳🇱
[Nederlands](docs/i18n/nl/README.md) | 🇳🇴 [Norsk](docs/i18n/no/README.md) | 🇵🇹
[Portugiesisch (Portugal)](docs/i18n/pt/README.md) | 🇷🇴
[Română](docs/i18n/ro/README.md) | 🇵🇱 [Polski](docs/i18n/pl/README.md) | 🇸🇰
[Slovenčina](docs/i18n/sk/README.md) | 🇸🇪 [Svenska](docs/i18n/sv/README.md) | 🇵🇭
[Filipino](docs/i18n/phi/README.md) | 🇨🇿 [Čeština](docs/i18n/cs/README.md)

---

## 🆕 Was ist Neues in v3.0.0

> ** Upgrade von v2.9.5?** — Sehen Sie sich die[ komplette
> Änderungshistorie](CHANGELOG.md#300--2026-03-22-release-candidate--not-yet-merged-to-main)
> zum überall im Text fasslichen Änderung.

| Bereich                            | Änderung                                                                                                                                                                                                               |
| ---------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🔒 **CodeQL-Sicherheit**            | Fehler von 10+ CodeQL-Alerts: polynomial-redos, unzureichende Zufallszahlen, remediation für shell-injection: fixed                                                                                                    |
| ✅ **Route-Validierung**            | Alle 176 API-Routen werden nun mit Zod-Schemen validiert + `validateBody()` – CI- `Überprüfung:route-validation:t06` erfüllt                                                                                           |
| 🐛 **omniModel-Tags-Schleuderung**  | Interne `<omnimodel>`-Tags werden innerhalb von SSE-Streamingantworten nicht mehr an Kunden weitergegeben (#585)</omnimodel>                                                                                           |
| 🔑 **Registrierte Schlüssel-API**   | API-Schlüssel bereitstellen, indem Sie `post /api/v1/registered-keys` verwenden, wobei eine pro-Anbieter/Account-Quotenregelung, -Idempotenz,-SHA-256-Speicherung und optional GitHub-issue-Berichterstattung erfolgt. |
| 🎨 **Anbieter-Icons**               | 130+ Anbieter-Logos via `@lobehub/icons` (SVG) mit PNG → generischer Fall zurückkettungskette                                                                                                                          |
| 🔄 **Modell Auto-Sync**             | 24-Stunden-Scheduler und manueller GUI-Schalter, um Modellliste für eingebaute und benutzerdefinierte OpenAI-kompatible Anbieter synchron zu stellen                                                                   |
| 🌐 **OpenCode Zen/Go**              | Zwei neue Anbieter von Kang Heewon via PR #530: kostenlose Ebene + Abonnementsebene via `OpencodeExecutor`                                                                                                             |
| 🐛 **Gemini CLI OAuth**             | Interaktive Fehlermeldung, wenn `GEMINI_OAUTH_CLIENT_SECRET` im Docker-Container fehlt (war ursprünglich verschlüsselte Google-Fehlermeldung)                                                                          |
| 🐛 **OpenCode-Konfiguration**       | `saveOpenCodeConfig()` speichert nun korrekt TOML in `XDG_CONFIG_HOME`                                                                                                                                                 |
| 🐛 **Pinned-Modell-Überschreibung** | `body.model` wird nun korrekt auf `pinnedModel` auf der Kontext-Cache-Schutz gelegt                                                                                                                                    |
| 🐛 **Codex/Claude-Schleife**        | `tool_result`-Blöcke werden nun in Text umgewandelt, um Endlosschleifen zu verhindern                                                                                                                                  |
| 🐛 **Login-Routereintritt**         | Der Login verharrt nicht mehr aufgrund der übersprungenen Passwort-Einstellung                                                                                                                                         |
| 🐛 **Windows-Pfade**                | MSYS2/Git-Bash-Pfade (`/c/...`) werden auf `C:\...` automatisch normalisiert                                                                                                                                           |

---

## 🖼️ Hauptdashboard

<div align="center">
  <img src="./docs/screenshots/MainOmniRoute.png" alt="OmniRoute Dashboard" width="800"/>
</div>

---

## 📸 Dashboard-Vorschau

<details>
<summary><b>Click to see dashboard screenshots</b></summary>

| Seite                  | Bildschirmfoto                                       |
| ---------------------- | ---------------------------------------------------- |
| **Anbieter**           | ![Anbieter](docs/screenshots/01-providers.png)       |
| **Kombos**             | ![Kombos](docs/screenshots/02-combos.png)            |
| **Analytics**          | ![Analytics](docs/screenshots/03-analytics.png)      |
| **Gesundheit**         | ![Gesundheit](docs/screenshots/04-health.png)        |
| **Übersetzer**         | ![Übersetzer](docs/screenshots/05-translator.png)    |
| **Einstellungen**      | ![Einstellungen](docs/screenshots/06-settings.png)   |
| **CLI-Tools**          | ![CLI-Tools](docs/screenshots/07-cli-tools.png)      |
| **Nutzungsprotokolle** | ![Nutzungsprotokolle](docs/screenshots/08-usage.png) |
| **Endpunkte**          | ![Endpunkte](docs/screenshots/09-endpoint.png)       |

</details>

---

### Roboter 🤖 Free AI Provider for your favorite Coding Agenten

_Jeden beliebigen AI-gesteuerten IDE oder CLI-Tool über OmniRoute — Kostenlos
API-Gateway für unbeschränkten Coding._

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

<sub>📡 Alle Agenten verbinden sich über <code>http://localhost:20128/v1</code>
oder <code>http://cloud.omniroute.online/v1</code> — eine Konfiguration,
unbeschränkte Modelle und Quote</sub>

---

## 🤔 Warum OmniRoute?

**Vermeiden Sie es, sich um Geld Sorgen zu machen und Limits zu erreichen:**

- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Abgelaufene Abonnementquoten verfallen ungenutzt jeden Monat
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Grenzwerte verhindern, dass Sie mitten in der Codierung platzen
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Kostenlose APIs ($20-50/monat pro Anbieter)
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Manuelle Wechsel zwischen Anbietern

**OmniRoute löst diesen:**

- ✅ **Maximieren der Abonnements** - Quotenverfolgung, nutzen Sie jeden Bit,
  bevor Sie zurückgegeben wird
- ✅ **Fehler-Toleranz** - Abonnement → API-Schlüssel → Prepaid → Kostenlos,
  nahtlose Downtime
- ✅ **Multi-Konto** - Abwechselnd zwischen Konten pro Anbieter
- ✅ **Universal** - Funktioniert mit Claude Code, Codex, Gemini CLI, Cursor,
  Cline, OpenClaw, jedem CLI-Tool

---

## 📧 Unterstützung

> 💬 **Betreten Sie unsere Community!**
> [WhatsApp-Gruppe](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)
> — Hilfe, Tipps teilen und sich auf dem Laufenden halten.

- **Website**: [omniroute.online](https://omniroute.online)
- **GitHub**:
  [github.com/diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute)
- **Issue**:
  [github.com/diegosouzapw/OmniRoute/issues](https://github.com/diegosouzapw/OmniRoute/issues)
- **WhatsApp**:
  [Community-Gruppe](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)
- **Beitragende**: Siehe [CONTRIBUTING.md](CONTRIBUTING.md), öffnen Sie einen PR
  oder wählen Sie ein `gutes Erstes Issue`
- **Original Projekt**: [9router by decolua](https://github.com/decolua/9router)

### 🐛 Fehlermeldugen melden?

Wenn Sie ein Problem melden, bitten wir Sie, den Befehl system-info auszuführen
und das generierte Datei anzuhängen:

```bash
npm run system-info
```

Dies generiert eine `system-info.txt` mit Ihrer Node.js-Version,
OmniRoute-Version, OS-Details, installierten CLI-Tools (iflow, gemini, claude,
codex, antigravity, droid, usw.), Docker/PM2-Zustand und -anwendungen – alles,
was wir brauchen, um Ihre Probleme schnell nachzubilden. Hängen Sie die Datei
direkt an Ihrer GitHub-Aktivität an.

---

## Wie es funktioniert

```
┌─────────────┐
│  Ihre CLI-   │  (Claude Code, Codex, Gemini CLI, OpenClaw, Cursor, Cline...)
│   Tool      │
└──────┬──────┘
       │ http://localhost:20128/v1
       ↓
┌─────────────────────────────────────────┐
│           OmniRoute (Intelligenter Router) │
│  • Format-Umwandlung (OpenAI ↔ Claude) │
│  • Quotenverfolgung + Embeddings + Bilder │
│  • Auto-Token-Vorschub                  │
└──────┬──────────────────────────────────┘
       │
       ├─→ [Schicht 1 SUBSCRIPTION] Claude Code, Codex, Gemini CLI
       │   ↓ Quotenablauf
       ├─→ [Schicht 2 API SCHLÜSSEL] DeepSeek, Groq, xAI, Mistral, NVIDIA NIM, usw.
       │   ▼ Budgetlimit
       ├─→ [Schicht 3 CHEAP] GLM (0,6 $/1M), MiniMax (0,2 $/1M)
       │   ↓ Budgetlimit
       └─→ [Schicht 4 KOSTENLOS] iFlow, Qwen, Kiro (unbegrenzt)

Ergebnis: Das Koden bleibt stehen, minimalen Kosten
```

---

## 🎯 Was OmniRoute löst – 30 reale Schmerzpunkte & Use-Cases

> **Jeder Entwickler, der auf AI-Tools zurückgreift, trifft auf diese Probleme
> täglich.** OmniRoute wurde entwickelt, um sie alle zu lösen – von
> Kostenüberschreitungen bis hin zu regionalen Blockaden, von kaputten
> OAuth-Flügen bis hin zu Protocol-Verfahren und Enterprise-Beobachtung.

<details>
<summary><b>💸 1. "I pay for an expensive subscription but still get interrupted by limits"</b></summary>

Entwickler zahlen 20–200 $/Monat für Claude Pro, Codex Pro oder GitHub Copilot.
Auch beim Zahlen liegt eine Leistungsgrenze – 5 h Sitzung, wöchentliche Grenzen
oder Leistungszeitlimits pro Minute. Im Bauschritt ist der Anbieter nicht mehr
zugänglich und der Entwickler verliert den Durchblick und Produktivitätsverlust.

**Wie OmniRoute es löst:**

- **Intelligente 4-Schicht Rücksprung** – Wenn die Abonnement-Quoten auslaufen,
  wechselt automatisch zu API-SCHLÜSSEL -> Cheap -> KOSTENLOS mit null Manuell
  Intervention
- **Echtzeit-Quotenverfolgung** – Zeigt den Token-Verbrauch in Echtzeit mit
  Zählerabruf (5h, täglich, wöchentlich)
- **Mehrfachkonto-Unterstützung** – Mehrere Konten pro Anbieter mit Auto-Wechsel
  – wenn eines ausgeht, wechselt es auf das nächste
- **Benutzerdefinierte Combinations** – Benutzerdefinierte Rücksprungketten mit
  6 Balance-Strategien (fill-first, round-robin, P2C, random, least-used,
  cost-optimiert)
- **Codex Geschäftsquoten** – Geschäfts-/Team-Arbeitsplatz-Quotenüberwachung
  direkt im Dashboard

</details>

<details>
<summary><b>🔌 2. "I need to use multiple providers but each has a different API"</b></summary>

OpenAI verwendet einen Format, Claude (Anthropic) einen anderen, Gemini einen
anderen. Wenn ein Entwickler die Modelle aus verschiedenen Anbietern testen oder
zwischen ihnen umschalten möchte, müssen sie die SDKs neu konfigurieren, die
Endpunkte ändern und mit inkompatiblen Formaten kämpfen. Benutzerdefinierte
Anbieter (FriendLI, NIM) haben nicht-standardmäßige Model-Endpunkte.

**Wie OmniRoute es löst:**

- **Gemeinsame Endpunkt** – Ein einziger `http://localhost:20128/v1` stellt sich
  als Proxy für alle 67+ Anbieter dar
- **Format-Umwandlung** – Automatische und transparente Umwandlung: OpenAI ↔
  Claude ↔ Gemini ↔ Antworten- API
- **Antwortbereinigung** — Entfernt nicht-standardmäßige Felder (`x_groq`,
  `usage_breakdown`, `service_tier`) die OpenAI SDK v1.83+ stören
- **Rollenvernetzung** — Konvertiert `Entwickler` → `System` für
  nicht-OpenAI-Anbieter; `System` → `Benutzer` für GLM/ERNIE
- **Think-Tag-Extraktion** — Extrahiert `<think>` -Blöcke aus Modellen wie
  DeepSeek R1 in standardisierte `reasoning_content`</think>
- **Strukturierte Ausgabe für Gemini** — `json_schema` →
  `responseMimeType`/`responseSchema` automatische Konvertierung
- **`stream` standardmäßig auf `false`** — Passt sich der OpenAI-Spezifikation
  an, um unerwartete SSE in Python/Rust/Go-SDKs zu vermeiden

</details>

<details>
<summary><b>🌐 3. "My AI provider blocks my region/country"</b></summary>

Anbieter wie OpenAI/Codex sperren Zugriff aus bestimmten geografischen Regionen.
Benutzer erhalten error-Code wie `unsupported_country_region_territory` während
der Authentifizierung und API-Verbindungen. Dies ist besonders frustrierend für
Entwickler aus Entwicklungsländern

**Wie OmniRoute es löst:**

- **Proxy-Konfiguration auf 3 Ebenen** — Konfigurierbare Proxy auf 3 Ebenen:
  Globale (alle Verkehr), pro Anbieter (eine Anbieter pro) und pro
  Verbindung/Schlüssel
- **Farbliche Proxy-Badges** — Visuelle Indikatoren: 🟢 globale Proxy, 🟡
  Provinizer-Proxy, 🔵 Verbindungssproxy, immer der IP-Anzeige
- **OAuth-Token-Übertragung über Proxy** — OAuth-Flow geht auch über den Proxy,
  löst `unsupported_country_region_territory`
- **Verbindungstests über Proxy** — Verbindungstests verwenden den
  konfigurierten Proxy (keine mehr direkte Umgehung)
- **SOCKS5-Unterstützung** — Vollständige SOCKS5-Proxy-Unterstützung für den
  Ausgabeverkehr
- **TLS-Fingerprint-Spoofing** — Browserartige TLS-Fingerabdruck Übertragung via
  `wreq-js`, um Bot-Detektion zu umgehen
- **🔏 CLI-Fingerprint-Matching** — Ändert den Header- und Body-Feldernordnung,
  um native CLI-Binärsignaturen zu matchen, schränkt die Konto-Fahnen-Kenner
  stark ein. Bei gleichzeitiger Proxy-IP-Preservierung erhalten Sie simultanes
  **Schlund** und IP-Schatten

</details>

<details>
<summary><b>🆓 4. "I want to use AI for coding but I have no money"</b></summary>

Nicht jeder kann 20-200 US-Dollar pro Monat für AI-Abo-Zahlungen bezahlen.
Studenten, Entwickler aus Entwicklungsländern, Freiberufler und Hobbyisten
benötigen Zugriff auf Qualität-Modelle zu Null-osten Kosten

**Wie OmniRoute es löst:**

- **Free-Tier-Anbieter-Aufbau** — Ingebauter Support für 100 %-Free-Anbieter:
  iFlow (5 unabdingbare Model-Kompatibilität via OAuth: kimi-k2-thinking,
  qwen3-coder-plus, deepseek-r1, minimax-m2, kimi-k2), Qwen (4 unabdingbare
  Model-Kompatibilität: qwen3-coder-plus, qwen3-coder-flash, qwen3-coder-next,
  vision-model), Kiro (Claude + AWS BauwerwerKonto ID für freie), Gemini CLI
  (180K Tokens/Monateau gratis)
- **Ollama-Cloud** — Cloud-besetzte Ollama-Modelle unter `api.ollama.com` mit
  "Light Gebrauch" kostenlosem-Tarif ; Gebraucht `ollamacloud/<model>`
  Präfix</model>
- **Freibetrag-Kombis** — Kettet `gc/gemini-3-flash → if/kimi-k2-thinking →
  qw/qwen3-coder-plus` = 0 USD/Monat mit Null-Störigkeit
- **NVIDIA NIM Kostengunst-X-Kostenfaktor** — ~40 RPM dev-free Kosten-Zugriff
  auf 70+ Modelle an build.nvidia.com (Wechsel von Krediten auf
  Reklamente-Limits)
- **Kostenoptimierte Strategie** — Routenstrategie, die den günstigsten
  verfügbaren Anbieter automatisch auswählt

</details>

<details>
<summary><b>🔒 5. "I need to protect my AI gateway from unauthorized access"</b></summary>

Wenn man ein AI-Gateway dem Netzwerk (LAN, VPS, Docker) aussetzt, kann jeder mit
der Adresse das Token/Budget des Entwicklers konsumieren. Ohne eine
Schutzmaßnahme sind APIs für Missbrauch, Injecting von Prompt und Abusen
verletzlich.

**Wie OmniRoute es löst:**

- **API-Schlüsselverwaltung** — Erzeugung, -rotation und -Scope pro Anbieter mit
  einem eigenen `/Dashboard/Api-Manager`-Seite
- **Modellrechte auf der Ebene** — Einschränken von API-Schlüsslingen auf
  spezifische Modelle (`openai/*`, Stern-Wildcarte), mit
  zulassen/beschränken-Schalter
- **API-Endpunkt-Schutz** — Anforderung eines Schlüssels für `/v1/models` und
  sperren Sie bestimmte Anbieter vom Abschreibung
- **AuthGuard + CSRF-Schutz** — Alle Routen im Dashboard besitzt mit
  `withAuth`-Middleware + CSRF-Token geschützt
- **Rateschwellenbeschräncker** — Eines-IP- Schwellenbeschränker mit
  konfigurierbaren Fenstern
- **IP-Filter** — Allowlisten/Blocklisten für die Kontrollzugriff
- **Prompt-Injecting-Wächter** — Sanitization gegen üble Prompt-Muster
- **AES 256 GCM-Verschlüsselung** — Anforderungen verschlüsselt bei Ruhezustand

</details>

<details>
<summary><b>🛑 6. "My provider went down and I lost my coding flow"</b></summary>

AI-Anbieter können instabil werden oder 5xx Fehler zurückliefern, zufällige
Rate-Änderung, oder temporären Limits. Wenn ein dev auf einen einzelnen Anbieter
abhängig ist, werden sie unterbrochen. Ohne die Unterbrecher, wiederholte
Versuche, die Anwendung zu schmelzen

**Wie OmniRoute es löst:**

- **Circuit-Breaker-proz-model** — Automatik-Offen/ Schließen-Schwellenwerte-
  und Abkühlzeit (Offen/Geschlossen/Hälfte-Offen), skaliert proz-model-Model um
  Fassaden blocken
- **Exponential-Backoff** — progressive-schrittweite Versuche, verzögert
  verluste
- **Anti-Stürmchen** — Mutex + semapore-Schutz gegen Einer-Übergreifung
- **Kombination-Notausgänge** — Wenn der Primär-Anbieter versagt, fällt der
  schienweite Verbindung durch den Kettenwechsel automatisch mit keiner
  Intervention
- **Kombination-Unterbrecher** — Auto-Ünaktivieren der versagenden Anbieter in
  einer Kombinati-Chenwertewechsel
- **Gesundheitssteuerpost** — Uptimmonitor, Schwellenüberschreitung-State,
  Sperrenstatistiken, p50/p95/p99 Latenz

</details>

<details>
<summary><b>🔧 7. "Configuring each AI tool is tedious and repetitive"</b></summary>

Entwickler nutzen Cursor, Claude Code, Codex-CLI, OpenClaw, Gemini-CLI, Kilo
Code, Jeder Tool benötigt eine unterschiedliche Konfiguration (API Endpunkt,
Schlüssel, Model). Wiederealisieung, wenn zwischen Anbietern oder Modeln
gewechselt wird, ist Zeitverschwendung.

**Wie OmniRoute es löst:**

- **Dashboard für CLI-Tools** — Dedicatede Seite mit einem-Klick-Setzeup für
  Claude Code, Codex CLI, OpenClaw, Kilo Code, Antigravity, Cline
- **GitHub Copilot-Config-Generator** — Generiert `chatLanguageModels.json` für
  VS-Code mit großem Modellauswahl
- **Einführungs-Assistent** — Leiteter 4-stufiges Setzeup für Neuanwender
- **Ein Endpoint, alle Modelle** — Configure `http://localhost:20128/v1` einmal,
  Zugang zu 67+ Providern

</details>

<details>
<summary><b>🔑 8. "Managing OAuth tokens from multiple providers is hell"</b></summary>

Claude Code, Codex, Gemini CLI, Copilot — alle verwenden OAuth 2.0 mit
ablaufenden Tokens. Entwickler müssen ständig wiederhin autorisieren, Probleme
mit `fehlender client_secret`, `übersprungenem redirect_uri` und Fehlern auf
Remote-Servern auftreten lassen. OAuth auf LAN/VPS ist besonders schwierig.

**Wie OmniRoute es löst:**

- **Auto Token Refresh** — OAuth-Tokens werden im Hintergrund vor dem Ablauf
  automatisch erneuert
- **OAuth 2.0 (PKCE) Built-in** — Automatischer Flow für Claude Code, Codex,
  Gemini CLI, Copilot, Kiro, Qwen, iFlow
- **Multi-Account OAuth** — Mehrere Accounts pro Anbieter via
  JWT-ID-Zertifikat-Erstellung
- **OAuth LAN/Remote-Fix** — Erkennung privater IP-Adressen für `redirect_uri` +
  manuelles URL-Modus für Remote-Servern
- **OAuth hinter Nginx** — Verwendung von `window.location.origin` für
  Umkehrproxy-Kompatibilität
- **Remote OAuth-Leitfaden** — Schritt-für-Schritt-Anleitung für
  Google-Cloud-Zertifikate auf VPS/Docker

</details>

<details>
<summary><b>📊 9. "I don't know how much I'm spending or where"</b></summary>

Entwickler verwenden mehrere bezahlte Anbieter, haben jedoch keinen
einheitlichen Überblick über die Ausgaben. Jeder Anbieter hat seinen eigenen
Budget-Überblick, aber es gibt keinen konsolidierten Überblick. Unvorhergesehene
Kosten können sich stapeln.

**Wie OmniRoute es löst:**

- **Kostenanalyse-Dashboard** — Kostenverfolgung pro Token und Budgetmanagement
  pro Anbieter
- **Budgetlimits pro Schicht** — Ausgabenbeschränkung pro Schicht, die
  automatische Umleitung auslöst
- **Prazise Modell-Konfiguration pro Modell** — Konfigurierbare Preise pro
  Modell
- **Benutzungsstatistiken pro API-Schlüssel** — Anfordere-zahl und letzter
  verwendeter Timestamp pro Schlüssel
- **Analyse-Dashboard** — Statistenkarten, Modellverwendung-Stammwert,
  Anbieter-Tabellen mit Erfolgsraten und Verzögerungen

</details>

<details>
<summary><b>🐛 10. "I can't diagnose errors and problems in AI calls"</b></summary>

==WEBLATE_PART==\
[Benachrichtigungen bei fehlenden Aufrufen] Informieren Sie sich nicht darüber,
ob es sich um eine Ratebegrenzung, um einen abgelaufenen Token, um einen
falschen Format, oder um einen Fehler des Anbieters handelt. Ohne Beobachtung
ist das Debuggen eine Zufallsprobing.

**Wie OmniRoute es löst:**

- **Konsolendashboards für Eiern** — 4 Tabellen: Anforderungsprotokolle,
  Proxyprotokolle, Auditprotokolle, Konsolen
- **Konsole-Lesezeichenansicht** — Echtzeit-Lesezeichen-Ansicht mit
  farbcodierten Ebenen, Auto-Vertikalliegen, Suchen, Filtern
- **SQLite-Proxypython Script** — Persistente Protokolle, die über
  Serverneustarts überleben
- **Translator-Playground** — 4 Debug-Modi: Playground (Format-Übersetzung),
  Chat-Tester (Zweirichtungsprüfung), Testbrett (Ausführung), Live-Monitor
  (Echtzeit)
- **Anforderungstelemetrie** — p50/p95/p99 Latenzen +
  X-Beitrag-Id-Nachverfolgung
- **Dateibasierter Logging mit Rotation** — Konsoleninterceptor hat alles auf
  JSON-Belieferung mit Größengesteuerte Rotation
- **System-Info-Report** — `npm system-Info ausführen` generiert
  `system-Info.txt` mit Ihrem vollständigen Umfeld (Node-Version,
  OmniRoute-Version, Betriebssystem, CLI-Tools, Docker/PM2-Status). Attachieren
  Sie sie beim Melden von Problemen zur einstweiligen Überprüfung.

</details>

<details>
<summary><b>🏗️ 11. "Deploying and maintaining the gateway is complex"</b></summary>

Die Installation, Konfiguration und Wartung eines AI-Proxys in verschiedenen
Umgebungen (lokal, VPS, Docker, Cloud) sind zeitaufwändig. Probleme wie
hardecodierte Pfads, `EACCES ` auf Verzeichnisses, Portkonflikte und
plattformübergreifende Builds verhindern den Prozess.

**Wie OmniRoute es löst:**

- **NPM-Globale Installation** — `npm install -g omniroute &amp;&amp; omniroute`
  — abgeschlossen
- **Docker-Mehrdrehsysteme** — AMD64 + ARM64 nativ (Apple-Silicon, AWS-Graviton,
  Raspberry-Pi-Treiber)
- **Docker-Komponennt-Profiles** — ` basic` (ohne CLI-Tools) und `cli` (mit
  Claude-Code, Codex, Openclaw)
- **Elektron-Desktop-App** — Native-Anwendung für Windows/macOS/Linux mit
  Systemeinschluss, automatischer Start, Offline-Modus
- **Multiport-Modus** — Anbieter und Dashboard auf separaten Ports für
  erweiterte Szenarien (rückwärts Komponenten Verbindungen)
- **Cloud-Synchronisierung** — Konfigurationssynchronisierung über Geräte über
  Cloudflare-Arbeiter
- **Backups von Datenbanken** — Automatische Sicherung, Wiederherstellung,
  Export und Import aller Betriebsparameter

</details>

<details>
<summary><b>🌍 12. "The interface is English-only and my team doesn't speak English"</b></summary>

In Nicht-Anglophonen-Ländern, insbesondere in Lateinamerika, Asien und Europa,
haben die Teams Schwierigkeiten mit den englischsprachigen Oberflächen.
Sprachbarrieren reduzieren Adoptionen und erhöhen Konfigurationfehler.

**Wie OmniRoute es löst:**

- **Benutzeroberfläche i18n — 30 Sprachen** — Alle 500+ Schlüssel wurden
  übersetzt, einschließlich Arabisch, Bulgarisch, Dänisch, Deutsch, Spanisch,
  Finnisch, Französisch, Hebräisch, Hindi, Ungarisch, Indonesisch, Italienisch,
  Japanisch, Koreanisch, Maley, Niederländisch, Norwegisch, Polnisch,
  Portugiesisch (PT/BR), Rumänisch, Russisch, Slowakisch, Schwedisch, Thai,
  Ukrainisch, Vietnamesisch, Chinesisch, Filipino, Englisch
- **RTL-Support** — Rechtsschreibunterstützung für Arabisch und Hebräisch
- **Multi-Language READMEs** — 30 umfassende Dokumentationen
- **Sprachensteller** — Globus-Symbol im Header für Echtzeit-Wechsel

</details>

<details>
<summary><b>🔄 13. "I need more than chat — I need embeddings, images, audio"</b></summary>

AI ist nicht nur Chatvollkommenheit. Entwickler brauchen, um Bilder zu
generieren, Audiobänder zu transkribieren, Embeddings für RAG zu erstellen,
Dokumente wiederzuordnen und Inhalte zu modifizieren. Jeder API hat einen
anderen Endpunkt und eine andere Formatierung.

**Wie OmniRoute es löst:**

- **Embeddings** — `/v1/embeddings` mit 6 Providern und 9+ Modellen
- **Bildschneidewerk** — `/v1/images/generation` mit 10 Providern und 20+
  Modellen (OpenAI, xAI, Together, Fireworks, Nebius, Hyperbolic, NanoBanana,
  Antigravity, SD WebUI, ComfyUI)
- **Text-in-Video** — `/v1/videos/generation` — ComfyUI (AnimateDiff, SVD) und
  SD WebUI
- **Text-in-Musik** — `/v1/music/generation` — ComfyUI (Stabile Audio Offen,
  Musikgenerator)
- **Audiobandstranskription** — `/v1/audio/transkription` — Whisper + Nvidia
  NIM, HuggingFace, Qwen3
- **Text-zu-Sprache** — `/v1/audio/sprache` — ElevenLabs, Nvidia NIM,
  HuggingFace, Coqui, Tortoise, Qwen3, **Inworld**, **Cartesia**, **PlayHT**, +
  bestehende Anbieter
- **Inhaltsmoderation** — `/v1/morderation` — Inhaltsicherheitsprüfungen
- **Wiederauffaltung** — `/v1/wiederauf` — Dokumentrelevanzwiederauffaltung
- **Response API** — Vollständige `/v1/response` - Unterstützung für Codex

</details>

<details>
<summary><b>🧪 14. "I have no way to test and compare quality across models"</b></summary>

Entwickler wollen wissen, welches Modell am besten zu ihrem Verwendungszweck
passt – Codeerzeugung, Übersetzung, Logik – aber das manuelle Vergleichen ist
langsam. Es existieren keine integrierten Bewertungstools.

**Wie OmniRoute es löst:**

- **LLM-Bewertungen** — Goldsatzprüfungen mit 10 vorbeoaderfassenen Szenarien,
  die Grußworte, Matheoperation, Geografie, Codeerzeugung, JSON-Konformität,
  Übersetzung, Markdown, Sicherheitsweigerung beinhalten
- **4 Übereinstimmungsstrategie** — `genauer`, `enthält`, `Regex`,
  `Benutzerdefiniert` (JS Funktion)
- **Benutzerinterface-Testfeld** — Batcherprobung mit mehreren Eingaben und
  erwarteten Output-Werten, Kreuzlieferungsvergleich zwischen Anbietern
- **Chat-Tester** — Vollständiger Rundweg mit visueller Antwortanzeige
- **Live-Monitor** — Echtzeit-Ström von allen Durchführungen, die durch den
  Proxy fließen

</details>

<details>
<summary><b>📈 15. "I need to scale without losing performance"</b></summary>

Mit steigendem Anfragenvolumen generieren die gleichen Fragen ohne
Zwischenspeicherung Duplikate an Kosten. Ohne Idempotenz verschwenden Duplikate
bei der Verarbeitung Ressourcen. Die Ratenbeschränkungen jedes Anbieters müssen
beachtet werden.

**Wie OmniRoute es löst:**

- **Semantic-Cache** — Zweistufiges Caching (Signatur + semantisch) reduziert
  Kosten und Latenzzeit
- **Request-Idempotenz** — 5s-Duplikationsfenster für identische Anfragen
- **Ratenbegrenzungserkennung** — Ratenpro-Kennzahlen, Mindestpuffer und
  maximale Konkurrenz-Angabe pro Anbieter
- **Bearbeitbare Ratenbegrenzungen** — Konfigurierbare Standards in
  Einstellungen → Resilienz mit Persistenz
- **API-Schlüssel-Validierungs-Zwischenspeicher** — 3-Tier-Zwischenspeicher für
  Produktionsleistung
- **Gesundheitsdashboard mit Wetterdaten** — p50/p95/p99 Latenzzeit,
  Cachestatistiken, Auslastung

</details>

<details>
<summary><b>🤖 16. "I want to control model behavior globally"</b></summary>

Entwickler, die alle Antworten in einer bestimmten Sprache wollen, eine
bestimmte Tonalität bevorzugen oder die Vermittler-Tokens limitieren möchten,
ist die Konfiguration in jedem Werkzeug oder Anfrage unmöglich.

**Wie OmniRoute es löst:**

- **System-Prompt-Erprobung** — Globale Einführung von Hinweisen für alle
  Anfragen
- **Gedankenzuweisungsbewertung** — Kontrolle der Vermittler-Tokens pro Anfrage
  (Durchgang, automatisch, benutzerdefiniert, adaptiv)
- **6 Routenstrategien** — Globale Strategien, die bestimmen, wie Anfragen
  verteilt werden
- **Wildcard-Router** — `Provider/*` Muster senden dynamisch an jeden Provider
- **Kombinations-Ermöglichung/Löschung-Toggle** — Kombinationen können direkt
  vom Dashboard direkt aktiviert oder deaktiviert werden
- **Anbieter-Toggle** — Alle Anbieter mit einem Klick aktivieren/deaktivieren
- **Blockierte Anbieter** — Spezifische Anbieter aus der `/v1/models`-Auflistung
  ausschließen

</details>

<details>
<summary><b>🧰 17. "I need MCP tools as first-class product capabilities"</b></summary>

Viele AI-Gateway-Implementierungen offenbaren den MCP nur als versteckte
Implementationsdetails. Teams benötigen einen sichtbaren und managierbaren
Betriebszustand.

**Wie OmniRoute es löst:**

- MCP erscheint in der Oberflächenavigation und in der
  Abschnittsprotokoll-Tabelle
- Dedikierter MCP-Verwaltungsbereich mit Prozess, Werkzeugen, Umgebungen und
  Audit
- Eigene Schnellstart-Funktion für `omniroute --mcp` und Client-Registrierung

</details>

<details>
<summary><b>🧠 18. "I need A2A orchestration with sync + stream task paths"</b></summary>

Benutzerarbeitsabläufe benötigen sowohl direkte Antworten als auch lang dauernde
gestreamte Ausführung mit Lebenszyklussteuerung.

**Wie OmniRoute es löst:**

- A2A-JSON-RPC-Endpunkt (`POST /a2a`) mit `nachricht/send` und
  `nachricht/stream`
- SSE-Streaming mit Terminalzustand ausbreitung
- Aufgabenlebenszyklus-APIs für `aufgaben/abrufen` und `aufgaben/stornieren`

</details>

<details>
<summary><b>🛰️ 19. "I need real MCP process health, not guessed status"</b></summary>

Betriebsaufgaben benötigen wissen, ob MCP tatsächlich lebendig ist und nicht
nur, ob eine API erreichbar ist.

**Wie OmniRoute es löst:**

- Echtzeit-Herzfrequenzdatei mit PID, Zeitstempeln, Transport, Werkzeuganzahl
  und Umgebungsmodus
- MCP-Zustands-API, die Herzfrequenz + jüngste Aktivität kombiniert
- UI-Zustandskarten für Prozess/Arbeitszeit/Herzfrequenz-Neuigkeit

</details>

<details>
<summary><b>📋 20. "I need auditable MCP tool execution"</b></summary>

Wird Werkzeuge Konfiguration ändern oder opskript-Aktionen auslösen, benötigen
Teams forensische Nachvollziehbarkeit.

**Wie OmniRoute es löst:**

- SQLite-basierte Audit-Log-Datei für MCP-Werkzeugaufrufe
- Filter auf Werkzeug, Erfolg/Schaden, API-Schlüssel und Paginierung
- Dashboard-Audit-Tabelle + Statistik-Endpunkte für Automation

</details>

<details>
<summary><b>🔐 21. "I need scoped MCP permissions per integration"</b></summary>

Verschiedene Clients sollten beim Werkzeugkategorien Zugriff mit geringsten
Rechten haben.

**Wie OmniRoute es löst:**

- 9 granular MCP Scopes für steuerbare Zugriffszugriffs-zugriff
- Umfangsentfaltung und -sichtbarkeit in der MCP-Verwaltungsoberfläche
- Sichere Standard-Postur für operative Werkzeuge

</details>

<details>
<summary><b>⚙️ 22. "I need operational controls without redeploying"</b></summary>

Teams benötigen schnelle Änderungen während der Ausfallereignisse oder
Kostenevents.

**Wie OmniRoute es löst:**

- Kombinations-Schaltfläche Aktivierung direkt von der MCP-Dashboard-Oberfläche
- Wiedergabe von Ausfallsicherheitsprofile aus vorgegebenen Richtliniendateien
- Zuweisung von Aufschaltzerstörszenarien von derselben Betriebsansicht

</details>

<details>
<summary><b>🔄 23. "I need live A2A task lifecycle visibility and cancellation"</b></summary>

Ohne Lebenszyklus-Übersichtigkeit werden Aufgabenereignisse schwer
durchschaubar.

**Wie OmniRoute es löst:**

- Nachschau von Aufgabenlisten/Filtrierung nach Zustand/Fähigkeit mit
  Pagerwechsel
- Aufschlüsselung von Aufgabendaten Ereignissen und Artefakten
- Aufgabenabbestellung-Endpunkt und UI-Aktion mit Bestätigung

</details>

<details>
<summary><b>🌊 24. "I need active stream metrics for A2A load"</b></summary>

Strömungsbetrieb erfordert operative Einblicke in Konkurrenz und lebendige
Verbindungen.

**Wie OmniRoute es löst:**

- Aktive Schaltflächeninhalte zur Überprüfung innerhalb der A2A-Status-Angaben
- Letzte Aufgabestempelung und pro-Zustand-Zähler
- A2A-Dashboardkarten zum Echtzeitanzeige für die operative Monitoring

</details>

<details>
<summary><b>🪪 25. "I need standard agent discovery for clients"</b></summary>

externe Clienten und Orchestrator benötigen maschinenlesbare Metadaten für die
Einschreibung.

**Wie OmniRoute es löst:**

- Agent-Karte öffnet `/.well-known/agent.json`
- Fähigkeiten und Fertigkeiten werden in der Management-Oberfläche gezeigt
- A2A-Status-API enthält Entdeckungsdaten für die Automatisierung

</details>

<details>
<summary><b>🧭 26. "I need protocol discoverability in the product UX"</b></summary>

Wenn Benutzer die Protokolloberflächen nicht entdecken können, sinkt die
Annahme- und Unterstützungsqualität.

**Wie OmniRoute es löst:**

- Gemeinsame **-Endpunkte-X24X] Seite mit Rechertabs für Proxy, MCP, A2A und
  API-Endpunkte
- Offline-Status-Taster direkt in den MCP- und A2A-Diensten (Online/Offline)
- Übergeordnete Links zu dedizierten Management-Tabs

</details>

<details>
<summary><b>🧪 27. "I need end-to-end protocol validation with real clients"</b></summary>

Mocktests sind nicht ausreichend, um die Protokollkompatibilität vor der
Veröffentlichung zu validieren.

**Wie OmniRoute es löst:**

- E2E-Suite, die die App startet und das reale MCP-SDK-Client-Transport
  verwendet
- A2A-Klient-Tests für Entdeckung, senden, streamen, abrufen und widerrufen
- Überprüfung von Behauptungen gegenüber MCP-Audit- und A2A-Tasks-APIs

</details>

<details>
<summary><b>📡 28. "I need unified observability across all interfaces"</b></summary>

Unterteilung der Beobachtbarkeit nach Protokollen schafft Blinde Flecken und
eine längere MTTR.

**Wie OmniRoute es löst:**

- Einheits-Überwachungsdashboards/logs/analytics in einem Produkt
- Gesundheit + Audit + Anforderungstelemetrie über alle OpenAI-, MCP- und
  A2A-Schichten
- Operationale APIs für Status und Automatisierung

</details>

<details>
<summary><b>💼 29. "I need one runtime for proxy + tools + agent orchestration"</b></summary>

Durch Betrieb vieler separater Dienste steigt der operative Aufwand und
Fehlermodi.

**Wie OmniRoute es löst:**

- Eines konsistenten Proxys, MCP-Servers und A2A-Servers in einem Stack
- Weite Verwendung von Authentifizierung, Resilienz, Datenbank und Observability
- Konsistenter Policy-Modell über allen Interaktionsflächen

</details>

<details>
<summary><b>🚀 30. "I need to ship agentic workflows without glue-code sprawl"</b></summary>

Teams verlieren an Geschwindigkeit, wenn sie mehrere ad-hoc-Dienste und Scripts
zu verschachteln haben.

**Wie OmniRoute es löst:**

- Einsatzstrategie für einheitliche Endpunkte für Kunden und Agenten
- Eingebaute Management-UIs für Protokolle und schmutzige Validierungswege
- Produktionsreife Grundlagen (Sicherheit, Protokollierung, Resilienz, Backup)

</details>

### Beispiel-Playbooks (Integrierte Use Cases)

**Playbook A: Maximiere bezahlte Abonnements und kostengünstiges Backup**

```txt
Kombination: "maximiere-klausel"
  1. cc/claude-opus-4-6
  2. glm/glm-4.7
  3. if/kimi-k2-denkend

Monatlicher Kosten: $20 + geringer Backup-Aufwand
Ausgänge: erhöhte Qualität, nahe Null-Störung
```

**Playbook B: Kostengünstige Kompilationsschicht**

```txt
Kombination: "kostenlos-immer"
  1. gc/gemini-3-flasche
  2. if/kimi-k2-denkend
  3. qw/qwen3-coder-plus

Monatlicher Kosten: $0
Ausgänge: stabilere kostenlose Kompilation
```

**Playbook C: Störungsfreie 24/7-Ausfallkette**

```txt
Kombination: "immer-on"
  1. cc/claude-opus-4-6
  2. cx/gpt-5.2-codex
  3. glm/glm-4.7
  4. minimax/MiniMax-M2.1
  5. if/kimi-k2-denkend

Ausgänge: tiefer Ausfalltiefe für Fristenkritische Last
```

**Playbook D: Agent-OPs mit MCP und A2A**

```txt
1) Starte Transport MCP (`omniroute --mcp`) für tool-getriebene Operationen
2) Läuft A2A-Aufgaben über `message/send` und `message/stream`
3) Beobachte via /dashboard/endpoint (MCP- und A2A-Tabs)
4) Aktiviere Dienste via Inline-Statussteuerungen
```

---

## 🆓 Starte kostenlos – Null-Konfiguration-Kosten

> Setup AI-Verschachtelung in Minuten zu **0 $/Monat**. Verbinde diese
> kostenlosen Konten und nutze die verbaute **kostenlose Schicht** Kombination.

| Schritt | Aktion                                                | Anbieter freigeschaltet                                               |
| ------- | ----------------------------------------------------- | --------------------------------------------------------------------- |
| 1       | Verbinden **Kiro** (AWS Builder-ID OAuth)             | Claude Sonnet 4.5, Haiku 4.5 — **unbegrenzt**                         |
| 2       | Verbinden **iFlow** (Google OAuth)                    | kimi-k2-denkprozeß, qwen3-coder-plus, deepseek-r1... — **unbegrenzt** |
| 3       | Verbinden **Qwen** (Gerät-Code)                       | qwen3-coder-plus, qwen3-coder-Flash... — **unbegrenzt**               |
| 4       | Verbinden **Gemini CLI** (Google OAuth)               | gemini-3-Flash, gemini-2.5-Pro — **180K/Stunde kostenlos**            |
| 5       | `/dashboard/combos` → **Freie Stack (0 $)** - Vorlage | Runden alle kostenlosen Anbieter automatisch ab                       |

**Belege zur Ide / CLI an: ** `http://localhost:20128/v1` · API-Schlüssel:
`jeder-String` · Fertig.

> **Optional: kostenlose Zusatzabdeckung (auch kostenlos): **Groq-API-Schlüssel
> (30 RPM kostenlos), NVIDIA NIM (40 RPM kostenlos, 70+ Modelle), Cerebras (1M
> tok/Tag), LongCat-API-Schlüssel (50M Token/Tag!), Cloudflare-Workers-AI (10K
> Neuronen/Tag, 50+ Modelle).

## Schnellstart

### 1. Installieren und ausführen

```bash
npm install -g omniroute
omniroute
```

> **pnpm Benutzer:** Führen Sie nach der Installation `pnpm
> genehmigen-baubeschlüsse -g` aus, um native Bauanweisungen für
> `better-sqlite3` und `@swc/core` zu aktivieren:
> 
> ```bash
> pnpm install -g omniroute
> pnpm genehmigen-baubeschlüsse -g   # Alle Pakete auswählen → genehmigen
> omniroute
> ```

Die Benutzeroberfläche öffnet sich unter `http://localhost:20128` und die API-
Basis-URL ist `http://localhost:20128/v1`.

| Befehl                  | Beschreibung                                                       |
| ----------------------- | ------------------------------------------------------------------ |
| `omniroute`             | Server starten (`PORT=20128`, API und Dashboard auf gleicher Port) |
| `omniroute --port 3000` | Kanonen-Port auf 3000 setzen                                       |
| `omniroute --mcp`       | MCP-Server starten (stdio-Transport)                               |
| `omniroute --no-open`   | Browser nicht automatisch öffnen                                   |
| `omniroute --help`      | Hilfe anzeigen                                                     |

Optionaler Spalten-Port-Modus:

```bash
PORT=20128 DASHBOARD_PORT=20129 omniroute
# API:       http://localhost:20128/v1
# Dashboard: http://localhost:20129
```

### 1) Verbinden Sie Anbieter und erstellen Sie Ihre API-Schlüsselfolge

1. Öffnen Sie das Dashboard ↣ `Anbieter` und verbinden Sie mindestens einen
   Anbieter (OAuth oder API-Schlüssel).
2. Öffnen Sie das Dashboard ↣ `Endpunkte` und erstellen Sie eine API-Schlüssel.
3. (Optional) Öffnen Sie das Dashboard ↣ `Combos` und setzen Sie Ihre
   Ausfallschematik.

### 2) Verbinden Sie Ihre Entwicklungswerkzeug mit OmniRoute

```txt
URL: http://localhost:20128/v1
API-Schlüssel: [kopieren Sie es von der Seite Endpunkte]
Modell:   wenn/kimi-k2-denkend (oder jeder Anbieter/Modell vorstrich)
```

Kompatibel mit Claude Code, Codex CLI, Gemini CLI, Cursor, Cline, OpenClaw,
OpenCode und OpenAI-kompatiblen SDKs.

### 3) Aktivieren und validieren Sie die Protokolle (v2.0)

**MCP (für Werkzeug-gesteuerte Operationen):**

```bash
omniroute --mcp
```

Verbinden Sie dann Ihre MCP-Klient über `stdio` und testen Sie Werkzeuge wie:

- `omniroute_get_health`
- `omniroute_list_combos`

**A2A (für Agent-zu-Agent-Abläufe):**

```bash
curl http://localhost:20128/.well-known/agent.json
```

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"quickstart","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"Geben Sie mir eine kurze Quotenübersicht."}]}}'
```

### 4) Testen Sie alles vom Ende zum Ende (empfohlen)

```bash
npm run test:protocols:e2e
```

Dieses Suite validiert reale MCP- und A2A-Klient-Flüsse gegen eine laufende
Anwendung.

### Alternative: Aus den Quellen ausführen.

```bash
cp .env.example .env
npm install
PORT=20128 DASHBOARD_PORT=20129 NEXT_PUBLIC_BASE_URL=http://localhost:20129 npm run dev
```

---

## 🐳 Docker

OmniRoute ist als öffentliche Docker-Image auf {Docker
Hub}(https://hub.docker.com/r/diegosouzapw/omniroute) verfügbar.

**Schnelle Anleitung:**

```bash
docker run -d \
  --name omniroute \
  --restart unless-stopped \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:latest
```

**Mit Umgebungsdatei:**

```bash
# Kopieren Sie und bearbeiten Sie .env zuerst
cp .env.example .env

docker run -d \
  --name omniroute \
  --restart unless-stopped \
  --env-file .env \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:latest
```

**Mit Docker Compose:**

```bash
# Basis-Profil (keine CLI-Tools)
docker compose --profile base up -d

# CLI-Profil (Claude Code, Codex, OpenClaw eingebaut)
docker compose --profile cli up -d
```

| Bild                     | Version  | Größe  | Beschreibung             |
| ------------------------ | -------- | ------ | ------------------------ |
| `diegosouzapw/omniroute` | `latest` | ~250MB | Letzter stabiler Release |
| `diegosouzapw/omniroute` | `1.0.3`  | ~250MB | Aktuelle Version         |

---

## 🖥️ Desktop-Anwendung — Offline & immer an

> 🆕 **NEU!** OmniRoute ist jetzt als **Desktop-Anwendung** für Windows, macOS
> und Linux verfügbar.

Starten Sie OmniRoute als eigenständige Desktop-Anwendung – ohne Terminal,
Browser oder Internet sind lokale Modelle nicht erforderlich. Die auf Electron
basierende App enthält:

- 🖥️ **Eigenes Fenster** – dedizierte App-Fenster mit Systemtray-Integration
- 🔄 **Automatisches Starten** – Starts OmniRoute bei Systemanmeldung
- 🔔 **Native Benachrichtigungen** – erhält Benachrichtigungen für
  Quotenverbrauch oder Anbieterprobleme
- ⚡ **Eines-Klick-Installieren** – NSIS (Windows), DMG (macOS), AppImage (Linux)
- 🌐 ** Offline-Modus** – funktioniert vollständig offline mit eingebetteter
  Server-Ausführung

### Schnellstart

```bash
# Entwicklermodus
npm run electron:dev

# Bereite deine Plattform auf

npm run electron:build         # aktuelle Plattform
npm run electron:build:win     # Windows (.exe)
npm run electron:build:mac     # macOS (.dmg) — x64 &amp; arm64
npm run electron:build:linux   # Linux (.AppImage)
```

### Systemtray

Wenn man minimiert, lebt OmniRoute in Ihrem Systemtray mit schnell aufrufbaren
Aktionen:

- Öffnen Sie das Dashboard
- Serverport ändern
- Anwendung beenden

📖 Vollständige Dokumentation: [`electron/README.md`](electron/README.md)

---

## 💰 Eine rasche Übersicht über die Preise

| Tarif               | Anbieter                   | Kosten                                 | Quoten-Zyklus                                                  | Best For                                   |
| ------------------- | -------------------------- | -------------------------------------- | -------------------------------------------------------------- | ------------------------------------------ |
| **💳 ABO**           | Claude-Code (Pro)          | $20/Monat                              | 5h + wöchentlich                                               | Schon abonniert                            |
|                     | Codex (Plus/Pro)           | $20-$200/Monat                         | 5h + wöchentlich                                               | OpenAI-Nutzer                              |
|                     | Gemini CLI                 | **KOSTENLOS**                          | 180T/Monat + 1T/Tag                                            | Allen!                                     |
|                     | GitHub-Copilot             | $10-$19/Monat                          | Monatlich                                                      | GitHub-Nutzer                              |
| **🔑 API-SCHLÜSSEL** | NVIDIA NIM                 | **KOSTENLOS** (entwickler für immer)   | ~40 Umdrehungen pro Minute                                     | 70+ offene Modelle                         |
|                     | Cerebras                   | **gratis** (1M Token Tag/day)          | 60.000 Transaktions pro Minute / 30 Umdrehungen pro Minute     | Schnellstes der Welt                       |
|                     | Groq                       | **gratis** (30 Umdrehungen pro Minute) | 14.400 Echtzeit-Präzisions-Produktivitäts-Metriken pro Sekunde | Ultra-schnelle Llama/Gemma                 |
|                     | DeepSeek V3.2              | 0,27$/1,10 pro 1M                      | Keine                                                          | Bester Preis-Leistungs-Verhältnis-Grund    |
|                     | xAI Grok-4 Schnell         | **0,20$/0,50 pro 1M** 🆕                | Keine                                                          | Schnellster + Werkzeugaufruf, ultralow     |
|                     | xAI Grok-4 (standard)      | 0,20$/1,50 pro 1M 🆕                    | Keine                                                          | Flaggschiff-Denken des xAI                 |
|                     | Mistral                    | Freie Probe + kostenpflichtig          | Preis begrenzt                                                 | europäische KI                             |
|                     | OpenRouter                 | Zahlagetragt                           | Keine                                                          | Mehr als 100 Modelle zu einem Satz         |
| **💰 CHEAP**         | GLM-5 (per Z.AI) 🆕         | 0,50 $/1 Mio.                          | Täglich 10 AM                                                  | 128 K Output, Flaggschiff der Neuigkeiten  |
|                     | GLM-4.7                    | 0,60 $/1 Mio.                          | Täglich 10 AM                                                  | Budget-Backup                              |
|                     | MiniMax M2.5 🆕             | 0,30 $/1 Mio. Input                    | 5-stündige Welle                                               | Argumentation + agenteische Aufgaben       |
|                     | MiniMax M2.1               | $0,20/1M                               | 5-stündige Welle                                               | Billigster Option                          |
|                     | Kimi K2.5 (Moonshot API) 🆕 | Zahlagetragt                           | Keine                                                          | Direkter Zugriff auf die Moonshot-API      |
|                     | Kimi K2                    | $9,00/mo Ebene                         | 10 Mio. Token/mo                                               | Prädiktiver Kosten                         |
| **🆓 KOSTENLOS**     | iFlow                      | **$0**                                 | Unbegrenzt                                                     | 5 Modelle unbegrenzt                       |
|                     | Qwen                       | **$0**                                 | Unbegrenzt                                                     | 4 Modelle unbegrenzt                       |
|                     | Kiro                       | **$0**                                 | Unbegrenzt                                                     | Claude Sonnet/Haiku (AWS Builder)          |
|                     | LongCat Flash-Lite 🆕       | **$0** (50 Mio. Tok/day 🔥)             | 1 RPS                                                          | Das größte kostenlose Kontingent auf Erden |
|                     | Pollinations AI 🆕          | **$0** (ohne Schluessel notwendig)     | 1 Anfrage pro 15s                                              | GPT-5, Claude, DeepSeek, Llama 4           |
|                     | Cloudflare Workers AI 🆕    | **$0** (10K Neuronen/Tag)              | ~150 Antworten/Tag                                             | 50+ Modelle, globale Edge                  |
|                     | Scaleway AI 🆕              | **$0** (1M Token insgesamt)            | Preis begrenzt                                                 | EU/GDPR, Qwen3 235B, Llama 70B             |

> 🆕 **Neue Modelle hinzugefügt (März 2026):** Grok-4 Fast Familie für
> $0,20/0,50/Tag (gestuft an 1143ms – 30% schneller als Gemini 2.5 Flash), GLM-5
> über Z.AI mit 128K Ausgabe, MiniMax M2.5 reasoning, DeepSeek V3.2
> aktualisierte Preise, Kimi K2.5 über Moonshot direkte API.

**💡 $0 Kombistapel — Der Vollständige kostenlose Setup:**

```
# 🆓 Ultimatives kostenlose Stapel 2026 — 11 Provider, $0 für immer
Kiro (kr/)         → Claude Sonett/Haikunetz UNLIMITED
iFlow (if/)         → kimi-k2-denking, qwen3-coder-plus, deepseek-r1 UNLIMITED
LongCat Lite (lc/)  → LongCat-Flash-Lite – 50M Token je Tag 
Pollinations (pol/)→ GPT-5, Claude, DeepSeek, Llama 4 – kein Schluessel notwendig
Qwen (qw/)          → qwen3-coder-plus, qwen3-coder-Flash, qwen3-coder-nächst UNLIMITED
Gemini (gemini/)     → Gemini 2.5 Flash – 1,500 Anfragen pro Tag kostenlos API-Schluessel
Cloudflare AI (cf/)  → Llama 70B, Gemma 3, Mistral – 10K Neuronen/Tag
Scaleway (scw/)     → Qwen3 235B, Llama 70B – 1M kostenlose Token (EU)
Groq (groq/)         → Llama/Gemma ultra-leicht – 14,4K Anfragen pro Tag
NVIDIA NIM (nvidia/)→ 70+ offene Modelle – 40 RPM für immer
Cerebras (cerebras/) → Llama/Qwen welt-schnell – 1M-Tok/Tag
```

**Kein Kosten. Nie aufhör coden.** Konfigurieren diesen als einen
OmniRoute-Kombistapel und alle Fallbacks tun sich automatisch – keine manuelle
Abtastung erforderlich.

---

---

## 🆓 Kostenlose Modelle — Was Du genau bekommst

> Alle Modelle unten sind **100% kostenlos mit keiner Kreditkarte
> erforderlich**. OmniRoute routet sich automatisch zwischen ihnen um, wenn das
> eine Kontingent aufgebraucht ist – kombinieren sie alle für einen
> unzerbrechlichen $0-Kombistapel.

### 🔵 CLAUDE-MODELLE (via Kiro – AWS-Builder-Schluessel)

| Modell              | Präfix | Obergrenze     | Ratenbegrenzung                    |
| ------------------- | ------ | -------------- | ---------------------------------- |
| `claude-sonnet-4.5` | `kr/`  | **Unbegrenzt** | Keine tägliche Obergrenze gemeldet |
| `claude-haiku-4.5`  | `kr/`  | **Unbegrenzt** | Keine tägliche Obergrenze gemeldet |
| `claude-opus-4.6`   | `kr/`  | **Unbegrenzt** | Letztes Opus über Kiro             |

### 🟢 IFlow-Modelle ( Kostenloser OAuth-Konto — Keine Kreditkarte notwendig)

| Modell             | Präfix | Obergrenze     | Ratenbegrenzung           |
| ------------------ | ------ | -------------- | ------------------------- |
| `kimi-k2-denken`   | `if/`  | **Unbegrenzt** | Keine Obergrenze gemeldet |
| `qwen3-Coder-Plus` | `if/`  | **Unbegrenzt** | Keine Obergrenze gemeldet |
| `deepseek-r1`      | `if/`  | **Unbegrenzt** | Keine Obergrenze gemeldet |
| `minimax-m2.1`     | `if/`  | **Unbegrenzt** | Keine Obergrenze gemeldet |
| `kimi-k2`          | `if/`  | **Unbegrenzt** | Keine Obergrenze gemeldet |

### 🟡 GERAT MODELS (Gerät Code Auth)

| Modell              | Präfix | Obergrenze     | Ratenbegrenzung           |
| ------------------- | ------ | -------------- | ------------------------- |
| `qwen3-Coder-Plus`  | `qw/`  | **Unbegrenzt** | Keine Obergrenze gemeldet |
| `qwen3-coder-flash` | `qw/`  | **Unbegrenzt** | Keine Obergrenze gemeldet |
| `qwen3-coder-next`  | `qw/`  | **Unbegrenzt** | Keine Obergrenze gemeldet |
| `vision-model`      | `qw/`  | **Unbegrenzt** | Multimodal (Bilder)       |

### 🟣 GEMINI CLI (Google OAuth)

| Modell                    | Präfix | Obergrenze                                          | Ratenbegrenzung      |
| ------------------------- | ------ | --------------------------------------------------- | -------------------- |
| `Gemini-3-Flash-Vorschau` | `gc/`  | **180.000 Token pro Monat / + 1.000 Token pro Tag** | Monatlicher Neustart |
| `Gemini-2.5-Pro`          | `gc/`  | 180.000 Token pro Monat (geteilter Pool)            | Hohe Qualität        |

### ⚫ NVIDIA Nim (Kostenloser API-Schlüssel — build.nvidia.com)

| Tarif                  | Tageslimit             | Ratenbegrenzung | Notizen                                                                                    |
| ---------------------- | ---------------------- | --------------- | ------------------------------------------------------------------------------------------ |
| Kostenlos (Entwickler) | Keine Token-Begrenzung | **~40 RPM**     | 70+ Modelle; Umstellung auf reine Leistungsfähigkeitsgrenzen in der Hälfte des Jahres 2025 |

Beliebte kostenlose Modelle: `moonshotai/kimi-k2.5` (Kimi K2.5), `z-ai/glm4.7`
(GLM 4.7), `deepseek-ai/deepseek-v3.2` (DeepSeek V3.2),
`nvidia/llama-3.3-70b-instruct`, `deepseek/deepseek-r1`

### ⚪ CEREBRAS (Kostener API-Schlüssel — inference.cerebras.ai)

| Tarif     | Tageslimit         | Ratenbegrenzung                                            | Notizen                                                 |
| --------- | ------------------ | ---------------------------------------------------------- | ------------------------------------------------------- |
| Kostenlos | **1M Tokenen/Tag** | 60.000 Transaktions pro Minute / 30 Umdrehungen pro Minute | Weltweit Schnellste Inferenz von LLM; tägliche Neustart |

Verfügbar kostenlos: `llama-3.3-70b`, `llama-3.1-8b`,
`deepseek-r1-distill-llama-70b`

### 🔴 GROQ (Kostenloser API-Schlüssel — console.groq.com)

| Tarif     | Tageslimit    | Ratenbegrenzung  | Notizen                                             |
| --------- | ------------- | ---------------- | --------------------------------------------------- |
| Kostenlos | **14,4K RPD** | 30 RPM pro Model | Keine Kreditkarte; 429 auf Limit, nicht abgerechnet |

Verfügbar kostenlos: `llama-3.3-70b-versatile`, `gemma2-9b-it`, `mixtral-8x7b`,
`whisper-large-v3`

### 🔴 LONGCAT AI (Kostofser API-Schlüssel — longcat.chat) 🆕

| Modell                      | Präfix | Täglich Freiwillige Vertragsklausel | Notizen                        |
| --------------------------- | ------ | ----------------------------------- | ------------------------------ |
| `Langkat-Flash-Lite`        | `lc/`  | **50 M Token** 💥                    | Größte kostenlose Quote jemals |
| `Langkat-Flash-Chat`        | `lc/`  | 500.000 Token                       | Mehrfach-Wechsel-Chat          |
| `Langkat-Flash-Denken`      | `lc/`  | 500.000 Token                       | Argumentation / CoT            |
| `Langkat-Flash-Denken-2601` | `lc/`  | 500.000 Token                       | Januar 2026 Version            |
| `Langkat-Flash-Omni-2603`   | `lc/`  | 500.000 Token                       | Multimodal                     |

> 100 % kostenlos, solange im öffentlichen Beta-Test. Beantragen Sie sich unter
> [langkat.chat](https://longcat.chat) mit E-Mail oder Telefon. Tägliche Reset
> 00:00 UTC.

### 🟢 POLLINATIONS AI (Keine API-Schlüssel erforderlich) 🆕

| Modell     | Präfix | Ratenbegrenzung   | Anbieter Rückseite |
| ---------- | ------ | ----------------- | ------------------ |
| `openai`   | `pol/` | 1 Anfrage pro 15s | GPT-5              |
| `claude`   | `pol/` | 1 Anfrage pro 15s | Anthropic Claude   |
| `gemini`   | `pol/` | 1 Anfrage pro 15s | Google Gemini      |
| `deepseek` | `pol/` | 1 Anfrage pro 15s | DeepSeek V3        |
| `llama`    | `pol/` | 1 Anfrage pro 15s | Meta Llama 4 Scout |
| `mistral`  | `pol/` | 1 Anfrage pro 15s | Mistral AI         |

> ✨ **Keine Reibung:** Keine Registrierung, keinen API-Schlüssel erforderlich.
> Fügen Sie den Pollinations-Anbieter mit einem leeren Schlüsselfeld hinzu und
> es funktioniert sofort.

### 🟠 CLOUDFLARE WORKERS AI (Kostenloser API-Schlüssel — cloudflare.com) 🆕

| Tarif     | Tagesneuronen | Gleichwertige Verwendung                                   | Notizen                   |
| --------- | ------------- | ---------------------------------------------------------- | ------------------------- |
| Kostenlos | [10,000], [8] | ~ 150 LLM Prozessoren / 500 Sekunden audio / 15.000 Embeds | Globale Edge, 50+ Modelle |

Beliebte kostenlose Modelle: [cf/meta/llama-3.3-70b-instruct],
[google/gemma-3-12b-it], [openai/whisper-large-v3-turbo] (kostenloser Audio!),
[qwen/qwen2.5-coder-15b-instruct]

> Richtet sich nach API-Schlüssel + Account-Id aus
> [dash.cloudflare.com](https://dash.cloudflare.com). Speichert Account-Id in
> den Anbietersätzen.

### 🟣 SCALEWAY AI (1M Free Tokens — scaleway.com) 🆕

| Tarif     | Gratis-Grenze | Standort     | Notizen                                                      |
| --------- | ------------- | ------------ | ------------------------------------------------------------ |
| Kostenlos | [1M token]    | 🇫🇷 Paris, EU | Kein Kreditkartenbesitzer erforderlich innerhalb der Grenzen |

Verfügbar kostenlos: [qwen3-235b-a22b-instruct-2507] (Qwen3 235B!),
[llama-3.1-70b-instruct], [mistral-small-3.2-24b-instruct-2506],
[deepseek-v3-0324]

> EU/GDPR-kompatibel. Erhalten Sie API-Schlüssel an
> [console.scaleway.com](https://console.scaleway.com).

> [💡 Die ultimative kostenlose Stapel (11 Anbieter, $0, immer)]
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

| Anbieter         | Free Credits           | Best Model                                   | Ratenbegrenzung              |
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

Dann in `/Dashboard/Media` → **Transkription** -Tab: Haken Sie ein beliebiges
Audiodatei oder ein Videodatei hoch – Wählen Sie Ihren Combo-Endpunkt aus –
erhalten Sie Transkription in unterstützten Formaten.

## 🔑 Schlüsselmerkmale

OmniRoute v2.0 ist als Betriebsplattform erstellt und nicht nur als Relaisproxy.

### 🆕 Neu — ClawRouter-Inspirierte Verbesserungen (März 2026)

| Funktion                                 | Was es tut                                                                                                         |
| ---------------------------------------- | ------------------------------------------------------------------------------------------------------------------ |
| ⚡ **Grok-4 Fast Family**                 | xAI-Modelle kosten 0,20/0,50 pro M — getestet auf 1143ms (30 % schneller als Gemini 2.5 Flash)                     |
| 🧠 **GLM-5 über Z.AI**                    | 128K Ausgabekontext, 0,50/1M — neuestes Flaggschiff aus der GLM-Familie                                            |
| 🔮 **MiniMax M2.5**                       | Argumentation + agente Aufgaben kosten 0,30/1M — bedeutender Upgrade von M 2.1                                     |
| 🎯 **toolCalling -Flag pro Modell**       | Per-Modell `toolCalling: true/false` in Registry — AutoCombo überspringt Modelle, die keine Werkzeuge können       |
| 🌍 **Multilinguale Intentionserkennung**  | PT/ZH/ES/AR -Schlüsselworter in AutoCombo-Ranking — bessere Modellauswahl für Inhalte, die nicht auf Englisch sind |
| 📊 **Benchmark-getriebene Ausfallmuster** | Echte p95-Latenz von Live-Anfragen bereitstellt Komboscore — AutoCombo lernet aus tatsächlichen Daten              |
| 🔁 **Anfrage-Duplizierung**               | Inhaltshashes-basierte Duplikationsfenster — Mult-Agent-sicher, verhindert doppelte Chargen                        |
| 🔌 **Einsteckbare RouteStrategie**        | Erweiterbare `RouteStrategie` - Schnittstelle  — Hinzufügen von benutzerdefinierter Routenlogik als Plugins        |

### 🚀 Vorherige v2.0.9+ — Playground, CLI Fingerprints & ACP

| Funktion                                            | Was es tut                                                                                                                                                                                                                                                                                                |
| --------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🎮 **Modell-Playground**                             | Übersichtsseite, auf der jeder Modell direkt getestet werden kann — Provider/Modell/Aufzeichnung auswählen, Monaco-Editor, Streaming, Abbruch, Zeitverlauf                                                                                                                                                |
| 🔏 **CLI-Fingerabdruckleistung**                     | Anbieterabhängige Header/Body-Anordnung zur Anpassung von nativen CLI-Signaturen — Anpassen des Anbieters pro Anbieter in Einstellungen > Sicherheit. **Ihr Proxy-IP wird gesichert**                                                                                                                     |
| 🤝 **ACP-Unterstützung (Agent Client Protocol)**     | CLI-Agentenentdeckung (Codex, Claude, Goose, Gemini CLI, OpenClaw + 9 weitere), Prozessstarter, `/api/acp/agents`-Abschnitt                                                                                                                                                                               |
| 🤖 **ACP-Agenten-Übersicht**                         | Debugger › Agenten-Übersicht — Gitter mit 14 Agenten, Installationsstatus, Version, benutzerdefiniertes Agentenformular für jede CLI-Zeit. **OpenCode**-Benutzer erhalten einen "Download opencode.json"-Button, der automatisch eine mit allen verfügbaren Modellen geoptimierte Konfiguration erstellt. |
| 🔧 **Benutzerdefinierte Modell `apiFormat`-Routing** | Benutzerdefinierte Modelle mit `apiFormat: „Antworten“` werden nun richtig an den Antworten-API-Übersetzer weitergeleitet                                                                                                                                                                                 |
| 🏢 **Codex-Arbeitsplatz-Isolation**                  | Mehrere Codex-Arbeitsplätze pro E-Mail — OAuth trennt Verbindungen korrekt durch Workspace-ID                                                                                                                                                                                                             |
| 🔄 **Elektron-Selbstaktualisierung**                 | Desktop-Anwendung prüft Updates & aktualisiert sich automatisch beim Neustart                                                                                                                                                                                                                             |

### 🤖 Agent und Protokolloperationen (v2.0)

| Funktion                              | Was es tut                                                                                                        |
| ------------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| 🔧 **MCP-Server (16 Werkzeuge)**       | IDE/V-Agent Werkzeuge via 3 Transportprotokolle: stdio, SSE (`/api/mcp/sse`), Streamable HTTP (`/api/mcp/stream`) |
| 🤝 **A2A-Server (JSON-RPC + SSE)**     | Agent-zu-Agent-TASK-Execution mit synchroner und stromorientierter Flussführung                                   |
| 🧭 **Konsolidierte Endpunkte-Seite**   | Fensterbedienungsseite mit Endpunktproxy, MCP, A2A u. API-Endpunkten                                              |
| 🎚️ **Dienst-Enable/Disable-Schalter** | Ein- / Ausschalter für MCP und A2A mit Einstellungspersistenz (Standard: AUS)                                     |
| 🛰️ **MCP Laufzeit-Herzhub**           | Echtzeit-Prozessstatus (pid, uptime, Herzschlag-Alt, Transport, Bereichsmodus)                                    |
| 📋 **MCP Audit-Zeichenkette**          | Filterierbare Auditspuren mit Erfolg/missglückte Transaktionen und Schlüsselzuschreibung                          |
| 🔐 **MCP Bereichszustimmung**          | 9 feingranulare Zutrittsberechtigungen für kontrollierte Werkzeugzugriffe                                         |
| 📡 **A2A-Aufgaben-Status-Verwaltung**  | Listen- / Filterfunktionen für Aufgaben, Ereignisse/Künstlersitze, Abbruch-Runaufgaben                            |
| 📋 **Agentkarte-Entdeckung**           | `/.well-known/agent.json` für Klient-Automatikentdeckung                                                          |
| 🧪 **Protokoll E2E-TestHarness**       | Echt-MCP SDK + A2A-Klient-Flows in `test:protocols:e2e`                                                           |
| ⚙️ **Betriebsregelungen**             | Schaltkombo, Anwendung von Resilienz-Profilen, Neustart von Breakern aus einer Regelungsfläche                    |

### 🧠 Routen und Intelligenz

| Funktion                                     | Was es tut                                                                                          |
| -------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| 🎯 **Intelligenter 4-Ebenen-Absturz**         | Automatisches Routen: Abonnement → API-Schlüssel → P1 → P0                                          |
| 📊 **Echtzeit-Auftrags-Verfolgung**           | Lebendes Token-Zähler + Neustart- Zähler pro Anbieter                                               |
| 🔄 **Format-Umstellungen**                    | OpenAI ↔ Claude ↔ Gemini ↔ Antworten mit schemabezüglichen Umstellungen                             |
| 👥 **Unterstützung vieler Konten**            | Mehrere Konten pro Anbieter mit inteller Selektion                                                  |
| 🔄 **Auto-Access-Token-Wiederherstellung**    | OAuth-Tokens werden automatisch mit Wiederholung wiederhergestellt                                  |
| 🎨 **Benutzerdefinierte Combinations**        | 6 Ausgleichsstrategien + Fallback-Kettensicherung                                                   |
| 🌐 **Wildcard-Router**                        | `provider/*` dynamische Routen                                                                      |
| 🧠 **Finanzbudgetierung denken**              | Durchlass, Auto, benutzerdefiniert und adaptive Einschränkungen für das Verständnis                 |
| 🔀 **ModellAlias**                            | Baum integrierte + benutzerdefinierte Modell aliasing und Migrationssicherheit                      |
| ⚡ **Hintergrundverschlechterung**            | Routen Sie die Aufgaben für die Hintergrundaufgaben zu billigeren Modellen                          |
| 🧪 **Aufgabenbewusstes Intelligenter Routen** | Wählen Sie automatisch das Modell über den Inhaltstyp (Kodierung/ Vision/ Analyse/ Zusammenfassung) |
| 💬 **System-Prompt-Enthaltung**               | Globale Verhaltenssteuerungen werden konsistent angewendet                                          |
| 📄 ** Antworten des API-Kompatibilität**      | Vollständige `/v1/responses` Unterstützung für Codex und fortgeschrittene agente Arbeitsabläufe     |

### 🎵 Mehrmodalen-APIs

| Funktion                  | Was es tut                                                                                                                                                                              |
| ------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🖼️ ** Bild Generation**   | `/v1/images/generations` mit Cloud- und lokalen Backends                                                                                                                                |
| 📐 ** Embeddings**         | `/v1/embeddings` für die Suche und RAG Pipelines                                                                                                                                        |
| 🎤 **Audio Transkription** | `/v1/audio/transkriptionen` — 7 Anbieter (Deepgram Nova 3, AssemblyAI, Groq Whisper, HuggingFace, ElevenLabs, OpenAI, Azure), automatische Sprache erkennung, MP4/MP3/WAV Unterstützung |
| 🔊 **Text-to-Speech**      | `/v1/audio/sprache` — 10 Anbieter (ElevenLabs, OpenAI, Deepgram, Cartesia, PlayHT, HuggingFace, Nvidia NIM, Inworld, Coqui, Tortoise) mit korrekten Fehlermeldungen                     |
| 🎬 **Videoerzeugung**      | `/v1/videos/erzeugungen` (ComfyUI + SD WebUI Workflows)                                                                                                                                 |
| 🎵 **Musikerzeugung**      | `/v1/music/erzeugungen` (ComfyUI Workflows)                                                                                                                                             |
| 🛡️ **Moderation**         | `/v1/moderations` Sicherheitsprüfungen                                                                                                                                                  |
| 🔀 **Reranking**           | `/v1/rerank` für Relevanzberechnung                                                                                                                                                     |
| 🔍 **Web Suche** 🆕         | `/v1/search` — 5 Anbieter (Serper, Brave, Perplexity, Exa, Tavily), 6.500+ kostenlos pro Monat, automatisches Failover, Cache                                                           |

### 🛡️ Resilienz, Sicherheit & Governance

| Funktion                                                      | Was es tut                                                                                                      |
| ------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- |
| 🔌 **Sicherheitszünder**                                       | Per-Modell-Trip/Recover mit Schwellenkontrollen                                                                 |
| 🎯 **Modell-gewahrte Endpunkte**                               | 🛡️ [X3X]Sicherung gegen Blitzeherde[X25X]                                                                       |
| Sperre + Semaphore-Schutz bei Wiederholungs-/Rate-Ereignissen | Kosten/Geschwindigkeit-Einsparungen mit zwei Layer-Cache                                                        |
| 🧠 **Semantic-Signature-Cache**                                | Kosten-/Latenzreduktion durch zwei Schichten Caching                                                            |
| ⚡ **Idempotenz von Anfragen**                                 | Schutz vor Duplikaten für Fenster                                                                               |
| 🔒 **TLS-Fingerprint-Betrug**                                  | Browserähnlicher TLS-Fingerprint ** reduziert Bot-Detektion und Kontoauflag **                                  |
| 🔏 **CLI-Fingerabdruckleistung**                               | Übereinstimmt mit native CLI-Anforderungsunterzeichnungen ** reduziert Ban-Risiko bei Erhaltung von Proxy-IP ** |
| 🌐 **IP-Filtering**                                            | Allowlist/Blocklist-Kontrolle für freigegebene Bereitstellungen                                                 |
| 📊 **Bearbeitbare Obergrenzen pro Zeit**                       | Konfigurierbare globale/Richtlinien-seitige Obergrenzen mit Persistenz                                          |
| 🔑 **API-Schlüssel-Verwaltung + Umfänge**                      | Sichere Schlüsselausstellung/Drehung und Modell/Provider-Kontrolieren                                           |
| 🛡️ **Schutz des `/models`**                                   | Optionale Authentifizierungs-Gatter und Provider-Verbergen für Modell-Katalog                                   |

### 📊 [X2X]Beobachtbarkeit + Analytik

| Funktion                                  | Was es tut                                                          |
| ----------------------------------------- | ------------------------------------------------------------------- |
| 📝 **Anfrage + Proxy-Loggen**              | Voller Anforderungs-/Antwort- und Proxy-Loggen                      |
| 📋 **Zentrierte Protokollebenenübersicht** | Anforderungs-, Proxy-, Audit- und Konsole-Ansichten auf einer Seite |
| 🔍 **Anfragemetriken**                     | Latenz (p50/p95/p99) und Anfragetracing                             |
| 🏥 **Gesundheitsüberwachung**              | Verfügbarkeit, Breaker-Zustände, Sperren, Cache-Statistiken         |
| 💰 **Kosten-Nachverfolgung**               | Budget-Kontrolle und Preisanzeigen pro Modell                       |
| 📈 **Analysevisualisierungen**             | Modellanbieter-Verwendungsinsights und Trendsichtungen              |
| 🧪 **Evaluation-Schichten**                | Golden Set-Testen mit konfigurierbaren Anpassungstrategien          |

### ☁️ Plattform und Einrichtung

| Funktion                               | Was es tut                                                                      |
| -------------------------------------- | ------------------------------------------------------------------------------- |
| 🌐 **Überallige Bereitstellung**        | Localhost, VPS, Docker, Cloud-Umgebungen                                        |
| 💾 **Cloud Sync**                       | Konfigurationssynchronisierung via Cloud-Worker                                 |
| 🔄 **Backup/Restore**                   | Export/Import- und Notfallwiederherstellungsfelder                              |
| 🧙 **Onboarding Wizard**                | Einführungsrichtlinie für die Erstkommunikation                                 |
| 🔧 **CLI-Häckchen Dashboard**           | Einstellung für beliebte Code-Tools mithilfe von One-Click                      |
| 🎮 **Modell-Playground**                | Testen Sie jeden Anbieter/Modell/Endpunkt über die Oberfläche                   |
| 🔏 **CLI-Abpraller-Knopf**              | Anbieter-abhängige Fingerabdruck-Mitgliedschaften in Einstellungen > Sicherheit |
| 🌐 **I18n (30 Sprachen)**               | Vollständige Oberfläche + Dokumentation für Spracherkennung mit LTR-Coverage    |
| 🧹 **Alle Modelle löschen**             | Mit einem Klick werden alle Modelle in den Anbieter Details entfernt            |
| 📋 **Vorlagen für Issue**               | Mithilfe von GitHub werden Standardvorlagen für Bugs und Features erstellt      |
| 📂 **Benutzerdefinierte Dateispeicher** | `Datenordner` Überschreibwert für Speicherort                                   |

### Feature-Deep-Dive

#### Intelligente Stornierung mit praktischer Kostendrosselung

```txt
Kombi: "Meine-Entwicklungsumgebung"
  1. cc/claude-opus-4-6
  2. nvidia/llama-3.3-70b
  3. glm/glm-4.7
  4. if/kimi-k2-denkprozess
```

Wenn bei der Quota, Rate oder Health eine Fehlfunktion auftritt, verlagert
OmniRoute automatisch auf den nächsten Kandidaten, ohne manuelles Umstellen.

#### Protokoll-Management, das sichtbar und bedienbar ist

- MCP + A2A sind im UI und in Dokumenten erkennbar (wurde nicht versteckt)
- Protokollzustands-APIs geben live-operative Daten `/api/mcp/*`, `/api/a2a/*`
  frei
- Dashboard-Inhalte beinhalten Aktionen für das Day-2-Vorhersage
  (Kombi-Schalter, Breaker-Neustart, Aufgaben-Kannellung)

#### Übersetzer + Validierungsworkflow

Die Übersetzer-Bereich enthält:

- **Playground**: Anfrage-Transformation-Überprüfung
- **Chat-Tester**: Vollständige Request/Response-Umweg
- **Testbench**: Mehrere Fälle in einem Lauf
- **Live-Monitor**: Echtzeit-Verkehrs-Ansicht

Zusätzlich zur Protokollvalidierung werden über `npm run test:protocols:e2e`.
echte Clients verwendet.

> 📖 **[MCP-Server-README](open-sse/mcp-server/README.md)** — Werkzeug-Referenz,
> IDE-Konfigs, Client-Beispiele
> 
> 📖 **[A2A-Server-README](src/lib/a2a/README.md)** — Fähigkeiten,
> JSON-RPC-Methode, Streaming und Aufgabenlebenszyklus

## 🧪 Evaluations (Evals)

OmniRoute enthält eine integrierte Evaluierungsframework, um die Qualität der
LLM-Echos gegen einen goldenen Satz zu überprüfen. Zugreifen Sie über
**Analytics → Evals** im Dashboard.

### Built-in Golden Set

The pre-loaded "OmniRoute Golden Set" contains test cases for:

- Greetings, math, geography, code generation
- JSON format compliance, translation, markdown generation
- Safety refusal (harmful content), counting, boolean logic

### Bewertungsstrategien

| Strategie  | Beschreibung                                     | Beispiel                               |
| ---------- | ------------------------------------------------ | -------------------------------------- |
| `exact`    | Output must match exactly                        | `"4"`                                  |
| `contains` | Output must contain substring (case-insensitive) | `"Paris"`                              |
| `regex`    | Output must match regex pattern                  | `"1.*2.*3"`                            |
| Brauch     | Custom JS function returns true/false            | `(output) =&gt; Ausgabe.länge &gt; 10` |

---

## 📖 Setup Anleitung

### Protokoll-Setup (MCP + A2A)

<details>
<summary><b>🧩 MCP Setup (Model Context Protocol)</b></summary>

MCP-Transport starten im Stdio-Modus:

```bash
omniroute --mcp
```

Empfehlte Validierungsablauf:

1. Verbinden Sie Ihren MCP-Klienten über Stdio.
2. Ausführen `omniroute_get_Health`.
3. Ausführen `omniroute_list_Combos`.
4. Öffnen Sie `/dashboard/mcp`, um Herzschlag, Aktivität und Protokoll zu
   bestätigen.

Nützliche APIs für die Automatisierung:

- `GET /api/mcp/status`
- `GET /api/mcp/tools`
- `GET /api/mcp/audit`
- `GET /api/mcp/audit/stats`

</details>

<details>
<summary><b>🤝 A2A Setup (Agent2Agent)</b></summary>

Der Agent entdecken:

```bash
curl http://localhost:20128/.well-known/agent.json
```

Senden Sie eine Aufgabe:

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'inhalts-typ: Anwendung/Json' \
  -d '{"jsonrpc":"2.0","id":"setup-a2a","method":"message/send","params":{"fähigkeit":"Ressourcenzuweisung","nachrichten":[{"rolle":"benutzer","inhalt":"Zusammenfassung der Quotenstatus."}]}}'
```

Lebenszyklus-Verwaltung:

- `GET /api/a2a/status`
- `GET /api/a2a/tasks`
- `GET /api/a2a/tasks/:id`
- `POST /api/a2a/tasks/:id/cancel`

Betriebs-UI:

- `/dashboard/a2a` für Aufgaben/Zustand/Stream-Beobachtung und Rauchhandlungen

</details>

<details>
<summary><b>🧪 End-to-end protocol validation</b></summary>

Federführend sind die beiden Protokolle mit echten Clients überprüfen:

```bash
npm run test:protocols:e2e
```

Das überprüft:

- MCP SDK-Klient verbinden/listen/Aufrufen
- A2A-Entdeckung/SENDEN/STREAMSVERFÜGUNG/ABBRECHEN
- Konsolidierungs-Daten ab MCC-Audit und A2A-Aufgaben-Management-APIs

</details>

<details>
<summary><b>💳 Subscription Providers</b></summary>

### Claude-Code (Pro/Max)

```bash
Bildschirmsicht → Anbieter → Claude-Code verbinden
→ OAuth-Anmeldung → Automatischer Token-Refresh
→ 5-Stunden-Zeitfenster + wöchentlicher Quotentracking

Modelle: 
  cc/claude-opus-4-6
  cc/claude-sonnet-4-5-20250929
  cc/claude-haiku-4-5-20251001
```

**Pro Tipp:** Verwenden Sie Opus für komplexe Aufgaben, Sonnet für
Geschwindigkeit. OmniRoute verfolgt Quotenangaben pro Modell!

### OpenAI-Codex (Plus/Pro)

```bash
Bildschirmsicht → Anbieter → Codex verbinden
→ OAuth-Anmeldung (Port 1455)
→ 5-Stunden + wöchentlicher Neustart

Modelle:
  cx/gpt-5.2-codex
  cx/gpt-5.1-codex-max
```

#### Codex-Konto-Begrenzungsbetreuung (5h + Woche)

Jedes Codex-Konto verfügt nun über Richtlinien-Toggle in
`Bildschirm-Beschränkungen -&gt; Anbieter`:

- `5h` (EINSTELLUNGEN): erzwingen Sie das
  5-Stunden-Obergrenzen-Richtlinie-Threshold-policy.
- `Wöchentlich ` (AN/OFF): Ermutigung der
  Wochenfenster-Schwellen-Einstellungspolitik.
- Schwelleneinstellung: Wenn ein eingeschaltetes Fenster >=90% Auslastung
  erreicht, wird das Konto übersprungen.
- Rotationsverhalten: OmniRoute wird automatisch zum nächsten geeigneten
  Codex-Konto geroutet.
- Neustart-Einstellung: Sobald das Anbieter `resetAt` Zeit verstrichen ist, wird
  das Konto wieder automatisch wählbar.

Szenarien:

- `5h ON` + `Wöchentlich ON`: Das Konto wird übersprungen, wenn ein Fenster die
  Schwellenzahl erreicht hat.
- `5h OFF` + `Wöchentlich ON`: Nur die wöchentliche Auslastung kann das Konto
  blockieren.
- `5h ON` + `Wöchentlich OFF`: Nur die 5-stündige Auslastung kann das Konto
  blockieren.
- `resetAt` erreicht: Das Konto wird automatisch wieder in Rotation aufgenommen
  (keine manuelle Wiederverbindung erforderlich).

### Gemini CLI (KOSTENLOS 180K/MONAT!)

```bash
Bildschirm → Anbieter → An Gemini CLI anschließen
→ Google OAuth
→ 180K Ausfüllungen/Monat + 1K/Tag

Modelle:
  gc/gemini-3-flash-vorschau
  gc/gemini-2.5-Pro
```

**Best Value:** Großzügige kostenlose Ebene! Nutzen Sie dies, bevor Sie die
kostenpflichtige Ebene nutzen.

### GitHub-Copilot

```bash
Bildschirm → Anbieter → An GitHub anschließen
→ OAuth via GitHub
→ Monatlicher Neustart (1. des Monats)

Modelle:
  gh/gpt-5
  gh/claude-4.5-sonnet
  gh/gemini-3-Pro
```

</details>

<details>
<summary><b>🔑 API Key Providers</b></summary>

### NVIDIA NIM (KOSTENLOSer Entwickler- Zugang — 70+ Modelle)

1. Registrieren: [build.nvidia.com](https://build.nvidia.com)
2. Kostenloses API-Schlüssel erhalten (1000 Anfragereintraege enthalten)
3. Bildschirm → Anbieter hinzufügen → NVIDIA NIM:
   - API-Schlüssel: `nvapi-Ihr-Schlüssel`

**Modelle:** `nvidia/llama-3.3-70b-anweisung`, `nvidia/mistral-7b-anweisung` und
50+ mehr

Pro Tip: **OpenAI-kompatibles API — funktioniert nahtlos mit
OmniRouten-Formatübersetzung!

### DeepSeek

1. Registrieren: [platform.deepseek.com](https://platform.deepseek.com)
2. API-Schlüssel erhalten
3. Dashboard → Hinzufügen → DeepSeek

**Modelle:** `deepseek/deepseek-chat`, `deepseek/deepseek-coder`

### Groq (Kostenlose Ebene verfügbar!)

1. Registrieren: [console.groq.com](https://console.groq.com)
2. API-Schlüssel erhalten (gehalt die kostenlose Ebene)
3. Dashboard → Hinzufügen → Groq

**Modelle:** `groq/llama-3.3-70b`, `groq/mixtral-8x7b`

**Pro Tip:** Hochgeschwindige Inference — Perfekt für Echtzeit-Programmierung!

### OpenRouter (100+ Modelle)

1. Registrieren: [openrouter.ai](https://openrouter.ai)
2. API-Schlüssel erhalten
3. Dashboard → Hinzufügen → OpenRouter

**Modelle:** Zugriff auf 100+ Modelle von allen wichtigen Providern über ein
einzelner API-Schlüssel.

</details>

<details>
<summary><b>💰 Cheap Providers (Backup)</b></summary>

### GLM-4.7 (Täglich reset, $0,6/1M)

1. Registrieren: [Zhipu AI](https://open.bigmodel.cn/)
2. API-Schlüssel vom Coding-Plan erhalten
3. Bildschirmansicht → API-Schlüssel hinzufügen:
   - Anbieter: `glm`
   - API-Schlüssel: `deine-Schlüssel`

**Verwende: ** `glm/glm-4.7`

**Pro-Tipp: ** Mit Coding Plan 3-fach die Quoten bei 1/7 des Preises! Neustart
täglich 10:00 Uhr.

### MiniMax M2.1 (5h Neustart, 0,20 $/1M)

1. Registrieren: [MiniMax](https://www.minimax.io/)
2. API-Schlüssel erhalten
3. Bildschirmansicht → API-Schlüssel hinzufügen

**Verwende: ** `minimax/MiniMax-M2.1`

**Pro-Tipp: ** Kostengünstigste Option für lange Kontexte (1M Token)!)

### Kimi K2 (9 $/Monat fest)

1. Abonnieren: [Moonshot AI](https://platform.moonshot.ai/)
2. API-Schlüssel erhalten
3. Bildschirmansicht → API-Schlüssel hinzufügen

**Verwende: ** `kimi/kimi-latest`

**Pro-Tipp: ** Fester Preis von 9 $/Monat für 10M Token = 0,90 $/1M effektiver
Kosten!

</details>

<details>
<summary><b>🆓 FREE Providers (Emergency Backup)</b></summary>

### iFlow (5 FREIE Modelle über OAuth)

```bash
Bildschirmansicht → iFlow verbinden
→ iFlow OAuth-Login
→ Unbegrenzte Nutzung

Modelle:
  if/kimi-k2-thinking
  if/qwen3-coder-plus
  if/glm-4.7
  if/minimax-m2
  if/deepseek-r1
```

### Qwen (4 FREIE Modelle über Gerätekodierung)

```bash
Dashboard → Konto Kiro aufnehmen
→ Gerätekodesanmeldung
→ unbegrenzte Verwendung

Modelle:
  qw/qwen3-coder-plus
  qw/qwen3-coder-flash
```

### Kiro (Claude GRATIS)

```bash
Dashboard → Konto Kiro aufnehmen
→ AWS-Buildernummer oder Google/GitHub
→ unbegrenzte Verwendung

Modelle:
  kr/claude-sonnet-4.5
  kr/claude-haiku-4.5
```

</details>

<details>
<summary><b>🎨 Create Combos</b></summary>

### Beispiel 1: Abonnement maximieren → Prepaid Backup

```
Dashboard → Kombos → Neues erstellen

Name: premium-coding
Modelle:
  1. cc/claude-opus-4-6 (Abonnement primär)
  2. glm/glm-4.7 (Billiger Backup, 0,6 $/1 Mio.)
  3. minimax/MiniMax-M2.1 ( cheapest Backup, 0,20 $/1 Mio.)

Verwenden Sie im CLI: premium-coding
```

### Beispiel 2: Kostenlos (Keine Kosten)

```
Name: free-combo
Modelle:
  1. gc/gemini-3-flash-preview (180K kostenlos pro Monat)
  2. if/kimi-k2-thinking (unbegrenzt)
  3. qw/qwen3-coder-plus (unbegrenzt)

 Kosten: 0 $ für immer!
```

</details>

<details>
<summary><b>🔧 CLI Integration</b></summary>

### Cursor-IDE

```
Einstellungen → Modelle → Erweitert:
  OpenAI-API- Basis- URL: http://localhost:20128/v1
  OpenAI-API- Schlüssel: [aus OmniRoute-Dashboard]
  Modell: cc/claude-opus-4-6
```

### Claude Code

Verwenden Sie die **CLI-Werkzeuge**-Seite im Dashboard für eine-klickige
Konfiguration oder bearbeiten `~/.claude/Einstellungen.json` manuell.

### Codex CLI

```bash
export OPENAI_BASE_URL="http://localhost:20128"
export OPENAI_API_KEY="Ihr- OmniRoute- API-Schlüssel"

codex "Ihr Prompt"
```

### OpenClaw

**Option 1 — Dashboard (empfohlen): **

```
Dashboard → CLI-Werkzeuge → OpenClaw → Modell auswählen → Anwenden
```

**Option 2 — Manuell: ** bearbeiten Sie `~/.openclaw/openclaw.json`:

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

> **Hinweis: ** OpenClaw funktioniert nur mit lokalem OmniRoute. Verwenden Sie
> `127.0.0.1` anstatt `localhost`, um IPv6-Auswertungsprobleme zu vermeiden.

### Cline / Fortsetzen / RooCode

```
Einstellungen → API-Konfiguration:
  Anbieter: OpenAI-Kompatibel
  Basis-URL: http://localhost:20128/v1
  API-Key: [aus OmniRoute-Dashboard]
  Modell: if/kimi-k2-thinking
```

### OpenCode

**Schritt 1:** Fügen Sie OmniRoute als eigenen Anbieter hinzu:

```bash
opencode
/connect
# Wählen Sie "Sonstiges" → Geben Sie die ID "omniroute" ein → Geben Sie Ihre OmniRoute-API-Schlüssel ein
```

**Schritt 2:** Erstellen oder bearbeiten Sie `opencode.json` in Ihrem
Projektverzeichnis:

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

**Schritt 3:** Wählen Sie das Modell in OpenCode:

```bash
/models
# Wählen Sie einen OmniRoute-Modell aus der Liste aus
```

> **Tip:** Fügen Sie auch ein Modell aus Ihrem OmniRoute-`/v1/models`-Endpunkt
> in die `models`-Sektion hinzu. Verwenden Sie die Formatierung
> `Anbieter/Modell-ID` vom OmniRoute-Dashboard.

</details>

---

## Fehlerbehebung

<details>
<summary><b>Click to expand troubleshooting guide</b></summary>

**"Language model lieferte keine Nachrichten"**

- Durchlaufende API-Deckung → Überprüfen Sie den Quoten-Tracker im Dashboard
- Lösung: Fallback zu einem Kombi-Modell oder zum günstigeren Tarif wechseln

**Rate Limiting**

- Abgeschriebene Abonnements-Quoten → Fallback zu GLM/MiniMax
- Hinzufügen: `cc/claude-opus-4-6 → glm/glm-4.7 → if/kimi-k2-thinking`

**OAuth-Tokener läuft ab**

- Automatischer Neubestellung durch OmniRoute
- Bei anhaltenden Problemen: Dashboard → Anbieter → Wiederherstellen

**Hohe Kosten**

- Überprüfen Sie den Nutzungsstatistik im Überblick → Kosten
- Primärmodell auf GLM/MiniMax schalten
- Führen Sie für nicht kritische Aufgaben die kostenlose Tarrif (Gemini CLI,
  iFlow) aus

**Überblick/API-Ports sind falsch**

- `PORT` ist die kanonische Basis-Port (und API-Port standardmäßig)
- `API_PORT` überschreibt nur den OpenAI-kompatiblen API-Hörer
- `DASHBOARD_PORT` überschreibt nur den Überblick-/Next.js-Hörer
- Setzen Sie `NEXT_PUBLIC_BASE_URL` auf Ihre Übersicht/öffentliche URL (für
  OAuth-Rückruf)

**Cloud-Synchronisierungsfehler**

- Überprüfen Sie, dass `BASE_URL` auf Ihre laufende Instanz zeigt
- Überprüfen Sie, dass `CLOUD_URL` auf Ihre erwartete Cloud-Endpunkt zeigt
- Halten Sie `NEXT_PUBLIC_*`-Werte im Einklang mit den serverseitigen Werten

**Erfolgreiche erste Anmeldung nicht funktioniert**

- Überprüfen Sie `INITIAL_PASSWORD` im `.env`
- Wenn nicht gesetzt, fällt auf ein `123456` zurück

**Keine Request-Logs**

- Setzen Sie `ENABLE_REQUEST_LOGS=true` im `.env`

**Verbindungstest zeigt " ungültig" für OpenAI-kompatible Anbieter**

- Viele Anbieter offenbaren kein `/models`-Endpunkt
- OmniRoute v1.0.6+ enthält fallback-Validierung über Chat-Ergebnisse
- Bitte stellen Sie sicher, dass der Basis-URL den Suffix `/v1` enthält

### 🔒 OAuth auf einem Remote-Server

<a name="oauth-on-a-remote-server"></a> <a name="oauth-em-servidor-remoto"></a>

> **⚠️ Wichtig für Benutzer, die OmniRoute auf einem VPS, Docker oder einem
> anderen Remote-Server installieren**

#### Warum funktioniert die Antigravität / Gemini CLI OAuth auf Remote-Servers nicht?

Die **Antigravität**- und die **Gemini CLI**-Anbieter verwenden **Google OAuth
2.0**. Google erfordert, dass der `redirect_uri`-Parameter im OAuth-Flow genau
einer der im Google Cloud Console registrierten URIs entspricht.

Die in OmniRoute bundelten OAuth-Zugangsdaten sind für den **`localhost`-Server
nur registriert**. Sobald Sie OmniRoute auf einem Remote-Server (z.B.
`https://omniroute.myserver.com`) aufrufen, lehnt Google die Authentifizierung
mit:

```
Fehler 400: redirect_uri_mismatch
```

#### Lösung: Konfigurieren Sie Ihre eigenen OAuth-Zugangsdaten

Sie müssen im Google Cloud Console eine **OAuth 2.0-Zugriffsanmelde-ID** mit
Ihrem Server-URI erstellen

#### Schritt-für-Schritt

**1. Öffnen Sie den Google Cloud Console**

Gehe zu:
[https://console.cloud.google.com/apis/credentials](https://console.cloud.google.com/apis/credentials)

**2. Erstellen Sie eine neue OAuth 2.0-Zugriffsanmelde-ID**

- Klicken Sie auf **+Create Credentials"** → **"OAuth client ID"**
- Anwendungsart: **"Webanwendung"**
- Name: beliebig (z.B. `OmniRoute Remote`)

**3. Fügen Sie autorisierte Zugriffs-URI hinzu**

Im **"Authorized redirect URIs"-Feld" fügen Sie hinzu:

```
https://your-server.com/callback
```

> Ersetzen Sie `your-server.com` durch Ihre Server-Domäne oder -IP
> (einschließlich des Ports, wenn erforderlich, z.B.
> `http://45.33.32.156:20128/callback`).

**4. Eine Sitzung speichern und die Zugriffskennungen kopieren**

Nach der Erstellung zeigt Google **Client-ID** und **Client-Secret-XWert**.

**5. Umgebungsvariablen setzen**

In Ihrem `.env` (oder Docker-Umgebungsvariablen):

```bash
# Für Antigravity:
ANTIGRAVITY_OAUTH_CLIENT_ID=your-client-id.apps.googleusercontent.com
ANTIGRAVITY_OAUTH_CLIENT_SECRET=GOCSPX-your-secret

# Für Gemini CLI:
GEMINI_OAUTH_CLIENT_ID=your-client-id.apps.googleusercontent.com
GEMINI_OAUTH_CLIENT_SECRET=GOCSPX-your-secret
GEMINI_CLI_OAUTH_CLIENT_SECRET=GOCSPX-your-secret
```

**6. OmniRoute neu starten**

```bash
# npm:
npm run dev

# Docker:
docker restart omniroute
```

**7. Beim nächsten Versuch noch einmal anbinden**

Benutzeroberfläche → Anbieter → Antigravity (oder Gemini CLI) → OAuth

Google wird nun korrekt auf `https://your-server.com/callback` umlenken.

---

#### Zum vorübergehenden Workaround (ohne eigene Anmeldeinformationen)

Wenn Sie keine eigenen Anmeldeinformationen einrichten möchten, können Sie den
**manuellen URL-Flow** nutzen:

1. OmniRoute öffnet die Google-Berechtigung-URL
2. Nachdem Sie autorisiert haben, versucht Google, auf `localhost` (was auf dem
   Remote-Server fehlschlägt) umzuleiten
3. **Die vollständige URL aus der Adressleiste Ihres Webbrowsers kopieren**
4. Daten in das Feld einfügen, das im OmniRoute-Verbindungsanzeige angezeigt
   wird
5. Dann klicken Sie auf **"Verbinden"**

> Das funktioniert, da der Autorisierungscode in der URL trotzdem gültig ist,
> unabhängig davon, ob die Seite geladen wurde.

---

<details>
<summary><b>🇧🇷 Versão em Português</b></summary>

#### Warum funktioniert der OAuth des Anitigravity/Gemini CLI nicht auf Remote-Servers?

Die Anbieter **Antigravity** und **Gemini CLI** verwenden **Google OAuth 2.0**
zur Authentifizierung. Der Google erfordert, dass die `redirect_uri` verwendet
wird, die im OAuth-Fluss verwendet wird, genau eine der im Google Cloud Console
des Apps. eingetragenen vorausbestimmten URIs.

As Credenciae OAuth integriert in OmniRoute sind nur für `localhost`**
aufgeführt **. Wenn Sie OmniRoute auf einem Remote-Server zugreifen (z. B.
`https://omniroute.meuservidor.com`), lehnt Google die Authentifizierung ab:

```
Fehler 400: redirect_uri_mismatch
```

#### Lösung: Legen Sie Ihre eigenen OAuth-Credentials auf

Sie müssen einen **OAuth 2.0 Client ID** im Google Cloud Console mit der URI
Ihres Servers erstellen.

#### Schritt-für-Schritt-Anleitung

**1. Melden Sie sich bei Google Cloud Console**

Öffnen Sie: [ 1 https://console.cloud.google.com/apis/credentials ]

**2. Erstellen Sie einen neuen OAuth 2.0 Client ID**

- Klicken Sie auf **+ Erstellen Sie Credentials** → **"OAuth Client ID"**
- Anwendungsart: **"Webanwendung"**
- Name: Wählen Sie einen beliebigen Namen (z. B. `OmniRoute Remote`)

**3. Fügen Sie genehmigte Callback-URLs hinzu**

Im Feld **"genehmigte Callback-URLs"** fügen Sie hinzu:

```
https://seu-servidor.com/callback
```

> Ersetzen Sie `seu-servidor.com` durch Ihren Domänennamen oder IP-Adresse Ihres
> Servers (einschließlich Port, z. B. `http://45.33.32.156:20128/callback`).

**4. Speichern und Kreditkarteninformationen kopieren**

Nachdem Sie erstellt haben, zeigt Google den **Client-Id** und die
**Client-Secret**.

**5. Konfigurieren Sie die Umgebungsvariablen**

In Ihrem [.env]`-Datei (oder den Umgebungsvariablen Ihres Docker-Containers):

```bash
# Für Antigravity:
ANTIGRAVITY_OAUTH_CLIENT_ID=seu-client-id.apps.googleusercontent.com
ANTIGRAVITY_OAUTH_CLIENT_SECRET=GOCSPX-seu-secret

# Für Gemini CLI:
GEMINI_OAUTH_CLIENT_ID=seu-client-id.apps.googleusercontent.com
GEMINI_OAUTH_CLIENT_SECRET=GOCSPX-seu-secret
GEMINI_CLI_OAUTH_CLIENT_SECRET=GOCSPX-seu-secret
```

**6. Die OmniRoute neu starten**

```bash
# Falls Sie npm verwenden:
npm run dev

# Falls Sie Docker verwenden:
docker restart omniroute
```

**7. Verbinden Sie sich erneut**

Dashboard → Anbieter → Antigravity (oder Gemini CLI) → OAuth

Die Google-Direktanweisung wird nun korrekt auf
`https://seu-servidor.com/callback` umgeleitet und die Authentifizierung
funktioniert.

---

#### Arbeitsumgangsmethode (ohne eigene Anmeldedaten zu konfigurieren)

Wenn Sie nicht eigene Anmeldedaten erstellen möchten, können Sie auch den
**manuellen-URL-Fluss** verwenden:

1. Der OmniRoute öffnet die Google-Benutzeranmelde-URL
2. Nachdem Sie autorisiert haben,versucht Google, auf `localhost` (was auf dem
   Remote-Server fehlschlägt) umzuleiten
3. ** Kopieren Sie die gesamte URL** aus der Browser-Adresseleiste (auch wenn
   die Seite nicht geladen wird)
4. Fügen Sie diese URL in das Feld im Modal-Steuerungsdialog ein
5. Klicken Sie auf **"Verbinden"**

> Diese Arbeitsumgangsmethode funktioniert, weil der Autorisierungscod in der
> URL unabhängig von der Umzuleitung gültig ist.

</details>

---

</details>

## 🛠️ Tech Stack

<details>
<summary><b>Click to expand tech stack details</b></summary>

- ** Runtime**: Node.js 18–22 LTS (⚠️ Node.js 24+ ist **nicht unterstützt** —
  `better-sqlite3`-Native-Binärpakete sind inkompatibel)
- **Sprache**: TypeScript 5.9 — **100% TypeScript** über `src/` und `open-sse/`
  (kein `any` in Kernmodulen seit v2.0)
- ** Framework**: Next.js 16 + React 19 + Tailwind CSS 4
- ** Datenbank**: LowDB (JSON) + SQLite (Domanenzustand + Proxy-Protokoll +
  MCP-Audit + Routenentscheidungen)
- ** Schemata**: Zod (MCP-Werkzeug I/O-Validierung, API-Verträge)
- ** Protokolle**: MCP (stdio/HTTP) + A2A v0.3 (JSON-RPC 2.0 + SSE)
- **Streaming**: Ereignisse vom Server (sse)
- **Auth**: OAuth 2.0 (PKCE) + JWT + API-Schlüssel + MCP-Scope-Berechtigungen
- **Testing**: Node.js-Tester + Vitest (900+ Tests einschließlich Einzellisten,
  Integrationstests, E2E)
- **CI/CD**: GitHub Actions (Auto-Veröffentlichung von npm + Docker Hub bei
  Veröffentlichung)
- **Website**: [omniroute.online](https://omniroute.online)
- **Package**:
  [npmjs.com/package/omniroute](https://www.npmjs.com/package/omniroute)
- **Docker**:
  [hub.docker.com/r/diegosouzapw/omniroute](https://hub.docker.com/r/diegosouzapw/omniroute)
- **Resilience**: Strombrecher, exponentielle Rücklaufzeit, Antithundering-Herd,
  TLS-Täuschung, Selbstheilung

</details>

---

## Dokumentation

| Dokumentieren                                   | Beschreibung                                                       |
| ----------------------------------------------- | ------------------------------------------------------------------ |
| [Benutzerführer](docs/USER_GUIDE.md)            | Anbieter, Kombinationen, CLI-Integration, Bereitstellung           |
| [Referenz für die API](docs/API_REFERENCE.md)   | Alle Endpunkte mit Beispielen                                      |
| [Server von MCP](open-sse/mcp-server/README.md) | 16 MCP-Werkzeuge, IDE-Konfigurationen, Clients für Python/TS/Go    |
| [Server von A2A](src/lib/a2a/README.md)         | JSON-RPC 2.0-Protokoll, Fähigkeiten, Streaming, Aufgabenverwaltung |
| [Auto-Kombinations-Engine](docs/auto-combo.md)  | Sechsfaktor-Bewertung, Modulpakete, Selbstheilung                  |
| [Troubleshooting](docs/TROUBLESHOOTING.md)      | Häufige Probleme und Lösungen                                      |
| [Architecture](docs/ARCHITECTURE.md)            | Systemarchitektur und interne Funktionen                           |
| [Contributing](CONTRIBUTING.md)                 | Entwicklungsumgebung und Leitlinien                                |
| [OpenAPI Spec](docs/openapi.yaml)               | Offene API 3.0-Spezifikation                                       |
| [Security Policy](SECURITY.md)                  | Meldung von Sicherheitslücken und Sicherheitspraktiken             |
| [VM Deployment](docs/VM_DEPLOYMENT_GUIDE.md)    | Vollständiger Leitfaden: VM + nginx + Cloudflare-Setup             |
| [Features Gallery](docs/FEATURES.md)            | Visualer Dashboard-Tour mit Screenshot                             |
| [Release Checklist](docs/RELEASE_CHECKLIST.md)  | Prüfungsritte vor der Veröffentlichung                             |

---

## 🗺️ Roadmap

OmniRoute hat **210+ Funktionen geplant**, die sich über mehrere
Entwicklungsphasen erstrecken. Hier sind die Schlüsselfelder:

| Kategorie                       | Geplante Funktionen | Hervorhebungen                                                                                                           |
| ------------------------------- | ------------------- | ------------------------------------------------------------------------------------------------------------------------ |
| 🧠 **Routen- und Intelligenz**   | 25+                 | Route mit niedrigster Latenz, Routenzuordnung anhand von Tags, Ermittlung der Ermächtigungen sowie Auswahl der P2C-Konto |
| 🔒 **Sicherheit und Compliance** | 20+                 | SSRF-Stärkung, Kredentialenkloaking, Endpunkt-gruppierung, Management-Schlüssel-Zuweisung                                |
| 📊 **Beobachtbarkeit**           | 15+                 | Integration von OpenTelemetry, reale Quotenüberwachung, Kostentracking pro Modell                                        |
| 🔄 **Provider-Integrations**     | 20+                 | Dynamische Modellregistrierung, Anbieter-Kühllasten, mehrere Codeds, Codex-Zuweisungskommutation                         |
| ⚡ **Leistung**                  | 15+                 | Dual Cache-Schicht, Prompt-Cache, Antwort-Cache, strömensbestehtende Kommunikation, Batch-API                            |
| 🌐 **Ökosystem**                 | 10+                 | WebSocket-Application, Konfiguration-Hotreload, verteilte Konfigurationsdatei, kommerzieller Modus                       |

### Demnächst

- 🔗 **OpenCode-Integration** — Inbegriff von Anbieterfunktionen für die
  OpenCode-AI-Codierungsumgebung
- 🔗 **Integration mit TRAE** — Vollständige Unterstützung für die TRAE
  AI-Entwicklungsframework
- 📦 **Batch-API** — Asynchrone Verarbeitung von Bulk-Anfragen
- 🎯 **Tag-basierter Routing** — Routen Sie Anfragen basierend auf
  Benutzerdefinierten-Tags und -Metadaten
- 💰 **Wenigstpreis-Strategie** — Wählen Sie automatisch den günstigsten
  verfügbaren Anbieter

> 📝 Vollständige Funktionsspezifikationen finden Sie in
> [`docs/Neue-Funktionen/`](docs/new-features/) (217 detaillierte
> Spezifikationen)

---

## 👥 Beiträge

[![Beiträge](https://contrib.rocks/image?repo=diegosouzapw/OmniRoute&max=100&columns=20&anon=1)](https://github.com/diegosouzapw/OmniRoute/graphs/contributors)

### Wie zum Beitrag

1. Fork das Repository
2. Erstellen Sie eine Feature-Branche (`git checkout -b
   feature/amazing-feature`)
3. Komittieren Sie Ihre Änderungen (`git commit -m 'Fügen Sie eine
   beeindruckende Funktion hinzu'`)
4. Pushen Sie in den Branch (`git push origin feature/amazing-feature`)
5. Öffnen Sie eine Pull-Forderung

Siehe [CONTRIBUTING.md](CONTRIBUTING.md) für detaillierte Informationen

### Veröffentlichen Sie eine Neue Version

```bash
# Eine Veröffentlichung erstellen — npm publish geschieht automatisch
gh release create v2.0.0 --title "v2.0.0" --generate-notes
```

---

## 📊 Sternengeschichte

## Sternengauer über die Zeit

## [![Sternengauer über die Zeit](https://starchart.cc/diegosouzapw/OmniRoute.svg?variant=adaptive)](https://starchart.cc/diegosouzapw/OmniRoute)

## 🙏 Erwähnungen

Sehr besondere Dank an **[CLIProxyAPI](https://github.com/decolua/9router)[X36X]
— dem ursprünglichen Go-Implentierun, der diese JavaScript-Zuordnung
inspirierte.

OmniRoute setzt diese faszinierende Grundlag außerdem mit zusätzlichen
Funktionen, multi-modaler APIs und einer vollständigen TypeScript-Umgeschreibung
fort.

---

## 📄 Lizenz

MIT-Lizenz - siehe [LICENSE](LICENSE) für Details.

---

<div align="center">
  <sub>Built with ❤️ for developers who code 24/7</sub>
  <br/>
  <sub><a href="https://omniroute.online">omniroute.online</a></sub>
</div>
<!-- GitHub Discussions enabled for community Q&A -->
