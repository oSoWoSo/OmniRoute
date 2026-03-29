# 🚀 OmniRoute — A Szabad AI Kapu

### Nem állj le a kódolásban. Intelligens csomagolás a **KIFEJEZÉSÉRTÉKÉRT és olcsó AI modellekhez ** automatikus fallback-vel.

_A világon minden API-proxynak ez a kényelmi pontja — 67+ szolgáltató, nulladik
leállás garantált. Most már elérhető _MCP és A2A-es ügynök-orchestráció.

**Chat Üzleti Befejezések • Beágyazási szolgáltatások • Képgenerálás • Videó •
Zene • Audio • Reranking • **A webes keresés** • MCP Szerver • A2A Protokoll •
100%-os TypeScript**

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
[![Licenc](https://img.shields.io/github/license/diegosouzapw/OmniRoute)](https://github.com/diegosouzapw/OmniRoute/blob/main/LICENSE)
[![Website](https://img.shields.io/badge/Website-omniroute.online-blue?logo=google-chrome&logoColor=white)](https://omniroute.online)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-Community-25D366?logo=whatsapp&logoColor=white)](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

[🌐 Oldal](https://omniroute.online) • [🚀 Gyors Kezdés](#-quick-start) • [💡
Funkciók](#-key-features) • [📖 Dokumentáció](#-documentation) • [💰
Árak](#-pricing-at-a-glance) • [💬
WhatsApp](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

</div>

🌐 A **költségmentes verzióiban** elérhető: 🇺🇸 [Angol](README.md) | 🇧🇷 [Portugál
(Brazília)](docs/i18n/pt-BR/README.md) | 🇪🇸 [Spanyol](docs/i18n/es/README.md) |
🇫🇷 [Francia](docs/i18n/fr/README.md) | 🇮🇹 [Olasz](docs/i18n/it/README.md) | 🇷🇺
[Orosz](docs/i18n/ru/README.md) | 🇨🇳 [Egyszerűsített
kínai](docs/i18n/zh-CN/README.md) | 🇩🇪 [Német](docs/i18n/de/README.md) | 🇮🇳
[hindi](docs/i18n/in/README.md) | 🇹🇭 [Thai](docs/i18n/th/README.md) | 🇺🇦
[Ukrán](docs/i18n/uk-UA/README.md) | 🇸🇦 [Arab](docs/i18n/ar/README.md) | 🇯🇵
[Japán](docs/i18n/ja/README.md) | 🇻🇳 [Vietnamese](docs/i18n/vi/README.md) | 🇧🇬
[Bulgár](docs/i18n/bg/README.md) | 🇩🇰 [Dán](docs/i18n/da/README.md) | 🇫🇮
[Finn](docs/i18n/fi/README.md) | 🇮🇱 [Héber](docs/i18n/he/README.md) | 🇭🇺
[Magyar](docs/i18n/hu/README.md) | 🇮🇩 [Indonéz](docs/i18n/id/README.md) | 🇰🇷
[Koreai](docs/i18n/ko/README.md) | 🇲🇾 [Malaj](docs/i18n/ms/README.md) | 🇳🇱
[Holland](docs/i18n/nl/README.md) | 🇳🇴 [Norvég](docs/i18n/no/README.md) | 🇵🇹
[Portugál (Portugália)](docs/i18n/pt/README.md) | 🇷🇴
[Román](docs/i18n/ro/README.md) | 🇵🇱 [Lengyel](docs/i18n/pl/README.md) | 🇸🇰
[Slovak](docs/i18n/sk/README.md) | 🇸🇪 [Svéd](docs/i18n/sv/README.md) | 🇵🇭
[Filippínó](docs/i18n/phi/README.md) | 🇨🇿 [Cseh](docs/i18n/cs/README.md)

---

## 🆕 A v3.0.0 új funkciói

> **Az v2.9.5-ből frissít?**? — Lásd a [teljes VÁLTTABLE
> CHANGELOG](CHANGELOG.md#300--2026-03-22-release-candidate--not-yet-merged-to-main)
> az összes változat részleteit.

| Terület                                     | Változás                                                                                                                                                                                                                                  |
| ------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🔒 **CodeQL Biztonság**                      | Szerelték 10-nél több CodeQL-bajnokot: polynomial-redos, insecure-randomness, shell-injection remediation                                                                                                                                 |
| ✅ **Útvonal-igazolás**                      | Az összes 176 API-utat most már zod-sémával igazolják + `validateBody()` — CI `ellenőrzi: route-validation:t06`                                                                                                                           |
| 🐛 **omniModel címkelés**                    | Belülről `<omnimodel>` címkékből kitérik a klientekhez a SSE-áramlásban (#585)</omnimodel>                                                                                                                                                |
| 🔑 **Regisztrált kulcsok API**               | Automatikusan szállíthatja a regisztrált kulcsokat az ` /api/v1/registered-keys POST` művelettel a szolgáltató által megadott szintű, azonosítón hajtott módon, 256 bites SHA-256 tárolással és opcionálisan GitHub probléma jelentéssel. |
| 🎨 **Szolgáltató ikonok**                    | 130+ szolgáltató ikonja a `@lobehub/icons` (SVG) a PNG-hez tartozó általános lecserélési lánc  -> fallback lánc                                                                                                                           |
| 🔄 **Modell Automatikus Sínkron**            | 24 órás ütemezővel és kézi UI kapcsolóval szinchronizálják a modelleket listákat a belső és a szabványos OpenAI-hozamszolgáltatók számára                                                                                                 |
| 🌐 **Megtörölt Zen/Beszel**                  | Két új szolgáltatót kapunk @kang-heewon  köszönhetően a PR #530: ingyenes szint + előfizetési szint a `OpencodeExecutor`-szal                                                                                                             |
| 🐛 **Gemini CLI OAuth**                      | Aktíva hibaüzenet, ha `GEMINI_OAUTH_CLIENT_SECRET` hiányzik a Dockerben (korábban titkosozó Google hiba)                                                                                                                                  |
| 🐛 **OpenCode konfigur**                     | `saveOpenCodeConfig()` most sokszorosan írja le a `XDG_CONFIG_HOME`-ba a TOML-t                                                                                                                                                           |
| 🐛 **Folyamatosan lefagyasztott modellezés** | `body.model` helyesen állítja be a `pinnedModel`-t a kontext- puffer-protektorokon                                                                                                                                                        |
| 🐛 **Codex/Mintvégzéstöredék**               | `tool_result` blokkok most szöveggé változtatnak, hogy megszüntessék az egybefolyó köröket                                                                                                                                                |
| 🐛 **Regisztráció visszinavig**              | Regisztráció nincs megakadályozva a jelentkezés elutasítása helyett                                                                                                                                                                       |
| 🐛 **Windowsútvonalat**                      | MSYS2 / Git-Bash utak (`/c/...`) normálisabban váltanak `C:\...`-re automatikusan                                                                                                                                                         |

---

## 🖼️ Fő oldal

<div align="center">
  <img src="./docs/screenshots/MainOmniRoute.png" alt="OmniRoute Dashboard" width="800"/>
</div>

---

## 📸 Prezentációs oldal

<details>
<summary><b>Click to see dashboard screenshots</b></summary>

| Lap                       | Képernyőkép                                           |
| ------------------------- | ----------------------------------------------------- |
| **Szállítók**             | ![Szállítók](docs/screenshots/01-providers.png)       |
| **Kombinációs elemek**    | ![Kombinációs elemek](docs/screenshots/02-combos.png) |
| **Analitika**             | ![Analitika](docs/screenshots/03-analytics.png)       |
| **Egészség**              | ![Egészség](docs/screenshots/04-health.png)           |
| **Fordító**               | ![Fordító](docs/screenshots/05-translator.png)        |
| **Beállítások**           | ![Beállítások](docs/screenshots/06-settings.png)      |
| **CLI-es eszközök**       | ![CLI eszközök](docs/screenshots/07-cli-tools.png)    |
| **Felhasználási naplók**' | ![Felhasználási](docs/screenshots/08-usage.png)'      |
| **Végpontok**             | ![Végpontok](docs/screenshots/09-endpoint.png)        |

</details>

---

### 🤖 Ingyenes AI-szállító a kedvenc kódoló ügynökeihez

_ Kapcsolódjon bármely AI-hajtású IDE vagy CLI eszközt az OmniRoute-on keresztül
— ingyenes API gateway a korlátlan kódolásra._

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

<sub>📡 Az összes ügynök csatlakozik <code>http://localhost:20128/v1</code> vagy
<code>http://cloud.omniroute.online/v1</code> — egy konfiguráció, korlátfutól
tér és kvóták</sub>

---

## 🤔 Miért az OmniRoute?

** Több ezer forintot és határok terhelését hagyja maga mögött:**

- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  A felhasználható kvóta minden hónap végén eltűnik
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  A korlátozások a kódolás folyamatban abbahagyják
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Drága API-k ($20-50 hónapnyi szolgáltató/és)
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Egyéni váltógyorsítók kezelése

**Az OmniRoute megoldja mindezt:**

- ✅ ** Maximális licencek - Figyelje a kvótát, és használja fel minden sort a
  lejárattal
- ✅ **Automatikus visszapapucs ** - Licence → API Kód → Ár ~ 0, sem egyetlen
  pillanat leállás nélkül
- ✅ **Multi-számla** - Fordítson az egyes fiókok között a szolgáltatók
- ✅ **Univerzális** - Működik a Claude Code, Codex, Gemini CLI, Cursor, Cline,
  OpenClaw, tetszés szerinti CLI eszközzel

---

## 📧 Támogatás

> 💬 **Csatlakozzon a közösségünkhöz!** [WhatsApp
> csoport](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t) —
> Kaptassa meg a segítséget, és ossza meg az ötleteket!

- **Honlap**: [omniroute.online](https://omniroute.online)
- **GitHub**:
  [github.com/diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute)
- **Hibák**:
  [github.com/diegosouzapw/OmniRoute/issues](https://github.com/diegosouzapw/OmniRoute/issues)
- **WhatsApp**: [Közösségi
  csoport](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)
- **Hozzájárulás**: tekintse meg a [CONTRIBUTING.md](CONTRIBUTING.md) - nyisson
  egy pull requestet, vagy válasszon egy `jó első probléma`
- **Eredeti Projekt**: [9útvonal by decolua](https://github.com/decolua/9router)

### 🐛 Hibajelentés?

Amikor problémafelderjesztést hoz létre, futassa a rendszerinformáció parancsot,
és csatolja a generált fájlt:

```bash
npm run system-info
```

🔄 Hogyan működik

---

## Hogyan működik

```
🎯 Mi az OmniRoute, ami [30] valós problémákat és használhatósági eseteket  személyre szab!
```

---

## [X0X]Minden olyan fejlesztő, akinek van AIIal isznak mindennap e problémákat[X60X] .  OmnitRoutet építették ezek megoldásához — az ingyen felújítási probléma, regionális blokkok, töredék OAuth folyamok, protokolloperációk és az összszembenzésől való személyiség és produktivitás.

> Fejlesztők az [X17X]Claude Pro[X20X], [X17X]Codex Pro[X20X], vagy a
> [X13X]GitHub Copilot[X11X] utazásáért 20–200 Dollár havonta fizetnek. Egyedül
> is fizetés ellenére, a kredit leáll 5 óra hasznás, heti korlátok, és alap ár
> szintek. Képbeszerzési folyamat közben, a szolgáltató nem válaszol, és a
> fejlesztő elveszti a termelékenységét.

<details>
<summary><b>💸 1. "I pay for an expensive subscription but still get interrupted by limits"</b></summary>

[X0X]Intelligens 4 Rendfokozatú esés[X23X] — Ha a szolgáltató leáll a
regisztrációs kredit, a automatikusan áttervel a API kulcs → A olcsóbb → A
INGYEN, beleértve a kérői segédleteket is.

**Hogy a OmniRoute megoldja:**

- ** Valós Idö Kredit nyilvántartás[X26X] — Megjeleníti a a kredit fogyasztást
  valós időben a megszüntetési idéző órával 5 óra ,nap, heti.
- **A Multipotenciázott szolgáltatás allokáció X23X] — Több szolgáltatóhoz
  hozzáfér a automatikusz alapcsoport.
- **Kilépés személyre szabás[X15X] — A kiegyeztetési sorrend és a kiépítéses
  sorrend változatos álmazolás.
- **Kodex üzleti Kredit[X23X] — Kreditnyilvántartás a Dashboardon.
- Az OpenAI az egyik fomratot használja valaki a Claude, míg Gemini egy másikat
  és több szkedaros eszközök is másformát. Leáll az eszköz működésé,
  valószínűleg a modell folyamat a válaszok API kulcs kód esetében szükséges az
  a formátum adhat.

</details>

<details>
<summary><b>🔌 2. "I need to use multiple providers but each has a different API"</b></summary>

[X0X]együtített szolgáltatás végpont[X18X] — a szolgáltatás
[X32X]http://localhost:20128/v1[X58X] valt a [67] többik összes kérést a a API
szolgáltatónál.

**Hogy a OmniRoute megoldja:**

- ** Format fordítás[X20X] — Fornatoátviteli fordítás minden esetben kéri a
  automatikus lefordítást azon érintetett formában — OpetAIFordítás a Claue
  fordításként és Gemini formátumnak kéri kódra fordítás a válaszként kódra
  kiállítási feladatként
- Egy weboldaltól több másik oldal felé is kérdezheti a szolgáltatás ad a valós
  példány számának megfelelő valós válasz küldete megadva hogy melyik
  végpontokra és kérjék támogatását a kérésre , de a kérés útvonalának a kérés
  támogatott formátumairól a szolgáltatás hajtja végre a fordítást.
- **Visszafejlesztésbiztonság** – Törli a nem szabványos mezőket (`x_groq`,
  `használati statisztika`, `szolgáltatói réteg`) amelyek törvényellenesek az
  OpenAI SDK v1.83+
- **Szerepkör Egyszerűsítése** – Konvertálja ` fejlesztő` → ` rendszer` az
  OpenAI szolgáltatók számára; ` rendszer` → ` felhasználó` a GLM/Ernier számára
- **Vélekedési cimkézet kinyerése** – Kinyeri a `` blokkokat a DeepSeek R1
  modelből a standardizált `indokolás` tartalomra
- **Tagolva kimenet a Gemini számára** – `Json szabvány` →
  `eredménytípus`/`eredmény szabvány` automatikus konverzió
- **A `stream` alapértelmezés a `false`-ra** – Sajtó alatt a szabványos OpenAI
  megoldást alkalmazza

</details>

<details>
<summary><b>🌐 3. "My AI provider blocks my region/country"</b></summary>

Néhány szolgáltató eltiltja a bizonyos földrajzi régiókból származó
felhasználókhoz való könnyű hozzáférést, és a felhasználók `támogatott ország
területi régiója` üzenetet kapnak az autentikációnál és az API kapcsolódáskor

**Hogy a OmniRoute megoldja:**

- **3 Ürüknél Proxy Konfiguráció** – Konfigurálható a proxy a különböző
  szinteken, például globálisan, egyetlen szolgáltatónál, vagy a szolgáltatásra
  kiterjedő hozzáférés nélkül
- **Színkódolt Proxy Jelzések** – Jellegek: 🟢 globális proxy, 🟡 szolgáltatói
  proxy, 🔵 kapcsolodási proxy, mindig megmutatja az IP címet
- **OAuth Jelszócseré [Proxyon** – Az OAuth folyamat is áthalad a proxyon,
  megoldva a ` nem támogatott ország területi régiója` problémáját
- **Féltéri Kapcsolódási Tesztek proxyon** – A kapcsolódási tesztek is
  áthaladnak a proxyon (másnapos késleltetés nélkül)
- **SOCKS5 Támogatás** – Teljes támogatás a SOCKS5 proxy számára a kimenő
  útvonalhoz
- ** TLS Fingerprin Csalás** – Ügynöki kapcsolat-szimuláció a ` wreq-js `
  segítségével a bot-detektáláshoz
- ** 🔏 CLI Címtartalmi Megfeleltetés** – Újrafogja a fejlécek és a test mezőit
  hogy megfeleljenek a natív CLI alapértelmezett binárszámlálóségi jeleihez,
  amely drasztikusan csökkenti a számlatartomány-veszélyfaktort a számítógépen
  is. A proxy-IP-t is megőrzi, így mind a szöveges és az IP-jelazási mód
  szimulálható

</details>

<details>
<summary><b>🆓 4. "I want to use AI for coding but I have no money"</b></summary>

Nem mindenki fizetheti az egyesülési felügyeltséghez $20–200–havi díjat. A
hallgatók, a fejlesztők az útkereső országokból, az amatőrök, az útonállók és a
szegény országokból származó fejlesztők számára szüksége van az áttűnően magas
minőségű modellhez a végleges díj nélkül

**Hogy a OmniRoute megoldja:**

- **Free Tier szolgáltatók beépítve** – Teljes támogatás a 100%- árajánlati
  jelenléte: iFlow (5 korlátlan modellhez az OAuth-nál: kimi-k2-gondolat,
  qwen3-coder-plus, deepseek-r1, minimax-m2, kimi-k2) Qwen (4 korlátlan modell:
  qwen3-coder-plus, qwen3-kód-verzió és fejlesztő, qwen3-kód-verzió és
  következő, vízió-modell), Kiro (Claude + AWS Fejlesztői azonosító számára
  ingyenes), Gemini CLI (180K token szabadon az ingyenes “fényes hozzáférés”
  rétegekkel)
- **Ollama felhő ** – Ollama-modell környezet elhelyezve ` api.ollama.com`
  ingyen “fényes használat” rétegekkel; használja a `ollama felhő/` prefikszet
- ** Kombináció Függ[18X] – Számolja össze a ` gc/gemini-3-verziós –
  gondolat/kimi-k2-gondolat verziót és a meghibásodással/kw/kwen3-coder-plussz
  verziót` = $0–dij növekedést az áttűnő nélkül
- ** NVIDIA NIM ingyenes elérése**– Körülbelül 40 RPM (modell/felszabadítások)
  szintű ingyenes hozzáférés 70-egyebek modellhöz a építőnél build.nvidia.com
  (átmenet a díjugyénttől a teljes növekedésig)
- Költségcsökkentő Stratégia — Ügynökségi stratégia, amely automatikusan
  kiválasztja az olcsóbban elérhető megfelelő szolgáltatót

</details>

<details>
<summary><b>🔒 5. "I need to protect my AI gateway from unauthorized access"</b></summary>

Amikor az AI-ügynököd számítógép-állomások, VPS, Docker elérést biztosít az
interneten (LAN, VPS, Docker), valaki a címével fogyasztja a fejlesztő
tokeneit/quórumát. Az expozíció nélkülvédelmetlen a véleménynyilvánítási
csatolókhoz kötődő API-ek túladást okozhatja, folyamatosabb működéshez, és
bántalmazáshoz.

**Hogy a OmniRoute megoldja:**

- API Legosztó Kezelés — API generálása, rotatívája és skálázása a megfelelő
  szolgáltatókkal, egy dedikált felület külön / felügyeleti oldalon
- Modell szintű hozzáférési jogosultságok — Korlátozza az API kulcsokat az adott
  modellekre (Openai/*, villámjelek halmazok) , hozzájárul a felhasználás,
  megszünteti tű
- API Végpontvédelem — Minden védjegy külön /v1/models és megakadályozza szöveg
  alapú szolgáltató lista felsorolás
- Hitelesített védjegy + CSRF védelem — Az összes felületalábizási útvonal
  védett a Auth kódolóval + CSRF token
- Háztartási korlátozó — IP alapú csatlakozási korlátozások szoftverben
  csatlakozásokkal korlátozott
- IP Továbbítás — Megengedett lista/blokklistarendszer felügyelet
- Mámorolt szövegszűrés védelme — Szövegszűrési patterekhez szánt mánia elleni
  védelme
- AES-256-GCM Titkosítás — Ellenőrzött jelszó titkosítás.

</details>

<details>
<summary><b>🛑 6. "My provider went down and I lost my coding flow"</b></summary>

Az AI szolgáltatások elhagyásához való vállalás nem stabil, 5XX HIBÁS érzetet
okozhat, vagy elérhető ideiglenes sebesség korlátokat be lehet kapcsolni. Egy
dev függ az egyszerűbb szolgáltatótól, akkor ismerkedik meg. A circuit Breaker
nélküli folyamatos ismétlések lehet, hogy az alkalmazást katasztrófára téríti

**Hogy a OmniRoute megoldja:**

- Költségcsökkentő Modell alapú — Automatikusan nyit/csoport alapú
  nyit/bezáráshoz szükség van
- Exponenciális Hátrameneti — Már sikerült hátramenetet alkalmazzék 2. szintű
- Antitenger szimuláció biztosítja védelmében 1. szintű és hátrameneti
  ellenállást
- Kombinációs válaszlánc a beázárok által előidézett hibák megjavításához
- Kombinációs Circuit — Auto szakítja fel az összeomlásokat a kombinált láncokat
- Egészségügyi felügyelet — Aktuális időkig tartó folyamatot\
  tartományok, lockouts cache-ek szigorú adatok, , p50 latencia

</details>

<details>
<summary><b>🔧 7. "Configuring each AI tool is tedious and repetitive"</b></summary>

Szerzők Cursor, Claude Kodokok, Gemini CLI.,, kilókod.... , Az összes eszközhöz
más és más konfigurációs állapot megfelelő API elérhetővé tétele, kulcs
adományozását, modullal kapcsolatos késik, az áthaladás a szolgáltatói által
előidézett újrakonfigurálás elhagyásnak az adott időszakon belül van szem
elvonásához.

**Hogy a OmniRoute megoldja:**

- **CLI Tools dashboard** — Speciális oldal az egyetlen kattintásos beállítással
  **Claude Code** -s, **Codex CLI**-hez, **OpenClaw**-hez, **Kilo Code**-hoz,
  **Antigravitáció**hoz, **Cline**hez
- **GitHub Copilot konfigurációs generátor** — `chatLanguageModels.json`
  generálja VS Code -bal tömbösztatú modellválasztással
- **Üzetelvő varázsló** — Első alkalommal használó felhasználók 4 lépéses
  beállítása
- **Egy endpoint, tizenhét modell** — Konfigurálja `http://localhost:20128/v1`-t
  csak egyszer, hozzáférjen 67 felett a szolgáltatókhoz

</details>

<details>
<summary><b>🔑 8. "Managing OAuth tokens from multiple providers is hell"</b></summary>

[X21X]Claude Code[X21X], [X21X]Codex[X21X], [X21X]Gemini CLI[X21X] és
[X21X]Copilot[X21X] mind OAuth 2.0-t használ feleződő jogkivonattal. A
fejlesztőknek állandó újrajelentkezésre van szüksége, megoldást kell találniuk a
` client_secret hiányára`, a ` redirect_uri mérlegelés`-re és hibaelhárításra
távoli szervereken. Az OAuth különösen problémás LAN/VPS környezetben.

**Hogy a OmniRoute megoldja:**

- **Autópályát megújítva** — Az OAuth-jogkivonatok automatikusan frissülnek a
  lejárati idő előtt
- **OAuth 2.0 (PKCE) beállítva** — Automatikus folyamat [X21X]Claude Code[X21X],
  [X21X]Codex[X21X], [X21X]Gemini CLI[X21X], [X21X]Copilot[X21X],
  [X21X]Kiro[X21X], [X21X]Qwen[X21X] és [X21X]iFlow[X21X]-hez
- **Multi-Account OAuth** — Több fiók/kiszolgáló érhető el JWT/ ID-tokenek
  kivonásával
- **OAuth LAN/Remote Fix** — magán IP-detektálás a ` redirect_uri`-re és tárolt
  URL módban távoli szervereknek
- **OAuth mögött Nginx** — ` window.location.origin` használatával
  visszaprofesszívtatás kompatibilitás
- **Távoli OAuth útmutató** — Lépésről lépésre a hibainformációk VPS/Docker-ben

</details>

<details>
<summary><b>📊 9. "I don't know how much I'm spending or where"</b></summary>

A fejlesztők több fizetős szolgáltatót használnak, de nincs közös megjelenítésük
a kiadásokról. Minden szolgáltatónak megvan maga a kiadási panelje, de nincs
egyeztetett megjelenítés. A váratlan kiadások felhalmozódnak.

**Hogy a OmniRoute megoldja:**

- **Kiadási analitikai panel** — Token-költség nyomon követése és a szolgáltatók
  által létrehozott költség kezelése egy személyen
- **Kiadási határolt értékek szinten** — Össztőke érték határolt korlátig, amely
  után automatikusan lecserél.
- **Beállítható ármodell konfiguráció** — Beállítható árak modellhez
- **Használati statisztika API billentyűn** — Látogatási szám és az utolsó
  felhasználási időpont API billentyűn.
- **Analitika panel** — Statisztikai kártyák, modellek használati diagrama,
  szolgáltatók táblázata sikerességi arányokkal és késési idővel.

</details>

<details>
<summary><b>🐛 10. "I can't diagnose errors and problems in AI calls"</b></summary>

==WEBLATE_PART==\
Amikor egy hívás megbukik, akkor a fejlesztő nem tudja megállapítani, hogy az
volt-e az oka a sűrűségkorlátozás, lejárt token, rossz formátum vagy
szolgáltatói hiba. A különböző terminálokon terjedt el a szétvált hibaüzenetek
nélkül a nyomon követés. Az observabilitás hiányában a hibakeresés kísérleti
módon zajlik.

**Hogy a OmniRoute megoldja:**

- **Egyesített naplók panela** — 4 lap: Kérés naplók, Szimulátor naplók,
  Átvevőfelügyeleti naplók, Konszol
- **Konszol napló nézegető** — Valós idejű terminálszerű nézete a színezett
  szintekkel, automatikus átfedők, kereshetőség, szűrhetőség
- **SQLite szimulátor naplók** — Állomáson túl megmaradó, rögzített naplók, ami
  fennmarad a szerver újraindítása után is
- **Fordító öntöző** — Nyolc fejlesztési módban vizsgálhatja a fordítását,
  kísérleti modell vizsgálat, visszaalapú, házhoz kész tesztben, élő
  monitorozásban, fordítás nézetben
- **Kérési azonosíto mélységrend vizsgálata** — p50/p95/p99 késedelem vizsgálat
  + X-Request-Id azonosító követés
- **Fájl alapú rögzítés a méret alapú szétválasztással** — Konzol-átvevő a JSON
  alapú naplóval, a méret alapú megújítással
- **Vegyes információk jelentése** — Vegyél fel `npm run system-info` parancsot
  `system-info.txt` fájllal, ami egész rendszer adatait mutatja (Node verzió,
  OmniRoute verzió, OS, parancssoros eszközök, Docker/PM2 értesültsége) a
  hibakereséshez gyors triászhoz az elszámoláshoz. Kössön rá, amikor el akarja
  küldeni a hibással együtt

</details>

<details>
<summary><b>🏗️ 11. "Deploying and maintaining the gateway is complex"</b></summary>

Egy szoftver alatt levő intelligens proxy alapú automatizálást támogató
szervezetek számára számos kihívás áll fenn. A különböző környezetekben történő
konfigurálás és karbantartás a legfőbb probléma. A rendszerben bekövetkezett
hibákat és problémákat könnyedén nyomon tudjuk követni a felülvizsgálat.

**Hogy a OmniRoute megoldja:**

- **npm globális telepítése** — `npm install -g omniroute &amp;&amp; omniroute`
  — kész
- **Docker közönséges alaprendszer** — AMD64 + ARM64 értelmezhető kimenetet
  (Gizdokoló Apple Silicon, AWS Graviton, Raspberry Pi
- **Docker összetett profiljai** — kétféle fejlesztési kialakítás támogatja
  (szkript nélkül `base` és Claude kód, Codex, OpenClaw kialakítású `cli`
- **Electron asztali alkalmazás** — Natív alkalmazás a Windows, Mac vagy Linux
  rendszerhez is értelmezhető, a rendszer ikonján megmutatja, a háttérben
  futásban, átmenetlanül is fut a program
- **Háromszórdító módi** — Különböző eszköz (inverz proxy, csomópont eszközök)
  környezetében a különböző mód felülvizsgátlan kereséssel
- **Nuvolazúrással együtt ** — Konfigurációs központítás a különbözö készülékek
  között a Cloudflare munkásokkal
- **Bd visszafejezással** — automatikus vissza fejezet, vissza adt szükség
  szerint adatokhoz kapcsolva

</details>

<details>
<summary><b>🌍 12. "The interface is English-only and my team doesn't speak English"</b></summary>

A nemzetközi vállalatok támogatják az egyéb nem angol anyanyelvű országok
lakosainak a vállalatukhoz való bejelentkezését. Rendszeresül erősen
viszonyulnak az angol nyelvhez, ezért az angol nyelvegyenyebb rendszerrel
kapcsolatos kihívások elcsökkennek.

**Hogy a OmniRoute megoldja:**

- **Irányítópult beállítások — 30 nyelv, beleértve az arabot, bolgárt, dánia,
  németet, spanyolt, finnt, franciót, hébert, hindikat, magyart, indonézit,
  olaszot, japánt, koreait, malájot, hollandot, norvégit, lengyelet, portugál
  (PT/BR), románt, oroszot, szlovákot, svédet, thai, ukrán, vietnámi és kínai
- **RTL támogatás ** – A jobbról balra irányú támogatás arab és héber számára
- **Multi-Lang READMEs** – 30 teljes dokumentációs fordítás
- **Nyelv kiválasztó** – A globusz ikon a fejlécben valós idejű váltásra

</details>

<details>
<summary><b>🔄 13. "I need more than chat — I need embeddings, images, audio"</b></summary>

A mesterséges intelligencia nem csak chat kiegészítés. A fejlesztőknek kéne
generálnia képeket, átírnia audiókat, létrehozni beágyazásokat RAG számára,
úsztassanak dokumentumokat és moderálják a tartalmat. Minden API-nak más a
végpontja és formátuma.

**Hogy a OmniRoute megoldja:**

- **Beágyazások** – `/v1/beágyazások` 6 szolgáltatóval és 9+ modelllel
- **Kép generálás** – `/v1/képek/ generálások` 10 szolgáltatóval és 20+ modellel
  (OpenAI, xAI, Together, Fireworks, Nebius, Hyperbolic, NanoBanana,
  Antigravity, SD WebUI, ComfyUI)
- **Szöveg-videó** – `/v1/video/generálások` – ComfyUI (AnimateDiff, SVD) és SD
  WebUI
- **Szöveg-zene** – `/v1/zene/generálások` – ComfyUI (Stable Audio Open,
  MusicGen)
- **Audió feljegyzés** – `/v1/audió/feljegyzések` – Whisper + Nvidia NIM,
  HuggingFace, Qwen3
- **Szöveg-beszéd** – `/v1/audió/beszéd` – ElevenLabs, Nvidia NIM, HuggingFace,
  Coqui, Tortoise, Qwen3, **Inworld**, **Cartesia**, **PlayHT**, + létező
  szolgáltatók
- **Módosítások** – `/v1/módosítások` – Tartalom biztonsági ellenőrzések
- **Úsztatások** – `/v1/úsztatások` – Dokumentumok relevanciájának úsztatása
- **Válaszok API-ja** – `/v1/válaszok` támogatás Codex számára

</details>

<details>
<summary><b>🧪 14. "I have no way to test and compare quality across models"</b></summary>

A fejlesztők akarják tudni, hogy melyik modell a legjobb a feladatukhoz — kód,
fordítás, logika — de manuálisan összevetni azokat több időbe kerül. Nem
léteznek integrált értékelési eszközök.

**Hogy a OmniRoute megoldja:**

- **LLM értékelések** – Aranyított beállítások tesztelése 10 előre betöltött
  esetvel, amelyek közzé tartalmazza köszöntéseket, matematikai feladatokat,
  geográfiát, kódgenerálást, JSON egyezőséget, fordítást, markdownt, biztonsági
  megtagadást
- **4 Hasonlósági stratégiák** – `teljes[H31X], `tartalmaz`,
  `összefüggésszintű`, `élszintű` (JS függvény)
- **Fordító Játsszó szabályozó Tesztelő bánya** – Többlépcsős tesztelés több
  bemenettel és várható kimenettel, szörfözéses összehasonlítás
- **Hívási Tesztelő** — Teljes körrel megjelenő visszavert válasz-ábrázolás
- **Élő Monitor** — Valós idejű áramlást mutató összes kérelmező forgalom

</details>

<details>
<summary><b>📈 15. "I need to scale without losing performance"</b></summary>

Ahogy a kérelemvolumen növekszik, anélkül, hogy a kiegészítést használnák a
megismételt kérdések duplikálják a költségeket. Azonos kérelmek nélküli
idempotenciáció használata után az időpontok duplikálják a feldolgozást.

**Hogy a OmniRoute megoldja:**

- A per-fordító törvényeknek tartósaknak kell lenniük.\
  **Semantic Cache** — Kétfokú kiegészítés (jellemző + szemantikus) csökkenti a
  költségeket és a késedelemet
- **Kérés Idempotencia** — 5 másodperc idejű deduplikációs ablak azonos
  kérelmekhez
- **Limit Detektálás** — Per-fordító RPM, minimum távolság és maximális egyidejű
  nyomon követés
- **Szerkeszthető Lényegi Korlátok** — Alapértelmezett konfigurálható
  beállítások a Beállítások → Szilárdságban való fennmaradással
- **API Kulcs Változtatási Kiegészítés** — 3 fokú kiegészítés az előállítás
  biztonsága érdekében
- **Egészségügyi Főpult Telemetria** — p50/p95/p99 késésektelenség, kiegészítési
  statisztika, rendszerfelügyele

</details>

<details>
<summary><b>🤖 16. "I want to control model behavior globally"</b></summary>

A fejlesztők, akikeknek minden válasz külön kifejezett nyelvet kíván, egy adott
hangnemben, vagy akik akarják korlátozni az érvelési tokeneket. A konfigurálást
minden eszköz/kérelemhez való kiruházás realiszta praktikus lenne.

**Hogy a OmniRoute megoldja:**

- **Rendszer Jelzési Beemelés** — Globális jelzés, amit az összes kérést
  megjeleníti
- **Gondolkodási Budget Ellenőrzés** — Az érvelési tokenek szállításának
  kontrollja kérésemhez (átmenyélés, auto, custom, adaptív)
- **6 Útvonal Stratégia** — Globális stratégia, ami meghatározza, hogy a kérések
  hogyan osztódnak el a szerverekre
- **Felszabadult Router** — `nyúlványnév/*` minták útvonali dinamikus rendelés a
  bármely szerverre
- **Gomb Csatornamentes Toggel** — Gomb megcsatornázása az első oldalakról
- **Fehérvár Forrás Aktivál/X17X] — Aktivál/leállít egyetlen gombbal
- **Elzárva Kiválasztani Forráski** — Bizonyos választos forráskódok elzárása
  /v1/models` listaról

</details>

<details>
<summary><b>🧰 17. "I need MCP tools as first-class product capabilities"</b></summary>

Sok érzelmi kapcsolat kínálja megcsapoljuk csomónak felfedezési. Az egység
tesztelő csapatoknak egy látható folyamodás réteget kell felmutatniuk.

**Hogy a OmniRoute megoldja:**

- Navigációs menüre és végponti protokoll ablakra jelzés MCP
- Alkalmazás MCP-kezelésére felkészítő oldal eljárások, eszközök, tárhelyek és
  felügyelet
- Ügyfélön onboardolásra, mivel a `omniroute --mcp` beépített, gyorskezdő
  eljárás MCP és ügyfél beállítási felületével

</details>

<details>
<summary><b>🧠 18. "I need A2A orchestration with sync + stream task paths"</b></summary>

Az ügynök munkafolyamatok az ügyfélképesség mellett szükségessé teszi a hosszan
futó, streamelt kimenő adatküldést életciklus-szabályozással

**Hogy a OmniRoute megoldja:**

- Az A2A JSON-RPC végpontja (`POST /a2a`) támogatja a `üzenet/küldés` és
  `üzenet/stróma` HTTP funkciókat
- A végpont egyidejűleg áramkörökkel együtt streamelt kimenő adatküldést
  biztosít
- Feladat életciklus-kezelési API-k a `feladat/kiv[/X34X] és `feladat/megsz`
  felületet kínálja

</details>

<details>
<summary><b>🛰️ 19. "I need real MCP process health, not guessed status"</b></summary>

A felhasználók munkacsoporthoz való hozzáféréshez szükséges tudni, hogy
valójában működik-e az MCP, vagy csak nem lehet elérni a rendszerének APIikat

**Hogy a OmniRoute megoldja:**

- Aktuális lelövési fájl a MCP statikus lelövésének biztosítása a PID-vel,
  időbélyegekkel, a kapcsolat típusával, eszközszámával és a tárhely
  módosításával
- Az MCP működési APIja együttesen hasznosítja az aktív lelövési fájl és az
  utóbbi tevékenység aktuális információit
- Processzus életciklusének és aktív lelövésének frissességi feltüntetése

</details>

<details>
<summary><b>📋 20. "I need auditable MCP tool execution"</b></summary>

A beállítások során tett eszköz-módosítások és az operációs műveleteket aktiváló
csomópok által előidézett áthajtásnak lehetővé kell tennie a nyomozó felületet

**Hogy a OmniRoute megoldja:**

- Az MCP hívásainak auditálásával lehet egy olyan alaplapra szállítani a nyomozó
  felületet, amelyen a SQLite adatbázis használatával elmentve vannak a
  folyamatok adatai
- A tolografikus audit folyamat filteres lesz, és környezeti szabályozást
  tartalmaz majd
- A felületen audittáblák és statisztikai végpontok hozzáféréssel rendelkeznek a
  rögzítési mechanizmussal kapcsolatos műveletek aláfestéséhez

</details>

<details>
<summary><b>🔐 21. "I need scoped MCP permissions per integration"</b></summary>

Az ügyfeleknek legbővebb privilégia áramkörhöz való biztosításának szüksége van
a kategóriák szintjén.

**Hogy a OmniRoute megoldja:**

- 9 részletes MCP-áttekintési lehetőség a kontrollált eszköz hozzáféréshez
- Az MCP-fitetés és láthatósága az MCP-gazdász összetett ÜI-ben
- Operatív eszközök gyorsabb biztonságos alapállapotának biztosítása

</details>

<details>
<summary><b>⚙️ 22. "I need operational controls without redeploying"</b></summary>

Csapatoknak sürgős runtime-módosításokra van szükségük események vagy
költség-helyzetek során.

**Hogy a OmniRoute megoldja:**

- A Combo gyors aktiválása közvetlenül az MCP-asztalfelülettől
- A rezillencia-profilok alkalmazása a meghatározott policy-packekből
- A Circuit Breaker-állapot visszaállítása a megfelelő műveleti ponthoz

</details>

<details>
<summary><b>🔄 23. "I need live A2A task lifecycle visibility and cancellation"</b></summary>

Nélkülözendő életciklus-láthatóság anélkül, hogy a feladat-helyzetek
megkönnyebbülése bonyolult lesz

**Hogy a OmniRoute megoldja:**

- Feladatok listázása/tulajdonságok/kezdeményezések azzal, hogy a későbbi
  oldalakkal
- Feladat-velői adatok/lépések és műszaki lemezek megjelenítése
- Feladat-azonosítót végrehajt és UI-AZM-val megjelenítőt a megerősítéssel
  társítva

</details>

<details>
<summary><b>🌊 24. "I need active stream metrics for A2A load"</b></summary>

Streaming-üzleti követelmények biztosítják a műveleti figyelmet az egyidejűségre
és élő csatlakozásokra.

**Hogy a OmniRoute megoldja:**

- Aktív stream-számlálók a másik-azonosító (A2A) státuszba integrálva
- Adott feladat-időbélyeg és az állapotonkénti számok
- A2A-asztal kártyák az éles üzemmenedzsment figyelemmel kísérésére

</details>

<details>
<summary><b>🪪 25. "I need standard agent discovery for clients"</b></summary>

Külső ügyfelek és koordinátoroknak szükségük van machina-olvaszható metaadatokra
a regisztrációhoz.

**Hogy a OmniRoute megoldja:**

- Ügynök kártya megjelenítése a `/.ismeretlen/ ` fájlban
- Képességek és készségek a kezelési felületen megjeleníthetők
- Az A2A státusz API-ja magában foglalja a automatizáláshoz szükséges
  felderítési metadatokat

</details>

<details>
<summary><b>🧭 26. "I need protocol discoverability in the product UX"</b></summary>

Ha a felhasználók nem tudják felismerni a protokoll felületeket, az elfogadás és
az együttműködés minősége csökken

**Hogy a OmniRoute megoldja:**

- Összehangolt **Üzenetszállítási pontok**oldal a Proxy, MCP, A2A és API
  Üzenetszállítási Állomások lapjai közötti átjárókkal
- A MCP és A2A ügynököknek offline/online állapotát szemléltető alapbeépsletek
  (Online/Offline)
- A megtekintésből áthívott speciális kezelési lapokra mutató hivatkozások

</details>

<details>
<summary><b>🧪 27. "I need end-to-end protocol validation with real clients"</b></summary>

A mock tesztek nem elégé elégségesek a protokoll kompatibilitásának
megerősítésére a megjelenés előtt

**Hogy a OmniRoute megoldja:**

- Teljesítmény-optimalizáló teszt szimuláció, amely beindítja az alkalmazást és
  a valós MCP SDK ügyfelet alkalmazza
- A2A ügyféltesztek felderítéshez, küldéshez, streamhez, megkapásához és
  lemondáshoz tartozó folyamatspecifikációk számára
- A MCP audit és A2A feladatok APi-einek összehasonlításával kamerák képeket
  készítünk

</details>

<details>
<summary><b>📡 28. "I need unified observability across all interfaces"</b></summary>

Az observability oszlopok által megosztása protokoll szerinti sötétségre és
hosszabb MTTR kiváltására

**Hogy a OmniRoute megoldja:**

- Az összefonódott dashboardok/naplók/analitikaiakat egy termékből nyújtó
  egységnyomtató
- Általános nyilvántartások a HP, MCP és A2A rétegekben
- Operációs APi-k az állapotról és az automatizálásról szóló infókért

</details>

<details>
<summary><b>💼 29. "I need one runtime for proxy + tools + agent orchestration"</b></summary>

Több, sokféle szolgáltatás futtatása növeli az operatív költségeket és a
kudarcmódosait.\
==WEBLATE_PART==

**Hogy a OmniRoute megoldja:**

- Egy Webblaze-kompatibilis proxy, MCP-szerver és A2A-szerver egyetlen
  szállalban
- Megosztott hitelesítés, fenntarthatóság, adatáruház és követési megfigyelés
- Az összes érintkezési felületen átívelő konszolidált politikamodellek

</details>

<details>
<summary><b>🚀 30. "I need to ship agentic workflows without glue-code sprawl"</b></summary>

A csapatok elvesztik a sebességet, miközben különböző ideiglenes szolgáltatások
és parancsfájlok beépítését csinálják.

**Hogy a OmniRoute megoldja:**

- Egyesített végponti stratégia ügyfél- és ügynök-számára
- Az épített protokollkezelő felhasználói felületeket és sűrített validációi
  utakat
- Termelésre készen álló alapok (biztonság, naplófájl, fék, visszaállítás)

</details>

### Példa Playbookek (integrált felhasználói esettanulmány)

**Játékszabályzat A: Maximális fizetett előfizetés + olcsó visszaállítási**

```txt
Kombináció: "maximális-claude"
  1. cc/claude-opus-4-6
  2. glm/glm-4.7
  3. if/kimi-k2-gondolkodik

Havi költség: $20 + kis visszaállítási költség
Eredmény: magasabb minőség, alacsony nulla szünetelés
```

**Játékszabályzat B: Zéró költségű kódolási tömb**

```txt
Kombináció: "ingyen-folyamatos"
  1. gc/gemini-3-FLASH
  2. if/kimi-k2-gondolkodik
  3. qw/qwen3- kódkódolt Plus

Havi költség: $0
Eredmény: stabil ingyenes forgalmazhatók kódolási folyamat
```

**Játékszabályzat C: 24/7 folyamatosan-fáll visszaállási lánc**

```txt
Kombináció: " mindig-aktiv"
  1. cc/claude-opus-4-6
  2. cx/gpt-5.2-codex
  3. glm/glm-4.7
  4. minimax/MiniMax-M2.1
  5. if/kimi-k2-gondolkodik

Eredmény: mély visszaállási mélység kritikus határidős terheléshez
```

**Játékszabályzat D: Ügynök-operációk MCP + A2A-X38X

```txt
1) Indítsa el a MCP-szervereket (`omniroute --mcp`) a felhasználói műveletekhez
2) Ejtsen le A2A-tasks A2A folyamatokon keresztül (`message/küldj ki`, illetve `message/áramkört`)
3) Figyelje meg /dashboard/endpoint-öt (MCP és A2A sáv)
4) Háborgasson szolgáltatásokat az inline bekapcsoló vezérlőkön
```

---

## 🆓 Kezdés ingyenes – Kártalanítás nélküli konfigurálás

> Pár perc alatt konfigurálja az AI kódolását a **$0/havi** összege. Kapcsolja
> be ezeket az ingyenes fiókokat és használja a beépített **Ingyenes tétel**
> kombinációt.

| Ütvonal | Akció                                              | Szállítók Megnyitva                                                    |
| ------- | -------------------------------------------------- | ---------------------------------------------------------------------- |
| 1       | Csatlakozás **Kiro** (AWS Builder ID OAuth)        | Claude Sonnet 4.5, Haiku 4.5 — **korlátozatlan**                       |
| 2       | Csatlakozás **iFlow** (Google OAuth)               | kimi-k2-thinking, qwen3-coder-plus, deepseek-r1... — **korlátozatlan** |
| 3       | Csatlakozás **Qwen** (Device Code)                 | qwen3-coder-plus, qwen3-coder-flash... — **korlátozatlan**             |
| 4       | Csatlakozás **Gemini CLI** (Google OAuth)          | gemini-3-flash, gemini-2.5-pro — **180K/ hónapban ingyen**             |
| 5       | `/dashboard/combos` → **Ingyenes kör (0$)** sablon | Roundszerűen automatikusan kapcsolja át a szállítókra                  |

**Helyezzen bármely IDE/CLI címkéjébe:** `http://localhost:20128/v1` · API
Kulcs: `Bármilyen szöveg` · Folytatás.

> **Nem kötelező, de kiegészítő fedéskísérletnek minősül (szintén ingyen):**
> Groq API-kulcs (30 RPM ingyen), NVIDIA NIM (40 RPM ingyen, 70+ modellek),
> Cerebras (1M tok/ nap), LongCat API-kulcs (50 millió token naponta!),
> Cloudflare Workers AI - (10 ezer Neuron/d, 50+ modellek).

## Gyors kezdés

### 1. Telepítse és futtassa

```bash
npm install -g omniroute
omniroute
```

> **pnpm felhasZNók:** Futtassa `pnpm jóváhagy-bét-teljesítményeket - g` az
> install után, hogy engedélyezze az natív build szkripteket `jobb sqlite3`-hez
> és `@ swc/`korehez:
> 
> ```bash
> pnpm install -g omniroute
> pnpm jóváhagy-bét-teljesítményeket - g   # Válassza ki az összes csomagot → jóváhagyás
> omniroute
> ```

A Dashbord nyitogatása `http://localhost:20128` és az API alap URL-ja
`http://localhost:20128/v1`.

| Parancs                      | Leírás                                                                          |
| ---------------------------- | ------------------------------------------------------------------------------- |
| `omniroute`                  | Kiszolgáló indítása   (`PORT=20128`,  kiszolgáló és Dashboard ugyanazon porton) |
| `omniroute --port 3000`      | Kanonikus / API port beállítása 3000-ra                                         |
| `omniroute --mcp`            | MCP kiszolgáló elindítása (stdio átviteli mód)                                  |
| `omniroute --no-open`        | Ne nyisson automatikusan a böngészőt                                            |
| `omniroute --segédkapcsolók` | Megjeleníti a segédkapcsolókat                                                  |

Opciózó split-port módo:

```bash
PORT=20128 DASHBOARD_PORT=20129 omniroute
# API:       http://localhost:20128/v1
# Dashboard: http://localhost:20129
```

### 2) Csatlakoztassa a szolgáltatókat és hozzon létre API kulcsot

1. Nyissa meg az irányítópultot → `Szolgáltatók` és csatlakozzon legalább egy
   szolgáltatóhoz (OAuth vagy API kulcs).
2. Nyissa meg az irányítópultot → `Végpontok` és hozzon létre API kulcsot.
3. (Lehetőség van arra, hogy) Nyissa meg az irányítópultot → `Kombinációk` és
   állítson be backupláncot.

### 3) Hajítsa a kódolási eszköz elé az OmniRoutet

```txt
Alap URL: http://localhost:20128/v1
API Kulcs:  a Végpont oldalról másolja be
Modell:    ha/kimi-k2-gondolkodás (vagy bármilyen szolgáltató/modell prefiksz)
```

Működik a Claude Code, Codex CLI, Gemini CLI, Cursor, Cline, OpenClaw, OpenCode
és OpenAI-bővítménnyel kompatibilis SDK-kal is.

### 4) Engedélyezze és validálja a protokollokat (v2.0)

**MCP (eszköz-hajtott műveletekhez): **

```bash
omniroute --mcp
```

Aztán csatlakoztassa az MCP klijentet a `stdio` hoz és tesztelje például az
alábbi műveletekhez társított eszközökkel:

- `omniroute_get_health`
- `omniroute_list_combos`

**A2A (ügynököt-ügynök munkafolyamatokhoz): **

```bash
curl http://localhost:20128/.well-known/agent.json
```

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"quickstart","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"Adjon meg egy rövid kvóta összefoglalót."}]}}'
```

### 5) Validálja mindenhol a végződő hosszútávú (ajánlott)

```bash
npm run test:protocols:e2e
```

Ezek a tesztek valós MCP és A2A ügyfél áramlásait vizsgálják egy futó
alkalmazással szemben.

### Alternatíva: futtassa a forráskódból.

```bash
cp .env.példa .env
npm telepítés
PORT=20128 DASHBOARD_PORT=20129 NEXT_PUBLIC_BASE_URL=http://localhost:20129 npm run dev
```

---

## Docker

OmniRoute elérhető nyilvános Docker-kép formájában [Docker
Hub]-on(https://hub.docker.com/r/diegosouzapw/omniroute).

**Gyors futás:**

```bash
docker run -d \
  --név omniroute \
  --restart unless-stopped \
  -p 20128:20128 \
  -v omniroute-data:/app/adatok \
  diegosouzapw/omniroute:latest
```

**Környezeti fájl használata:**

```bash
Első lépés a .env első másolása és szerkesztése:
cp .env.példa .env
docker run -d \
  --név omniroute \
  --restart unless-stopped \
  --env-fájl .env \
  -p 20128:20128 \
  -v omniroute-data:/app/adatok \
  diegosouzapw/omniroute:latest
```

**Docker Compose használata:**

```bash
Alap profil (CLI eszközök hiányában)
docker compose --profile alap profil felhozható -d

 CLI profil (Claude Code, Codex, OpenClaw egybeépítve)
docker compose --profile cli felhozható -d
```

| Kép                      | Címke       | Méret  | Leírás                  |
| ------------------------ | ----------- | ------ | ----------------------- |
| `diegosouzapw/omniroute` | `legutóbbi` | ~250MB | Legutóbbi stabil kiadás |
| `diegosouzapw/omniroute` | `1.0.3`     | ~250MB | Aktuális verzió         |

---

## Desktop alkalmazás — Offline & mindig aktív 🖥️

> 🆕 **ÚJ!** OmniRoute most szerkesztő-keszítő alkalmazás most elérhető a
> Windows, macOS, és Linux operációs rendszerekhez.

IndÍtsa el a OmniRoute -st merevlemez alkalommal őrhöz – nincs központi
terminál, böngésző, és internet helyi modellhez . A rendszer Electron alapul a
következőket:

- 🖥️ ** Natív ablak** – Kült ablak rendszer integráció
- 🔄 ** Automatikai indÍtás** – IndÍtsuk el az OmniRoute -t rendszer
  bejelentkezés során
- 🔔 ** Natív értesítések**[ /WEBLATE_PART == \
  Ertesítés a készlet fogyására, vagy biztonsági okok miatt
- ⚡ ** Egy-nyomásos telepítés**[ /WEBLATE_PART ==\
  NSIS (Windows), DMG (macOS), AppImage (Linux)
- 🌐 ** Offline üzemmód**[ /WEBLATE_PART ==\
  Teljesen működnek offline, a szervert tartalmazza

### Gyors kezdés

```bash
# fejlesztési mód
npm run electron:dev

# Konkrét platformra épít
npm run electron:build         # A jelenlegi platform
npm run electron:build:win     # Windows (.exe)
npm run electron:build:mac     # macOS (.dmg) — x64 &amp; arm64
npm run electron:build:linux   # Linux (.AppImage)
```

### Systém asztali

Minimálizálva szélsőben tartja az OmniRoute, gyors cselekvéseikkel:

- Nyissa meg az Irányítópultot
- Szervert csatlakozás
- Kilépés

📖 Teljes dokumentáció: [`electron/README.md`][/READ.md][ /WEBLATE_PART]]

---

## 💰 Árajánlat röviden

| Fokozat            | Szolgáltató                | Költség                           | Kizárás                    | Legjobb                                            |
| ------------------ | -------------------------- | --------------------------------- | -------------------------- | -------------------------------------------------- |
| **💳 ELTÁRASÁS[16X] | Claude Kód (Pro)           | 20$/hó                            | 5h + heti                  | Már feliratkoztam                                  |
|                    | Codex (Plus/Pro)           | 20-200$/hó                        | 5h + heti                  | OpenAI felhasználói                                |
|                    | Gemini CLI                 | **INGYEN**                        | 180K/hó + 1K/nap           | Mindenki!                                          |
|                    | GitHub másodpilóta         | 10-19$/hó                         | Havi                       | GitHub felhasználói                                |
| **🔑 API KULCS**    | NVIDIA NIM                 | **INGYEN** (fejlesztői örökké)    | A 40-asos RPm              | 70 feletlencsi modell van nyitva                   |
|                    | Cerebras                   | **INGYENES** (1M token/nap)       | 60K TPM / 30 RTP           | Az egész világon a leghasznosabb                   |
|                    | Groq                       | **INGYENES** (30 RTP)             | 14.4K RPD                  | Ultra-gyors Llama/Gemma feldolgozás                |
|                    | DeepSeek V3.2              | 0,27/1,10 dollár 1M-ért           | Egyik sem                  | Ahhoz a legjobb árhoz/eredményhez                  |
|                    | xAI Grok-4 Gyorssal        | **20 cent/$0,50 dollár 1M-ért** 🆕 | Egyik sem                  | A leggyorsabb + eszközfelhívás, ultralow ár        |
|                    | xAI Grok-4 (átlagos)       | 0,20/1,50 dollár 1M-ért 🆕         | Egyik sem                  | xAI úttörője                                       |
|                    | Mistral                    | Fköziút ingyen + fizetés          | Ára korlátozott            | Európai mesteralgoritmus                           |
|                    | OpenRouter                 | Használati díj                    | Egyik sem                  | +100 modell kombinálása                            |
| **💰 TIPICUS**      | GLM-5 (Z.AI által) 🆕       | 0,5$/1M                           | Napként 10AM               | újabb flagszippelős 128K                           |
|                    | GLM-4.7                    | 0,6$/1M                           | Napként 10AM               | Budget visszajelzés                                |
|                    | MiniMax M2.5 🆕             | 0,3$/1M bevitel                   | 5 órás rollo               | Eseményfeldolgozás + agenciós feladatok            |
|                    | MiniMax M2.1               | 2¢/10M                            | 5 órás rollo               | Legolag legesleges opciója                         |
|                    | Kimi K2.5 (Moonshot API) 🆕 | Használati díj                    | Egyik sem                  | Direkt társított csatlakozás a Holdra Moonshot API |
|                    | Kimi K2                    | 9 dollár/kh bruttó díj            | 10M adatok/másodpercenként | Megbízható költség                                 |
| **🆓 INGYENES**     | iFlow                      | **$0**                            | Korlátlan                  | 5 modell + korlátlan hozzáférés                    |
|                    | Qwen                       | **$0**                            | Korlátlan                  | 4 modell + korlátlan hozzáférés                    |
|                    | Kiro                       | **$0**                            | Korlátlan                  | Claude Sonnet/Haiku (AWS Builder)                  |
|                    | LongCat Flash-Lite 🆕       | **$0** (50M tok/délcz 🔥)          | 1 RPS                      | Nagyságú ingyenes kvóta Földön                     |
|                    | Pollinations AI 🆕          | **$0** (nincs kulcs szükséges)    | 1 kérés/15s                | GPT-5, Claude, DeepSeek, Llama 4                   |
|                    | Cloudflare Workers AI 🆕    | **$0** (10K Neuron naponta)       | ~150 válasz naponta        | 50+ modell, globális él                            |
|                    | Scaleway AI 🆕              | **$0** (1M token összesen)        | Ára korlátozott            | EU/GDPR, Qwen3 235B, Llama 70B                     |

> 🆕 **Új modell hozzáadva (Mar 2026):** Grok-4 Fast család $0,20/$0,50/M
> (tesztelve 1143ms – 30%-kal gyorsabb, mint a Gemini 2,5 Flash), GLM-5 Z.AI
> keresztül 128K kimenet, MiniMax M2,5 észlelés, DeepSeek V3,2 frissített
> árazás, Kimi K2,5 Moonshot közvetlen API.

**💡 $0 Combo Stacks — Teljes Ingyenes Felállás:**

```
# 🆓 Bármilyen Ingyenes Stack 2026 — 11 Providerek, $0 Mindörökké
Kiro (kr/)             → Claude Sonnet/Haiku Végtelen
iFlow (if/)            → kimi-k2-gondolkodás, qwen3-kód-plusz, deepseek-r1 Végtelen
LongCat Lite (lc/)     → LongCat-Flash-Lite – 50M token/nap 🔥
Pollinations (pol/)    → GPT-5, Claude, DeepSeek, Llama 4 – nincs kulcs szükséges
Qwen (qw/)             → qwen3-kód-plusz, qwen3-kód-flash, qwen3-kód-következő Végtelen
Gemini (gemini/)       → Gemini 2,5 Flash — 1 500 kérés/nap ingyenes API kulcs
Cloudflare AI (cf/)    → Llama 70B, Gemma 3, Mistral — 10K Neuron naponta
Scaleway (scw/)        → Qwen3 235B, Llama 70B — 1M ingyenes token (EU)
Groq (groq/)           → Llama/Gemma extrém gyors — 14,4K kérés/nap
NVIDIA NIM (nvidia/)   → 70+ nyitott modell — 40 RPM örökre
Cerebras (cerebras/)   → Llama/Qwen leggyorsabb világon — 1M tok/nap
```

**Ingyenes. Soha nem áll meg.** Ez a kombókonkon állíthatja be Omnipathot és
minden visszaállítás automatikusan megy – nincsen kéziszekció sehol.

---

---

## 🆓 Ingyenes_modellek — Mit Fog Megkaphatni

> Az alábbi összes modell **100% ingyenes, $0-val kezdve nincs bankkártya
> szükségeltet**. OmniPath által automatikusan irányítja őket, ha egyes kvóta
> lemerül – kombinálja csak [X32X] őket a megtörhetetlen $0 Combo-ért

### 🔵 CLAUDE MODELLEK (Kiro - AWS Builder ID-én keresztül)

| Modell              | Előtag | Határ              | Túlkorlátozás             |
| ------------------- | ------ | ------------------ | ------------------------- |
| `claude-sonnet-4.5` | `kr/`  | **Korlatoonlanul** | Nincs jelentett napi cap  |
| `claude-haiku-4.5`  | `kr/`  | **Korlatoonlanul** | Nincs jelentett napi cap  |
| `claude-opus-4.6`   | `kr/`  | **Korlatoonlanul** | Legfrissebb Ágenszis Opus |

### 🟢 JÁRAT SZERKEZETEKBELI MODELLEK (Ingyenes OAuth — Nem Szükséges Kártyaszám)

| Modell             | Előtag | Határ              | Túlkorlátozás       |
| ------------------ | ------ | ------------------ | ------------------- |
| `kimi-k2-thinking` | `if/`  | **Korlatoonlanul** | Nincs jelentett cap |
| `qwen3-coder-plus` | `if/`  | **Korlatoonlanul** | Nincs jelentett cap |
| `mélykeresés-r1`   | `if/`  | **Korlatoonlanul** | Nincs jelentett cap |
| `minimax-m2.1`     | `if/`  | **Korlatoonlanul** | Nincs jelentett cap |
| `kimi-k2`          | `if/`  | **Korlatoonlanul** | Nincs jelentett cap |

### ✨ KÉSZ MODELLEK (Készülék Kódosztó)

| Modell               | Előtag | Határ              | Túlkorlátozás       |
| -------------------- | ------ | ------------------ | ------------------- |
| `qwen3-coder-plus`   | `qw/`  | **Korlatoonlanul** | Nincs jelentett cap |
| `qwen3-kódoló-flick` | `qw/`  | **Korlatoonlanul** | Nincs jelentett cap |
| `qwen3-kódoló-kilép` | `qw/`  | **Korlatoonlanul** | Nincs jelentett cap |
| `látóhatár-minta`    | `qw/`  | **Korlatoonlanul** | Multimódus (kép)    |

### 🟣 GEMINI CLI (Google OAuth)

| Modell                             | Előtag | Határ                                     | Túlkorlátozás   |
| ---------------------------------- | ------ | ----------------------------------------- | --------------- |
| `Géminál-3-előnézeti megjelenítés` | `gc/`  | **180K/tömbhónaponként** + 1K/napon       | Havi újrakezdés |
| `Géminál-2.5 Pro`                  | `gc/`  | 180K/tömbhónaponként (megosztott tárhely) | Magas minőségű  |

### ⚫ NVIDIA NIM (Ingyenes API Kulcs - build.nvidia.com)

| Fokozat              | Napi limit             | Túlkorlátozás | Megjegyzések                                                       |
| -------------------- | ---------------------- | ------------- | ------------------------------------------------------------------ |
| Ingyenes (fejlesztő) | Nincs token korlátozás | **~40 RPM**   | 70+ modell; 2025 közepéig átáll a tisztább korlátozási határidőkre |

Saját többnyire ingyenes modellek: `moonshotai/kimi-k2.5` (Kimi K2.5),
`z-ai/glm4.7` (GLM 4.7), `deepseek-ai/deepseek-v3.2` (DeepSeek V3.2),
`nvidia/llama-3.3-70b-instruct`, `deepseek/deepseek-r1`

### ⚪ CEREBRAS (Ingyenes API Kulcs - inference.cerebras.ai)

| Fokozat  | Napi limit              | Túlkorlátozás    | Megjegyzések                                                        |
| -------- | ----------------------- | ---------------- | ------------------------------------------------------------------- |
| Ingyenes | **1M darab tokene/nap** | 60K TPM / 30 RTP | A világ leghosszabb LLM-kísérleti végrehajtása naponta újrakezdődik |

Az elérhető ingyen: `llama-3.3-70b`, `llama-3.1-8b`,
`deepseek-r1-distill-llama-70b`

### 🔴 GROQ (Ingyenes API kulcs — console.groq.com)

| Fokozat  | Napi limit    | Túlkorlátozás       | Megjegyzések                                                         |
| -------- | ------------- | ------------------- | -------------------------------------------------------------------- |
| Ingyenes | **14,4K RPD** | Egy modellre 30 RPM | Nincs hitelkártya; a limit elérésével 429 értesítés, nem töltjük fel |

Az elérhető ingyen: `llama-3.3-70b-versatile`, `gemma2-9b-it`, `mixtral-8x7b`,
`whisper-large-v3`

### 🔴 LONGCAT AI (Ingyenes API kulcs — longcat.chat) 🆕

| Modell                                | Előtag | Napi Szabályzat | Megjegyzések                      |
| ------------------------------------- | ------ | --------------- | --------------------------------- |
| `HosszúMacska-Flash-Lite`             | `lc/`  | **50M tokent**  | Nagyobb ingyenes quotát egy ideig |
| `HosszúMacska-Flash-Chat`             | `lc/`  | 500K token      | Multiturbulens beszélgetés        |
| `HosszúMacska-Flash-Gondolkodás`      | `lc/`  | 500K token      | Érvelés / CoT                     |
| `HosszúMacska-Flash-Gondolkodás-2601` | `lc/`  | 500K token      | Január 2026 verzió                |
| `HosszúMacska-Flash-Omni-2603`        | `lc/`  | 500K token      | Multimódszertani                  |

> 100% ingyenes addig, amíg a publikus bétafázisban vagyunk. Regisztrálni
> [hosszumacska.chat](https://longcat.chat) címen lehet e-mail vagy telefonon,
> regisztráció után ezzel a nap 00:00 UTC-vel automatikusan frissülnek az
> adatok.

### 🟢 POLLINATIONS AI (Nincs API-kulcs szükséges) 🆕

| Modell     | Előtag | Túlkorlátozás | Közszolgáltató Háttér |
| ---------- | ------ | ------------- | --------------------- |
| `openai`   | `pol/` | 1 kérés/15s   | GPT-5                 |
| `claude`   | `pol/` | 1 kérés/15s   | Anthropic Claude      |
| `gemini`   | `pol/` | 1 kérés/15s   | Google Gemini         |
| `deepseek` | `pol/` | 1 kérés/15s   | DeepSeek V3           |
| `llama`    | `pol/` | 1 kérés/15s   | Meta Llama 4 Scout    |
| `mistral`  | `pol/` | 1 kérés/15s   | Mistral AI            |

> ✨ **Semmi kele azután: ** Regisztráció nélkül, nincs API-kulcs, mégpedig üres
> kulcsmezővel adjuk hozzá a Pollinations szolgáltatót, és rögtön működik.

### 🟠 CLOUDFLARE WORKERS AI (Ingyenes API-kulcs - cloudflare.com) 🆕

| Fokozat  | Napi Neuronnal | Egyenértékű Felhasználás                             | Megjegyzések                  |
| -------- | -------------- | ---------------------------------------------------- | ----------------------------- |
| Ingyenes | 10 000,**      | ~ 150 LLM felhasználó / 500s audio / 15K embdeddedes | Globális szélső, 50+ modellek |

Légy népszerű ingyenes modellek: `@cf/meta/llama-3.3-70b-instruct`,
`@cf/google/gemma-3-12b-it`, `@cf/openai/whisper-large-v3-turbo` (ingyenes
hangos!), `@cf/qwen/qwen2.5-coder-15b-instruct`

> API kulcs + számlaszám szükséges
> [dash.cloudflare.com](https://dash.cloudflare.com). A számlaszámot
> adatfolyamkezelő beállítások mentése.

### 🟣 MEGVALÓSÍTÁSI TÉRINTÉSZETEK AI (1M Ingyen Kód - scaleway.com) 🆕

| Fokozat  | Ingyenes Kredit | Hely          | Megjegyzések                                         |
| -------- | --------------- | ------------- | ---------------------------------------------------- |
| Ingyenes | 1M kód**        | 🇫🇷 Párizs, EU | Nincs szükség kártyaigénylésre a korlátoásokon belül |

Elérhető ingyen: `qwen3-235b-a22b-instruct-2507` (Qwen3 235B!),
`llama-3.1-70b-instruct`, `mistral-small-3.2-24b-instruct-2506`,
`deepseek-v3-0324`

> EU/GDPR kompatibilis. API kulcs megszerzése a
> [console.scaleway.com](https://console.scaleway.com).

> ** 🔍 A Végső Ingyenes Stak: **
> 
> ```
> Kiro (kr/)             → Claude Sonnet/Haiku TELITLÉTETETL
> iFlow (if/)            → kimi-k2-thinking, qwen3-coder-plus, deepseek-r1 TELITÉRT
> LongCat Lite (lc/)     → LongCat-Flash-Lite – 50M token/nap/d nap
> Pollinations (pol/)    → GPT-5, Claude, DeepSeek, Llama 4 – nincs regisztráció szükséges
> Qwen (qw/)             → qwen3-coder modellek TELITÉRT
> Gemini (gemini/)       → Gemini 2.5 Flash – 1 500 kérés/d free
> Cloudflare AI (cf/)    → 50+ modell – 10K Neuron/d nap
> Scaleway (scw/)        → Qwen3 235B, Llama 70B – 1M ingyen token (EU)
> Groq (groq/)           → Llama/Gemma – 14.4K kérés/d nagyon gyors
> NVIDIA NIM (nvidia/)   → 70+ nyitott modell – 40 RPM örökre
> Cerebras (cerebras/)   → Llama/Qwen világon gyorsabb – 1M tok/d nap
> ```

## 🎙️ Ingyenes Transzkripció Combo

> Bármilyen audio/video transzkribálható az alábbi áron: **$0** – Továbbítja az
> ingyenes Deepgram 200-, AssemblyAI 50- dollárt, Groq Whisper pedig korlátlan
> vészhelyzetben tartja.

| Szolgáltató      | Ingyenes Kredit                | Legjobb Model                                 | Túlkorlátozás                     |
| ---------------- | ------------------------------ | --------------------------------------------- | --------------------------------- |
| 🟢 **Deepgram**   | **$200 ingyen** (regisztráció) | `nova-3` – a legmagasabb pontosság, 30+ nyelv | Nincs korlát az ingyenes krediten |
| 🔵 **AssemblyAI** | **$50 ingyen** (regisztráció)  | `universal-3-pro` – fejezetek, érzelmek, PII  | Nincs korlát az ingyenes krediten |
| 🔴 **Groq**       | **Ingyen örökre**              | `whisper-large-v3` – OpenAI Whisper           | 30 RPM (korlátozott sebesség)     |

**Sajátan javasolt kombó a `/dashboard/combos` alatt:**

```
Név: ingyenes-transzkripció
Stratégia: különleges
Nodek:
  [1] deepgram/nova-3          → használja az első sorra a $200 ingyen
  [2] assemblyai/universal-3-pro → fallback, amikor a Deepgram kreditje leszámol
  [3] groq/whisper-large-v3    → ingyen örökre, vészhelyzet esetén használjuk.
```

Then a médiafájlok ` → ** Transzkripció** fülében: feltöltsen
a `/dashboard/media` → **Transcription** lapot audio vagy videó fájlt → válassza
ki kombinálási végpontját → kapsolja be a transzkripciót támogatott formátumban.

## 💡 Kulcsfontosságú tulajdonságok

OmniRoute 2.0 építéséül operatív platformot hoztak létre, nem csak csatlakozó
proxyt.

### 🆕 Új — ClawRouter-Inspirált Fejlesztések (2026)

| Jellemző                               | Mire van jó                                                                                                                                                         |
| -------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ⚡ **Grok-4 Fast Family**               | xAI modellek 0,20/0,50/A - 1143 ms (30%-kal gyorsabb, mint a Gemini 2.5 Flash)                                                                                      |
| 🧠 **GLM-5 a Z.AI **n keresztül         | 128 K az eredménykontextus, 0,5/1A - az újabb GLM családració legújabb tagja                                                                                        |
| 🔮 **MiniMax M2.5**                     | Logika + ügynök feladatok 0,30/1A - jelentős javulás a M2.1 -től                                                                                                    |
| 🎯 **modellhez kapcsolódó Zászló **     | A felhasználó által adott `modell kapcsolódó: igaz / hamis` értéke a regisztrációs lapban  -  AutoCombo eltekint az egyes modellektől, amely nem képes eszközökhöz. |
| 🌍 **Multilinguális Szándék észlelés**  | Az AutoCombo pontozása: PT/ZH/ES/AR kulcsszavak a nem angol tartalmért                                                                                              |
| 📊 **Benchmark alapú Visszafordulások** | A valós p95 késés azonnal elküldött kérésekből kap követési pontokat - AutoCombo megtanul az igazi adatokból                                                        |
| 🔁 **Kérelem Duplikálás**               | A Tartalom-hash alapú dedukáló ablak -multiközpontú, duplikált feladatok elkerülésére.                                                                              |
| 🔌 **Csatlakozható RouterStrategy**     | Építhető `RouterStrategy` interfész — adjon hozzá kiegészítő útvonal-vezérlési logikát pluginokként                                                                 |

### 🚀 korábbi v2.0.9+ — Játterű, CLI Kezelője & ACP

| Jellemző                                         | Mire van jó                                                                                                                                                                                                                                                                                     |
| ------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🎮 **ModelljátékTERÜLETE**                        | Tesztmodellterület, ahol bármilyen modellt közvetlenül tesztelhet — provider/model/endpoint kiválasztó, Monaco Szerkesztő, streaming, lemondás, időzítés                                                                                                                                        |
| 🔏 **CLI Fingerprint Összevetés**                 | Főszolgáltatóra szabályozott fejléc/testkezelés az eredeti CLI aláíráshoz való megfeleléshez — aktiválja a főszolgáltatót a Beállítások > Biztonság menüben. **A proxy IP-je megtartott**                                                                                                       |
| 🤝 **ACP támogatás (Küldő Kiszolgáló Protokoll)** | CLI ügynök-felderítés (Codex, Klaud, Goose, Genümi CLI, Nyitott Szemek + 9 további), folyamatindító, `/api/acp/ügynökök` végpont                                                                                                                                                                |
| 🤖 **ACP ÜgynökFolyamatos felület**               | Hibakeresés > Ügynök lap — szabályozható 14 ügynök hálózata a telepítési állapottal, verzióval, bármely CLI eszközzel csere végző eljárással.   **Nyitott kód** felhasználók egy „Letöltés opencode.json” gombokat kapnak, amire az elérhető mindegyik modell elérhető konfigurációt generálja. |
| 🔧 **Külső Modell `apiFormat` Útvonalak**         | Custom modellök `apiFormat: „válaszok}` most már a választó API fordítóhoz vonatkozik                                                                                                                                                                                                           |
| 🏢 **Codex MunkaterületKülönválasztás**           | Külön választott Codex munkaterületek egy hitelesített e-mail-figyelő – OAutó korrekten választja el a kapcsolatokat a munkaterülettulajdonosi azonosítóban                                                                                                                                     |
| 🔄 **Elektron Átvitt frissítések**                | Asztali alkalmazás - ellenőrzi az üzeneteket + automatikus bekövetkeztét a újrakezdésné                                                                                                                                                                                                         |

### 🤖 Ügynök és Protokoll Műveletek (v2.0)

| Jellemző                                       | Mire van jó                                                                                               |
| ---------------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| 🔧 **MCP Szerver (16 eszköz)**                  | IDE/ügynök eszközök által: 3 transzport: stdio, SSE (`/api/mcp/sse`), Streamable HTTP (`/api/mcp/stream`) |
| 🤝 **A2A Szerver (JSON-RPC + SSE)**             | Ügynök-ügynök feladat végrehajtása összehangolt és streaming alapú folyamatokkal                          |
| 🧭 **Konszolidált Végpontok Lapja**             | Laphoz tartozó végpont-kezelő lap (Proxy, MCP, A2A és API Végpontok)                                      |
| 🎚️ **Szolgáltatás Aktiválás/Letiltás Keverők** | A MCP-k és A2A-k ON/OFF kapcsolói automatikus beállítással (default: LETILTVA)                            |
| 🛰️ **MCP Futtatási Szívritmus**                | Valós folyamat státusz (pid, uptime, szívritmus kor, transzport, scope mód)                               |
| 📋 **MCP Nyilvántartás**                        | Siker/failures és kulcsszavattributionnal rendelkező filterezhető nyilvántartások                         |
| 🔐 **MCP Környezet Biztosítása**                | 9 specifikus jogosultság engedélyezése speciális eszköz hozzáférés szabályozása érdekében                 |
| 📡 **A2A Feladat Életciklus Menedzsment**       | Feladat lista/filter alapú menedzsment, esemény és műsorlap megtekintése, futó feladatok leállítása       |
| 📋 **Ügynök Kártya Felfedezése**                | `/.well-known/agent.json` ügyfél automatikus felfedezéshez                                                |
| 🧪 **Protokoll végigmenni teszt-berendezés**    | Valós MCP SDK + A2A ügyféláramlatok a `teszt:protokollok:végigmenni` folyamatokban                        |
| ⚙️ **Működési ellenőrzési eszközök**           | Átállási kombinációk, rezisztencia profilok alkalmazása, ágensek újravesztese egyetlen vezérlőfelületből  |

### 🧠 Útvonal- és intelligencia

| Jellemző                                             | Mire van jó                                                                                        |
| ---------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| 🎯 **Smarts az intelligens visszalépéshez**           | Önálló útvonal: Regisztráció → API-Kulcs → Összgeköltség → Ingyenes                                |
| 📊 **Valós idejű kvóta következetes nyomon követése** | Egyedi tokenlekövetés + visszaállítási számláló a szolgáltatókhoz                                  |
| 🔄 **Szerkesztési átfordítás**                        | OpenAI ↔ Claude ↔ Gemini ↔ Ötlet-szeminárisztikus áthubadáskonverziók                              |
| 👥 **Többfelhasználói támogatás**                     | Különböző felhasználók száma szolgáltatóknál intelligens választással                              |
| 🔄 **Automatikus token-frissítés**                    | Következő OAuth-token önamatos frissítése retrállal                                                |
| 🎨 **Egyszínű kombinációk**                           | 6 egyensúlyozási stratégiák + visszalépési láncozás irányítása                                     |
| 🌐 **Világosítót tartalmazó útvonal**                 | `szállító/*` dinamikus útválasztás                                                                 |
| 🧠 **Gondolkodás határoló Szabályzatok**              | Összekapcsolódás, automatikus, egyedi és összehasonlító indítás-limits                             |
| 🔀 **Modell-Álnevek**                                 | Bővítve lekvár + egyedi modell-álnevek kezelés és művelet biztonságosság                           |
| ⚡ **Háttérsértés**                                   | Rövidhírkiosztás alacsony-koroszlop háttérműveletek olcsóbb modellekhez                            |
| 🧪 **Feladat-érzékeny intelligens útválasztás**       | Ürülési-modell választás automata tartalomtípus szerint (kódolás/pontozás/analízis/ összefoglalás) |
| 💬 **Rendszer-összehívási injekció**                  | Erősen alkalmazott rendszer-műveletek összehangolása                                               |
| 📄 **VálaszAPI[X5X]-kompatibilitás**                  | Teljes `/v1/válasz/X19X] támogatás a Codex és kiterjesztett agencialis folyamatok számára          |

### 🎵 Összetett modális API-k

| Jellemző                                   | Mire van jó                                                                                                                                                                                        |
| ------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🖼️ **Képképzés**                           | `/v1/images/kezdeménye` a felhő- és lokális háttérrel                                                                                                                                              |
| 📐 **Becsapások**                           | `/v1/becsapások` a keresés és az RAG áramlatok céljára                                                                                                                                             |
| 🎤 **Hangsely A hangszórási Transzkripció** | `/v1/hangszer/audio/transzkripciók` — 7 szolgáltató (Deepgram Nova 3, AssemblyAI, Groq Whisper, HuggingFace, ElevenLabs, OpenAI, Azure), automatikus nyelvészeti detektálás, MP4/MP3/WAV támogatás |
| 🔊 **Hangsuly Text-to-Speech**              | `/v1/audio/speech` — 10 szolgáltató (ElevenLabs, OpenAI, Deepgram, Cartesia, PlayHT, HuggingFace, Nvidia NIM, Inworld, Coqui, Tortoise) a hibaüzenetekkel együtt                                   |
| 🎬 **Film Generálás**                       | `/v1/videos/generálást` (ComfyUI + SD WebUI folyamatok)                                                                                                                                            |
| 🎵 **Zene Generálás**                       | `/v1/music/generálást` (ComfyUI folyamatok)                                                                                                                                                        |
| 🛡️ **Moderálások**                         | `/v1/moderálások` biztonsági ellenőrzések                                                                                                                                                          |
| 🔀 **Újrasorolás**                          | `/v1/rerank` relevanciás pontozás                                                                                                                                                                  |
| 🔍 ** Webkeresés**  🆕                       | `/v1/search` — 5 szolgáltató (Serper, Brave, Perplexity, Exa, Tavily), 6 500+/hó, automatikus lecserélés, cache                                                                                    |

### 🛡️ Állandóság, Biztonság & Kormányzás

| Jellemző                           | Mire van jó                                                                            |
| ---------------------------------- | -------------------------------------------------------------------------------------- |
| 🔌 ** Áramló Kapcsolók**            | Model-specifikus újrakapcsolás/gyökerezzék műveletekkel és küszöbkontrollokkal         |
| 🎯 **Modellvégpontú Modellek**      | Custom models declare supported endpoints + API format                                 |
| 🛡️ **Anti-Thundering Herd**        | Mutex + semaphore protections on retry/rate events                                     |
| 🧠 **Semantic + Signature Cache**   | Cost/latency reduction with two cache layers                                           |
| ⚡ **Request Idempotency**          | Duplicate protection window                                                            |
| 🔒 **TLS Fingerprint Spoofing**     | Browser-like TLS fingerprint — **reduces bot detection and account flagging**          |
| 🔏 **CLI Fingerprint Összevetés**   | Matches native CLI request signatures — **reduces ban risk while preserving proxy IP** |
| 🌐 **IP Filtering**                 | Allowlist/blocklist control for exposed deployments                                    |
| 📊 **Editable Rate Limits**         | Configurable global/provider-level limits with persistence                             |
| 🔑 **API Key Management + Scoping** | Secure key issuance/rotation and model/provider controls                               |
| 🛡️ **Protected `/models`**         | Optional auth gating and provider hiding for model catalog                             |

### 📊 Observability & Analytics

| Jellemző                       | Mire van jó                                                              |
| ------------------------------ | ------------------------------------------------------------------------ |
| 📝 **Kérés + proxy naplózási**  | Teljes kérés/válasz és proxy naplózás                                    |
| 📋 **Unifikált naplók felület** | Egy oldalon a kérés, proxy, audit és konzolnézetek                       |
| 🔍 **Kérési adattovábbítás**    | p50/p95/p99 késés és kérés nyomkövetés                                   |
| 🏥 **Egészségügyi felület**     | Aktualitás, csomópont állapotok, leblokkolások, gyorsítótár statisztikák |
| 💰 **Kiadási nyomon követés**   | költségirányítás és árképzési láthatóság modellek szinten                |
| 📈 **Analitikai vizualizációk** | Modell/felhasználó használati megértése és trendnézetek                  |
| 🧪 **Vizsgálati keretrendszer** | Aranyhalmaz tesztelés a konfigurálható megegyezési stratégiával          |

### ☁️ Deploy & Platform

| Jellemző                                      | Mire van jó                                                                                 |
| --------------------------------------------- | ------------------------------------------------------------------------------------------- |
| 🌐 **Bármelyütköztetettség**                   | Helyi gép, VPS, Docker, felhőkörnyezetek                                                    |
| 💾 ** Felhő mentése**                          | Konfiguráció szinkronizálása felhősbekerőssel                                               |
| 🔄 ** Vissza/Regenerálás**                     | Export/import és ügyfélszolgálati biztonság                                                 |
| 🧙 ** Bevezető varázsló**                      | Bezárásnál idegenvezetett beállítás                                                         |
| 🔧 ** CLI-es szerszámos panel**                | Egy kattintással hozzáfér másik kódoló eszközökhöz                                          |
| 🎮 **ModelljátékTERÜLETE**                     | Tesztelje az adatforrásokat bármelyik szolgáltatóval                                        |
| 🔏 ** CLI-mezőnyomtatás kapcsoló**             | Szállítói fegyvertől függő nyomonkövetés konfiguráció az Adatvédelem > Biztonság szekcióban |
| 🌐 ** Nemzetközi karaktertényezők (30 nyelv)** | A teljes panel + dokumentáció támogatása több nyelven és kezdő-irányultság                  |
| 🧹 ** Modell törlés gomb**                     | Modell listájának rögzítése gomb egy kattintással az adatforráson                           |
| 📋 ** Jegyzet sablonok**                       | Standardizált GitHub sablonok a hibákhoz és a hozzáadási lehetőséghez                       |
| 📂 ** Személyre szabott adattér**              | `ADIROZÁS_Helye` megadása töltési hely helyett                                              |

### A mélységi felmérés

#### Intelligens visszaállás a gyakorlati költési ellenőrzéssel

```txt
Kombináció: "Az én kódolócsomópontom"
  1. cc/claude-opus-4-6
  2. nvidia/llama-3.3-70b
  3. glm/glm-4.7
  4. if/kimi-k2-gondolkodás
```

Amikor a kvóta, az ár vagy a mentés meghiúsul, az OmniRoute automatikusan a
következő jelöltre csatlakozik, anélkül, hogy az embernek manuálisan kellene
váltania.

#### Vizsgálati folyamat, amely látható és működtethető

- Az MCP + A2A felfedezhető a felhasználói felületben és a dokumentumokban (nem
  rejtett)
- A protokoll státusz API-k a élő működési adatokat teszik elérhetővé (
  `/api/mcp/*`, `/api/a2a/*` )
- A táblázatokban nap-2 napos műveletek elérhetők (kombináció kapcsolók,
  megszakító visszaállítás, feladatok törlése)

#### A tolmács és a validációs folyamat

A tolmács területéhez tartozó szolgáltatások:

- **Játszópályák**: kérés alapú átalakítási ellenőrzések
- **Chat ellenőrző**: teljes kérés/válaszváltó kör
- **Próbaterület**: több eset egyben futtatása
- **Élő Monitor**: valós idejű forgalomnézet

Emellett létezik protokoll validáció valódi klienseken keresztül a `npm futtat:
protokollok: környezeti teszt` használatával.

> 📖 **MCP Szerver README(open-sse/mcp-server/README.md)** — Szerszámleírás,
> szerkesztői konfigurációk és klienspéldák
> 
> 📖 **A2A Szerver README(src/lib/a2a/README.md)** — Készségek, JSON-RPC
> metódusok, streaming, és feladatok életciklusa

## Vizsgálati szetrek (Vizsgálatok)

Az OmniRoute tartalmaz egy beépített értékelési modult a LLM válasz minőségének
elemzéséhez egy arany alapvonalhoz. Elérhető a **Analitika → Vizsgálatok**
menüpontban a táblázatban.

### Built-in Golden Set

Az beépített "OmniRoute Golden Set" tartalmaz teszt eseteket:

- Üdvözlés, matematika, földrajz, kódgenerálás
- JSON formátum kompatibilitás, fordítás, markdown generálás
- Baleset elutasítás (káros tartalom), számlálás, boole logika

### Értékelési stratégiák

| Stratégia   | Leírás                                                                   | Példa       |
| ----------- | ------------------------------------------------------------------------ | ----------- |
| `pontos`    | A kimenetnek pontosan meg kell egyeznie                                  | `"4"`       |
| `tartalmaz` | A kimenet tartalmazza az alábbi szöveget (esetlegesség figyelembevétele) | `"Paris"`   |
| `regex`     | A kimenetnek meg kell egyeznie a regex mintával                          | `"1.*2.*3"` |
| `gyakorlat` | Kulcsó JavaScript funkció igaz/atértelmezi                               | `(kiirási)  |

---

## 📖 Ügyfélkezelési útmutató

### Protokoll beállítás (MCP + A2A)

<details>
<summary><b>🧩 MCP Setup (Model Context Protocol)</b></summary>

Indítsa el az MCP kommunikációt a parancssor módban:

```bash
omniroute --mcp
```

Javasolt ellenőrzési folyamat:

1. Kapcsolódjon az MCP klienshez parancssorban.
2. Futtassa a `omniroute_get_health`-t.
3. Futtassa a `omniroute_list_combos`-t.
4. Nyissa meg a `/dashboard/mcp`-ot a heartbeat, a tevékenység és az audit
   bejárati oldalra.

Ügyféloldali API-aktusok az automatizáláshoz:

- `GET /api/mcp/status`
- `GET /api/mcp/tools`
- `GET /api/mcp/audit`
- `GET /api/mcp/audit/stats`

</details>

<details>
<summary><b>🤝 A2A Setup (Agent2Agent)</b></summary>

Felfedezze a ügynököt:

```bash
curl http://localhost:20128/.well-known/agent.json
```

Küldje el a feladatot:

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"setup-a2a","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"Összefoglalja a rövid távú tárhely státust."}]}}'
```

Életciklus kezelése:

- GET /api/a2a/status`
- GET /api/a2a/tasks`
- GET /api/a2a/tasks/:id`
- POST /api/a2a/tasks/:id/cancel`

Kezelési UI:

- `/a2a/folyamat` kezelésének és smoke akciómegfigyelésének a ` felületén

</details>

<details>
<summary><b>🧪 End-to-end protocol validation</b></summary>

Validerje mindkét protokollt valódi ügyfelekkel:

```bash
npm run test:protocols:e2e
```

Ez ellenőrzi:

- MCP SDK ügyfél csatlakoztatása/kivétele/hívása
- A2A felismerése/küldése/stream-get/jelzése
- Ellenőrizze az adatokat a MCP audit és az A2A feladatkezelő API-kban

</details>

<details>
<summary><b>💳 Subscription Providers</b></summary>

### Klauz Kód (Pro/Max)

```bash
Felület → Szolgáltatók → Kapcsolódás Klauz Kódhoz
→ OAuth bejelentkezés → Automatikus token frissítés
→ 5 órás + heti kvótameghatározás

Modellek:
  cc/claude-opus-4-6
  cc/claude-sonnet-4-5-20250929
  cc/claude-haiku-4-5-20251001
```

**Pro tip**: használja az Opust bonyolult feladatokhoz, a Sonnetet sebességhez.
Az OmniRoute követi a modellek kvótáját!

### Nyílt AI Codex (Plus/Pro)

```bash
Felület → Szolgáltatók → Kapcsolódás Codexhez
→ OAuth bejelentkezés (1455. port)
→ 5 órás + heti újrainítás

Modellek:
  cx/gpt-5.2-codex
  cx/gpt-5.1-codex-max
```

#### Codex Számlányszabályozás (5h + Heti)

Minden Codex fiók mostantól megfelelő beállítókat tartalmaz az ` Felület -&gt;
Szolgáltatók ` lapon:

- `5h` (ON/OFF): akkor érvényesítenek a 5 órás időkeretet és szabályt\
  ==WEBLATE_PART==
- `Heti` (BE/AZ): kötelező az heti időablak határtételügyi politika betartása.
- Példányviselkedés: amikor egy engedélyezett ablak eléri az >=90%-os
  használatot, az adott fiók esetlegesen lekerül a listáról.
- Rotációs viselkedés: az OmniRoute az alapértelmezett Codex fiókot
  automatikusan a következő alkalommal a legközelebbi alkalomnak megfelelően
  juttatja.
- Mentés utáni viselkedés: a szolgáltató `resetAt` idejének letelte után az
  adott fiók automatikusan újra aktiválódik.

Forgatókönyvek:

- `5h ON` + `Heti ON`: olyan esetben, ha bármely ablak a határtételt éri el, a
  fiók kizárásra kerül.
- `5h OFF` + `Heti ON`: akkor a Heti használat dönti el, hogy a fiók kizárásra
  kerül-e.
- `5h ON` + `Heti OFF`: akkor a 5 órás használat dönti el, hogy a fiók kizárásra
  kerül-e.
- `Mentés után` lejárt: az adott fiók újra aktiválódik és újra bekerül a
  forgatókönyvekbe, nem szükséges manuális újracípés.

### Gemini CLI (INFORMÁCIÓSZÁMÍTÁSOKAT INGYEN adjon; 180K havi!)

```bash
Jelentés → Szolgáltatók → Jelentkezés Gemini CLIRA
→ Google OAuth
→ 180K bemeneti információs célkeresztben havi plusz 1K naponta

Módszerek:
  gc/gemini-3-jelentkezés-átmérő-összefoglaló
  gc/gemini-2.5-sériás
```

**Legjobb érték:** Hatalmas ingyenes szintje! Közbejelenjen mielőtt fizetős
szintként férne hozzá ehhez.

### GitHub másodpilóta

```bash
Jelentés → Szolgáltatók → Jelentkezés GitHub
→ GitHub által engedélyezett OAuth út
→ 1. napjával havonta frissítési ütemterv

Módszerek:
  gh/gpt-5
  gh/claude-4.5-versenyzési
  gh/gemini-3-komfortos
```

</details>

<details>
<summary><b>🔑 API Key Providers</b></summary>

### NVIDIA NIM (100% ingyenes fejlesztői hozzáférés érhető el – 70+ modell)

1. Regisztráció: [build.nvidia.com](https://build.nvidia.com)
2. Ingyenes API kulcs (1 billiónyi kijelzés kreditet tartalmazó alapértelmezett
   szoftververzió)
3. Jelentés → Szolgáltatók → Új szolgáltató hozzáadása → NVIDIA NIM:
   - API kulcs: `nvapi-your-key`

**Modell:** `nvidia/llama-3.3-70b-vezérelt injekcióval`,
`nvidia/mistral-7-instruktivitásra`, és több mint 50 más\
**Mód: **Közzététel[X10X], [X10X]Minősített közzététel[X21X]\
**Más: **hasonló elemekkel[X10X], [X10X]különleges elemekkel[X21X]

**Pro Tip:** Pro tip: ** OpenAI-kompatibilis API — kiválóan összehangolja az
OmniRoute formátum-átalakítási munkásságát!

### DeepSeek

1. Regisztráláshoz: [platform.deepseek.com](https://platform.deepseek.com)
2. API kulcs lekérése
3. Felület → Szolgáltató hozzáadása → DeepSeek

**Modulok:** `deepseek/deepseek-chat`, `deepseek/deepseek-coder`

### Groq (Ingyenes szintterület elérhető!)

1. Regisztráláshoz: [console.groq.com](https://console.groq.com)
2. API kulcs lekérése (több ezer utasítássorhoz ingyenes)
3. Felület → Szolgáltató hozzáadása → Groq

**Modulok:** `groq/llama-3.3-70b`, `groq/mixtral-8x7b`

**Pro Tip:** Rendkívül gyors kiértékelés — a valós idejű ködítéshez a legjobb!

### OpenRouter (100+ modul)

1. Regisztráláshoz: [openrouter.ai](https://openrouter.ai)
2. API kulcs lekérése
3. Felület → Szolgáltató hozzáadása → OpenRouter

**Modulok:** Az összes fő szolgáltató által kínált 100-nál több modulhoz
egyetlen API kulcs keresztül hozzáférhetsz.

</details>

<details>
<summary><b>💰 Cheap Providers (Backup)</b></summary>

### GLM-4.7 (Napi újrablokölés, 0,6 dollár/millió utasítás)

1. Regisztráláshoz: [Zhipu AI](https://open.bigmodel.cn/)
2. A kodolási tervből érhető el API kulcs
3. felületkezelő → API-t hozzon létre:
   - Típus: `glm`
   - API kulcs: `your-key`

**Használd: ** `glm/glm-4.7`

**A pro tip:** A Coding Plan 3-szoros díjat, 1/7-es áron kínálja! Mindennap
10:00 AM-kor frissül!

### MiniMax M2.1 (5 órás feltöltés, $0,20/1M)

1. Regisztrálj: [MiniMax](https://www.minimax.io/)
2. API kulcs lekérése
3. felületkezelő → API-t hozzon létre

**Használd: ** `minimax/MiniMax-M2.1`

**A pro tip:** Legalább 1 millió token mellett a leghatékonyabb és a legolcsóbb
opció!

### Kimi K2 (9 dollár havonta fix)

1. Regisztrálj: [Moonshot AI](https://platform.moonshot.ai/)
2. API kulcs lekérése
3. felületkezelő → API-t hozzon létre

**Használd: ** `kimi/kimi-latest`

**A pro tip:** 10 millió tokenos díjszabására 9 dollárt adunk, így hatékonyan 90
centes áron megteheted!

</details>

<details>
<summary><b>🆓 FREE Providers (Emergency Backup)</b></summary>

### iFlow (5 ingyenes modell adott az OAuth-n keresztül)

```bash
Felületkezelő → csatlakoztassa az iFlow-et
→ iFlow OAuth bejelentkezés
→ Korlátozás nélküli használat

Modulok:
  if/kimi-k2-thinking
  if/qwen3-coder-plus
  if/glm-4.7
  if/minimax-m2
  if/deepseek-r1
```

### Qwen (4 ingyenes modell kapcsolódvaDevice kode-készlet)\

```bash
Dashboard → Kapcsolat Kiro
→ Eszköz kód hitelesítés
→ Korlátozás nélküli használat

Modelljei:
  qw/qwen3-kódoló-plussz
  qw/qwen3-kódoló-akció
```

### Kiro (Claude KÉSZ)

```bash
Dashboard → Kapcsolat Kiro
→ AWS Builder ID vagy Google / GitHub
→ Korlátozás nélküli használat

Modellek:
  kr/claude-szonett-4.5
  kr/claude-haiku-4.5
```

</details>

<details>
<summary><b>🎨 Create Combos</b></summary>

### Példa 1: Maximálisabb Állapot → Önköltséges Védelmi Mentés

```
Dashboard → Kombinációk → Új elem hozzáadása

Név: premium-kódolás
Modelljei:
  1. cc/claude-opusz-4-6 (Alapdíjas primér)
  2. glm/glm-4.7 (Önköltséges mentés, $0.6/1M)
  3. minimax/MiniMax-M2.1 (A legolcsóbb alternatív, $0.20/1M)

A CLI-ben használatban: premium-kódolás
```

### Példa 2: Szabad Csak (Semmi meg nem áll)

```
Név: ingyenes-kombináció
Modellek:
  1. gc/geminisz-3-akció-előnézet (180K ingyen hónap)
  2. if/kimi-k2-gondolkodás (korfíkorlátozás)
  3. qw/qwen3-kódoló-plussz (korfíkorlátozás)

Költség: 0 dolár életrevaló!
```

</details>

<details>
<summary><b>🔧 CLI Integration</b></summary>

### Kurzor IDE

```
Beállítások → Modelljei → Fejlett:
  NyíltAI API alapú IP-cím: http://localhost:20128/v1
  NyíltAI API Kulcs: [az OmniRoute felületéről származik]
  Modell: cc/claude-opusz-4-6
```

### Claude Kód

Használja a ** CLI Eszközök** lapot a felületen egykattintással, vagy
szerkesztesse `~/.claude/beállítások.json` kézzel.

### Codex CLI

```bash
export NYÍLTBASE_URL="http://localhost:20128"
export OPENAI_API_KEY="az omniroute api kulcsa"

codex "az ön ajánlata"
```

### OpenClaw

**Válasz 1 — Felület (javasolt):**

```
Felület → CLI Eszközök → OpenClaw → Model választása → Alkalmaz
```

**Válasz 2 — Manuális:** Szerkesztesse `~/.openclaw/openclaw.json`:

```json
{
  "modell": {
    "szolgáltatók": {
      "omniroute": {
        "baseUrl": "http://127.0.0.1:20128/v1",
        "apiKey": "sk_omniroute",
        "api": "openai-completions"
      }
    }
  }
}
```

> **Megjegyzés:** Az OpenClaw csak helyi OmniRoute-rel működik. A `127.0.0.1`-t
> használja helyett `localhost`-ot, hogy megkerüljük az IPv6 dekódolásban
> fellépő problémákat.

### Cline / Folytatás / RooCode

```
Beállítások → API Konfiguráció:
  Szolgáltató: OpenAI Kompatibilis
  Alap URL: http://localhost:20128/v1
  API Kulcs: [a OmniRoute felületéről]
  Modell: if/kimi-k2-thinking
```

### OpenCode

**Lépés 1:** Adja hozzá a OmniRoute-t a rendszerének custom szolgáltatóját:

```bash
opencode
/csatlakozás
# Vegye ki "Egyéb"  →  ID-nak adja:  "omniroute"  →  Beírja az OmniRoute API kulcsát
```

**Lépés 2:** Töltse le/fel `opencode.json` fájlt a kiindulási gyökérfolderbe:

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
      "modell": {
        "cc/claude-sonnet-4-20250514": { "name": "Claude Sonnet 4" },
        "gg/gemini-2.5-pro": { "name": "Gemini 2.5 Pro" },
        "if/kimi-k2-thinking": { "name": "Kimi K2 (Free)" }
      }
    }
  }
}
```

**Lépés 3:** Válassza ki a modellt az OpenCode-ban:

```bash
/modellek
# Válasszon bármilyen OmniRoute modellt a listából
```

> **Tipp:** Adja hozzá bármilyen modellt, amely a OmniRoute `/v1/modellek`
> végpontján elérhető, a `modell` szakaszba. Formátum:
> `szolgáltatás/modell-azonosító` a rendszere OmniRoute felületéről

</details>

---

## Hibaelhárítás

<details>
<summary><b>Click to expand troubleshooting guide</b></summary>

**"A nyelvi modellek nem adtak vissza üzenetet"**

- A szolgáltatási körlemény kimerült → Ellenőrizze a letevő táblázatot az
  alkalmazásdashboard
- Megoldás: Használja a kombó-fallbackat, vagy választson a olcsóbb díjszabási
  szintre

**Sebességkorlát**

- Regisztrációs kötélkimerülés → Váltson a GLM/MiniMax-re
- Hozzon létre kombót: `cc/claude-opus-4-6 → glm/glm-4.7 → if/kimi-k2-thinking`

**OAuth-jegyet lejárt**

- Automatikus újrakapcsolás az OmniRoute-nál
- Ha továbbra is problémák jelentkeznek: Megoldás → Szolgáltató → Újra
  csatlakozás

**Magas költségek**

- Kereshet a felhasználói statisztikákat a Dashboard → Költségek panelen
- Váltson az alapértelmezett modellt GLM/MiniMax-re
- Használja a tömegesen (Gemini CLI, iFlow) ingyenes szintjét a nem kritikus
  feladatokra

**Dashboard/API Ports rossznak érzékelte**

- `PORT` a kanonikus alapértelmezett port (és.api-port alapértelmezetet is)
- `API_PORT` csak az OpenAI-kompatibilis API-kiszolgálóra lép
- `DASHBOARD_PORT` csak a dashboard/Next.js kiszolgálóra lép
- Állítsa be `NEXT_PUBLIC_BASE_URL`-t a dashboard/public URL-jára (a
  hitelesítési visszavételezésekhez)

** Felhő-hiba csomagolások**

- Jelentsse ellenőrizze, hogy `BASE_URL` mi ellenőrzi menő kereskedelmi
  változaton
- Jelenterze, hogy `CLOUD_URL` valóban mi ellenőrzi lejáró visszavétellel
- Tartsa egybe `NEXT_PUBLIC_*`-t a szerver-közi átszúrással

**Az első bejelentkezés nem működik elvégzése**

- Jelentse ellenőrzi, hogy `INITIAL_PASSWORD` kitölti .env fájloban
- Ha törlődik, hibahatása alapértelmezet `123456`

**A nem talál kívánsagyad kérést**

- Állítsa be `ENABLE_REQUEST_LOGS=true`-t .env fájlba

**A kapcsolat teszt "Inválid" értéket ad OpenAI-kompatbilek felületke során**

- Sok szolgáltatás nem ad hatást [/ models` endpointet
- A OmniRoute verzon 1.0.6+ tartalmaza visszavett határolvani visszavételen
  keresztül
- A biztonsági jel 🔒 alatt az Egyéb szervereken történő OAuth beállítása

### A fő URL-cím tartalmaznia kell a [X25X]/v1[X29X] előtagot

<a name="oauth-on-a-remote-server"></a> <a name="oauth-em-servidor-remoto"></a>

> **⚠️ Fontos a OmniRoute alkalmazás futtatásához a VPS, Docker, vagy a bármely
> távoli szerver** feltétele

#### Miért nem sikerül a távoli szervereken az Antigravity / Gemini CLI OAuth beállítás?

Az Antigravity** és a Gemini CLI** szolgáltatók **Google OAuth 2.0**-t
használnak. A Google a OAuth folyamattól a `redirect_uri`-t követeli meg
pontosan azon URI-k egyikével, amelyek előre regisztrálva vannak az alkalmazás
Google Cloud konzoljában.

Az OmniRoute-ben csomagolt OAuth-kul cs és kredenciák csak a `localhost`-ra
kicsomagolva lettek regisztrálva**. Amikor a remoteszerverről (pl
`https://omniroute.myserver.com`) próbálja például megjeleníteni az
OmniRoute-ot, a Google a következő hibát adja vissza:

```
Hiba 400: redirect_uri_mismatch
```

#### Helyes megoldás: Konfigurálja az összevont OAuth-kul css és kredenciákat

Saját OAuth-kul cs és kredenciákra van szüksége

#### Ahhoz, hogy el lehessen végeznie a kérést lépésről lépésre, az alábbiakra lesz szüksége:

**1. Nyissa meg a Google Cloud Console-t**

Másolja be ezt a címet:
[https://console.cloud.google.com/apis/credentials](https://console.cloud.google.com/apis/credentials)

**2. Hozzon létre új OAuth 2.0-szolgáltatói azonosítót**

- Kattintson **"+" Új hitelesítési adatok hozzáadása"** → **"OAuth 2.0 kliens
  azonosítója"**
- Alapján az alkalmazás: **"Webes alkalmazás"**
- Név (amit a szolgáltatói regisztrálnak): bármit (pl: `OmniRoute távoli
  szerver`)

**3. Hozzon létre bejegyzéseket a megengedett visszazáráshoz az URL-címekhez**

A **"Megengedett visszazáráshoz való URI-k"** mezőbe írjon:

```
https://a-szervertípus.com/visszaigazolási-hely
```

> Cserélje le `a-szervertípus.com` az Ön által használt szervernek, a
> `szervertípus vagy `IPv4 címmel, esetleg `http://45.33.32.136:20128/callback`)

**4. Mentse meg a hitelesítő adatokat**

Google majd megjeleníti a **Klienst ID**-t** és a **Hitelesítő kód**-ot.

**5. Beállításként ható változók beállítása**\
==WEBLATE_PART ==\
Önnek az alábbi hitelesítő adatokat adnia kell Önnek a [.env][X13X] állományába
(vagy a Docker környezeti változókba):

# Antigravity esetében:\
ANTIGRAVITY_OAUTH_CLIENT_ID=googleprojekt azonosító.apps.googleusercontent.com\
ANTIGRAVITY_OAUTH_CLIENT_SECRET=hitelesités kód GOCSPX-\
\
# A Gemini CLI esetében:\
GEMINI_OAUTH_CLIENT_ID=googleprojekt azonosító.apps.googleusercontent.com\
GEMINI_OAUTH_CLIENT_SECRET=hitelesités kód GOCSPX-\
GEMINI_CLI_OAUTH_CLIENT_SECRET=hitelesités kód GOCSPX-

```bash
[X0X]6. Restart OmniRoute[X22X]
```

# npm:\
npm run dev\
\
# Docker:\
docker restart omniroute

```bash
[X0X]7. Próbálja újraindítani a kapcsolatát[X25X]
```

Jegyzetfüzet > Szolgáltatások > Antigravity (vagy Gemini CLI) > Oauth

A Google most szabályosan átirányít az [X38X]URL-címet[ X71X] a
[X38X]http://localhost[ X57X]-t\
[X38X]http://your-server.com/callback[X71X]-ba

Ideiglenes munkamenet (vagyis a felhasználó saját hitelesitést nem állított meg)

---

#### Ha most felhasználja a [X82X]Manzila útvesztőség[X99X] hitelesitési folyamatot:

Az OmniRoute megnyitja a Google engedélyeztetési URL címét

1. Ha meg szeretné hitelesitést az [X47X]helyi szervere[X57X] beállításakor, a
   felé nem válik sikerrel. Ekkor visszarázza a [X47X]helyi szervere[X57X]
2. [X0X]Mentse a teljes URL-címet [X19X] a böngésző felső sorn a címtóla
3. ** Másolja be az URL - címet, és az modális melyben a csatlakozási mezőbe
   másolja be
4. Kattintson a ["Csatlaka"][X6X] [X6X]gombra[X17X]
5. Ez működik ugyanis a **böngészőben megjelenő hitelesitési készülé általi a
   összesítő ** átirányíta, ezzel visszatelepíti **a bökönget a
   visszairányíta.az **szörzést**

> Miként okozhatja az Oauth megsérültődését a következő helyen [X14X]

---

<details>
<summary><b>🇧🇷 Versão em Português</b></summary>

#### A szolgáltatók [X14X]  Antigravity[X27X]  és a [X32X] Gemini Cli[X44X]  felhasználja az  [X52X]  Goole Oauth 2 [X70X]-t  a  [X52X] felhíveneti adataihoz

A felhíveni adataihoz milyen helyre érvényeltse ezzéket az ** URL címet** a
Google \
klnf \
Ez alapja `a URL címére **és az átirányítás hitelesitést**

As credenciais OAuth embutidas no OmniRoute estão cadastradas **apenas para
`localhost`**. Quando você acessa o OmniRoute em um servidor remoto (ex:
`https://omniroute.meuservidor.com`), o Google rejeita a autenticação com:

```
Hiba 400: redirect_uri_mismatch
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

**6. Indítsa újra az OmniRoute-t**

```bash
# Amennyiben npm-t használ:
npm run dev

# Amennyiben Docker-t használ:
docker restart omniroute
```

**7. Próbálja újra csatlakozni**

Kezdőlapon → Szolgáltatók → Antigravitációs (vagy Gemini CLI) → OAuth

Most a Google kereken irányít át `https://se-szervere.com/callback` és a
hitelesítés működni fog.

---

#### Ideiglenes munkafüggő megoldás (nem konfigurálja az egyedi hitelesítő adatokat)

Ha nem akarja a jelenlegi hitelesítő adatok konfigurálását, a **manuális
lehatározási URL** segítségével mégis használhatja a folyamatot:

1. Az OmniRoute megnyitja a Google hozzájárulási URL-ét
2. Amint engedélyezte, a Google megpróbál átterelni a `helyi szervere`-re (ami a
   távoli szerveren függetlenül megbukik)
3. **Összegyűjtse általános URL-ét** a böngésző címkeresőjéből (annak
   függetlenül, hogy a lap betöltődik-e)
4. Illessze be ezt az URL-t a megjelenő kapcsolatmodulban található mezőbe
5. Kattintson az ** "Csatlakozás"** gombra

> Ez a megoldás hatékony, mert az engedélyezési kód, bármilyen sikertelen
> átirányítás után is érvényes marad.

</details>

---

</details>

## 🛠️ Technológiai háttér

<details>
<summary><b>Click to expand tech stack details</b></summary>

- **Kiszolgálók**: Node.js 18–22 LTS (🚨 Node.js 24+ nem **támogatott** – a
  `native sqlite3` binárisok [X87X]összeegyeztethetetlenek[X91X])
- **Nyelv**: TypeScript 5.9 — 100%-os **TypeScript-használat** az `forrás` és
  `nyitott összetevők` esetében (a `.zéró` hibátlan modulban sincs hibás
  .any[X88X] eladás)
- **Felhasználói felület**: Next.js 16 + React 19 + Tailwind CSS 4
- **Adatbázis**: LowDB (JSON) + SQLite (tartományi állapot + proxy feljegyzések
  + MCP audit + útvonalvezetés információk)
- **Sémák**: Zod (MCP segédprogram a beadvonalon, API -szerződés)
- **Protokollok**: MCP (stdio + HTTP) + A2A v0.3 (JSON-RPC 2.0 + SSE)
- **Streamzés**: Server-Sent Események (SSE)
- **Hitelesítés-X**: OAuth 2.0 (PKCE) + JWT + API Kulcsok + MCP Szabályozott
  Hozzáférés
- **Tesztelés**: Node.js tesztelő + Vitest (900+ teszt, ideértve a unit,
  integrációs és E2E teszteket is)
- **CI/CD**: GitHub Akciók (auto-npm publikálás + Docker Hub kiadáskor
- **Honlap**: [omniroute.online](https://omniroute.online)
- **Csomag**:
  [npmjs.com/package/omniroute](https://www.npmjs.com/package/omniroute)
- **Docker**:
  [hub.docker.com/r/diegosouzapw/omniroute](https://hub.docker.com/r/diegosouzapw/omniroute)
- **Erőforrás-patológia**: Körbezáró áramkör, exponenciális visszahatás,
  anti-thundering erőforrás-hordó, TLS-spoofing, önellátó öngyógyulás

</details>

---

## Dokumentáció

| Dokumentál                                                 | Leírás                                                                           |
| ---------------------------------------------------------- | -------------------------------------------------------------------------------- |
| [Felhasználói útmutatót](docs/USER_GUIDE.md)               | Fejlesztők, kombinációk, parancssori integráció, telepítés                       |
| [A API-referenciálja](docs/API_REFERENCE.md)               | Mindek összes endpoint a példákkal együtt                                        |
| [MCP Servert](open-sse/mcp-server/README.md)               | 16 MCP eszköz, IDE-konfigurációk, Python/TS/GO kliens                            |
| [A2A Szervert](src/lib/a2a/README.md)                      | JSON-RPC 2.0 protokoll, készségek, streaming, feladatkezelés                     |
| [Ön-összeállító Motorjat](docs/auto-combo.md)              | Hatásosság 6 tényezőre alapított skála, modulok serege, önmegiszegeződő képesség |
| [Troubleshootálás](docs/TROUBLESHOOTING.md)                | Befejezésének problémái és megoldásai                                            |
| [Architektúra](docs/ARCHITECTURE.md)                       | A rendszer architektúrája és belső működése                                      |
| [Közreműködés](CONTRIBUTING.md)                            | Fejlesztési beállítások és irányelvek                                            |
| [OpenAPI Spec](docs/openapi.yaml)                          | OpenAPI 3.0-specifikáció                                                         |
| [Biztonsági stratégia](SECURITY.md)                        | Fogyatékosságok jelentése és biztonsági gyakorlatok                              |
| [Kiszolgáló-deploy](docs/VM_DEPLOYMENT_GUIDE.md)           | Teljes útmutató: VM + nginx + Cloudflare beüzemelés                              |
| [Szolgáltatások katalógusa](docs/FEATURES.md)              | Mikrografikus tájékozódó panel szkriptekkel                                      |
| [Preliminary ellenőrzési lista](docs/RELEASE_CHECKLIST.md) | Előzetes hitelesítések lépjei                                                    |

---

## 🗺️ Útmutató

Az OmniRoute 210+ funkcióval rendelkezik** tervben**, amelyet több fejlesztési
szakaszban hajtanak végre. Az alábbi területekben érhetők el a kulcsfontosságú
elemek:

| Kategória                                 | Tervezett Jellemzők | Kimagasló változók                                                                                                     |
| ----------------------------------------- | ------------------- | ---------------------------------------------------------------------------------------------------------------------- |
| 🧠 Utazás & Inteligencia **Routelés **     | 25+                 | A legnagyobb késést produkáló útválasztás, címkét jelölő útválasztás, számláló felülvizsgálat, P2C fiók kiválasztása   |
| 🔒 **Biztonság & A felhőbe való betartás** | 20+                 | HARD sérülékenység, titkosítási takargatás, védelmi időtartam minden pontonként, menedzs mentesség összefüggés-kódolás |
| 📊 ** Megfigyelések**                      | 15+                 | Nyitott szenzorintegrációk, valós idejű kvóta-monitorozás, költség nyomonkövetés egy modellenként                      |
| 🔄 ** Provider Integrációk**               | 20+                 | Dinamikus modell-regiszter, szállító időzítések, több fiók Codex, Copilot kvóta elemzés                                |
| ⚡ ** Teljesítmény**                       | 15+                 | Dvojkémnyomást betükrző rétegek, megjelölési környezet, válasz környezet, stream-élnival, többfeladatú API             |
| 🌐 ** Ekokeret**                           | 10+                 | WebSocket API, konfig konfigurációs frissítés, szórópont konfire-konfiguráció, kereskedelmi mód                        |

### 🔜 Hamarosan elérhető

- 🔗 **OpenCode Integráció**– Native szállító támogatás az OpenCode azonosító AI
  kód-IDE-jéhez
- 🔗 ** Integráció a TRAE kerettel ** — Teljes támogatás a TRAE AI fejlesztési
  Keretrendszerhez
- 📦 **Batch API ** — Szinkron, batch feldolgozási kérelmek számára
- 🎯 **Tárolt lekérdezési útvonal hozzáadása ** — Fordítsa le az útvonalakat
  alapvető címkéknek és metaadatnak megfelelően
- 💰 ** Legalább költség elv ** — Kiválasztsa a legolcsóbb árú szolgáltatót

> 📝 Teljes körű funkció specifikációk a
> [`dokumentáció/jól-ismereti-új-szolgáltatások/`](docs/new-features/) felében (
> 217 részletes vázlat)

---

## 👥 Szerzők

[![Szerzők] ](https://github.com/diegosouzapw/OmniRoute/graphs/contributors)

### Hogyan lehet Kontribálni

1. Foglalom el egy elágazást a repository
2. Hozzon létre új fejlesztői ágat (`git checkout -b fejlesztés/amazing
   szolgáltatás`)
3. Mentse a változtatásokat (`git commit -m 'Hozza létre egy amazings
   szolgáltatást'`)
4. Adja hozzá a szolgáltatásokat a tárolóhoz (`git push origin
   fejlesztés/amazing szolgáltatás`)
5. Nyisson új Pull kérelmet

Látogasson el a [CONTRIBUTING.md](CONTRIBUTING.md) oldalt a részletes
irányelvekért.

### Új verzió kibocsátása

```bash
# hozzon létre új kiadást  — az npm publish automatikusan megtörténik
gh release create v2.0.0 --title "v2.0.0" --generate-notes
```

---

## 📊 Számítási folyamata  Története

## Csillagszámolás folyamának  Eredményei

## ![Csillagszámolók Eredményei szemléletéhez](https://starchart.cc/diegosouzapw/OmniRoute.svg?variant=adaptive)](https://starchart.cc/diegosouzapw/OmniRoute)

## 🙏 Köszönetnyilvántartás

Külön köszönet **[router](https://github.com/decolua/9router)**-nek,
**[decolua](https://github.com/decolua)**-től, az eredeti projekt alapjául
szolgáló forkhoz. Az OmniRoute ehhez a fantasztikus alapzathoz további
funkciókkal, multi-modális API-kkal és teljes TypeScript átírásokkal bővíti.

Külön köszönet
**[CLIProxyAPI](https://github.com/router-for-me/CLIProxyAPI)**-nek - az eredeti
Go implementációnak, mely inspirálta ezt a JavaScript portot.

---

## 📄 Számlásvédelem

MIT-licenc - részletekért lásd [LICENSE](LICENSE)-ot.

---

<div align="center">
  <sub>Built with ❤️ for developers who code 24/7</sub>
  <br/>
  <sub><a href="https://omniroute.online">omniroute.online</a></sub>
</div>
<!-- GitHub Discussions enabled for community Q&A -->
