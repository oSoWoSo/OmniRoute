# Omniroute — Vapaahierontyökalu - AI-portaal

### Koodaa jatkuvasti. Kiehtova oikaisu **VAPAAT & alhaiset AI-mallit** [H22X]Keskitetyn vajan[X69X] automatikalla. Salli jatkuva toiminta.

_Yli 67 IP-seivästä ja tarjontaa 100% -tyypin _API-proksimaattinen lähde[X123X]

**Keskusteleminen, Koodaamisen tulkitseminen • Hahmojen koot • Kuva • Video •
Musiikki • Ääni • Reranking • **Verkkosivun hakupalvelu**• MCP-palvelin • A2A:
Käyttäjä-agentin ohjelmointi • 100% TypeScript**

---

<div align="center">

[![npm-versio](https://img.shields.io/npm/v/omniroute?color=cb3837&logo=npm)](https://www.npmjs.com/package/omniroute)
[![npm
lataukset](https://img.shields.io/npm/dm/omniroute?color=cb3837&logo=npm&label=npm%20downloads)](https://www.npmjs.com/package/omniroute)
[![Docker
Hub](https://img.shields.io/docker/v/diegosouzapw/omniroute?label=Docker%20Hub&logo=docker&color=2496ED)](https://hub.docker.com/r/diegosouzapw/omniroute)
[![Docker
Pulls](https://img.shields.io/docker/pulls/diegosouzapw/omniroute?logo=docker&color=2496ED&label=docker%20pulls)](https://hub.docker.com/r/diegosouzapw/omniroute)
[![Lisenssi](https://img.shields.io/github/license/diegosouzapw/OmniRoute)](https://github.com/diegosouzapw/OmniRoute/blob/main/LICENSE)
[![Verkkosivu](https://img.shields.io/badge/Website-omniroute.online-blue?logo=google-chrome&logoColor=white)](https://omniroute.online)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-Community-25D366?logo=whatsapp&logoColor=white)](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

[🌐 Verkkosivu](https://omniroute.online) • [🚀 Kirjaudu sisään](#-quick-start) •
[💡 ominaisuudet](#-key-features) • [📖 Dokumentaatio](#-documentation) • [💰
Hinnat](#-pricing-at-a-glance) • [💬
WhatsApp](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

</div>

🌐 **On saatavilla[ X17X] 🇺🇸 [Englanti](README.md) | 🇧🇷
[Portugali](docs/i18n/pt-BR/README.md) | 🇪🇸 [Espanja](docs/i18n/es/README.md) |
🇫🇷 [Ranska](docs/i18n/fr/README.md) | 🇮🇹 [Italiano](docs/i18n/it/README.md) | 🇷🇺
[Venäjä](docs/i18n/ru/README.md) | 🇨🇳 [Kiina
(yksinkertaistettu)](docs/i18n/zh-CN/README.md) | 🇩🇪
[Saksa](docs/i18n/de/README.md) | 🇮🇳 [Hindi](docs/i18n/in/README.md) | 🇹🇭
[Thai](docs/i18n/th/README.md) | 🇺🇦 [Ukraina](docs/i18n/uk-UA/README.md) | 🇸🇦
[Arabi](docs/i18n/ar/README.md) | 🇯🇵 [Japani](docs/i18n/ja/README.md) | 🇻🇳
[Vietnam](docs/i18n/vi/README.md) | 🇧🇬 [Bulgaria](docs/i18n/bg/README.md) | 🇩🇰
[Tanska](docs/i18n/da/README.md) | 🇫🇮 [Suomi](docs/i18n/fi/README.md) | 🇮🇱
[Heprea](docs/i18n/he/README.md) | 🇭🇺 [Unkari](docs/i18n/hu/README.md) | 🇮🇩
[Indonesian](docs/i18n/id/README.md) | 🇰🇷 [Korea](docs/i18n/ko/README.md) | 🇲🇾
[Malaiji](docs/i18n/ms/README.md) | 🇳🇱 [Alankomaat](docs/i18n/nl/README.md) | 🇳🇴
[Norja](docs/i18n/no/README.md) | 🇵🇹 [Portugali](docs/i18n/pt/README.md) |
[Romania](docs/i18n/ro/README.md) | [Puola](docs/i18n/pl/README.md) |
[Tšekki](docs/i18n/sk/README.md) | [Ruotsi](docs/i18n/sv/README.md) |
[Filippiinit](docs/i18n/phi/README.md)

---

## 🆕 Uutta v3.0.0 -versiossa

> **Etsi päivitystä v2.9.5 pistorajojen rajoittamiseksi?** - Katso
> [täysimittainen
> Vaihteluindeksi](CHANGELOG.md#300--2026-03-22-release-candidate--not-yet-merged-to-main),
> kaikki muutokset.

| Alue                                  | Vaihto                                                                                                                                                                                                                                                                                                                                                                          |
| ------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🔒 **CodeQL Vaihdejärjestelmä**        | Korjattu: kaksitoista CodeQL-merkintää: monisteiden palautustiedot, turvattomia sattuman tekemisiä, pallonvaihtokeskusteluyhteys korjattiin                                                                                                                                                                                                                                     |
| ✅ **Tievalidointi**                   | Kaikki 176 API-reittien vahvistetaan nyt Zod skeemoilla + `tarkista vastaanottava koodi[ X67X] Kaikki testit `käynnistä ylintä: reitin vahvistus t:06` tehdään                                                                                                                                                                                                                  |
| 🐛 **omniModel Tag Leak**              | Alkuperäiset `<omnimodel>`merkinnät eivät siirtyny pääseteen olemassaolevien asiakkaiden asemesta [H55X]Oikaisua tukevia päätestää [H70X] SSE lähetystiedot</omnimodel>                                                                                                                                                                                                         |
| 🔑 ** Rekisteröity yhteys API  **      | Sisäinen asiakasrekisterin otsikon oikeutusoimassa aina lähes kaikille asiakkaille ja per-asiakas/tili rajat huolimatta asiakaskentän ydinsubrakoa `POST /api/v1/registered-keys` lähettää tarpeesta pihdeksi, yhteentunnustetulla päätestä [H92X]tuntemustekijä [H96X], energeettiseen [H104X]tiedonpidätytö[ H129X] päätestiä lähdeerää [H113X]GitHub- otsikon tarkistusvihje |
| 🎨 ** Asiakaslogoit**                  | 130+ toimittajan logoa `@lobehub/icons` (SVG) PNG:siin vaihtuneen yleisFallback ketjun avulla                                                                                                                                                                                                                                                                                   |
| 🔄 **Mallin Automaatti-Synkki**        | 24-tuntinen aikataulu ja käyttäjän ohjaama toiminto varten mallilistojen synkronointi rakennetulle ja mukautetulle avoimen lähdekoodin yhteensopiville toimittajille                                                                                                                                                                                                            |
| 🌐 **Avoimuksen Zen/Go**               | Kaksi uutta toimittajaa @kang-heewon kautta PR:stä #530: ilmaiskiertuetta ja lukukoirtoen mukainen yhteensopivuus `OpencodeExecutor`                                                                                                                                                                                                                                            |
| 🐛 **Geminin CLI Otaat**               | Toiminnallinen virhe kun `GEMINI_OAUTH_CLIENT_SECRET` puuttuu Dockerissa (oli kryptinen Googlen virheilmoitus)                                                                                                                                                                                                                                                                  |
| 🐛 **Avoimuksen asetus**               | `saveOpenCodeConfig()` kirjoittaa nyt oikein TOML:in `XDG_CONFIG_HOME`                                                                                                                                                                                                                                                                                                          |
| 🐛 **Pienenutun mallinkerroin**        | `body.model` määritellään nyt `pinnedModel` säännöstön sääntelemiseen                                                                                                                                                                                                                                                                                                           |
| 🐛 **Koodiksen/Claude syyttelimäinen** | `tool_result` blokit muutetaan nyt tekstiksi estämään loppumatkan                                                                                                                                                                                                                                                                                                               |
| 🐛 **Kirjautumiskohdistuminen**        | Keskeytynyt [X0X]kirjautuminen ei jäädy nyt passwordin jättämisestä                                                                                                                                                                                                                                                                                                             |
| 🐛 **Windows tietorakenteet**          | MSYS2/Git-Bash tietorakenteet `/c/...` normalisoidaan automaattisesti `C:\...` -muotoon                                                                                                                                                                                                                                                                                         |

---

## 🖼️ Keskusvalikko

<div align="center">
  <img src="./docs/screenshots/MainOmniRoute.png" alt="OmniRoute Dashboard" width="800"/>
</div>

---

## 📸 Esikatseluvalikko

<details>
<summary><b>Click to see dashboard screenshots</b></summary>

| Sivu                        | Tallennuskuva                                             |
| --------------------------- | --------------------------------------------------------- |
| **Palvelinannokset**        | ![Palvelinannokset](docs/screenshots/01-providers.png)    |
| **Yhdistelmät**             | ![Yhdistelmät](docs/screenshots/02-combos.png)            |
| **Analytiikka**             | ![Analytiikka](docs/screenshots/03-analytics.png)         |
| **Terveydentunto**          | ![Terveydentunto](docs/screenshots/04-health.png)         |
| **Kääntäjä**                | ![Kääntäjä](docs/screenshots/05-translator.png)           |
| **Asetukset**               | ![Asetukset](docs/screenshots/06-settings.png)            |
| **CLI-työkit**              | ![CLI-työkit](docs/screenshots/07-cli-tools.png)          |
| **Käyttöäntennähdokkaiden** | ![Käyttöäntennähdokkaiden](docs/screenshots/08-usage.png) |
| **Päätepisteet**            | ![Päätepisteet](docs/screenshots/09-endpoint.png)         |

</details>

---

### Robotti: Ilmainen AI-annos Suomen suosikkeille koodinmalleille

_Liitä mihin tahansa AI-ytimellä varustettu IDE- tai CLI-pohjaistoimi omiin
reitittimellä – ilmaiseksi API-puolueuttaja Omnitien kautta, äärettömän
koodaamisen vapaudeksi._

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

<sub>📡 Kaikki agentit yhdistyvät <code>http://localhost:20128/v1</code> tai
<code>http://cloud.omniroute.online/v1</code> — yksi konfiguraatio, ääretön
määrä mallintamis- ja quota</sub>

---

## 🤔 Miksi Omnitie?

**Ehkä sästykset ja rajat aiheuttavat suunnitelmasta ongelmia:**

- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Voimassaoloaikajakso ajautuu jälkeen jokaisen kuukauden päättyessä
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Rate-limiitti pysäyttää työryhmän koodaessa
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Kallis API (20–50 euroa kussakin toimittajassa kuukaudessa)
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Manuaalinen siirtyminen toimittajista toiseen

**Omitie ratkaisee ongelman:**

- ✅ **Maksimin ja seuraamisen avulla** - Seuraa quota, käytä jokaista bitiä
  ennen resetointia
- ✅ **Automaattinen tuki** - Tilausesi → API-avain → Kiinteistö → Free, jopa
  yksi hetki
- ✅ **Monitoimimahdollisuuksia** - Siirro alue toiselle tililles tilaajien
  kesken toimitajana
- ✅ **Universaali** - Toimi sekä Codex, Gemini CLI, Cursor, Cline, OpenClaw,
  joka laite

---

## 📧 Avainasiat

> 💬 **Liity yhteisöömme!** [Yksityinen
> WhatsApp-ryhmä](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t) —
> Pääset saamaan apua ja pysyt yhteydessä tiiviisesti

- **Sivusto**: [omniroute.online](https://omniroute.online)
- **GitHub**:
  [github.com/diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute)
- **Ongelmat**:
  [github.com/diegosouzapw/OmniRoute/issues](https://github.com/diegosouzapw/OmniRoute/issues)
- **WhatsApp**:
  [Yhteisö-ryhmä](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)
- ** Avustaminen**: Lue [CONTRIBUTING.md](CONTRIBUTING.md), avaa
  lisäyshakemuksen , avaa suunnitelmia, etsi `hyvä aloitettava tehtävä`
- **Alkuperäinen Projekt**: [9rooli
  deconetta](https://github.com/decolua/9router)

### 🐛 Mieliodotusta bugi?

Kirjoita tapahtuma ilmoitus, kun avaatte järjestelmän tiedot-päätöksen
käynnistää ja liitä luotu tiedosto:

```bash
npm run system-info
```

Tämä generoi `system-info.txt` Node.js version, OmniRoute version, vakaasi
ohjemetietoja, asennetut CLI -työkalut (iflow, gemini, claude, codex,
antigravity, droid, jne.), Docker / PM2 tilanne , systeemipaketteja -- kaikki,
mitä tarvitset nopeasti reproduoidaksesi tarkoituksenasi:\
Liitä suoraan GitHub-tapahtumaasi.

---

## Miten se toimii

```
┌─────────────┐
│  Your CLI   │  (Claude Koodi, Codex, Gemini CLI, Avoinkausiruna, Kiertääpiha, Cline...)
│   Työkalu      │
└──────┬──────┘
       │ http://localhost:20128/v1
       ↓
┌─────────────────────────────────────────┐
│           OmniRoute (Smart Router)        │
│  • Kiintiömuunnos (OpenAI ⬅️ Claude) │
│  • Kiintiön seuranta + lähetteet + kuvat │
│  • Auto token refresh                   │
└──────┬──────────────────────────────────┘
       │
       ├─→ [Taso 1: Tilauksessa] Claude Koodi, Codex, Gemini CLI
       │   ↓ kiintiömuunnos
       ├─→ [Taso 2: Avain] DeepSeek, Groq, xAI, Mistral, NVIDIA NIM, jne
       │   ↓ budjetti raja
       ├─→ [Taso 3: Lapsivaha] GLM (0,6 / 1M), MiniMax (0,2 / 1M)
       │   alimmassa budjettiraja
       └─→ [Taso 4: Ilmainen] iFlow, Qwen, Kiro (rajattomasti)

Tulos: Ei lopeta koskaan koodimusta, minimimäärä maksu
```

---

## 🎯  Mitä OmniRoute ratkaisee – 30 todellista ongelmaa ja käyttötapaa

> **Kuollut kulkuri joka käyttää AI-laitteita käsittelee näitä ongelmaa
> arki-arisevasti.** OmniRoute on suunniteltu ratkaisemaan ne kaikki – kullekin
> kystästä kuluvista maksuista, regionaalista blokeerauksista, murtuneista OAuth
> -virtauksista, käsittelyyksiköitä ja yrityksen havaintokykyyn.

<details>
<summary><b>💸 1. "I pay for an expensive subscription but still get interrupted by limits"</b></summary>

Käyttäjät maksavat 20–200 dollaria kuukausi kuitenkin Claude Pro , Codex Pro,
tai GitHub -Käyttämätön jättää edelleen kulkeutuviin. Kuitenkin, kiintiöllä on
suuri ilman kattoa — 5h käyttöaika, viikoittaiset rajoitukset tai
minuuttirajoitukset säännöst.\
Kesken koodijarjestelmässä käsittelykeskittäminen loppuu vastauksessa ja
palvelija menetää kääntöpyristo ja tuottavuus.

**Howin ratkaisu siihen**:

- **Smart 4-Tier Fallback** — If tilauksen kiintiö käytetty, automaattisesti
  ohjaa suoraan Avain → Halpo → Vapaasti jne. ilman manuaalista toimintaa
- **Real-Time Quota Tracking** — Noudattaa aikakone-tilanne sekä
  palautusaikaiseen muistinpäivänpalvelu. (5h, päivittäiset, viikoittaiset)
- **Multi-Account Support** — Monia tilitapoja, mistä vikaansaikaisesti, vastaa
  siirrun käännös uusimena ensin kunnasta määrä
- **Custom Combos** — Kostumoiduilla peruu muuntuu ketekunnan strategioiden
  pystyttäävyyksien peräännös tasoissa
- **Codex Business Quotas** — yritykset/työryhmän sisäinen käyttöönotto
  alkuilmoitusta käyttöönotetaan, mukaan lukien viikkojen kiertämisrajoitus.

</details>

<details>
<summary><b>🔌 2. "I need to use multiple providers but each has a different API"</b></summary>

OpenAI käyttää yhtä luomuta koodiketekunta, sitten Claude (Anthropic) käyttämäsi
tulosjärjestelmää, Gemini jne. Jos koodivirtalähteen haluaa testata kohtioksia
toisistaan tai kaksitasaisesta käännöksistä jne. Käyttäjän tarvitsee muuttaa SDK
-tarkastus muulla pino sormella ensin.

**Howin ratkaisu siihen**:

- **Unified Endpoint** — Pyyntö, joka vastaa koodiketekuta kyytöön vastaisesti
  kulkeutuvia kääntösolut tasan perällä, kulkee aika kyytöön yhdellä kärki, joka
  yksikymmentä + sataa koodilähteistä
- **Format Translation** — Mukaantultua automatisoiin sulku OpenAI -> Claude ->
  Gemini -> Viestintä
- **Viestintäpuhdistus** — Poistaa ei-standardsidonnaisia kenttiä (`x_groq`,
  `käyttötilasto`, `palvelutas`) johtuen avoimesta AI-ohjelmistokyvylle v1.83+
- **Oikeudenkäytön Järjestäminen** — Muuttaa `kehittäjä` → `järjestelmä`
  ei-OpenAI-palveluntarjoajille; `järjestelmä` → `käyttäjä`
  GLM/ERNIE-ohjelmistolle
- **Ajattelu Merkinnän Pysääminen** — Pysäyttää `` -blokit mallista kuten
  DeepSeek R1 standardoituihin `perusteleminen sisältö`
- **Rakenteisto Ominaisuudet Geminiälle** — `json_skeemi` →
  `palautteenMIME-tyyppi`/`palautteskeitto` automaattinen konversio
- **`virta` alkaa `false`** — Vastaa OpenAI- tyyppiä, estämällä epävarma SSE
  Python/Rust/Go SDK-aloille

</details>

<details>
<summary><b>🌐 3. "My AI provider blocks my region/country"</b></summary>

Erillisten maantieteellisten alueiden vuoksi palveluntarjoajat kuten
OpenAI/Codex kieltävät lähestymisen. Käyttäjät saavat virheen kuten `tukeman
alueen / alueen ` OAuth-tilien ja API-yhteyksien aikana. Tämä on erityisen
haitallista kehittyville maihin kuuluville kehittäjille

**Howin ratkaisu siihen**:

- **3 -Tason Proksy - Konfig.** — Käytännöllinen lokaatio 3-tason tasolla:
  globaali (kaikki liikenne), yksittäinen palveluntarjoaja (ainakin yksi), ja
  yksittäinen yhteys/avain
- **Sävyläväritetyt Proksy - Pysyt ** — Visuaaliset indicatorit: 🟢 globaaleilla
  prosokylle, 🟡 palveluntarjoaja -proksyille, 🔵 yksittäisille yhteys-proksiille,
  aina osoittamassa IP-siirtymää
- **OAuth Kokonaisten Prosokyllä** — OAuth virtaus myös kuluu prosokyllä,
  ratkaisemalla `tukevaa aluetta / aluetta`
- **Yhteysvälitykset prosokyllä** — Yhteystestit käyttävät määriteltynä
  prosokyllä (ei enää suoraa ohitus
- **SOCKS5 Suojaus** — Kokonaan SOCKS5-suojattu prosoky vailla poistoa
- **TLS- Nauha Fingerprint Taimenta[MK]\**- Malli toimin `wreq-js` vastaamaan
  robotti-detektoinien kiertämiseksi
- ** 🔏 CLI Fingerprint Matching** – Muuttaa päähakemistot sekä vastauskentät
  samankaltaisiksi kuin alkuperäinen CLI-tiedostojen alkuperäissignaaleilla,
  suurenmattavasti ehkäiseen account-merkinnän riskiä. Proxy IP -tiedot on
  pysyvästi säilytetty – saat saman aikaa salaus ja IP-siirtymän simuloin.

</details>

<details>
<summary><b>🆓 4. "I want to use AI for coding but I have no money"</b></summary>

Ei kenenkään pysty suuressa kulussa maksamaan 20–200€/kk. Tulee tarjota
käytännöllistä mallien pääsyä suoraan kosteuttaessa 0 €/kk.

**Howin ratkaisu siihen**:

- **Otsikolla 100 % -ilmaisia palveluntarjoajia[Taustaväri]** — Eroon
  käyttööntulo: iFlow (5 ilman rajoituksia käyttövoimalla: kimi-k2-ajattelu,
  qwen3-ohjaaja, deepseek-r1, minimax -2, kimi-k2), Qwen (4 ilman rajoituksia
  käyttövoimalla: qwen3 -ohjaaja, qwen3 -ohjaaja- Flash, qwen3-ohjaaja seuraava,
  visio-malli), Kiro (Claude + AWS Rakettomalli käyttöö
- **Ollama Pilvi** — Pilvestä Ollama-malleja käyttävällä `api.ollama.com`
  alueella
- **Suositeltu Kombinaatiot[Taustaväri]** — Kokeilee `GC/Gemini-3- Flash →
  IF/kimi -k2 -pilveä → qwen / qwen3 -ohjaaja- Pilvi` = 0 € kuukausina
- **NVIDIA Nimilta Ilmaiset Käyttöoikeudet ** — ~ 40 RPM -ilmaiset käyttöoikeut
  pääsy käyttööntulo 70+: mallit ** build.nvidia.com (pääsyn siirtymän
  tarkoituksena on vaihtuminen tekemisestä täysin rajoituksilla
- **Kustannustehoste-strategia** — Routti-strategia, joka automaattisesti
  valitsee halvin saatavissa olevan toimittelijoita

</details>

<details>
<summary><b>🔒 5. "I need to protect my AI gateway from unauthorized access"</b></summary>

Kun AI-verkon kuluttaja yhdistetään verkkoon (LAN, VPS tai Docker), jolla on
osoite, niin jokainen kyseisessä verkkoon liittynyt pääsee käyttämään kehittäjän
tokenia/etuudetta ilman suojausta. Ilman suojausta toimijat ovat tervetulleita
väärinkäyttöön, aiheuttamaan kysymysinjektioita ja ablooiheen.

**Howin ratkaisu siihen**:

- **API Avaimen hallinta** — Luo, keksit, kohti yksityiskohtaisten toimittajien
  avaimen sivustolla\
  ` dashboard/api-manager`
- **Mallitason oikeudet** — Riistä API-avaimia tiettyjen malleihin (`openai/*` ,
  wildcard malleja, yksipuolinen kaukosyötteen sijainti), kiertäminen
  kaikkimmaisella/riistäminen sijainti, niin ja niin
- **API Pääsyn suojaus** — Vaadi avainta `/v1/models` ja estä erityisesti ne
  Pääsyn listoilu
- **Kirjaudu ja CSRF-suojaus** — Kaikki Kirjaudu -yhteys ja kielletty pääsyn
  kautta `withAuth` yhdistelemällä + CSRF -tokenni
- **Ilmoituskynnys Määritelmä** — Ilmoituskäyttäyteen käyttäminen suojana, kun
  tarvitaan oleskivat toimittajat
- **IP-suojelu** — Oikeellisuus, tontille katsomisen olemassa oltuaan
- **Kysymysinjektioon suojaus** — Sanitosarjoon käyttämin aikana tullut malaiset
  Kysymysinjektio
- **AES-256-GCM -salausalgoritmi** — Tiedonsiirto salattuun

</details>

<details>
<summary><b>🛑 6. "My provider went down and I lost my coding flow"</b></summary>

AI toimittajista tulee epäsäännöllisiä ja palauttavat tulos, jotka ovat saaneet
virheellisempaa kunnossapitokirjoja. Olisi yksinosuudellinen toimija, näin tulee
tarpeeksi aikas, jotta sovinnostus tarvitaan muuttaa sivuja,

**Howin ratkaisu siihen**:

- **Sivutapahtumanesto malleja** — Automaattinen sulkeutuminen/Avaja
  sulkeutuminen yksikköä/estonsa rajojen sisältä läpikäytyessä, kerrannan
  tavoitus rajoilla ja laajenemista
- **Jyrähtävän keraamon hallinta** — Etenevä yksikköhyyttely
- **Älyä hajalle ja sammutettu** — Myöskään myllyäänsä ja sammuttaman ja
  käytäntöä
- **Heviketjuihin sivuketjuihin** — Jos eteenpäinkulu on muuttunut niin, niin
  myös ketjuketju on automaattisesti tuliin käykynnellä
- **Kombimurmuvirta** — Muuttunut etenkin toimija käynnistetään
- **Toki-ilmoitumismäärittely määrä** — Tuki-määritellyn palvelimien ylemmän
  taitolähteen tietojen lukuliikintä ja toiminta ja mahdollinen poistaminen
  tulevissa seuraavissa

</details>

<details>
<summary><b>🔧 7. "Configuring each AI tool is tedious and repetitive"</b></summary>

Kehittäjät ovat käyttäneet Cursoria, Claudia Koodia, Koodikomentoja (CLI),
OpenClawia, Claudiakomentoja(KLI), Kilo Kodia, Jatkuvien katsastuneiden
koetuksilla (CI). Joka kerralla, kehitysvaiheessa ja sovinnossuhteessa
marrastavat vastustaneet samma ja toteamattomat tarpeet on tarvittavissa
käyttämiseen niitä ja muuttavat yksikölle osoituksen tarvikkeita \
==WEBLATE_PART==

**Howin ratkaisu siihen**:

- **CLI Tarvikkeiden Pääsivu** — Kybertuoli sivu yhden napsautuksen
  asettamiselle Claude Code, Codex CLI, OpenClaw, Kilo Code, Antigravity ja
  Cline
- **GitHub Copilot Asetusgeneraattori** — Sisältää `chatiLanguage Models (JSON)`
  koodiin VS codelle massimallien valinnasta
- **Oppaan Käyttöohje** — Kulkien 4-askea asetusohjeet ensimmäisille käyttäjille
- **Yksi pääte, kaikki mallit** — Konfiguroida `http://localhost:20128/v1`
  kerran, ja pääsyyssä 67+ toimittajia

</details>

<details>
<summary><b>🔑 8. "Managing OAuth tokens from multiple providers is hell"</b></summary>

Claude Code, Codex, Gemini CLI, Copilot - kaikki käyttävät OAuth 2.0
käyttöoikeuden hylkäämisen jälkeisinä tokeneja. Ohjelmistoalueiden tekijöille on
erityisen hankala seurata yhtenäisesti OAuth käytön ja luonnollisen tokenin
kadon korvaus.

**Howin ratkaisu siihen**:

- **Automaattinen Token Muistiinpano** — Käytä OAuth tokenia jatkosuorituksen
  ennen hylkäysmäärää
- **OAuth 2.0 (PKCE) Sisäinen** — Automaattinen reititys Claude Code, Codex,
  Gemini CLI, Copilot, Kiro, Qwen ja iFlow
- **Useita OAuth-Kasikirjaa** — Useita reittejä per tunnus OIDT /
  EXraction-token
- **OAuth LAN / Pieni Ossi** — Viranomaisten yksityisten IP-osoitteiden
  detektoinnissa + automaattinen URL-muodostus jäädytetyssä palvelimessa
- **OAuth Nginxin Perässä** — Käyttää `window.location.origin` alueen käännös
  yhteensopimista
- **Pieni OAuth-Opas Suurinta** — Eritteliopas sijoitus Google- pakan VPS ja
  Dockerille

</details>

<details>
<summary><b>📊 9. "I don't know how much I'm spending or where"</b></summary>

Ohjelmistokehittäjät käyttää useita maksullisia toimittajia, mutta heillä ei ole
laskuja, näiden tietyn ja eteenpäin jatkuvasti pientä tietyn kulloisen tappiot
he saavat ja korjata

**Howin ratkaisu siihen**:

- **Kustannusanalytiikka Pääsivu** — Per-token-kustannusmäärittelyn seuranta
  budjettihallinnon tärkiä ja kunkia tukija
- **Budjettirajoitus Nivel** — Ongelmia mukana jaksen seuranta budjettihallinnon
  tapauksessa
- **Mallihintajassa Palkki Xh X33X] — Hinnat ja käyttömuodostus malleineen
- **Statistiikka Eri API-Löyöntien Käänäys** — Käyttäminen määrä ja viimeksi
  käytetty aika API Avion
- **Analytiikka-Pallo** — Tunnusluokat, malli käytöön kuvat, toimittaja kertas
  ja käynnistän suoritusmäärin laskimo sekä suoritusnopeus

</details>

<details>
<summary><b>🐛 10. "I can't diagnose errors and problems in AI calls"</b></summary>

When a call fails, the dev doesn't know if it was a rate limit, expired token,
wrong format, or provider error. Fragmented logs across different terminals.
Without observability, debugging is trial-and-error.

**Howin ratkaisu siihen**:

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

**Howin ratkaisu siihen**:

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

**Howin ratkaisu siihen**:

- **Hallinnonkäyttöpaneeli i18n — 30 kieltä** — Kaikki 500+ avaimen käännökset,
  mukaan lukien arabia, bulgaria, tanska, saksa, espanja, suomi, ranska, heprea,
  hindi, unkarilainen, indonesia, italia, japanilainen, korealainen, malaiji,
  hollanti, norja, puola, portugali (PT/BR), romanialainen, venäjä, slovakki,
  ruotsi, thain, ukraina, vietnam, kiina, filippiini, englanti
- **RTL-tuke** — Oikeanreunaista tukea arabiaa ja hepreaa varten
- **Monikieliset luetelmat** — 30 täysin käännetyt asiakirjavertailut
- **Kielivalikko** — Globi-pallo päätehtävän kuten suoritusaikaisia vaihtoehtoja

</details>

<details>
<summary><b>🔄 13. "I need more than chat — I need embeddings, images, audio"</b></summary>

Tietokoneoperaattorit tarvitsevat lisäksi aiheiden kuvauksen, ääninkäsittelyn,
RAG:läkäistyksen, asiakirjojen uudelleenjärjestämisen, yksityiskohtien
tarkistuksen ym. toimenpidea joista kukin käyttää vaikka eri APIa.

**Howin ratkaisu siihen**:

- **Polttoainefyysiot** — `/v1/polttoainefyysiot` 6 tarjoajan ja 9 + malleilla
- **Kuvien luoaminen** — `/v1/kuvien luomistilaisuuksia` 10 tarjoajan ja 20 +
  malleilla (OpenAI, xAI, Yhdessä, Kulkutartunta, Nebius, Hyperboliinen,
  NanoBanana, Antigraviteetti, SD WebUI, ComfyUI)
- **Tekstin kuvaamis** — `/v1/tekstin kuvailutilaisuuksia` — ComfyUI
  (AnimoidaFarkkua, SVD) ja SD WebUI
- **Tekstin sointimielessä** — `/v1/tekstin sointimielillä` — ComfyUI (Stabiili
  äänieristyksen avaaminen, musiikin synnyttäminen)
- **Äänikappaleen tulkinta** — `/v1/ääniä kappaleen tulkinnassa` — Whisper +
  Nvidia NIM, HuggingFace, Qwen3
- **Tekstikutsujen kutsukirja** — `/v1/ääniä puhukäyttö` — ElevenLabs, Nvidia
  NIM, HuggingFace, Coqui, Tortoise, Qwen3, **In world**, **Cartesia**,
  **PlayHT**, + olemassa olevat tarjoajat
- **Yksityiskohtien tarkistus** — `/v1/yksityiskohtinen tarkistus` — Sisällön
  turvallisuustarkastus
- **Reranking** — `/v1/reranking` — Asiakirjojen järjestelytarkastus
- **Vastauksen API** — `/v1/vastaus` tuet tuki Codexille

</details>

<details>
<summary><b>🧪 14. "I have no way to test and compare quality across models"</b></summary>

Kehittäjät haluavat tietää, mikä malli on paras tapauksensa käsitellessä --
koodaaminen, käännös, järjestelmä – mutta vertaileminen käsin on aikaan vaatava.

**Howin ratkaisu siihen**:

- **LLM-käyttäytymisikäytön** — 10 tarjottua tapauksessa sijoittamisoimennen
  katselmaa käsiteltävä kutsu, matematiikka, maantieteellinen tiede, koodaus,
  JSON tunnustus, käännös, markdown, turvallisuus, kieltäytyminen
- **4 Kiertotie- Strategioita** — `tarkka`, `sisältää`, ` regex`, ` eri`
  (JavaScript -funktio)
- **Käännetyn Tekstitestiä** – Monesta sisällöstä, odotetuilla tuloksilla &
  yhteistä verronnutaa
- **Keskustelu Testiluokka** — Kokoavoin retkiprosessi visuaalisen palautteen
  kanssa
- **Yksikkövalvonta** — Uudenaikaisin reaaliaikainen virta kaikkia pyyntöjä
  kulkien proxyssa

</details>

<details>
<summary><b>📈 15. "I need to scale without losing performance"</b></summary>

Kun pyyntömäärä kasvaa, pyynnön samanlaisuudesta aiheutuu samaa kysymystä
koskevia toistuvia kustannuksia ilman tallennusta. Ilman idempotenssia, samat
pyynnöt kuluttavat tilaa ja välttämättä menevät syrjään rajatilanteen vuoksi.

**Howin ratkaisu siihen**:

- **Semanttinen Tallennus** — Kaksi-tason tallennus (signaatti + semantiikka)
  pienentää kustannuksia ja viiveitä
- **Pyyntö Idempotenssi** — 5 s dekomponeerintiakseli samanarvoisille pyynnöille
- **Virta Rajoituspvm** — Tähän välilehteen RPM-harjoituksen, alempien
  vähimmäisjaksojen sekä kohtapistemäisten pääsykohtien palkkasäiliön edustajat
- **Muokattava rajoituspvm** — Asetuksen konfiguroidut oletukset Järjestäys →
  Keveys pitkäkestoisessa toistossa
- **API-tunnukseen valvontatallennus** — 3-teräinen tallennuksen tukeva
  tuotantokokemus
- **Salasanaohjelma Telemetri** — p50/p95/p99 hidastuminen, tallennustatistikat,
  ylin etäisyys

</details>

<details>
<summary><b>🤖 16. "I want to control model behavior globally"</b></summary>

Ohjelmoijat halusivat saada käännöset tiedoksi suomenkielisenä erityispyynnössä,
tietyllä yleisperiiöllä (esi- tai valintaperusteilla) tai rajaa siihen tarpeen
mukaan. Tässä olisi myös toinen erityinen edellytys, mutta kautta kaikki tällä
ongelmanratkaisuna.

**Howin ratkaisu siihen**:

- **Järjestelmä Prompt Injection** — Kokoja prompt määritykset kohtuuhin pääsyyn
  avaimen kanssa kaikille sähköoperaatiolle
- **Päätöksenteon lisätyö ** — Syynsä alkuperän muuntimien määrtykset ja
  määrätty määräytyminen sopeuttaen tarpeet
- **6 sijaintiohjelmoinnin strategioiden suuntaliuku** — Global-strategiat
  johtavat pyynnöt jokavuotisesti tasavirtaisemmissa pääsyssä
- **Vapaamuotoinen laskuri** — Vapausesima oletukset, kohdistamattomat oletukset
- **Paikka avata-paikka sulkea** — Suora kynnysliukki kaikkia pääsyssä
- **Toiminnon Poissulkeminen** — Klikkaa yksittäinen, automaattisesti
  tarkistetaan ja poistua kaikista pääsyssä
- **Kiinni osapuolet** — Hylkää oletusarvoista poistua vylle vakiointi käytössä
  / v1 / mallit`

</details>

<details>
<summary><b>🧰 17. "I need MCP tools as first-class product capabilities"</b></summary>

Monet AI- portaat kytkee jo ainoa MCP ilmiön sivuotteena. Tietoryhmät
tarvitsevat visuaalisen hallintatason.

**Howin ratkaisu siihen**:

- MCP näkyy päävalikossa navigaatiomenuissa ja endpoint-protokollasivulla
- Sekä konsolin kautta, että endpoint-protokollasivulla kohdeMCP:n käyttöönotto
  on ohjettu valmisasettelu
- Kliendille on saatavilla asiakkaan kautta MCP:n konsolin käyttöönotto ja
  katsastus

</details>

<details>
<summary><b>🧠 18. "I need A2A orchestration with sync + stream task paths"</b></summary>

ASE-työvaiheiden liittyy sekä suorat vastaukset että käynnissä olevien tehtävien
seuraaminen ja ohjaaminen

**Howin ratkaisu siihen**:

- V2B JSON-RPC endpoint (`POST /a2a`) viestin lähettämisessä ja seuraamisessa
- SSE-streaming ja terminaalivaiheen propagoiminen
- Palvelunkutsujen elinkaaren API:et `tasks/get` ja `tasks/cancel`

</details>

<details>
<summary><b>🛰️ 19. "I need real MCP process health, not guessed status"</b></summary>

Toiminnalliset joukkoihin tulee tietää, onko konsoli elossa vai vain onko API
saavutettavissa

**Howin ratkaisu siihen**:

- Ytimeksinäinen sydänasema tiedosto, joka sisältää PID, aikamerkit, sekä
  työnkulku.
- MCP:n tila API yhdistää sydänasema + sitten viimeinen toiminta
- Käyttöliittymä asiakirjat tila yksikön elinkaaren etäisyyteen ja sydänaseman
  uusimisuuruus

</details>

<details>
<summary><b>📋 20. "I need auditable MCP tool execution"</b></summary>

Työkalut muuttavat konfiguraatioita tai aktivoiden toimintoja, on saada
johtoliikkeiden jälki

**Howin ratkaisu siihen**:

- SQLite-perusteinen katsastustiedosto konsolin työkalutapauksille.
- Suodatimia [X24X]tools/X45X], [X26X]success/X47X], [X27X]api_key/X48X] ja
  ikärajat.
- Katsastustaulukko ja automaatiotilastot

</details>

<details>
<summary><b>🔐 21. "I need scoped MCP permissions per integration"</b></summary>

Toimivaltaiset käyttäjät saavat vähimmästikin tarvittavan pääsyn
työkaluryhmöihin.

**Howin ratkaisu siihen**:

- 9 erityispiirteysmallin MCP-sopimusten hallitun työkaluydinkäytön tueksi
- MCP-sopimustyön tarkastuksen tuki sekä näkyvyys käyttöliittymässä
- Turvallinen oletusrakenne käyttöjärjestelmän toolingiin

</details>

<details>
<summary><b>⚙️ 22. "I need operational controls without redeploying"</b></summary>

Ryhmien tarvitse tarkalleen ajoitettuja runtime-muutoksia tapauksissa tai
kustannuserojen yhteydessä

**Howin ratkaisu siihen**:

- Komponentti-switchin aktivointi suoraan MCP-työpöydältä
- Muistijälkiyhdistys profiilit sovitettaviksi pre-asemioitiin politiikkoihin
- Circuitikirkkauden tilan palautus samasta toiminnosta palkkalautta

</details>

<details>
<summary><b>🔄 23. "I need live A2A task lifecycle visibility and cancellation"</b></summary>

Lisätty tuki elinkaarensä näkemyksellä, kun tehtävätila muuttuu on vaikeasti
selvittää

**Howin ratkaisu siihen**:

- Tehtäväluettelossa/filtrauksen kerrontaa tehtävän tilasta/taidoilta, jossa on
  sivuja
- Drill-kaavio tehtävän metadatosta/tapahtumista/todistetuista, jotka on
  avattavissa seuraavaksi
- Tehtävän perusrakenteet toimistopäätökseen tuoten kiitos

</details>

<details>
<summary><b>🌊 24. "I need active stream metrics for A2A load"</b></summary>

Toiminto peräkkäisiin työympäristän viestejä niittäytämme palveluineen

**Howin ratkaisu siihen**:

- Aktiivien viestien rekisteröinty kättyi sivupalkin yhteen kohdennusasetusten
- Viimeinen tehtävä ajoitettu muuttuneesta tilasta kuukaudet yhden muistaamisen
  ajoitusten.
- A2A-työpöydän kortit reaalisia liikennevaiheita varten joustoa muassa

</details>

<details>
<summary><b>🪪 25. "I need standard agent discovery for clients"</b></summary>

Pinnalliseen ilmoitusyhteydessä tarvitaan tietyn luotettavasti tiedon yhdistävä\
luonnostaan, erinomaisesti joustoa pitää.

**Howin ratkaisu siihen**:

- Agentkortti näytetään `/.well-known/agent.json`
- Kykyjä ja taitoja näytetään hallintointerfacessa
- A2A-tilastoidan API sisältää automaation löytämismetadatia

</details>

<details>
<summary><b>🧭 26. "I need protocol discoverability in the product UX"</b></summary>

Jos käyttäjiä ei käyttämiä ilmi protocol pintaasia on adoptiotas ja
tuettaslaatua laskee.

**Howin ratkaisu siihen**:

- Yhdenmukaistettu **Päätepisteet** sivu sivuilla kohtuihin Proxy, MCP, A2A, ja
  API Päätepisteet
- Inline palvelun asema napit (Online / Offline ) MCP ja A2A
- Selville vastaanottovät yksittäisiä hallintointerbän napeita

</details>

<details>
<summary><b>🧪 27. "I need end-to-end protocol validation with real clients"</b></summary>

Yksinkertaista mock-vikat tukee ohjelmisto kiinnostuksen ja asettaminen ei
pelkästään kelpaa tukeako sääntöä

**Howin ratkaisu siihen**:

- E2E-sarja ylataan ohjelmaa käyttää realei MCP SDK client transport
- A2A asiakas kokeet löytämis, lähettää, virtaus, haku, ja Peru koke
- Tarkista vastoinky yhdessä kohtaa MCP audit ja A2A kokeet APIs

</details>

<details>
<summary><b>📡 28. "I need unified observability across all interfaces"</b></summary>

Yhdistä suoritettavuus etsii protocol luottojako pisteet ja lisää tällä aikaa.\
==

**Howin ratkaisu siihen**:

- Yhdenmukaistettu panelit tiedot /analyzissä
- Samaan tuotteeseen tarkkaavat kausityöntekijöitten ja tuottavuutena A2A
  audittia ja kokeet yleisissän sarajamista
- Käyttötilastot + audit + pyyntotiedostus avoimena A2A- ja MCP kerroksina

</details>

<details>
<summary><b>💼 29. "I need one runtime for proxy + tools + agent orchestration"</b></summary>

Tilaussopimusten API tilastot ja ilmoittavat yleiset \
!=WEBLATE_PART\
Monipohjainen palvelu lisää ilmoittaja kustannus ja ehdot \
==WEBLATE_PART==

**Howin ratkaisu siihen**:

- Yhteensäkkä OpenAI-ylellinen välittäjä, MCP-palvelin ja A2A-palvelin yhdessä
  pilverkossa
- Yhteinen kirjautuminen, kestävyys, tietotallennus ja havaintokyky
- Sekä käyttöympäristöjen sekä palvelujen yhäisen poliisi malli

</details>

<details>
<summary><b>🚀 30. "I need to ship agentic workflows without glue-code sprawl"</b></summary>

Ryhmät menettävät nopeutta, kun heidän on käännetty yhdenmukaisten, erilaisia
palveluja ja kirjoituksia.

**Howin ratkaisu siihen**:

- Yhden käyttöpäivityksen strategia yhdisti asiakkaiden ja agenttien
- Sisäänrakennetuista, käyttäjän keskittämien yhteensäkkäisiä protokollan
  hallinta näkymä ja savu tarkistukset
- Tuotantomäärät yhdyttämät perusteet (turvallisuus, tietojen kirjaaminen,
  kestävyys, tietosäilönäyttäminen)

</details>

### Esimerkkipeli (yhteen soveltaminen)

**Peli ABC: maximoida maksuttoman tilauksen + halvin vakuutus[X123X]

```txt
Combo: "maximoi-klausuli"
  1. cc/klausuli-opus-4-6
  2. glm/glm-4.7-esi
  3. if/kimi-k2-Piilotuksen

Kuukausikuluutusmaksu: 20 dollaria + pieni vakuutuksen kulu
Tulos: laadukas, lähellä-tiukka pysäyttäminen
```

**Peli B: Ilmainen luonnolliseen kirjoittamista asetta[X55X]

```txt
Combo: "vapaata aikaa"
  1. gc/vahtia-3-Flash
  2. if/kimi-k2-Piilotuksen
  3. qw/qwen3-koodarin Plus-pakkaus

Kuukausikuluutus: 0 dollaria
Tulos: stabiili vapaakodin käyttö
```

**Peli C: Kaikk'päiväiseen aina-olevassa -jäsenhän

```txt
Combo: "aina-olevassa"
  1. cc/klausuli-opus-4-6
  2. cx/gpt-5.2-kodex
  3. glm/glm-4.7-esi
  4. minimuksella/MiniMax-M2.1 
  5. if/kimi-k2-Piilotuksen

Säilytys: pakanut syvyys toteutus loma-tiukka tärkeiden kuukautiskuluutuksissa työtä
```

**Peli D: Agentin operoinnin yhdistää MCP + A2A/X25X

```txt
1) Alkamiseen MCP liiketoimintoille (`omniroute – mcp [X48X]) tilauksen kulkusuunnitelman hengen
2) Suorittaa A2A tehtävät `viesti/lähetä[X111X] ja `Viesti/onnistunut[X127X]
3) Nähdä oikeistolaidalla / dashboard/ endpoint (MCP ja A2A palkit)
4) Talttumalla ja muuttamistaan palvelut inline tarkastusvalikoissa riittää
```

---

## Käynnistä vapaata – Nolla määräpaikkaa

> Asenna koodin tietokoneen minuuteista palkkaa ** 0 dollaria kuukautta
> kulu[X42X], Sovela yhteen vapaat tilit ja käytä sisäisesti rakennettua
> **Vapaakoodi [X109X] vapaakoodin yhteneäksi.\
> ==WEBLATE_PART==

| Askele | Toiminta                                            | Tarjoajat Avoinna                                                   |
| ------ | --------------------------------------------------- | ------------------------------------------------------------------- |
| 1      | Yhdistä **Kiro** (AWS Builder ID OAuth)             | Claude Sonnet 4.5, Haiku 4.5 - **rajattomia**                       |
| 2      | Yhdistä **iFlow** (Google OAuth)                    | kimi-k2-thinking, qwen3-coder-plus, deepseek-r1... - **rajattomia** |
| 3      | Yhdistä **Qwen** (Device Code)                      | qwen3-coder-plus, qwen3-coder-flash... - **rajattomia**             |
| 4      | Yhdistä **Gemini CLI** (Google OAuth)               | gemini-3-flash, gemini-2.5-pro - **150.000 €/kuu ilmainen**         |
| 5      | `/dashboard/combos` → **Ilmainen Stack (0€)** malli | Yhdistä kaikki ilmainen palvelimet automaattisesti                  |

**Ohjelmoi minkä tahansa **IDE/CLI `: `http://localhost:20128/v1` ·
API-avain: `milloin tahansa ` · Valmis.

> **Valinnainen lisäkattaus (ilmainen kuten aikaisemmin): ** Groq API-avain (30
> RPM ilmaineet), NVIDIA NIM (40 RPM ilmaineet, 70+ mallit), Cerebras (1M
> tok/day), LongCat API avain (50M tokens/päivä!), Cloudflare Workers AI (10K
> Neuron/päivä, 50+ mallit).

## Pika-aloitus

### 1. Asenna ja suorita

```bash
npm install -g omniroute
omniroute
```

> **pnpm käyttäjät:** Suorita `pnpm hyväksy-asennukset -g` asennuksen jälkeen
> voit toimittaa natiivit rakennusskriptit pakettien `paras-sqlite3` ja
> `@swc/ytimen`:
> 
> ```bash
> pnpm asenna -g omniroute
> pnpm hyväksy-asennukset -g   # Valitse kaikki paketit → hyväksy
> omniroute
> ```

Dahsboard avautuu osoitteessa `http://localhost:20128` ja API-perustiedot
osoitteessa `http://localhost:20128/v1`.

| Komennos                | Kuvaus                                                                    |
| ----------------------- | ------------------------------------------------------------------------- |
| `omniroute`             | Käynnistä palvelin (`PÄÄSYRIKKO=20128`, API ja dashboard samaan porttiin) |
| `omniroute --port 3000` | Aseta kanonisen/API-portin 3000                                           |
| `omniroute --mcp`       | Käynnistä MCP-palvelin (stdio kuljettaja)                                 |
| `omniroute --ei-avautu` | Ei avaa automaattisesti selaimea                                          |
| `omnirute --apua`       | Näytä apu                                                                 |

Valinnainen erillississistystila:

```bash
PORT=20128 DASHBOARD_PORT=20129 omniroute
# API:       http://localhost:20128/v1
# Dashboard: http://localhost:20129
```

### 2) Lisää tarjoajia ja luonnollinen API-avain

1. Avaa Dashboard → `Tarjoajat` ja liitä vähintään yksi tarjoaja (OAuth tai
   API-avain).
2. Avaa Dashbboard → `Päätteet` ja luo API-avain.
3. (Valinnainen) Avaa Dashbroad → `Lohkoketjut` ja aseta kysi varausketju.

### 3) Osoita koodaamistooli Omiroutelle

```txt
Perustoisti: http://localhost:20128/v1
API-avain:  [Laita päätteessä kopioitu avain]
Malli:    if/kimi-k2-toiminta (tai mikä tahansa tarjoaja/malli -alakohta)
```

Tuo tukijoineen Clauden koodi, Codex CLIl, Gemini CLIl, Cursor, Cline, OpenClaw,
OpenCode ja OpenAI-keskinäisten SDK.

### 4) Aktivoi ja vahvista protokollat (v2.0)

****MCP (työvälinekäytössä):**

```bash
omniroute --mcp
```

Sitten yhdistä MCP-palvelimenne työskentelyä `standardeille` ja harjoita
työkaluja kuten:

- `omniroute_get_tilat`
- `omniroute_list_lohkoketjut`

**A2A (agent-tekojen väliliikenteen):**\
==

```bash
curl http://localhost:20128/.well-known/agent.json
```

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"nopeasti aloita", "metodi": "viesti/lähetä", "parametrit": {"taito": "kuitaushallinta", "viestit": [{"rooli": "käyttäjä", "sisältö": "Anna minulle lyhyt kuitausalue."}]}}'
```

### 5) Vahvista kaikki alusta alta (suositeltava)

```bash
npm run test:protokollit:e2e
```

Tämän luokan tarkistus vahvistaa oikeasti MCP ja A2A-asiakasmuistit kaikkia
käytännössä käyttöliittymän toiminnoista vastaan.

### Vaihtoehto: Käytä lähdettä suoraan.

```bash
cp .env-esimerkki .env
npm install
PORT=20128 DASHBOARD_PORT=20129 NEXT_PUBLIC_BASE_URL=http://localhost:20129 npm run dev
```

---

## 🐳 Docker

OmniRoute on saatavilla julkaisuna Docker-kaapelitekijän [Docker
Hub](https://hub.docker.com/r/diegosouzapw/omniroute)-sivustolla.

**Nopea käyttöönotto:**

```bash
docker run -d \
  --name omniroute \
  --restart unless-stopped \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:viimeisin
```

**Ympäristö-asetustiedoston käytössä:**

```bash
# Kopioi ja muokkaa .env ensin
cp .env-esimerkki .env

docker run -d \
  --name omniroute \
  --restart unless-stopped \
  --env-file .env \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:viimeisin
```

**Docker Compose-asetusten käytössä:**

```bash
# Perusprofiili (ei CLI-työkaluja)
docker compose --profile perus up -d

# CLI-profiili (Claude Code, Codex, OpenClaw sisäänrakennettu)
docker compose --profile cli up -d
```

| Kuva                     | Laji        | Koko   | Kuvaus                            |
| ------------------------ | ----------- | ------ | --------------------------------- |
| `diegosouzapw/omniroute` | `viimeisin` | ~250MB | Viimeisin vakaa julkaissut versio |
| `diegosouzapw/omniroute` | `1.0.3`     | ~250MB | Nykyinen versio                   |

---

## 🖥️ Pöytätietokone - Offline ja aina käytössä

> 🆕 **UUSI!** OmniRoute on nyt saatavilla **omalle pääteikäisille
> sovelluksille** Windows, macOS, ja Linux -ympäristöille.

Suorita OmniRoute -sovellus omalla pääteikäisellä sovelluksena — ei terminaan,
ei selaimessa, eikä verkkoon tarvita paikallisiin mallien ladataakseen.
Electron-perustuvassa sovelluksessa on mukana:

- 🖥️ **Ominainen ikkuna** — Omalle sovellukselle omistettu sovellusikkuna
  järjestelmän valikossa tarjolla oleva integrointi
- 🔄 **Autosta käynnistys** — Lähetä OmniRoute käynnistettäväksi järjestelmän
  näppäimistösaatavuuden mukaan
- 🔔 **Ominaiset ilmoitukset** — Saada varoituksia rajaton käytön esteestä tai
  toimittajan ongelmista
- ⚡ **Yksinkertainen asennus** — NSIS (Windows), DMG (macOS), AppImage (Linux)
- 🌐 **Erikoismoodi** — Toiminneeksi riittää paikallinen palvelin

### Pika-aloitus

```bash
# Kehitysmoodi
npm run electron:dev

# Koko ensimmäiste tuotteen muotoa
npm run electron:build       # Oletettu alusta
npm run electron:build:win   # Windows (tyyppi .exe)
npm run electron:build:mac   # macOS (tyyppi .dmg) — x64 &amp; arm64
npm run electron:build:linux # Linux (tyyppi .AppImage)
```

### Järjestelmän valikko

Kun sovellus on pienennetty, jätetään sovellus ikkunalta ja sen sijaan
järjestelmän valikolle, jonne on kaksikin nopeita toimintoja

- Avaa Dashboard
- Muuta palvelinporttia
- Lopeta sovellus

📖 Kokonaisen asiakirjan, josta löydä lisä tietoa:
[`electron/README.md`](electron/README.md)

---

## 💰 Käytilössä tätä näkevät

| Taso                 | Palveluntarjoaja                | Hinta                                 | Rajoitus resetointi                       | Paras                                 |
| -------------------- | ------------------------------- | ------------------------------------- | ----------------------------------------- | ------------------------------------- |
| **💳tilaus**          | Claude Kohde (Pro)              | 20 dollaria/mkk                       | 5h + viikoittainen                        | Milloin jo tilausta on omistanut      |
|                      | Codex (Plus/Pro)                | 20-200 dollaria/mkk                   | 5h + viikoittainen                        | OpenAI-käyttäjät                      |
|                      | Gemini CLI                      | **ILMAINEN**                          | 180000 dollaria/mkk + 1000 dollaria/päivä | Kaikille!                             |
|                      | GitHub Copilot                  | 10-19 dollaria/mkk                    | Kuukausittain                             | GitHub-käyttäjät                      |
| **🔑 AVATUSSANAKESI** | NVIDIA NIM                      | **ILMAINEN** (kehittäjäksi ikuisesti) | ~40 kierrosta/minuutissa                  | 70+ avoimessa mallissa                |
|                      | Cerebras                        | **ILMA** (1M sananpala/päivä)         | 60 000 TPM / 30 kierrosta/minuutissa      | Maailman nopein                       |
|                      | Groq                            | **ILMA** (30 kierrosta/minuutissa)    | 14 400 RPD                                | Ultra-nopea Llama/Gemma               |
|                      | DeepSeek V3.2                   | 0,27 $/1,10 dollaria 1M:sta           | Ei mitään                                 | Paras hinnanlaatu - syistejä          |
|                      | xAI Grok-4 Nopea                | **0,20$/$0,50 dollaria 1M:stä** 🆕     | Ei mitään                                 | Nopein + työkalun kutsu, ultramatala  |
|                      | xAI Grok-4 (standard)           | 0,20$/$1,50 dollaria 1M:stä 🆕         | Ei mitään                                 | xAI:n perusrakenne                    |
|                      | Mistral                         | Ilmainen kokeilu + maksullinen        | Hinta rajoitettu                          | Euroopan AI                           |
|                      | OpenRouter                      | Hae peruste                           | Ei mitään                                 | 100+ mallin kokoelma                  |
| ** 💰 Halvalla**      | GLM-5 (kautta Z.AI) 🆕           | 0,5 euroa/1 miljoonaa                 | Päivä 10                                  | 128K tulos, uusin merkillinen         |
|                      | GLM-4.7                         | 0,6 euroa/1 miljoonaa                 | Päivä 10                                  | Budget-tuet                           |
|                      | MiniMax M2.5 🆕                  | 0,3 euroa/1 miljoonaan sisääntulo     | Viisituntinen roikkaus                    | Päättely + agenteidenvyöt tehokkaasti |
|                      | MiniMax M2.1                    | $0,20/1M                              | Viisituntinen roikkaus                    | Halvin vaihtoehto                     |
|                      | Kimi K2.5 (Moonshot API) 🆕      | Hae peruste                           | Ei mitään                                 | Suoran Moonshot API -yhteys           |
|                      | Kimi K2                         | $9/muuatila flat                      | 10 miljoonaa tuntia/kk                    | Luotettava kulut                      |
| **🆓 ILMAINEN**       | iFlow                           | **$0**                                | Rajojoton                                 | 5 mallia rajatön määrä                |
|                      | Qwen                            | **$0**                                | Rajojoton                                 | 4 mallia rajatön määrä                |
|                      | Kiro                            | **$0**                                | Rajojoton                                 | Claude Sonnet/Haiku (AWS Builder)     |
|                      | LongCat Flash-Lite 🆕            | **$0** (50M tok/day 🔥)                | 1 RPS                                     | Suurin ilmainen erän maanpäällä       |
|                      | Uudet yhdistämiskäännökset AI 🆕 | **$0** (ei avainta tarvita)           | 1 pyyntö/15s                              | GPT-5, Claude, DeepSeek, Llama 4      |
|                      | Cloudflare Workers AI 🆕         | **$0** (10K Neuria päivässä)          | ~150 vastausta /päivä                     | 50+ malliä, globaalit reunat          |
|                      | Scaleway AI 🆕                   | **$0** (1M kokonaistä ei merkintää)   | Hinta rajoitettu                          | EU/GDPR, Qwen3 235B, Llama 70B        |

> 🆕 **Uudet mallit lisätty (Maaliskuu 2026):** Grok-4 Fast perheen $0,20/$0,50/M
> (mallinnettu 1143ms — 30% nopeampi kuin Gemini 2,5 Flash), GLM-5 via Z.AI 128K
> tulosteen kanssa, MiniMax M2,5 syyllisyys, DeepSeek V3,2 päivittyneet hinnat,
> Kimi K2,5 Moonshot suora API kautta.

**💡 $0 Combo Pino — Kanssa Ei Merkin Espanjahankinta:**

```
# 🔓 Ultimate Ilmainen Stack 2026 - 11 edustajia, $0 Ei Päätä
Kiro (kr/)             →  Claude Sonnet/Haiku UNLIMITED
iFlow (if/)            →  kimi-k2-ajatus, qwen3-koodari-plus, deepseek-r1 UNLIMITED
LongCat Lite (lc/)     →  LongCat-Flash-Lite — 50M merkintää päivässä 🔥
Pollinations (pol/)    →  GPT-5, Claude, DeepSeek, Llama 4 - ei avainta tarvita
Qwen (qw/)             →  qwen3-koodari-plus, qwen3-koodari-vikka, qwen3-koodari-seuraava UNLIMITED
Gemini (gemini/)       →  Gemini 2,5 Flash — 1 500 pyyntöä / vapaa API avain
Cloudflare AI (cf/)    →  Llama 70B, Gemma 3, Mistral — 10K Neuria päivässä
Scaleway (scw/)        →  Qwen3 235B, Llama 70B — 1M ilmaista ei merkintää (EU)
Groq (groq/)           →  Llama/Gemma ultra-nopea — 14,4K pyyntöä päivässä
NVIDIA NIM (nvidia/)   →  70+ avaamattomat mallit — 40 RPM jatkuu iän ikänsä
Cerebras (cerebras/)   →  Llama/Qwen maailman-nopein — 1M tok päivässä
```

**Kustannukset nolla. Ei lopata koskaan koodaamasta.** Konfignumista tämä
yhdistämispalvelu ja kaikki kääntymiset tapahtuvat automaattisesti - ei koskaan
manuaalista vaihtamista.

---

---

## 🔓 Ilmaiset mallit — Mitä Sinulla Oikeasti On

> Kuvaus alaosaa alhaalla on **100% ilmainen, ei kenenkään luettelossa**.
> Yhdistämispalvelu ohjauttaa automaattisesti niin, että sen ei tarvitse olla
> ollenkaan niitä ilmainen mallin avainta. Olette siis vapaana valita
> lopputulost.

### 🔵 CLAUDE MALLIT (Kiro - AWS Rakentajan ID)

| Malli                  | Etuliite | Raja                             | Käyttöraja                               |
| ---------------------- | -------- | -------------------------------- | ---------------------------------------- |
| `Claudin sonettia 4.5` | `kr/`    | [Tiedolle0T]Rajoittamaton[T139T] | Ei ole keskimäistä päivittäistä rajausta |
| `Claudin haikku 4.5`   | `kr/`    | [Tiedolle0T]Rajoittamaton[T139T] | Ei ole keskimäistä päivittäistä rajausta |
| `Claudinopusi 4.6`     | `kr/`    | [Tiedolle0T]Rajoittamaton[T139T] | Viimeisimmän Opusin kautta Kiron         |

### 🟢 IFLOW -MALLIT (Maksuton OAuth - ei tarvitse korttia)

| Malli                                 | Etuliite | Raja                             | Käyttöraja         |
| ------------------------------------- | -------- | -------------------------------- | ------------------ |
| `Kimi - k2- ajattelu`                 | ` IFF/`  | [Tiedolle0T]Rajoittamaton[T139T] | Ei raportoitu raja |
| [Tiedolle0T]qwen3-koodari-plus[T197T] | ` IFF/`  | [Tiedolle0T]Rajoittamaton[T139T] | Ei raportoitu raja |
| [Tiedolle0T]deepryhmä-r1[T128T]       | ` IFF/`  | [Tiedolle0T]Rajoittamaton[T139T] | Ei raportoitu raja |
| [Tiedolle0T]minimiaks-M2.1[T138T]     | ` IFF/`  | [Tiedolle0T]Rajoittamaton[T139T] | Ei raportoitu raja |
| [Tiedolle0T]kimi-k2[T12T]             | ` IFF/`  | [Tiedolle0T]Rajoittamaton[T139T] | Ei raportoitu raja |

### 🟡 QWEN MOEDIT (Laitekoodiarvio)

| Malli                                     | Etuliite              | Raja                             | Käyttöraja             |
| ----------------------------------------- | --------------------- | -------------------------------- | ---------------------- |
| [Tiedolle0T]qwen3-koodari-plus[T197T]     | [Tiedolle0T]qw/[T16T] | [Tiedolle0T]Rajoittamaton[T139T] | Ei raportoitu raja     |
| [Tiedolle0T]qwen3-koodari-pikkuuni[T198T] | [Tiedolle0T]qw/[T16T] | [Tiedolle0T]Rajoittamaton[T139T] | Ei raportoitu raja     |
| [Tiedolle0T]qwen3-koodari-seuraava[T197T] | [Tiedolle0T]qw/[T16T] | [Tiedolle0T]Rajoittamaton[T139T] | Ei raportoitu raja     |
| [Tiedolle0T]vision-malli[T135T]           | [Tiedolle0T]qw/[T16T] | [Tiedolle0T]Rajoittamaton[T139T] | Mukautuva kuvia kohden |

### 🟣 GEMINI CLI (Google OAuth)

| Malli                     | Etuliite | Raja                                        | Käyttöraja         |
| ------------------------- | -------- | ------------------------------------------- | ------------------ |
| `Gemini-3-akuuttilähetys` | `gc/`    | **180K marraskuu kuukauteen** + 1K päivässä | Kuukauden tasoitus |
| `Gemini-2.5-kuvaus`       | `gc/`    | 180K/myyntiä (yhteinen säiliö)              | Korkea laatu       |

### ⚫ NVIDIA NIM (Ilmainen API-avain — build.nvidia.com)

| Taso           | Päivittäinen raja | Käyttöraja  | Huomautuksia                                              |
| -------------- | ----------------- | ----------- | --------------------------------------------------------- |
| Ilmainen (Dev) | Ei token rajoitus | **~40 RPM** | 70+ mallia; siirtyminen puhdasta rajoitusta keskellä 2025 |

Suosittuja ilmaisia mallisia: `moonshotai/kimi-k2.5` (Kimi K2.5), `z-ai/glm4.7`
(GLM 4.7), `deepseek-ai/deepseek-v3.2` (DeepSeek V3.2),
`nvidia/llama-3.3-70b-instruct`, `deepseek/deepseek-r1`

### ⚪ CEREBRAS (Ilmainen API-avain — inference.cerebras.ai)

| Taso     | Päivittäinen raja     | Käyttöraja                           | Huomautuksia                                             |
| -------- | --------------------- | ------------------------------------ | -------------------------------------------------------- |
| Ilmainen | **1M tukiaika/päivä** | 60 000 TPM / 30 kierrosta/minuutissa | Maailman nopein LLM-tulkkaus; päivittäinen uusintaanomus |

Tarjolla ilmainen: `llama-3.3-70b`, `llama-3.1-8b`,
`deepseek-r1-pienennetty-llama-70b`

### 🔴 GROQ (Ilmainen API-avain — console.groq.com)

| Taso     | Päivittäinen raja | Käyttöraja                      | Huomautuksia                                         |
| -------- | ----------------- | ------------------------------- | ---------------------------------------------------- |
| Ilmainen | **14,4K RPD**     | 30 tuottokohtaa mallia päivässä | Ei luottokortteja; rajoitus 429, ei yhdistetä purkua |

Tarjolla ilmainen: `llama-3.3-70b-versatiili`, `gemma2-9b-it`, `mixtral-8x7b`,
`whisper-large-v3`

### 🔴 LONGCAT AI (Ilmainen API-avain — longcat.chat) 🆕

| Malli                                 | Etuliite | Ilmainen Päivittäinen Määrä | Huomautuksia                  |
| ------------------------------------- | -------- | --------------------------- | ----------------------------- |
| `Kauanpottasin-Flash-Lite`            | `lc/`    | **50 miljoonaa tokenia** 💥  | Suurin koskaan ilmainen määrä |
| `Kauanpottasin-Flash-Chat`            | `lc/`    | 500 tuhatta tokenia         | Monia käännöksiä              |
| `Kauanpottasin-Flash-Pohtimusta`      | `lc/`    | 500 tuhatta tokenia         | Päätöksenteko / CoT           |
| `Kauanpottasin-Flash-Pohtimusta-2601` | `lc/`    | 500 tuhatta tokenia         | Tammikuu 2026 version         |
| `Kauanpottasin-Flash-Omni-2603`       | `lc/`    | 500 tuhatta tokenia         | Monimediainen                 |

> 100% ilmaista, kun yhtiön tila on julkinen beta. Rekisteröidy osoitteella
> [longcat.chat](https://longcat.chat) sähköpostilla tai puhelimen avulla.
> Määrät nollataan joka päivä kello 00.00 UTC.

### 🟢 POLLINATIONS AI (API-avaimen vaatimaton) 🆕

| Malli        | Etuliite | Käyttöraja   | Laittaja Rahastaja |
| ------------ | -------- | ------------ | ------------------ |
| `avoimenaio` | `pol/`   | 1 pyyntö/15s | GPT-5              |
| `claude`     | `pol/`   | 1 pyyntö/15s | Anthropic Claude   |
| `geeni`      | `pol/`   | 1 pyyntö/15s | Google Geeni       |
| `syvänmetsä` | `pol/`   | 1 pyyntö/15s | Syvänmetsän V3     |
| `llama`      | `pol/`   | 1 pyyntö/15s | Meta Llama 4 Scout |
| `Mistrali`   | `pol/`   | 1 pyyntö/15s | Mistral AI         |

> ✨ **Nolla rikon **: Ei rekisteröitymistä, ei API-avainta. Lisää tämä
> Pollinations-palvelin tyhjällä avaimen kentällä ja se toimii välittömästi.

### 🟠 CLOUDFLARE WORKERS AI (Ilmainen API-avain — cloudflare.com) 🆕

| Taso     | Arkipäivän Neuronit | Vakiointi käyttämistä                            | Huomautuksia                       |
| -------- | ------------------- | ------------------------------------------------ | ---------------------------------- |
| Ilmainen | [10,000,X0X]**      | ≈ 150 LLM / 500 sekuntia ääntä / 15 000 sisältöä | Maailmanlaajuinen reuna, 50+ malli |

Suosittu maksuton malli: `@cf/meta/llama-3.3-70b-instruct`,
`@cf/google/gemma-3-12b-it`, `@cf/openai/whisper-large-v3-turbo` (vapaalla
äänenvoimakkuudella!), `@cf/qwen/qwen2.5-coder-15b-instruct`

> Tarvitsee API-tunnus + Tili-ID
> [dash.cloudflare.com](https://dash.cloudflare.com)-sivustolta. Tallenna
> Tili-ID asiakasedun.

### 🟣 SCALEWAY AI (1 miljoonan maksuton tunnukset — scaleway.com) 🆕

| Taso     | Maksuttomat annukset | Sijainti       | Huomautuksia                                 |
| -------- | -------------------- | -------------- | -------------------------------------------- |
| Ilmainen | [1M, X0X]tokeneja**  | 🇫🇷 Pariisi, EU | Kreditkorttia ei tarvita rajoitusten sisällä |

Käytettävissä ilman maksua: `qwen3-235b-a22b-instruct-2507` (Qwen3 235B!),
`llama-3.1-70b-instruct`, `mistral-small-3.2-24b-instruct-2506`,
`deepseek-v3-0324`

> EU/GDPR -yhteensopiva. Hae API-tunnus
> [console.scaleway.com](https://console.scaleway.com).

> **🔥 Ultimate maksuton Stack (11 tarjoajaa, 0 euroa ikuisesti):**
> 
> ```
> Kiro (kr/)             → Claude Sonnet/Haiku UNLIMITED
> iFlow (if/)            → kimi-k2-ajatus, qwen3-koodari, deepseek-r1 UNLIMITED
> LongCat Lite (lc/)     → LongCat-Flash-Lite — 50M tokenia päivässä
> Pollinations (pol/)     → GPT-5, Claude, DeepSeek, Llama 4 — ei salasanaa kaadettu
> Qwen (qw/)             → qwen3-koodari-mallit UNLIMITA
> Gemini (gemini/)       → Gemini 2.5 Flash — 1 500 pyyntöä päivässä ilmaiseksi
> Cloudflare AI (cf/)    → 50+ mallia — 10K hermosto/päivä
> Scaleway (scw/)        → Qwen3 235B, Llama 70B — 1 miljoonaa ilmaista tokensia (EU)
> Groq (groq/)           → Llama/Gemma — 14 400 pyyntöä päivässä äärimmäisen nopealla
> NVIDIA NIM (nvidia/)   → 70+ auki olevaa mallia — 40 hermoa/virtuaalipäivää/ikuisesti
> Cerebras (cerebras/)   → Llama/Qwen maailman nopeimmin — 1 miljoonaa tukemaa päivässä
> ```

## 🎙️ Ilmaiset Transkriptio Yhdistelmät

> Transkrioi mistä tahansa äänestä/ video näytöstä **0 ** — Deepgram johtaa $200
> ilmaisilla, AssemblyAI $50 turvavaralla, Groq Whisper ilman rajoituksia.

| Palveluntarjoaja | Ilmaiset krediitit                         | Paras Malli                                       | Käyttöraja                                      |
| ---------------- | ------------------------------------------ | ------------------------------------------------- | ----------------------------------------------- |
| 🟢 **Deepgram**   | **200 dollaria ilmaiseksi** (rekisteröidy) | `nova-3` – parhaan tarkkuuden, 30+ kieltä         | Ei rajoituksia ilmaisten krediittien yhteydessä |
| 🔵 **AssemblyAI** | **50 dollaria ilmaiseksi** (rekisteröidy)  | `universal-3-pro` – näkemyksiä, mielipiteitä, PII | Ei rajoituksia ilmaisten krediittien yhteydessä |
| 🔴 **Groq**       | **Ilmaiseksi ikuisesti**                   | `whisper-large-v3` — Avoin Whisper -malli         | 30 hermoa (rajoitettu)                          |

**Suositeltu yhdistelmä: /dashboard/combos **

```
Nimi: ilmainen-transkriptio
ratkaisuvetoinen
Solmut:
  [1] deepgram/nova-3          → käyttää $200 ilmaisia ensin
  [2] assemblyai/universal-3-pro → vakuutus, kun Deepgram krediitit riittää
  [3] groq/whisper-large-v3    → ilmaiseksi ikuisesti, hätäturvalle
```

Dashboard -> Kirjaudu sisään

## Pääteikkunat

Ominiroutti v2.0 on rakennettu toiminnalliseksi alusta, ei vain
toteamoyhteyspalvelimenä.

### 🆕 Uusia parannuksia ClawRouterin innoittamana (Maalis 2026)

| Esiitteen ominaisuus                                         | Mitä se tekee                                                                                                                 |
| ------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------- |
| ⚡ **Grok-4 Fast Family**                                     | AI-mallit edullisesti: 0,20/0,50/M euroa  - nopeampi kuin Gemini 2.5                                                          |
| 🧠 **GLM-5 Z.AI-kautta**                                      | 128 K:n output-kehys, 0,50/Euro/1M - uusin GLM- perheen edustaja                                                              |
| 🔮 **MiniMax M2.5**                                           | Päätös + agenstilläiset tehtävät 0,30/Euro/1M - merkittävä parannus M2.1:sta                                                  |
| 🎯 **toolCalling-lippu modelille**                            | Modelille kussakin `toolCalling: True/False` tietokannassa - automaattiasiirtimen ohittaa mallit, jotka eivät osaa siirtää    |
| 🌍 **Useita kielten ajoituksen ajoitus**                      | PT / ZH / ES / AR avainsanat automaattiasiirtimessä - parempi mallivalinta ei-englanninkieliselle sisällölle                  |
| 📊 **Ehdotus johtopäätökset[Benchmark-Driven Fallbacks ]X30X] | Oikea p95 latency reaaliaikaisista pyynnöistä toimii pistemäisessä arvosteluessaan - automaattiasiirtimessä oppii käytännössä |
| 🔁 **Pyynnön toistomääritys**                                 | Sisällön hash- pienenemisarvoinen toistomääräytyminen - monikortilla turvallinen - estää toistamiset                          |
| 🔌 **Liittämiskäytännön strategia**                           | Laajennettava `Routter-strategia` -käytäntö — lisää ominaisuuksia haluamallasi tavoin                                         |

### 🚀 Edellinen v2.0.9+ — Pelaamo, CLI Fingerprints & ACP

| Esiitteen ominaisuus                                     | Mitä se tekee                                                                                                                                                                                                                                                                                                                                                            |
| -------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 🎮 **Mallipelitasamo**                                    | Yhteyslomake, jolla voit tutkia haluamasi mallia suoraan — tarjoilija/malli/lähtöreitintarkastin, Monaco-toiminnonhallinta, lajittelijan ohjaus, tallennus ja ajanmäärittely                                                                                                                                                                                             |
| 🔏 **CLI-vilkkausvastaavuus **vilkkaushälytinlukkoinaan** | Asettaa tarjoilijan otsikoiden/materiaalijärjestykset toistamaan vakiomääritys tietokonemallitietolähteissä — toggle suurimmassa osassa tarjoilijoita vastaavassa Säännöt > Turvallisuus -valikossa   **Sukellusasi vaikuttaa**                                                                                                                                          |
| 🤝 **ACP-tuen (Agent Client Protocol)**                   | CLI agentin etsintä (Codex, Claude, Goose, Gemini CLI, OpenClaw + 9 muuta), prosessin lukija, `/API/WAP /ACPAgent`-pistekasikirjoitus                                                                                                                                                                                                                                    |
| 🤖 **ACP Agenttien sovelluskaappi**                       | Testaa-sivulla 14 agentin grid — agentti ylläpidoton statuksen lisäksi sekä versiotietojen tähyämiseen käytössä kuuluu mahdollistava Agentiliittäjä-agentti -lomake jokaiselle CLI-työkaluun. **Avattava koodi** -käyttäjille tulee "Lataa avattava.json" napin napautettua, joka automaattisesti luo valmiiksi käyttövalmiin rakenteen kaikille saatavilla mallillensa. |
| 🔧 **Mukautettu mallin `apiFormat` Routing**              | Mukautettu mallit, joiden `apiFormat[rikkomat]: "vastaukset"` lajitteleminen oikein menee todella näihin vastausten API -muuntajat                                                                                                                                                                                                                                       |
| 🏢 **Codex-isännön työskentelypohja **                    | Vain yhteys yksi/ email kerrallaan - OAuth sohvuun — perustoimitukseen vastaa työskentelytapaa                                                                                                                                                                                                                                                                           |
| 🔄 **Electron - aut. päivitys**                           | Työasuihin osoittuu sovellustuotteiden suuri osalle, hyljennykselle työskentäytyjen päivitysnäytön takaan päivitystä, + uusimmalle päivityksestetään automaattisesti sovellus                                                                                                                                                                                            |

### 🤖 Agentti ja -käyttäytymisasioperaatiot (v2.0)

| Esiitteen ominaisuus                               | Mitä se tekee                                                                                                             |
| -------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| 🔧 **MCP Palvelin (16 työkalua)**                   | IDE/agent-työkalut kautta 3 virtaa: stdio, SSE (`/api/mcp/sse`), Suoritettava HTTP (`/api/mcp/stream`)                    |
| 🤝 **A2A Palvelin (JSON-RPC + SSE)**                | Agenksuhteen tehtäväsuoritus äänetön ja suoritettavien virran mukaisesti                                                  |
| 🧭 **Yhdistetty Päätteet Sivu**                     | Vaihtoyksikkösivusto Endpoint-näytön, MCP, A2A ja API Päätteet-ikkunat                                                    |
| 🎚️ **Palvelin Edellytys/Liike Jankkeet**           | PYS/PYY sallijakkeet MCP ja A2A asetuksista säilyvät                                                                      |
| 🛰️ **MCP Ajo-kyky Tunteja**                        | Todelliset prosessityyppien aikaa, elinvaihepäivittäjän ikä, yksipaikkoissuhde ja toiminnot, ulottuvuuden asemakke        |
| 📋 **MCP Tapausten Kirja**                          | Merkityillä tapausten kirjanpitoteitä menestyksen epäonnistui, ja nähtävyyskaistojen suhteen.                             |
| 🔐 **MCP Aso-kuormituksen Koskemat**                | Matsineen koskemat 9 ylennyshyvityksentä oikeutta                                                                         |
| 📡 **A2A Tehtävien elämänkuolleet Säännöllisyyden** | Tehtäväkentän löytäminen/merkinnät tehtävissä, näistä kuuluviiin tehtävissä, lyhensi kunnon                               |
| 📋 **Agenti Kortilegio**                            | `/.tunnistavien Agentti Kartoon` jäljittävä klienttietojen löytäminen.                                                    |
| 🧪 **Ohjelmisto E2E Test Harness**                  | Reaalikäyttö Mackey-prosessi (MCP SDK) + A2A-palvelin virtaukset osoitteessa `test:protocols:e2e`                         |
| ⚙️ **Toiminnalliset Ohjausvalikot**                | Käytä napimerkintää, soveltuvat hankkijoille, restoaalloja [ X35X]test:protocols:e2e[X54X] hallinta yhden ohjausrintaalla |

### 🧠 Reitännöllisyys & tiedottaminen

| Esiitteen ominaisuus                             | Mitä se tekee                                                                                 |
| ------------------------------------------------ | --------------------------------------------------------------------------------------------- |
| 🎯 **Smart 4-Tasoinen Palautuminen**              | Automaattinen reitännöllisyys: Tilaus → API-avaimet → Halvin → Ilmainen                       |
| 📊 **Oikea-aikainen Joustoluokan Seuraaminen**    | Tämä hetkiset kokonaisuudet + loppukellon kutsu toimittajia                                   |
| 🔄 **Muotoilut Viestintä**                        | OpenAI ↔ Claude ↔ Gemini ↔ Vastausten rakenneyhteysmukaisia muuntamista                       |
| 👥 **Monikäyttäjä Tukea**                         | Monet käsittelyympäristöihin toimitettuja selkeyttäkoon itsevalintaa                          |
| 🔄 **Automaattinen Aseteu token**                 | OAuth-avaimet päivittyvät toistamiseen automaattisesti kääsmentoi                             |
| 🎨 **Mukautettu Väylämääritykset**                | 6 tasapainotusstrategioita + taustapurkkaohjaus                                               |
| 🌐 **Wildcadin Routaus**                          | `rekisteröintötarjoaja/*` dynaaminen sijoittaminen                                            |
| 🧠 **Ohjausmäääräysten Käytäntö**                 | Pitkä, automaattisen, määrätyn ja sopeutuvan määräysten rajat                                 |
| 🔀 **Mallien Nimikkeet**                          | Mukautettu + ominaisuustradisitaatio ja -turvallisuus                                         |
| ⚡ **Taustalla Pienennys**                        | Reitaa loputkin taustätöitä edullisempaa mallia kohti                                         |
| 🧪 **Tehtäväpohjainen Tietävä Smart Sijoitus**    | Automaata malleja sisältämällä sisältöyksiöiden mukaan (koodaus/näyttely/analysis/yhteenveto) |
| 💬 **Systeemin Aloitus injektoi**                 | Global kohdistus muodostaa vakavasti                                                          |
| 📄 **Vastauksien Rajapintoiminta yhteensopivuus** | Täys `/v1/responses` Kokemuksella Codexia ja -lämmetyt agenteilla työkentällä                 |

### 🎵 Useiden muuntorit

| Esiitteen ominaisuus      | Mitä se tekee                                                                                                                                                            |
| ------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 🖼️ **Kuvan luominen**     | `/v1/images/generations` pääpalveluilla ja paikallisen takana                                                                                                            |
| 📐 **Sijoitukset**         | `/v1/embeddings` hakemiselle ja RAG -virtapiirin aikana                                                                                                                  |
| 🎤 **Ääni-transkriptio**   | `/v1/ääni/transkriptiot` — 7 palveja (Deepgram Nova 3, AssemblyAI, Groq Whisper, HuggingFace, ElevenLabs, OpenAI, Azure), automaattinen kieli todennus, MP4/MP3/WAV-tuki |
| 🔊 **Tekstiääni**          | `/v1/ääni/ääni` — 10 palvelua (ElevenLabs, OpenAI, Deepgram, Cartesia, PlayHT, HuggingFace, Nvidia NIM, Inworld, Coqui, Tortoise) oikeiden virheviestien kanssa          |
| 🎬 **Videokuvaus**         | `/v1/video/kuvaus` (ComfyUI + SD WebUI-työntekijät)                                                                                                                      |
| 🎵 **Musiikin luominen**   | `/v1/musiikki/luomiset` (ComfyUI-työkalut)                                                                                                                               |
| 🛡️ **Suojaukset**         | `/v1/suojaukset` turvallisuus-tarkistukset                                                                                                                               |
| 🔀 **Uudelleenjärjestely** | `/v1/uudelleenjärjestys` vastuuvelvoite                                                                                                                                  |
| 🔍 **Verkkoselain** 🆕      | `/v1/haku` — 5 palveja (Serper, Brave, Perplexity, Exa, Tavily), 6 500+ ilmaista/kuukausi, automaattinen vikaosuusrajoitus, käytännön säilytys                           |

### 🛡️ Robustius, Turvallisuus & Hallintaa

| Esiitteen ominaisuus                                         | Mitä se tekee                                                                                                            |
| ------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------ |
| 🔌 **Sähkövirtapiirien välitys**                              | Per-mallin yhdysvälitys/sekasiointi kynnysarvot-ohjausten kanssa                                                         |
| 🎯 **Päähakkeistoituinen Mallit**                             | Kustomi mallit ilmoittavat tukeeman endpointeja + API-formaatti                                                          |
| 🛡️ **Sähkönsädeherkkojen määrä**                             | Viestintävalvonta + sulkumerkit toistolla/virtauksissa                                                                   |
| Kustannus/tarpeen vähentäminen kahdella mukaistuskerroksella | ⚡ [X2X]Pyyntö Idempotenssi[X23X]                                                                                         |
| Toistokuvioituminen suojanikkonakin                          | Epidemiaton suoja-ikkuna                                                                                                 |
| 🔒 **TLS-vilkkausmerkintä **tai[28X]salajuoksupidät[28X]      | Selkeä TLS-vilkkausmerkintä — **vähentää robottdetektoivia ja tilin tunnustetta**                                        |
| 🔏 **CLI-vilkkausvastaavuus **vilkkaushälytinlukkoinaan**     | Yhteensopivat CLI-pyyntötunnukset — **vähentää riskiä kielteisillä vastineilla olevan sijaintin**pääsuojautuminen        |
| 🌐 **IP-huoltelu**                                            | Pääsy-/ulkosäätö valikoitumisille tuotantoversion esillepallinnan sijaan                                                 |
| 📊 **Muokkaus-/käyttörajat**                                  | Järjestelmsglobaali/rakennepuolisko-rajien konfiguroimisellä/äskettömän sulkemisella olemassaoloaisteiden säädettävyyttä |
| 🔑 **API-salasananhallinta + rajoitukset**                    | Turvallinen salasankuorin/lisäysten ja malli/rakennepuu-rakennepuolikon tarkistukset                                     |
| 🛡️ **Säilytetty '/mallit'**                                  | Valinnaiset tunnistetiedonvirrat/tunnistetaan/rakennepuoliskoiden piilottaminen mallien katalogisolle                    |

### 📊 Tarkastettavuus & Analytiikka

| Esiitteen ominaisuus                          | Mitä se tekee                                                      |
| --------------------------------------------- | ------------------------------------------------------------------ |
| 📝 **Pyyntö + Suojattu Pyyntö Kirjauttaminen** | Koko pyyntö/vastaus tieto ja suojattu pyynnön kirjaaminen          |
| 📋 **Yhdistetty Kirjauspaneeli**               | Pyyntö, suojattu, tarkastelu- ja konsolivälilehdet yhdellä sivulla |
| 🔍 **Pyyntö Telemetri**                        | P50/ P95/ P99 viive ja pyynnön seuraaminen                         |
| 🏥 **Terveys Paneeli**                         | Toiminnan aika, muuttujatila, lomautukset, muistiinstatistikot     |
| 💰 **Kustannus Seuranta**                      | Sisaisten kustannustarkistus ja per-malli hintavuodennäyttäydet    |
| 📈 **Analytiikkakuvaukset**                    | Malleja/tarjoajat käytön tietoja- ja trendikatsastuksiä            |
| 🧪 **Arviointi Rakenne**                       | Havaittavan tietokannan tarkastelu strategioineen                  |

### ☁️ Lähetys ja Sovellus

| Esiitteen ominaisuus                  | Mitä se tekee                                                                              |
| ------------------------------------- | ------------------------------------------------------------------------------------------ |
| 🌐 **Kuvaus Kaikille**                 | Paikallisesti, VPS, Docker, pilvipohjaiset ympäristöt                                      |
| 💾 **Cloud Sync**                      | Kokoonpanon synchronointi pilvipalvelin työntekijän avulla                                 |
| 🔄 **Takaisinvaro/ Palmerotu**         | Siirtymiskäyntöjen tulostus ja katastrofigrafiareiskyttojen täsmennys                      |
| 🧙 **Onboarding Wizard**               | Ensimmäisen kerran käyttämisen opastettu asennusprosessi                                   |
| 🔧 **CLI -työkalut -pohja**            | Sivuttamaton asennus suosituksille koodaus-työkaluille                                     |
| 🎮 **Mallipelitasamo**                 | Testaa yhteyttä, malli sekä päätepisteen hallinnasta                                       |
| 🔏 **CLI -tunnistemerkinnän siirtymä** | Tunnistemerkinnän siirtymisen tuki yksittäisten toimijoiden käyttöön                       |
| 🌐 **I18N (30 kieltä)**                | Kansalaisten kielivalikoiman tuki kantopohjallalla sekä kirjaimenalaisen käsittelyn kanssa |
| 🧹 **Poista kaikki mallit**            | Yksinkertainen mallilistan poistaminen toimijan yksilöllisyyskohtaisessa yhteisössä        |
| 📋 **Vakiotekstit Mallit**             | GitHub asiakirjatavujen toimima tuki bugiin ja ominaisuuksiin                              |
| 📂 **Mukautettu datatrikootusjono**    | `TIEDOSTOHALIN` ylitys tallennuspaikaksi                                                   |

### Ominaisuuksien syvennyskatsaus

#### Savijännitys käytännöllisellä maksulaskentahoidolla

```txt
Yhdistelmä: "minun-koodinhallinta-työkalusi"
  1. cc/claude-opus-4-6
  2. nvidia/llama-3-3-70b
  3. glm/glm-4.7
  4. if/kimi-k2-päättely
```

Tilanteessa, kun käyttörantailähde, maksuhäiriö tai tilan indeksi loppuu,
OmniRoute siirtyy automaattisesti seuraavaan hakusanan ilman manuaalista
siirtymistä.

#### Näkyvästi käytettävä ja ohjattava protokollahallinta

- MCP + A2A ovat käyttöliittymässä ja dokumentaatioon näkyvissä (piilotettu)
- Käyttöliittymän tiedot ja protokollan tila-rajapinnat osoittavat
  reaalikäyttöympäristöön kuuluvaa toimintoa (protokolla/mcp/*`, a2a/*`)
- Valvojia ja toimintoja sisältävät hallintapaneeli ja toimenpidekartan
  sisältävät arvioinnin yhteydessä toiminnan arvioimista varten
  (yhdistelmälliset napit, hakupinnasteiden resetointi, tehtävän peruutus)

#### Kääntäjän työkalu + vahvistus-prosessi

Kääntäjän alueeseen kuuluvat:

- **Leikkauspeli**: pyynnön muodon tarkistus
- **Chat -testaaja**: koko pyynnön ja vastauksen kiertymä
- **Testilaajittelu**: useamman tapauksen yhdessä suorituksessa
- **Eloonjääneiden seuraaminen**: reaaliaikainen liikennevalvonta

Plussaa siis myös tapaukset:asiakas protokollan vahvistukseen
reaalikaistyöoloon. Npm: test:protokollakulunvaiheesta.

> 📖 **[MCP-serverin käyttö-opas](open-sse/mcp-server/README.md)** — Työkalujen
> rekisteri, IDE-asetukset ensin käyttäjien ja asiakastapaukeset ym. esimerkit
> 
> 📖 **[A2A-serverin käyttö-opas](src/lib/a2a/README.md)** — Taidontehtävät,
> JSON-RPC-tason toimintojoukko, putkien vahvistus ja tehtävien elinkaaripaikat

## Kokeilulaitteisto (Koeta)

Ominaisuudessamme on omia kokeilujärjestelmä ominaisuuksia reaalissa
käyttöolossa tasaista arviointia laajentamalla, testien käytön ja dokumentaation
tukipalveluineen. Omaksesi saat: **Analytiikat → koeta** näkyvyyttä yhteyden
käyttöliittymästä.

### Ominen Kultainen Asetelma

Pohjatietokannossa "Ominiradion Kultainen Asetelma" on asiakkaan testitapauksia:

- Hei, luvut, maantiede, koodin tuotto
- JSON-muodon valisaalis, käännös, markdownin tuotto
- Haitallinen sisältö (turvallisuus), lukeminen, boolin logiikka

### Arviointistrategiat

| strategia      | Kuvaus                                                    | Esimerkki                          |
| -------------- | --------------------------------------------------------- | ---------------------------------- |
| `tarkka`       | Tulos on tarkka                                           | `"4"`                              |
| `sisältää`     | Tulos sisältää alkiota (koosan puutteettoman tapauksessa) | `"Paris"`                          |
| `regiksi`      | Tulos vastaa regiksi mallia                               | `"1.*2.*3"`                        |
| `ominaisuudet` | Mukautettu JS -funktio palauttaa totuuden/väärää          | `(ulos) =&gt; ` (ulos pituus > 10` |

---

## 📖 Ohjeet asetukseen

### Protokollaan asetukset (MCP + A2A)

<details>
<summary><b>🧩 MCP Setup (Model Context Protocol)</b></summary>

Aloita MCP-liikenne stdiomuodossa:

```bash
omniroute --mcp
```

Suositeltu validointi- ja suoritusvirran:

1. Yhdistä MCP-palvelin stdion kautta.
2. Käynnistä `omniroute_get_health`.
3. Suorita `omniroute_list_combos`.
4. Avaa `/keskus/palvelin/mcp`, jotta vahvistetaan syke, aktiviteetti ja
   kirjatiedot.

Automatisointia varten käytettäviä API-sovellimia:

- `GET /api/mcp/status`
- `GET /api/mcp/tools`
- `GET /api/mcp/audit`
- `GET /api/mcp/audit/stats`

</details>

<details>
<summary><b>🤝 A2A Setup (Agent2Agent)</b></summary>

Etsi agentti:

```bash
curl http://localhost:20128/.well-known/agent.json
```

Lähetä tehtävä:

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"setup-a2a","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"Ota selvää rahtimäärää."}]}}'
```

Ohjata elinkaarihankkeita:

- `GET /api/a2a/tilaus`
- `GET /api/a2a/tiedostot`
- `GET /api/a2a/tiedostot/:id`
- `POST /api/a2a/tiedostot/:id/häiritse`

Palvelun käytöstä:

- `/pohjastiedot/a2a` tehtävä-/tilan-/virran havainnointi ja savun toimintoja
  varten

</details>

<details>
<summary><b>🧪 End-to-end protocol validation</b></summary>

Vahvista molempien protokollan toimivuus oikeilla klientsiä:

```bash
npm run test:protokollit:e2e
```

Tämä vahvistaa:

- MCP SDK -clienti yhdistä / listaa / puhetaan
- A2A -tiedon löytäminen / lähettäminen / virtanäytön haku / häiritseminen
- Tarkista dataa MCP -auditiin ja A2A -tehtäväjohdon avainten avulla.

</details>

<details>
<summary><b>💳 Subscription Providers</b></summary>

### Claude Code (Pro/Max)

```bash
Näyttöpaneli → Tarjoajat → Liitä Claude Code → OAuth -kirjautuminen → Automaattinen token- uudelleenlataus → 5 tunnin + viikkoaikakäyttötila
Mallit:
  cc/claude-opus-4-6
  cc/claude-sonnet-4-5-20250929
  cc/claude-haiku-4-5-20251001
```

**Pro neuvonen**: Opus käytä yhteiskunnallisissa tehtävissä, Sonnet nopeudelle.
OmniRoute kertoo mallittain käytössä olevaa quota!

### OpenAI Codex (Plus/Pro)

```bash
Näyttöpaneli → Tarjoajat → Liitä Codex → OAuth -kirjautuminen (portti 1455)
→ 5 tunnin + viikoittaista resetointia

Mallit:
  cx/gpt-5.2-codex
  cx/gpt-5.1-codex-max
```

#### Codex Tilausrajoitus hallinta (5h + Viikko)

Jokainen Codex-tilaus nyt koostuu käytettävissä olevasta poliittisista
siirroksista `Näyttöpaneli -&gt; Tarjoajat`:

- `5h` (Pysyvää/Vaihtelua): vahvista 5-tunnin aikakautta.
- `Viikoista` (PYÖRTEEN/POIS): voimuta tiukentamispolitiikan käyttö.
- Rajapyykki: kun käytettävillä ikkunoilla on saavutetut tai yli 90 prosentin
  käyttöaste, tili siirretään äkillisesti poispäälle.
- Rotointi: OmniRoute ohjaa liikenteen seuraavaan tarjoajana hyväksyttyyn Codex
  tilille automaattisesti.
- Puhdistus: kun tarjoaja `jälkipyykki` ajasta on kulunut, tili palautuu
  automaattisesti hyväksyttyyn.

Tilanteet:

- `5h YKS` + `Viikoista ON`: tilin yksityiskayttäjä ja/tai viikkojen kokemukset
  estävät tilin käytön.
- `5h POIS` + `Viikoista ON`: tilin viikkojen käyttötulos estää tilin käytön
- `5h ON` + `Viikoista POIS`: tilin 5- tuntien käyttötulos estää tilin käytön.
- `jälkipyykki` on kuluneen jälkeen: tilin käyttäjätalvotaan automaattisesti (ei
  tarvita tarjoajan vaihtamista).

### Gemini CLI (ILMA 180 000 käyttäjälle kuukaudessa!)

```bash
Päänäyttö → Tarjoajat → Yhdistä Gemini CLI
→ Google OAuth
→ 180 000 täyttäjäsiirtotulos / kuukausi ja 1 000 päivästä.

Mallit:
  gc/gemini-3-pilotointikatsaus
  gc/gemini-2.5-pro
```

**Paras arvo:** Monipuolinen ilmainen luokka. Käytä tätä eräiden
maksuvaihtoehtojen ennen.

### GitHub Copilot

```bash
Päänäyttö → Tarjoajat → Yhdistä GitHub
→ GitHubin kautta OAuth
→ Kuukautinen päättäminen (kuukauden 1 vastaan).

Mallit:
  gh/gpt-5
  gh/claude-4.5-sonnet
  gh/gemini-3-pro
```

</details>

<details>
<summary><b>🔑 API Key Providers</b></summary>

### NVIDIA NIM (ILMA kehittäjille tarjoaminen - 70+ malli)

1. Rekisteröidy: [build.nvidia.com](https://build.nvidia.com)
2. Saada ilmainen API avain (säädetettu 1000 inference-ehdoineen)
3. Päänäyttö → Käyttämö: Yhdistä NVIDIA NIM
   - API Avain: `nvapi-my-avain`

**Mallit**: `nvidia/llama-3.3-70b-instruct`, `nvidia/mistral-7b-instruct`, ja
50+ lisää mallia

**Vinkki:** Openn AI-yhteensopiva API — toimii kypsän Omniputkimuodon
muuntamisella!

### DeepSeek

1. Ota samassa: [platform.deepseek.com](https://platform.deepseek.com)
2. Saada API-avain
3. Valikko → Lisää toimittaja → DeepSeek

**Mallit:** `deepseek/deepseek-chat`, `deepseek/deepseek-coder`

### Groq (Ilmainen taso on saatavilla!)

1. Ota samassa: [console.groq.com](https://console.groq.com)
2. Saada API-avain (ilmainen taso sisältyy)
3. Valikko → Lisää toimittaja → Groq

**Mallit:** `groq/llama-3.3-70b`, `groq/mixtral-8x7b`

**Vinkki:** Erityisen nopea todentaminen — paras oikeassa ajoassa koodaamiseen!

### OpenRouter (yli 100 mallia)

1. Ota samassa: [openrouter.ai](https://openrouter.ai)
2. Saada API-avain
3. Valikko → Lisää toimittaja → OpenRouter

**Mallit:** Pääse 100+ malleihin kaikkien suurseurujen avulla yksittäinen
API-avain.

</details>

<details>
<summary><b>💰 Cheap Providers (Backup)</b></summary>

### GLM-4.7 (Päivittyvä 0,6$/1M)

1. Ota samassa: [Zhipu AI](https://open.bigmodel.cn/)
2. Saada API-avain Koodikerronnan suunnitelmasta
3. Pohjaruutina → Lisää API Avain:
   - Päätoimittaja: `glm`
   - API Avain: `asiakkaasi avaimeksi`

**Käytä:** `glm/glm-4.7`

**Pro Tip:** Koodaustoimenpide tarjoaa 3× luokkaa 1/7 kustannuksesta! Lopeta
päivässä 10:00 AM.

### MiniMax M2.1 (5h reset, 0,20 $/1M)

1. Lisää: [MiniMax](https://www.minimax.io/)
2. Saada API-avain
3. Pohjaruutina → Lisää API Avain

**Käytä:** `minimax/MiniMax-M2.1`

**Pro Tip:** Kustannukset lyhdestä on halvin valinta (1 Mil johtimella)!

### Kimi K2 ($9 kuukaudessa tasaisella kuukauden verran)

1. Tilaa: [Moonshot AI](https://platform.moonshot.ai/)
2. Saada API-avain
3. Pohjaruutina → Lisää API Avain

**Käytä:** `kimi/kimi-latest`

**Pro Tip:** Säännöllinen 9 dollarilta kuukaudesta 10 mil kuuta = 0,90 $
dollarilta toiminnanmukaiseen hintaan!

</details>

<details>
<summary><b>🆓 FREE Providers (Emergency Backup)</b></summary>

### iFlow (5 Tietää ilmaiseksi via OAuth-sidos)

```bash
Pohjaruutina → Liittyminen iFlow
→ iFlow OAuth-laitos
→ Suuri käyttömahdollisuus

Mallit:
  if/kimi-k2-thinking
  if/qwen3-coder-plus
  if/glm-4.7
  if/minimax-m2
  if/deepseek-r1
```

### Qwen (4 FREE mallia via Laitteekoodi)\

```bash
Dashboard → Yhdistä Qwen
→ Koneko koodiaikauksen hyväksyminen
→ Rajoittaomatka käyttö

Mallit:
  qw/qwen3-coder-plus
  qw/qwen3-coder-flash
```

### Kiro (Claude TILAA VAPAAT)

```bash
Dashboard → Yhdistä Kiro
→ AWS-kehykseen tai Google/GitHub
→ Rajoittaumatka käyttö

Mallit:
  kr/claude-sonnet-4.5
  kr/claude-haiku-4.5
```

</details>

<details>
<summary><b>🎨 Create Combos</b></summary>

### Esimerkki 1: Kaksintaistelu tariffeja → Halpoja varmuuskopiota

```
Dashboard → Kombot → Luo uusi

Nimi: premium-coding
Mallit:
  1. cc/claude-opus-4-6 (Tariffi päämalli)
  2. glm/glm-4.7 (Kustannuksella varmuuskopio, $0.6/1M)
  3. minimax/MiniMax-M2.1 (Kustannuksella varmuuskopio, $0.20/1M)

Käytä Komennolla: premium-coding
```

### Esimerkki 2: Vapaat (Ei kustannuksia)

```
Nimi: free-combo
Mallit:
  1. gc/gemini-3-flash-preview (180K vapaana kuukausina)
  2. if/kimi-k2-thinking (rajatonta)
  3. qw/qwen3-coder-plus (rajatonta)

Kustannukset: 0 dollarista ikinä ainakin!
```

</details>

<details>
<summary><b>🔧 CLI Integration</b></summary>

### Kohdistin IDE

```
Asetukset → Mallit → Korkea taso:
  OpenAI API-päätepiste: http://localhost:20128/v1
  OpenAI API-avain: [OmniRoute-näytnimestä]
  Malli: cc/claude-opus-4-6
```

### Claude-koodi

Käytä **CLI-työkaluita**-sivua yrityspalvelun katon alla yhden napsauksen
asetuksilla tai `~/.claude/settings.json`-tiedostoa manuaalisisesti muokkaa.

### Codex CLI

```bash
export OPENAI_BASE_URL="http://localhost:20128"
export OPENAI_API_KEY="OMNIRUTE-API-OMINEN-avain"

komento "kirjoita kohdename"
```

### OpenClaw

**Valinta 1 — Palvelun (suositelluin):**

```
Dashboard → CLI Työkalut → OpenClaw → Valitse mallit → Hyväksy
```

**Valinta 2 — Manuaalinen:** Muokkaa `~/.openclaw/openclaw.json`:

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

> **Lähdeluonnehdinta:** OpenClaw toimii vain paikallisella OmniRoute. Käytä
> `127.0.0.1` sijainnin sijaan `localhost`:n välttääksesi
> IPv6-resoluutiongelmat.

### Cline/ Käytä / RooCode

```
Asenssit =&gt; 
AI-kompatibilitaarinen toimittaja: OpenAI Compatible
Pääosoite: http://localhost:20128/v1
API-avain: [OmniRoute-ohjelmiston asiakkaalta]
Malli: if/kimi-k2-thinking
```

### OpenCode

**Vaihe 1** Lisää OmniRoute toimittajaksi:

```bash
opencode
/yhteydenpidon asetus
# Valitse "Muu" → Kirjoita ID: "omniroute" → Anna OmniRoute API-avaintesi
```

**Vaihe 2** Muokkaa `opencode.json`-tiedostoa [X61X]projektiohessa on:

```json
{
  "$schema": "https://opencode.ai/config.json",
  "provider": {
    "omniroute": {
      "npm": "@ai-sdk/openai-compatible",
      "nimi": "OmniRoute",
      "valinnat": {
        "pääosoite": "http://localhost:20128/v1"
      },
      "mallit": {
        "cc/claude-sonnet-4-20250514": { "nimi": "Claude Sonnet 4" },
        "gg/gemini-2.5-pro": { "nimi": "Gemini 2.5 Pro" },
        "if/kimi-k2-thinking": { "nimi": "Kimi K2 (Ilmainen)" }
      }
    }
  }
}
```

**Vaihe 3** Valitse malli OpenCodessa:

```bash
/mallit
# Valitse minkä tahansa OmniRoute-mallin listasta
```

> **Vinkki** Lisää jokaisella tahansa tallennauttamisessa saatavilla oleva malli
> kohdassa `/v1/mallit` `mallit`-osioon. Käytä muodostetta
> `toimittaja/malli-idi` yhdestä tuotteen kirjautumisen asetuksista.

</details>

---

## Vianetsintä

<details>
<summary><b>Click to expand troubleshooting guide</b></summary>

**"Käyttökuvalähteen ei tuottanut viestejä"**

- Toimittajan määräaika umpeutunut → Vaadi tarkistus ikkunasta kuluvaa
  määräaikaa
- Suojaus: Kombinoi aluennus tai siirrä halvempaan eriin

**Luvun rajittaminen**

- Keskitason loppumisaika → Keskitty to GML/Miniaks
- Lisää toinen kombinaatio: `cc/claude-opus-4-6 → glm/glm-4.7 →
  if/kimi-k2-thinking`

**OAuth -tokenni on vanhentunut**

- OmniRoutee irtauttoi tämän automaattisesti.
- Jos ongelmia jatkuu: Käytä kirjautumista -> Toimittaja -> Liitä takas

**Korkeat kustannukset**

- Tarkastele tilastot Dashboard → Kustannukset
- Vaihda päämallia GLM/MiniMax -malleihin
- Käytä ilmainen taso (Gemini CLI, iFlow) vähäarvoiseen tehtäviin

**Dashboard/API-kaapelit ovat väärin**

- `PORT` on kanavanumero (ja API-kaapeleista oletusarvo 0)
- `API_PORT` ylittää ainoastaan OpenAI-hajottimissa käytettävät API-kaapelit
- `DASHBOARD_PORT` ylittää ainoastaan dashboard/Next.js -kaapelit
- Aseta `NEXT_PUBLIC_BASE_URL` osoite teitse tuonti URL (OAuth-kutsun kohdalle)

**Cloud-syntekstitoksin virheet**

- Vahvista, että `BASE_URL` osoittaa käynnissä olevan sovelluksen
- Vahvista, että `CLOUD_URL` osoittaa oletettavan cloud-pisteen
- Pidä `NEXT_PUBLIC_*` -arvot samana suuntaa server-mallilla

**Ensimmäinen kirjautuminen ei toimi**

- Tarkista `INITIAL_PASSWORD` arvo `.env`
- Jos arvon ei aseteta, taustavuoro on `123456`

**Ei pyyntölaskelmia**

- Aseta `ENABLE_REQUEST_LOGS=true` arvo `.env`

**Yhteyskokeilu osoittaa "Virheellinen" omassa OpenAI-yhteisössä**

- Monet tarjoajat eivät kertomalli-rajapintaa
- OmniRoute v1.0.6+ sisältää tuki jälki-tarkistusten chat-suljetuksi
  pääsääntöisenä
- Käytä tietokoneen lokasivulla olevaa HTTPS osoitetta

### Salautta OAuth kilpailevalla palvelimella

<a name="oauth-on-a-remote-server"></a> <a name="oauth-em-servidor-remoto"></a>

> **⚠️ Tärkeää käyttäjille, jotka käyttävät OmniRoutea VPS:llä, Dockeria tai
> minkä tahansa kilpailevan palvelimen**

#### Miksi Antigravity / Gemini CLI OAuth epäonnistuu kilpailevalla palvelimella?

[TietoXAntigravityX17X]-sovelluksen ja [TietoX24X]Gemini CLI**-sovelluksen ovat
käytössä [TietoX53X]Google OAuth 2.0**-toimintoja. Google vaatii
[TietoX95X]suuntaan ohjaavan URI:X108X]-arvoa OAuth-siirrossa olla täsmääväksi
yksi siitä Google Cloud Consolessa rekisteröityneistä URIOsoitteista.

Omnirouten sisältyvien OAuth-tunnuksien sisältämä on rekisteröity vain
[TietoX58X]"localhost"-osoiterikollisuudelle**. Kun käytät Omniroutetta
kilpailevalla palvelimella (esimerkiksi
[TietoX135X]https://omniroute.myserver.com`), Google hylkää autentikointia
virhearvolla:

```
Virhe 400: redirect_uri_mismatch
```

#### Ratkaisu: Määrittele omat OAuth-tunnukset

Sinun tulee luoda [TietoX22X]OAuth 2.0 kännettäjä** - tunnusten Google Cloud
Console -sovelluksessa palvelimesi URI -osoitemerkillä.

#### Vaiheita eteenpäin

**1. Avaa Google Cloud Console**

Mene reiluun:
[https://console.cloud.google.com/apis/credentials](https://console.cloud.google.com/apis/credentials)

**2. Luo uusi OAuth 2.0 kännettajatunnuksilta**

- Napsauta [TietoX6X]"+"Luoda krediti"[TietoX30X] →
  [TietoX35X]"oauth-kännettajatunnukset"[TietoX54X]
- Sovellustyyppi: [TietoX18X]"Web-sovellus"[TietoX37X]
- Nimi: mitä tahansa (esimerkiksi [TietoX30X]OmniRoute kilpailija`)

**3. Lisää sallittuja palautus-OSOitteita**

Sovelluksen [TietoX7X]"sallittujen palautus-OSOittien** kentistä lisää:

```
https://asi-osiitteesi.com/palautus
```

> Vaihda [TietoX8X]asi-osiitteesi.com` sivustosi kohdemerkistä tai IP:stä
> (sisällytä portaalin noiden, jos on tarpeen, esimerkiksi
> [TietoX92X]http://45.33.32.156:20128/palautus`).

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
Virhe 400: redirect_uri_mismatch
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

**6. Käynnistä uudelleen OmniRoute**

```bash
# Jos käytät npm:
npm run dev

# Jos käytät Dockeria:
docker restart omniroute
```

**7. Yritä yhdistää uudelleen**

Päätäväli → Tarjoajat → Antigravitointi (tai Gemini CLI) → OAuth

Nyt Google ohjaa sinua oikein `https://seu-servidor.com/callback` -sivulle ja
kirjautuminen toimii.

---

#### Voimassaoleva ympäristö (ilman omia tunnuksia)

Jos et halua luoda omia tunnuksia nyt, voidaan vielä käyttää **manuaalista
URL-siirtymää**:

1. Omniroute avaa Google -kirjautumissivun
2. Kirjautumisen jälkeen Google yrittää ohjata sinua `localhost` -tapahtumaan
   (joka epäonnistuu kuitenkin palvelimella)
3. **Kopioi osoitekaappimasta oheinen URL[Y22X]
4. Laita se URL-osoite kohde-tunnuksen kohde-puoliin
5. Napsauta **"Connect"**

> Tämä ympäristö toimii, koska kirjautumiskoodi on validi riippumatta siitä
> päivität ohjautui onnistuiko vai ei.

</details>

---

</details>

## 🌐 Tekniikka

<details>
<summary><b>Click to expand tech stack details</b></summary>

- **Ajoitustaikutumus**: Node.js 18–22 LTS ( varoitus: Node.js 24+ ei **tuke** —
  `better-sqlite3` native binaries ovat incompatibel)
- **Kiele**: TypeScript 5.9 — **100 % TypeScript** kaikilla `src/` ja
  `open-sse/` (yksi `any` tärkeimmistä ytimen moduulit v1.0 alkaen)
- **Rakente**: Next.js 16 + React 19 + Tailwind CSS 4
- **Tietokanta**: LowDB (JSON) + SQLite (aluetiedot + proxy kirjanpito + MCp
  tarkastus sekä liikenteen ratkaisut)
- **Schemat**: Zod (MCp työkalut I/O tarkastus, API sopimukset)
- **Protokrollit**: MCP (stdio/HTTP) + A2A v0.3 (JSON-RPC 2.0 + SSE)
- **Lähettävä**: Palvelun välittämä Tapaus (SSE)
- **Kirjautuminen**: OAuth 2.0 (PKCE) + JWT + API- Avaimet + MCP-scopeen
  Käyttöoikeudet
- **Testaus**: Node.js -testijärjestelmä + Vitest (900+ testiasianna, mukaan
  lukien yksikkötestejärjestelmä, integraatio testit, E2E- testit)
- ** CI/CD**: GitHub Actions (auton npm julkaistava + Docker Hub päivitys
- **Sivusto**: [omniroute.online](https://omniroute.online)
- ** Paketti**:
  [npmjs.com/package/omniroute](https://www.npmjs.com/package/omniroute)
- **Docker**:
  [hub.docker.com/r/diegosouzapw/omniroute](https://hub.docker.com/r/diegosouzapw/omniroute)
- **Säilyvyys**: Jännite katkaisija, eksponentiaalinen perässä, vastaava
  herkkäsiima, TLS- väärennys, automaattinen -yksittäisen palvelimen
  palautuminen ja palauttaminen

</details>

---

## Dokumentaatio

| Dokumentoi                                           | Kuvaus                                                               |
| ---------------------------------------------------- | -------------------------------------------------------------------- |
| Käyttöohje                                           | Laitteita, palvelimia, CLI-integraatio ja asennus                    |
| API-opas                                             | Kokoa kaikki endpointit esimerkeillä                                 |
| [MCP-palvelin](open-sse/mcp-server/README.md)        | 16 MCP-työkalua, IDE -konfiguraatiot, Python / TS / Go -kliendit     |
| [A2A-palvelin](src/lib/a2a/README.md)                | JSON-RPC 2.0 -protokolla, taitavuudet, lähettäminen, tehtävähallinta |
| [Auto-Combo Engine](docs/auto-combo.md)              | Keskeinen kuuden pisteen arviointi, mallipaketteja, itsehoitaja      |
| [Tuotteenhuolto](docs/TROUBLESHOOTING.md)            | Yleisiä ongelma ja ratkaisuja                                        |
| [Aloite ja kehitys](docs/ARCHITECTURE.md)            | Järjestelmän rakenne ja sisällöt                                     |
| [ Avustaminen](CONTRIBUTING.md)                      | Kehitysohjelmien määritelmä ja ohjeet                                |
| [Avoimen APIn määritelmä](docs/openapi.yaml)         | OpenAPI 3.0 määritelmät                                              |
| [Turvallisuuspolitiikka](SECURITY.md)                | Turvallisuusraportointi ja -tiedotteet                               |
| [Kestoamiskäyttöönotto](docs/VM_DEPLOYMENT_GUIDE.md) | Virtuaalikone + nginx + Cloudflare asennusohjeet                     |
| [Tuotteen näyttökuvaus](docs/FEATURES.md)            | Kuvia ja grafiikat                                                   |
| [Julkaisutarkastuslista](docs/RELEASE_CHECKLIST.md)  | Pitkäaikainen yhteensopivuus testeistyöt                             |

---

## 🗺️ Tavoitearvoitus

OmniRoute on suunnitellut useita **210+ ominaisuutta, jotka toteutetaan
järjestyksessä. Tärkeimmät tärinöt liittyvät siihen, millä tasolla seuraavassa
kehitysjuhlahetkessä

| Kategoria                          | Planned Features | Valitut Ominaisuudet                                                                                 |
| ---------------------------------- | ---------------- | ---------------------------------------------------------------------------------------------------- |
| 🧠 **Reititys ja Älykkyys**         | 25+              | Alhaisin reititys, tunnuskielloitettu reititys, quota preflyfli, P2C-tili valintamenetelmä           |
| 🔒 **Turvallisuus ja Selkeys**      | 20+              | SSRF-vakautus, tunnuspiilotus, suoritussykkeisen palaute, hallintasanan rajaaminen                   |
| 📊 **Mitata Tehdään**               | 15+              | OpenTelemetry-yhteensopivuus, reaaliaikainen quota valvonta, käyttökohteen mukainen kustannusnäyttö  |
| 🔄 **Pääkohdemallien Liitännäiset** | 20+              | Toimija Määrittely, koodeaukset, usean tien Codex, Copilot kuormitus analysaor                       |
| ⚡ **Suorituskyky**                 | 15+              | Dual cache kerros, ohje koestokra, vastaus kokoelmamerkintä, puheviestiriistola, sarjais API         |
| 🌐 **Rakensilta**                   | 10+              | WebSocket API , konfiguraation uudelleen käynnistys, hajotettu konfiguraatiostalli, kaupallinen tila |

### 🔜 Tulevat Ominaisuudet

- 🔗 **OpenCode Integration** — Nativen tuki avattavalle OpenCode AI
  koodityökalulle
- 🔗 **TRAE-Integraatio** — Koko TRAE AI-kehitysrajoituksen tuki
- 📦 **Batch API** — Kokonaisuudessaan synkroninen batch-asinkroninen käsittely
  bulk-vaatimuksilla
- 🎯 **Tag-Based Routing** — Syyttä routaa pyynnöt haluamasi tagin ja
  meta-asetusten mukaan
- 💰 **Kustannustehokkain strategia** — Automaattisesti valitse parhaasta
  saatavilla tarjoaja kustannustehokas strategia

> 📝 Kaikki ominaisuudet voidaan lukea [yksityiskohtaisia oheislehtiä`docs/uusia
> ominaisuuksia`](docs/new-features/) (217 yksityiskohtaisessa todennäköisessä)

---

## 👥 Osallistujat

[![Contributors](https://contrib.rocks/image?repo=diegosouzapw/OmniRoute&max=100&columns=20&anon=1)](https://github.com/diegosouzapw/OmniRoute/graphs/contributors)

### Miten Osallistua

1. Sivusto lueteltiin forkasi hakemistossa
2. Luo oman ominaisuuden haaraa ( `git checkout -b feature/amazing-feature`))
3. Tallenna muutokset ( `git commit -m 'Lisää oikean ominaisuuden'`)
4. Siirrä ominaisuus kohuun ( `git push origin feature/amazing-feature`))
5. Kun aloittaas muutosesta haasteen (Pull Requesten avaus

Katso [CONTRIBUTING.md](CONTRIBUTING.md) yksityiskohdittain

### Julkaise uusi versio

```bash
1. Luo julkaisu (NPM julkaisee automaattisesti) 
gh luo julkaisun - h1: "v2.0.0" --generoi muistiinpanon
```

---

## 📊 Lihastettu historia

## Lihastettujen tähystä ajan mittaisesti

## [![Lihastettu historia](https://starchart.cc/diegosouzapw/OmniRoute.svg?variant=adaptive)](https://starchart.cc/diegosouzapw/OmniRoute)

## 🙏 Kiitokset

Erikuusinta ** [1] ja ** [2] tekijöille, jotka ovat luoneet tästä projektin
alun. OmniRoute rakentuu tähän perusteellisesti ylemmälle tasolle mukautamalla
alueiden yhdistelyä, monimutkaisia API:tä ja tekemällä täysjärjestelmällinen
TypeScript uudelleenkirjoitus.

Erikuusinta ** [1].

---

## 📄 Lisenssi

MIT-lisenssi — katso [LICENSE] [1] tarkemmin yksityiskohtaiset tiedot.

---

<div align="center">
  <sub>Built with ❤️ for developers who code 24/7</sub>
  <br/>
  <sub><a href="https://omniroute.online">omniroute.online</a></sub>
</div>
<!-- GitHub Discussions enabled for community Q&A -->
