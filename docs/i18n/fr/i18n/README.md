# 🚀 OmniRoute — Le Passerelle Gratuite AI

### N'arrêtez jamais de coder. Affichage intelligent jusqu'aux ** modèles AI gratuits et abordables ** avec un retour automatique.

_ Votre proxy API universel — un seul point de terminaison, 67 fournisseurs +, 0
downtime. Maintenant avec l'orchestration d'agents MCP & A2A. _

** Completions de conversations • Embeddings • Génération d'images • Vidéo •
Musique • Audio • Reranking • ** Recherche Web ** • Serveur MCP • Protocole A2A
• 100 % TypeScript **

---

<div align="center">

[![version
npm](https://img.shields.io/npm/v/omniroute?color=cb3837&logo=npm)](https://www.npmjs.com/package/omniroute)
[![téléchargements
npm](https://img.shields.io/npm/dm/omniroute?color=cb3837&logo=npm&label=npm%20downloads)](https://www.npmjs.com/package/omniroute)
[![Docker
Hub](https://img.shields.io/docker/v/diegosouzapw/omniroute?label=Docker%20Hub&logo=docker&color=2496ED)](https://hub.docker.com/r/diegosouzapw/omniroute)
[![Docker
Pulls](https://img.shields.io/docker/pulls/diegosouzapw/omniroute?logo=docker&color=2496ED&label=docker%20pulls)](https://hub.docker.com/r/diegosouzapw/omniroute)
[![Licence](https://img.shields.io/github/license/diegosouzapw/OmniRoute)](https://github.com/diegosouzapw/OmniRoute/blob/main/LICENSE)
[![Site
web](https://img.shields.io/badge/Website-omniroute.online-blue?logo=google-chrome&logoColor=white)](https://omniroute.online)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-Community-25D366?logo=whatsapp&logoColor=white)](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

[ Site web 🌐](https://omniroute.online) • [ Quick Start 🚀](#-quick-start) • [
Features 💡](#-key-features) • [ Documentation 📖](#-documentation) • [ Tarifs
💰](#-pricing-at-a-glance) • [ WhatsApp
💬](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

</div>

🌐 **Disponible dans:** 🇫🇷 [Françaises](README.md) | 🇪🇸
[Español](docs/i18n/pt-BR/README.md) | 🇧🇷 [Português
(Brasil)](docs/i18n/es/README.md) | 🇬🇧 [English](docs/i18n/fr/README.md) | 🇮🇹
[Italiano](docs/i18n/it/README.md) | 🇷🇺 [Русский](docs/i18n/ru/README.md) | 🇨🇳
[中文 (简体)](docs/i18n/zh-CN/README.md) | 🇩🇪 [Deutsch](docs/i18n/de/README.md) | 🇮🇳
[हिन्दी](docs/i18n/in/README.md) | 🇹🇭 [ไทย](docs/i18n/th/README.md) | 🇺🇦
[Українська](docs/i18n/uk-UA/README.md) | 🇸🇦 [العربية](docs/i18n/ar/README.md) |
🇯🇵 [日本語](docs/i18n/ja/README.md) | 🇻🇳 [Tiếng Việt](docs/i18n/vi/README.md) | 🇧🇬
[Български](docs/i18n/bg/README.md) | 🇩🇰 [Dansk](docs/i18n/da/README.md) | 🇫🇮
[Suomi](docs/i18n/fi/README.md) | 🇮🇱 [עברית](docs/i18n/he/README.md) | 🇭🇺
[Magyar](docs/i18n/hu/README.md) | 🇮🇩 [Bahasa Indonesia](docs/i18n/id/README.md)
| 🇰🇷 [한국어](docs/i18n/ko/README.md) | 🇲🇾 [Bahasa Melayu](docs/i18n/ms/README.md)
| 🇳🇱 [Nederlands](docs/i18n/nl/README.md) | 🇳🇴 [Norsk](docs/i18n/no/README.md) |
🇵🇹 [Português (Portugal)](docs/i18n/pt/README.md) | 🇷🇴
[Română](docs/i18n/ro/README.md) | 🇵🇱 [Polski](docs/i18n/pl/README.md) | 🇸🇰
[Slovenčina](docs/i18n/sk/README.md) | 🇸🇪 [Svenska](docs/i18n/sv/README.md) | 🇵🇭
[Filipino](docs/i18n/phi/README.md) | 🇨🇿 [Čeština](docs/i18n/cs/README.md)

---

## 🆕 Quoi de neuf dans v3.0.0

> **Mettre à niveau depuis v2.9.5?** — Consultez le [CHANGLOG
> complet](CHANGELOG.md#300--2026-03-22-release-candidate--not-yet-merged-to-main)
> pour toutes les modifications.

| Zone                                     | Modification                                                                                                                                                                                                               |
| ---------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🔒 **CodeQL Security**                    | Réparation de 10+ alertes CodeQL : polymorphism-redos, Randomness Insecure, rectification du shell-injection                                                                                                               |
| ✅ **Validation des routes **             | Toutes les 176 routes API sont désormais validées par des schémas Zod + `validateBody()` —  CI ` vérifie : validation-routes : t06` réussi                                                                                 |
| 🐛 **omniModel Tag Leak**                 | Les étiquettes ` interne <omnimodel> ` ne sont plus transmises aux clients dans les réponses flux en temps réel SSE (#585)</omnimodel>                                                                                     |
| 🔑 **API clés enregistrées**              | Étape d'approvisionnement automatique des API via ` POST /api/v1/clés enregistrées ` avec une limitation de quota par fournisseur/ compte, idempotence, stockage au SHA-256 et signalement facultatif des problèmes GitHub |
| 🎨 **Icônes fournisseurs**                | 130+ logos de fournisseurs via `@lobehub/icons` (SVG) avec PNG → chaîne fallback générique                                                                                                                                 |
| 🔄 Mise à niveau automatique du Modèle ** | Éditeur de programme et bouton de mise à niveau manuel pour synchroniser les listes de modèles pour les fournisseurs intégrés et personnalisés compatibles OpenAI                                                          |
| 🌐 **OpenCode Zen/Go**                    | Deux nouveaux fournisseurs de @kang-heewon via PR #530 : tarifs gratuits + tarifs souscriptions via `OpencodeExecutor`                                                                                                     |
| 🐛 **CLI Gemini OAUTH**                   | Erreur actionable lorsque `GEMINI_OAUTH_CLIENT_SECRET` est manquant dans Docker (étaient des erreurs cryptiques de Google)                                                                                                 |
| 🐛 **config OpenCode**                    | `saveOpenCodeConfig()` écrit maintenant correctement TOML dans `XDG_CONFIG_HOME`                                                                                                                                           |
| 🐛 **surclassement modèles**              | `body.model` est maintenant correctement défini sur `pinnedModel` auprès de la protection de cache de contexte                                                                                                             |
| 🐛 **boucle Codex/Claude**                | `tool_result` blocs sont maintenant convertis en texte pour mettre fin aux boucles infinies                                                                                                                                |
| 🐛 ** redirection de connexion**          | La connexion ne fige plus après avoir sauté la mise au point du mot de passe                                                                                                                                               |
| 🐛 **chemins Windows**                    | Chemins MSYS2/Git-Bash (`/c/...`) normalisés en `C:\...` automatiquement                                                                                                                                                   |

---

## 🖼️ Barre de navigation principale

<div align="center">
  <img src="./docs/screenshots/MainOmniRoute.png" alt="OmniRoute Dashboard" width="800"/>
</div>

---

## 📸 Aperçu de la barre de navigation

<details>
<summary><b>Click to see dashboard screenshots</b></summary>

| Page                     | Écran                                                 |
| ------------------------ | ----------------------------------------------------- |
| **Fournisseurs**         | ![Fournisseurs](docs/screenshots/01-providers.png)    |
| **Combos**               | ![Combos](docs/screenshots/02-combos.png)             |
| **Analyses**             | ![Analyses](docs/screenshots/03-analytics.png)        |
| **Santé**                | ![Santé](docs/screenshots/04-health.png)              |
| **Traducteur**           | ![Traducteur](docs/screenshots/05-translator.png)     |
| **Paramètres**           | ![Paramètres](docs/screenshots/06-settings.png)       |
| **Outils CLI**           | ![Outils CLI](docs/screenshots/07-cli-tools.png)      |
| **Journal de connexion** | ![Connexion](docs/screenshots/08-usage.png)           |
| **Points terminaux**     | ![Points terminaux](docs/screenshots/09-endpoint.png) |

</details>

---

### 🤖 Fournisseur AI gratuit pour vos agents de programmation préférés.

_Se connecter à tout IDE ou outil CLI de type intelligence artificielle via
OmniRoute — borne de routeur de l'API gratuite pour l'infini codage._

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

<sub>📡 Tous les agents se connectent via <code>http://localhost:20128/v1</code>
ou <code>http://cloud.omniroute.online/v1</code> — une seule configuration, un
infinite nombre de modèles et quota</sub>

---

## 🤔 Pourquoi OmniRoute?

**Arrêtez de gaspiller de l'argent et de frapper les limites :**

- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Le quota de la souscription expire inutilisé chaque mois
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Les limites de tarification vous empêchent de coder en milieu de session
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  APIs coûteuses (20 à 50 €/mois par fournisseur)
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  Passer en manuel entre fournisseurs

**OmniRoute résout ce problème :**

- ✅ **Maximiser les souscriptions** - Suivre le quota, utiliser chaque bit avant
  le redémarrage
- ✅ **Changement automatique** - Souscription → Clé API → Chère → Gratuite, zéro
  temps d'arrêt
- ✅ **Multi-compte** - Tourner entre les comptes par fournisseur
- ✅ **Universel** - Fonctionne avec Claude Code, Codex, Gemini CLI, Cursor,
  Cline, OpenClaw, tout outil CLI

---

## 📧 Support

> 💬 **Rejoignez notre communauté !** [Groupe
> WhatsApp](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t) —
> Obtenir de l'aide, partager des conseils, et rester à jour.

- **Site Web** : [omniroute.online](https://omniroute.online)
- **GitHub** :
  [github.com/diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute)
- **Problèmes** :
  [github.com/diegosouzapw/OmniRoute/issues](https://github.com/diegosouzapw/OmniRoute/issues)
- **WhatsApp** : [Groupe de la
  communauté](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)
- **Contribuer** : Voir [CONTRIBUTING.md](CONTRIBUTING.md), ouvrir une PR, ou
  choisir un `bon premier problème`
- **Projet d'origine **: [9le routeur de
  decolua](https://github.com/decolua/9router)

### 🐛 Signaler un bug?

Lorsque vous ouvrez un problème, veuillez exécuter la commande système-info et
attachez le fichier généré :

```bash
npm run system-info
```

Cela génère un `système-info.txt` avec votre version Node.js, la version
OmniRoute, les détails du système d'exploitation, les outils CLI installés
(iflow, gemini, claude, codex, antigravity, droid, etc.), le statut Docker/PM2,
les packages système — tout ce dont nous avons besoin pour reproduire rapidement
votre problème. Attachez le fichier directement à votre problème GitHub.

---

## Comment ça marche

```
┌─────────────┐
│  Votre Outil CLI   │  (Claude Code, Codex, Gemini CLI, OpenClaw, Cursor, Cline...)
│   outil      │
└──────┬──────┘
       │ http://localhost:20128/v1
       ↓
┌─────────────────────────────────────────┐
│           OmniRoute (Routage Intelligente)        │
│  • Format translation (OpenAI ↔ Claude) │
│  • Suivi des quotas + Embeddings + Images │
│  • Réactualisation automatique des jetons │
└──────┬──────────────────────────────────┘
       │
       ├─→ [Niveau 1: Abonnement] Claude Code, Codex, Gemini CLI
       │   ↓ quota épuisé
       ├─→ [Niveau 2: Clé API] DeepSeek, Groq, xAI, Mistral, NVIDIA NIM, etc.
       │   ↓ limite budgétaire
       ├─→ [Niveau 3: ÉCONOMIQUE] GLM ($0,6/1M), MiniMax ($0,2/1M)
       │   ↓ limite budgétaire
       └─→ [Niveau 4: GRATUIT] iFlow, Qwen, Kiro (infini)

Résultat : Ne cessez jamais de coder, coûts minimaux
```

---

## 🎯 Ce qu'OmniRoute résout — 30 problèmes réels et utilisations

> **Tout développeur utilisant des outils AI rencontre ces problèmes
> quotidiennement.** OmniRoute a été conçu pour les résoudre tous — des
> dérapages de coûts aux blocs régionaux, des flux OAuth brisés aux opérations
> de protocole et à l'observabilité d'entreprise.

<details>
<summary><b>💸 1. "I pay for an expensive subscription but still get interrupted by limits"</b></summary>

Les développeurs paient 20-200$/mois pour Claude Pro, Codex Pro ou GitHub
Copilot. Même payant, les quotas ont un plafond — 5h d'utilisation, des limites
hebdomadaires ou des limites par minute. Mi-session de codage, le fournisseur
cesse de répondre et le développeur perd la cadence et la productivité.

**Comment OmniRoute les résout :**

- **Fallback intelligent 4-niveaux** — Si le quota d'abonnement s'épuise,
  redirige automatiquement vers Clé API → ÉCONOMIQUE → GRATUIT avec aucune
  intervention manuelle
- **Suivi des quotas en temps réel** — montre la consommation de jetons en temps
  réel avec le décompte de réinitialisation (5h, quotidien, hebdomadaire)
- **Support Multi-Compte** — Plusieurs comptes par fournisseur avec rattrapage
  automatique — lorsqu'un est épuisé, il bascule sur le suivant
- **Combos personnalisés** — Chaines de fallback personnalisables avec 6
  stratégies de balancement (premier remplissage, rattrapage, P2C, aléatoire,
  moins utilisé, optimisé coût)
- **Quotas d'affaires Codex** — Suivi des quotas d'espace de travail
  d'affaires/équipe directement dans l'interface de dashboard

</details>

<details>
<summary><b>🔌 2. "I need to use multiple providers but each has a different API"</b></summary>

OpenAI utilise une seule forme, Claude (Anthropic) une autre, Gemini encore une
autre. Si un dev veut tester des modèles de différents fournisseurs ou se
basculer entre eux, il doit reconfigurer les SDK, changer les points d'entrée,
gérer les formats incompatibles. Les fournisseurs personnalisés (FriendLI, NIM)
ont des points de terminaison de modèle non standard.

**Comment OmniRoute les résout :**

- **Point de terminaison unifié** — Un seul `http://localhost:20128/v1` sert de
  proxy pour tous les 67+ fournisseurs
- **Traduction de format** — Automatique et transparence : openAI ↔ Claude ↔
  Gemini ↔ API Réponse
- [Réponse Sanitisation**] — Élimine les champs non standard (`x_groq`,
  `usage_breakdown`, `service_tier`) qui viole l'interopérabilité de OpenAI SDK
  v1.83+
- [Normalisation de Rôle**] — Convertit `développeur` → `système` pour les
  fournisseurs non OpenAI ; `système` → `utilisateur` pour GLM/ERNIE
- [Extraction de Balises de Pensement**] — Extraie les `balises de pensement`
  (`<think>`) à partir des modeles comme DeepSeek R1 dans des contenus
  standardisés `raisonnement contenu`</think>
- [Sortie Structuré pour Gemini**] — `schema JSON` →
  `responseMimeType`/`responseSchema` conversion automatique
- `stream` par défaut à `false**` — Aligne avec la spécification OpenAI, évitant
  les erreurs de SSE inattendues dans les SDK Python/Rust/Go

</details>

<details>
<summary><b>🌐 3. "My AI provider blocks my region/country"</b></summary>

Les fournisseurs comme OpenAI/Codex bloquent l'accès à certaines régions
géographiques. Les utilisateurs reçoivent des erreurs comme `Pays non pris en
charge` lors de l'OAuth et des connections API. C'est particulièrement frustrant
pour les développeurs d'aujourd'hui des pays en voie de développement.

**Comment OmniRoute les résout :**

- [Configuration des Proxies 3 Niveaux**] — Configuration du proxy à 3 niveaux :
  globaux (pour toute la trafic), par fournisseur (une seule fournisseur) et par
  connexion / clé
- [Indicateurs de Proxies en Couleurs**] — Indicateurs visuels : 🟢 proxy global,
  🟡 fournisseur proxy, 🔵 connexion proxy, toujours afficher l'adresse IP
- [Echange de jeton OAuth via le Proxy**] — Flux OAuth passe également par le
  proxy, résolvant `Pays non pris en charge`
- [Tentes de Connexion via le Proxy**] — Les tests de connexion utilisent le
  proxy configuré (pas plus de passage direct)
- [Support SOCLE 5**] — Support du proxy SOCKS5 pour canalisation de sortir
- [spoofage de Fingerprint TLS**] — Fingerprint du protocole TLS de navigateur
  via `wreq-js` afin de contourner la détection de bots
- [Traitement du Fingerprint CLI**] — Réordonne les champs de requête et du
  corps pour correspondre aux signatures natives des CLI binaires, réduisant
  drastiquement le risque de flagging des comptes. L’adresse IP du proxy est
  préservée — vous obtenez le même étanchéité ** et** masquage de l’adresse IP
  simultanément

</details>

<details>
<summary><b>🆓 4. "I want to use AI for coding but I have no money"</b></summary>

Personne ne peut payer $20–200/par mois pour les abonnements à l'IA. Les
étudiants, les développeurs d'aujourd'hui les pays émergents, les hobbyistes et
les freelances ont besoin d'accès à des modèles de qualité à coût zéro.

**Comment OmniRoute les résout :**

- [Tiers Gratuits des Fournisseurs Intégrés**] — Support intégré natif de
  fournisseurs gratuits : iFlow (5 modèles gratuits via OAuth :
  kimi-k2-pensement, qwen3-coder-plus, deepseek-r1, minimax-m2, kimi-k2), Qwen
  (4 modèles gratuits : qwen3-coder-plus, qwen3-coder-de-sprint,
  qwen3-coder-suivant, vision-model), Kiro (Claude + ID de constructeur AWS
  gratuite pour gratuits), Gemini CLI (180K jetons / mois gratuits)
- [Ollama Cloud**] — Ollama modèles hébergés en nuage à `api.ollama.com` avec le
  "utilisation gratuite" de la fournisseur ; utilisez `ollamacloud/` prefix
- [Combos uniquement gratuits**] — Chaîner `gc/gemini-3-de-sprint →
  si/kimi-k2-pensement → qw/qwen3-coder-plus` = 0 $/mois avec zéro panne en
  cours de service
- [D'accès gratuit NVIDIA NIM**] — ~40 accès dev-à jamais gratuits RPM ~70+
  modèles à build.nvidia.com (passage de crédits à limites pure rate)
- Stratégie optimisée par rapport au coût[Cost Optimized Strategy] — Stratégie
  de routage qui choisit automatiquement le fournisseur le moins cher disponible

</details>

<details>
<summary><b>🔒 5. "I need to protect my AI gateway from unauthorized access"</b></summary>

Lorsque l'on expose un portail d'intelligence artificielle au réseau (LAN, VPS,
Docker), quiconque possède l'adresse peut consommer les jetons/quotas du
développeur. Sans protection, les API sont vulnérables à l'abus, à l'injection
de prompt et au détournement.

**Comment OmniRoute les résout :**

- Gestionnaire d'API clé [API Key Management] — Génération, rotation et scoping
  par fournisseur avec une page dédiée [dashboard/api-manager] par fournisseur
- Permissions à niveau de modèle [Model-Level Permissions] — Limite les clés API
  aux modèles spécifiques ([openai/*], modèles sauvage), avec affichage de
  permettre tout/Réprimer
- Protection des points de terminaison API [API Endpoint Protection] — Rendez
  compte clé nécessaires pour [/v1/models] et bloque les fournisseurs
  spécifiques de la liste
- Garde de la sécurité Auth + protection CSRF [Auth Guard + CSRF Protection] —
  Toutes les routes du tableau de bord protégées avec le middleware [withAuth] +
  jetons CSRF
- Ebranleur par débit [Rate Limiter] — Débit par-IP avec fenêtres configurables
- Filtre IP [IP Filtering] — Black/white list pour le contrôle d'accès
- Garde d'injection de prompt [Prompt Injection Guard] — Sanitisation contre les
  modèles de prompt malveillants
- Le chiffrement AES-256-GCM [AES-256-GCM Encryption] — Chiffres les
  informations à l'état stationnaire

</details>

<details>
<summary><b>🛑 6. "My provider went down and I lost my coding flow"</b></summary>

Les fournisseurs AI peuvent devenus instables, renvoyer des erreurs 5xx ou
atteindre des plafonds temporaires de débit. Si un développeur dépend d'un seul
fournisseur, il est coupé. Sans les briseurs de circuit, les tentatives de
connexion répétées peuvent bloquer l'application.

**Comment OmniRoute les résout :**

- Circuit Breaker par modèle [Circuit Breaker per-model] — Ouverture/dossier
  automatique avec des seuils et intervalles de fraîcheur configurables
- Retarissement exponentiel [Exponential Backoff] — Délais progressifs
- Anti-tempête d'ancre [Anti-Thundering Herd] — Mutex + protection de semafor
  pour protéger contre les tempêtes de tentatives simultanées
- Champ de chasse en chaine de redondance [Combo Fallback Chains] — Si le
  fournisseur principal échoue, les chenilles automatiques s'abaisser avec
  aucune intervention
- Circuit Breaker Combo [Combo Circuit Breaker] — Automatique désactive les
  fournisseurs échouant dans une chaîne de combo
- Tableau de bord de santé [Health Dashboard] — Monitorage de l'uptime, états
  breaker de circuit, verrouillages, stats du cache, latances p50/p95/p99

</details>

<details>
<summary><b>🔧 7. "Configuring each AI tool is tedious and repetitive"</b></summary>

Les développeurs utilisant le Cursor, le Claude Code, le Codex CLI, l'OpenClaw,
le Gemini CLI, le Kilo Code... Chaque outil nécessite un config différent (point
fin API, clé, modèle). Reconfigurer quand en passant des fournisseurs ou des
modèles est une perte de temps.

**Comment OmniRoute les résout :**

- **Plateforme d'outils CLI[Désignée page avec un seul clic pour
  l'initialisation de la Code Claude, CLI Codex, OpenClaw, Kilo Code,
  Antigravity, Cline
- **Générateur de configuration de GitHub Copilot** — Génère
  `chatLanguageModels.json` pour VS Code avec sélection de modèle en masse
- **Assistant à l'inscription** — Installation guidée à 4 étapes pour les
  utilisateurs débutants
- **Un point de terminaison pour tous les modèles** — Configurez
  `http://localhost:20128/v1` une seule fois, accédez à 67+ fournisseurs

</details>

<details>
<summary><b>🔑 8. "Managing OAuth tokens from multiple providers is hell"</b></summary>

La Code Claude, Codex, Gemini CLI et Copilot utilisent OAuth 2.0 avec des jetons
qui expirent. Les développeurs doivent se réauthentifier constamment, gérer
`client_secret manquant`, `mismatch_redirection_uri` et les échecs sur les
serveurs distants. L'OAuth sur LAN/VPS pose une problématique particulière.

**Comment OmniRoute les résout :**

- **Rafraîchissement automatique des jetons** — Les jetons OAuth se
  réfrachissent en arrière-plan avant expiration
- **OAuth 2.0 (PKCE) Intégré** — Flux automatique pour la Code Claude, Codex,
  Gemini CLI, Copilot, Kiro, Qwen, iFlow
- **OAuth Multi-compte** — Comptes multiples par fournisseur via extraction de
  jeton/ID token
- **Solution OAuth LAN/Remote** — Détection d'adresse IP privée pour
  `redirect_uri` + mode de saisie manuel pour les serveurs distants
- **Guide d'authentication OAuth derrière un Nginx** — Utilise
  `window.location.origin` pour compatibilité de proxy inverse
- **Guide d'authentication OAuth sur un serveur distant** — Guide étape par
  étape pour les crédentials Cloud Google sur VPS/Docker

</details>

<details>
<summary><b>📊 9. "I don't know how much I'm spending or where"</b></summary>

Les développeurs utilisent plusieurs fournisseurs payants mais n'ont pas de vue
unifiée des dépenses. Chaque fournisseur a son propre tableau de bord de
facturation, mais il n'y a pas de vue consolidée. Des coûts imprévus peuvent
s'accumuler.

**Comment OmniRoute les résout :**

- **Tableau de bord d'analyse de coûts** — Suivi du coût par jeton et gestion
  budgétaire par fournisseur
- **Limite de budget par niveau** — Plafond de dépense par niveau qui déclenche
  une alternative automatique
- **Configuration de tarification par modèle** — Tarification configurable par
  modèle
- **Statistiques d'utilisation par clé d'API** — Comptage de requêtes et
  dernière utilisation déterminée par clé
- **Tableau de bord d'analyse** — Cartes statiques, charte d'utilisation de
  modèle, tableau de fournisseur avec taux de réussite et latence

</details>

<details>
<summary><b>🐛 10. "I can't diagnose errors and problems in AI calls"</b></summary>

When a call fails, the dev doesn't know if it was a rate limit, expired token,
wrong format, or provider error. Fragmented logs across different terminals.
Without observability, debugging is trial-and-error.

**Comment OmniRoute les résout :**

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

**Comment OmniRoute les résout :**

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

**Comment OmniRoute les résout :**

- **Tableau de bord i18n — 30 Langues** — Toutes les 500+ clés traduites, y
  compris l'arabe, le bulgare, le danois, l'allemand, l'espagnol, le finnois, le
  français, l'hébreu, l'hindi, le hongrois, l'indonésien, l'italien, japonais,
  coréen, malais, néerlandais, norvégien, polonais, portugais (PT/BR), roumain,
  russe, slovaque, suédois, thaï, ukrainien, vietnamien, chinois, filipino,
  anglais
- **Support RTL** — Support de droite à gauche pour l'arabe et l'hébreu
- **Feuilles de lecture Multi-Langues** — 30 traductions complètes de la
  documentation
- **Sélecteur de Langue** — Icône de la terre dans l'en-tête pour le changement
  en temps réel

</details>

<details>
<summary><b>🔄 13. "I need more than chat — I need embeddings, images, audio"</b></summary>

L'IA ne se limite pas qu'au complétion de conversation. Les développeurs doivent
générer des images, transcrire de l'audio, créer des embeddings pour RAG,
réévaluer des documents et modérer le contenu. Chaque API a une fin de requête
et un format différents.

**Comment OmniRoute les résout :**

- **Embandements** — `/v1/embeddings` avec 6 fournisseurs et 9+ modèles
- **Génération d'Images** — `/v1/images/generations` avec 10 fournisseurs et 20+
  modèles (OpenAI, xAI, Ensemble, Feux d'artifice, Nebius, Hyperbolique,
  NanoBanane, Antigravité, SD WebUI, ComfyUI)
- **Texte à Vidéo** — `/v1/videos/generations` — ComfyUI (AnimateDiff, SVD) et
  SD WebUI
- **Texte à Musique** — `/v1/music/generations` — ComfyUI (Audion Stable Open,
  MusicGen)
- **Transcription Audio** — `/v1/audio/transcriptions` — Whisper + Nvidia NIM,
  HuggingFace, Qwen3
- **Parole Synthèse** — `/v1/audio/speech` — ElevenLabs, Nvidia NIM,
  HuggingFace, Coquí, Tortue, Qwen3, **Inworld**, **Cartesia**, **PlayHT**, +
  fournisseurs existants
- **Modération** — `/v1/moderations` — Contrôles de sécurité pour le contenu
- **Réévaluation** — `/v1/rerank` — Réévaluation de la pertinence des documents
- **API de Réponses** — Support intégral de `/v1/responses` pour Codex

</details>

<details>
<summary><b>🧪 14. "I have no way to test and compare quality across models"</b></summary>

Les développeurs veulent savoir quel modèle est le meilleur pour leur cas
d'utilisation — code, traduction, raisonnement — mais la comparaison manuelle
est lente. Aucun outil d'évaluation intégré n'existe.

**Comment OmniRoute les résout :**

- **Évaluations des LLM** — Test avec ensemble d'or de 10 cas préréglés couvrant
  le bonjour, les mathématiques, la géographie, la génération de code, la
  conformité JSON, la traduction, le markdown, le refus de sécurité
- **4 Stratégies de correspondance** — `exacte`, `contient`, `regex`,
  `personnalisé` (fonction JS)
- **Banc d'essais des Traducteurs** — Essais en batch avec plusieurs entrées et
  sorties attendues, comparaison croisée entre fournisseurs
- **Chat Testeur** — L'ensemble du round-trip avec une représentation visuelle
  de la réponse
- **Mise en surveillance en temps réel** — Flux continu de toutes les requêtes
  traversant le proxy

</details>

<details>
<summary><b>📈 15. "I need to scale without losing performance"</b></summary>

Lorsque le nombre de requêtes augmente, sans mise en cache des mêmes questions
générer des coûts dupliqués. Sans idempotence, les requêtes dupliquées
gaspillent les traitements. Les taux par fournisseur doivent être respectés.

**Comment OmniRoute les résout :**

- **Cache Sémantique** — Cache à deux niveaux (signature + sémantique) réduit le
  coût et la latence
- **Idempotence des requêtes** — Fenêtre de 5s de dé duplication pour les
  requêtes identiques
- **Détection des Limites de Taux** — TPG par fournisseur, espacement minimal et
  suivi simultané maximal
- **Limites de Taux Éditable** — Défauts configuraibles dans Paramètres →
  Résilience avec persistance
- **Cache de validation de la clé API** — Cache à trois niveaux pour les
  performances en production
- **Tableau de bord de l'état de santé avec la téléémetrie** — Latence
  p50/p95/p99, statistiques cache, temps d'activité

</details>

<details>
<summary><b>🤖 16. "I want to control model behavior globally"</b></summary>

Les développeurs qui veulent que toutes les réponses soient dans une langue
spécifique, avec un ton spécifique ou qui veulent limiter les tokens de
raisonnement. La configuration de cela dans chaque outil/requête est
impraticable.

**Comment OmniRoute les résout :**

- **Injection de prompt du système** — Prompt global appliqué à toutes les
  requêtes
- **Validation du budget de pensée** — Contrôle d'allocation des tokens de
  raisonnement par requête (prise en charge, automatique, personnalisé,
  adaptatif)
- **6 stratégies de routage** — Stratégies mondiales qui déterminent comment les
  requêtes sont réparties
- **Routeur Wildcard** — Modèles `fournisseur/*` routent dynamiquement vers tout
  fournisseur
- **Bouton d'activation/désactivation des combinaisons** — Activer/désactiver
  les combinaisons directement depuis le tableau de bord
- **Bouton d'activation/désactivation des fournisseurs** — Activer/désactiver
  toutes les connections pour un fournisseur avec un clic
- **Fournisseurs bloqués** — Exclure des fournisseurs spécifiques de la liste
  `/v1/modèles`

</details>

<details>
<summary><b>🧰 17. "I need MCP tools as first-class product capabilities"</b></summary>

Beaucoup de passerelles AI exposent MDCP uniquement sous forme de détail
d'implémentation caché. Les équipes ont besoin d'une couche d'opération visible
et gérable.

**Comment OmniRoute les résout :**

- Menu de navigation pour MCP et page de protocole d'endpoint
- Page de gestion dédiée de MCP avec processus, outils, champs d'audits et
  tableaux de bord
- Démarrage rapide intégré pour `omniroute --mcp` et inscription client

</details>

<details>
<summary><b>🧠 18. "I need A2A orchestration with sync + stream task paths"</b></summary>

Les workflows de l'agent nécessitent les réponses directes et les éxecutions
longueurs en flux en direct avec contrôle de la durée de vie.

**Comment OmniRoute les résout :**

- Fin de pointe JSON-RPC (`POST /a2a`) avec `message/send` et `message/stream`
- Propagation du flux en flux avec propagation des états terminaux
- APIs de cycle de vie pour `tasks/get` et `tasks/cancel`

</details>

<details>
<summary><b>🛰️ 19. "I need real MCP process health, not guessed status"</b></summary>

Les équipes opérationnelles doivent savoir si MCP est bien en ligne, et non
juste si une API est accessible.

**Comment OmniRoute les résout :**

- Le dernier fichier de signalisation du cœur de la machine avec PID,
  timestamps, transport, nombre d'outil, mode de champ
- API de statut MCP combinant le cœur de la machine + dernière activité
- Les cartes de statut de la page de tableau de bord pour processus, uptime,
  fraîcheur du cœur de la machine

</details>

<details>
<summary><b>📋 20. "I need auditable MCP tool execution"</b></summary>

Lorsque les outils changent la configuration ou déclenchent les actions
d'opération, les équipes ont besoin de la traçabilité forensique.

**Comment OmniRoute les résout :**

- Le journalage d'audit en SQLite pour les appels de l'outil de MCP
- Les filtres en fonction de l'outil, succès/échec, clé API et pagination
- La table de tableau de bord d'audit + les finales de statistique de
  l'automatisation

</details>

<details>
<summary><b>🔐 21. "I need scoped MCP permissions per integration"</b></summary>

Les clients différents devraient avoir les accès les moins privilégiés aux
catégories d'outils.

**Comment OmniRoute les résout :**

- 9 niveaux de portée de MCP granulaires pour un accès contrôlé aux outils
- Contrôle de la portée et de la visibilité dans l'interface d'administration de
  MCP
- Politique de sécurisation par défaut pour la tooling opérationnelle

</details>

<details>
<summary><b>⚙️ 22. "I need operational controls without redeploying"</b></summary>

Les équipes ont besoin de modifications survenues en temps réel pour les
incidents ou les evenements de durée de coût.

**Comment OmniRoute les résout :**

- Activation de la combinaison de mise en prise directement depuis l'interface
  du tableau de bord de MCP
- Application de profils de résilience à partir des packs de politiques
  prédéfinis
- Réinitialisation de l'état de la rupture de circuit à partir du même panneau
  de gestion

</details>

<details>
<summary><b>🔄 23. "I need live A2A task lifecycle visibility and cancellation"</b></summary>

Sans visibilité du cycle de vie, les incidents des tâches deviennent difficiles
à classifier.

**Comment OmniRoute les résout :**

- Listage/filtrage des tâches par état/compétence avec pagination
- Centre de réexion vers les métadonnées, les événements et les artefacts
- Fin de la tâche : bouton de résiliation et action dans l'interface utilisateur
  avec confirmation

</details>

<details>
<summary><b>🌊 24. "I need active stream metrics for A2A load"</b></summary>

Les flux de streaming nécessitent une perception opérationnelle des concurrences
et des connexions en ligne.

**Comment OmniRoute les résout :**

- Comptes de streams actifs intégrés dans l'état de la A2A
- Dernier timestamp de la tâche et comptes par états
- Cartes de A2A pour la surveillance opérationnelle en temps réel

</details>

<details>
<summary><b>🪪 25. "I need standard agent discovery for clients"</b></summary>

Les clients externes et les orchestrateurs nécessitent des métadonnées lisibles
par machine pour l'onboarding.

**Comment OmniRoute les résout :**

- Carte de l'agent exposée à `/.well-known/agent.json`
- Les capacités et compétences sont affichées dans l'interface de gestion
- L'API E2E inclut les métadonnées de découverte pour l'automatisation

</details>

<details>
<summary><b>🧭 26. "I need protocol discoverability in the product UX"</b></summary>

Si les utilisateurs ne peuvent pas découvrir les surfaces du protocole, la
qualité de l'adoption et du soutien augmentent

**Comment OmniRoute les résout :**

- Page consolidée **Endpoints** avec des onglets pour Proxy, MCP, A2A et Api
  Endpoints
- Basculements de statut de service (En ligne/Hors ligne) pour MCP et A2A
- Liens depuis l'vue d'ensemble vers les onglets de gestion dédiés

</details>

<details>
<summary><b>🧪 27. "I need end-to-end protocol validation with real clients"</b></summary>

Les tests de simulation ne suffisent pas pour valider la compatibilité du
protocole avant la mise en production

**Comment OmniRoute les résout :**

- Ensemble de test E2E qui lance l'application et utilise un client de transport
  MCP de développement réel
- Tests du client A2A pour les flux de découverte, d'envoi, de flux en continu,
  de récupération et d'annulation
- Vérifier les assertions croisées contre les APIs audit MCP et A2A tâches

</details>

<details>
<summary><b>📡 28. "I need unified observability across all interfaces"</b></summary>

Diviser l'observabilité par protocole crée des zones d'ombre et des temps de
réparation plus longs

**Comment OmniRoute les résout :**

- Dashboards unifiés/logs/analytics dans un même produit
- Télémétrie de santé+audit+requête à travers les couches OpenAI, MCP et A2A
- API opérationnelles pour le statut et l'automatisation

</details>

<details>
<summary><b>💼 29. "I need one runtime for proxy + tools + agent orchestration"</b></summary>

Exécuter les services multiples augmente les coûts opérationnels et modes de
défaillance.

**Comment OmniRoute les résout :**

- Proxy OpenAI compatible, serveur MCP et serveur A2A dans une pile unique
- Auth partagée, résilience, magasin de données et observabilité
- Modèle de politique cohérent à travers les toutes les surfaces de
  l'interaction

</details>

<details>
<summary><b>🚀 30. "I need to ship agentic workflows without glue-code sprawl"</b></summary>

Les équipes perdent en vitesse lorsqu'elles assemblent plusieurs services et
scripts ad-hoc.

**Comment OmniRoute les résout :**

- Stratégie d'endpoint unifié pour les clients et les agents
- Panneaux de gestion des protocoles intégrés et chemins de validation de fumée
- Fondations prêtes à être utilisées en production (sécurité, journalisation,
  résilience, sauvegarde)

</details>

### Exemples Playbooks ( Cas d'utilisation intégrés )

**Playbook A: Maximiser l'abonnement payant + copie de sauvegarde peu coûteuse
**

```txt
Combinaison : "maximize-claude"
  1. cc/claude-opus-4-6
  2. glm/glm-4.7
  3. if/kimi-k2-pensée

Frais mensuels : 20 $ + petit coût de sauvegarde
Résultat : qualité plus élevée, quasi-interruption nulle
```

**Playbook B: Chaîne de codage à zero coût **

```txt
Combinaison : "libre-à-vivre"
  1. gc/gemini-3-étincelle
  2. if/kimi-k2-pensée
  3. qw/qwen3-coder-plus

Frais mensuels : 0 $
Résultat : flux de codage stable et gratuit
```

**Playbook C: Charte de fallback 24/7 toujours allumée **

```txt
Combinaison : "toujours-allumé"
  1. cc/claude-opus-4-6
  2. cx/gpt-5.2-codex
  3. glm/glm-4.7
  4. minimax/MiniMax-M2.1
  5. if/kimi-k2-pensée

Résultat : profondeur de fallback dédiée aux charges de travail à échéance critique
```

**Playbook D: Opérations d'agent avec MCP + A2A **

```txt
1) Lancer transport MCP (`omniroute --mcp`) pour les opérations dérivées de outils
2) Exécuter les tâches A2A via `message/envoyer` et `message/file`
3) Observez via /dashboard/endpoint (MCP et onglets A2A)
4) Basculer les services via les contrôles en ligne de statut
```

---

## 🆓 Démarrer la gratuité — Coût de configuration nul

> Configurer le codage à l'aide d'IA en quelques minutes à **0 $/mois**.
> Connectez ses comptes gratuits et utilisez la combinaison intégrée **du Staq
> gratuit**.

| Étape | Action                                                      | Fournisseurs Débloqués                                         |
| ----- | ----------------------------------------------------------- | -------------------------------------------------------------- |
| 1     | Se connecter au **Kiro** (AWS Builder ID OAuth)             | Claude Sonnet 4.5, Haïku 4.5 — **illimité**                    |
| 2     | Se connecter au **iFlow** (OAuth Google)                    | kimi-k2-pensé, qwen3-coder-plus, deepseek-r1... — **illimité** |
| 3     | Se connecter au **Qwen** (Code de l'appareil)               | qwen3-coder-plus, qwen3-coder-surtout... — **illimité**        |
| 4     | Se connecter au **Gemini CLI** (OAuth Google)               | gemini-3-scoop, gemini-2.5-pro — **180K/mois gratuits**        |
| 5     | `/ tableau de bord/combos` → **Stack gratuit (0 $)** modèle | Tout rouvrir automatiquement les fournisseurs gratuits         |

**Faites pointer n'importe quel IDE/CLI à : ** `http://localhost:20128/v1` · Clé
API : `chaîne-libre` · Terminé.

> **Couvreur supplémentaire facultatif (également gratuit) : **Clé d'API Groq
> (30 RPM gratuits), NVIDIA NIM (40 RPM gratuits, 70+ modèles), Cerebras (1M
> tok/jour), LongCat Clé d'API (50M jetons/jour !), Workers Cloudflare AI (10K
> Noyaux/jour, 50+ modèles).

## Démarrage rapide

### 1. Installez et exécutez

```bash
npm install -g omniroute
omniroute
```

> **pnpm users:** Exécutez `pnpm approve-builds -g` après l'installation pour
> activer les scripts de build natives nécessaires à `better-sqlite3` et
> `@swc/core` :
> 
> ```bash
> pnpm install -g omniroute
> pnpm approve-builds -g   # Sélectionnez tous les packages → approuvez
> omniroute
> ```

Le tableau de bord s'ouvre à `http://localhost:20128` et l'URL de base de l'API
est `http://localhost:20128/v1`.

| Commande                | Description                                                                 |
| ----------------------- | --------------------------------------------------------------------------- |
| `omniroute`             | Demarrer le serveur (`PORT=20128`, API et tableau de bord sur le même port) |
| `omniroute --port 3000` | Définir le port canonnique/API sur 3000                                     |
| `omniroute --mcp`       | Demarrer le serveur MCP (transport stdio)                                   |
| `omniroute --no-open`   | N'ouvrir pas automatiquement le navigateur                                  |
| `omniroute --help`      | Afficher l'aide                                                             |

Mode de split-port optionnel :

```bash
PORT=20128 DASHBOARD_PORT=20129 omniroute
# API :       http://localhost:20128/v1
# Tableau de bord : http://localhost:20129
```

### 1) Connectez les fournisseurs et créez votre clé API

1. Ouvrez le tableau de bord → `Fournisseurs` et connectez au moins un
   fournisseur (OAuth ou clé API).
2. Ouvrez le tableau de bord → `Point d'entrée` et créez une clé API.
3. (Optionnel) Ouvrez le tableau de bord → `Combos` et définissez votre chaîne
   de remplacement.

### 3) Pointez votre outil de codage sur OmniRoute

```txt
URL de base : http://localhost:20128/v1
Clé API :  [copiez de la page point d'entrée]
Modèle   : si/kimi-k2-pensant (ou le préfixe de fournisseur/modèle)
```

Fonctionne avec Claude Code, Codex CLI, Gemini CLI, Cursor, Cline, OpenClaw,
OpenCode et SDK OpenAI-compatible.

### 4) Activer et valider les protocoles (v2.0)

**MCP (pour les opérations gérées par l'outil): **

```bash
omniroute --mcp
```

Connectez ensuite votre client MCP via `stdio` et testez les outils comme :

- `omniroute_get_health`
- `omniroute_list_combos`

**A2A (pour les flux d'agent-à-agent) :**

```bash
curl http://localhost:20128/.well-known/agent.json
```

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"quickstart","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"Give me a short quota summary."}]}}'
```

### 5) Validez tout du début à la fin (recommandé)

```bash
npm run test:protocols:e2e
```

Ce jeu de tests valide les flux MCP et A2A clients réels contre une application
en cours d'exécution.

### Alternatif : exécutez à partir des sources.

```bash
cp .env.exemple .env
npm install
PORT=20128 DASHBOARD_PORT=20129 NEXT_PUBLIC_BASE_URL=http://localhost:20129 npm run dev
```

---

## 🐳 Docker

OmniRoute est disponible sous forme d'image public Docker sur [Docker
Hub](https://hub.docker.com/r/diegosouzapw/omniroute).

**Lancez rapidement :**

```bash
docker run -d \
  --name omniroute \
  --restart unleash-stopped \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:latest
```

**Avec fichier de configuration :**

```bash
# Copiez et éditez le fichier .env d'abord
cp .env.exemple .env

docker run -d \
  --name omniroute \
  --restart unleash-stopped \
  --env-file .env \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:latest
```

**Utilisez Docker Compose :**

```bash
# Profil de base (pas de outils CLI)
docker compose --profile base up -d

# Profil CLI (Claude Code, Codex, OpenClaw intégré)
docker compose --profile cli up -d
```

| Images                   | Étiquette  | Taille | Description                               |
| ------------------------ | ---------- | ------ | ----------------------------------------- |
| `diegosouzapw/omniroute` | `dernière` | ~250Mo | Version de la dernière mise à jour stable |
| `diegosouzapw/omniroute` | `1.0.3`    | ~250Mo | Version actuelle                          |

---

## 🖥️ Application de bureau — hors ligne & toujours dispo

> 🆕 **NOUVEL! ** OmniRoute est maintenant disponible en tant qu'**application
> desktop native** pour Windows, macOS et Linux.

Exécutez OmniRoute comme application portable de bureau — pas de terminal, ni de
navigateur, ni d'Internet requis pour les modèles locaux.\
La version basée sur Electron de l'application inclut :

- 🖥️ **Fenêtre native** — Fenêtre d'application dédiée avec intégration au
  tableau de notification du système
- 🔄 **Démarage automatique** — Lancer OmniRoute à l'ouverture du système
- 🔔 **Notifications natives** — Recevez les alertes en cas de dépassement de
  quota ou d'erreurs de fournisseur
- ⚡ **Installer en une étape** — NSIS (Windows), DMG (macOS), AppImage (Linux)
- 🌐 **Mode hors ligne** — Fonctionne intégralement en mode hors ligne avec le
  serveur intégré

### Démarrage rapide

```bash
# Mode de développement
npm run electron:dev

# Construire pour votre plate-forme
npm run electron:build           # Plate-forme actuelle
npm run electron:build:win       # Windows (.exe)
npm run electron:build:mac       # macOS (.dmg) — x64 &amp; arm64
npm run electron:build:linux     # Linux (.AppImage)
```

### Tableau de notification

Lorsque la fenêtre de l'application est minimisée, OmniRoute vit dans votre
tableau de notification du système avec des actions rapides :

- Ouvrir le tableau de bord
- Changer le port du serveur
- Quitter l'application

📖 Documentation complète : [`electron/README.md`](electron/README.md)

---

## Tarification à un coup d'œil

| Niveau           | Fournisseur                 | Coût                                 | Réinitialisation de la quotte | Meilleur choix                                 |
| ---------------- | --------------------------- | ------------------------------------ | ----------------------------- | ---------------------------------------------- |
| **💳 ABONNEMENT** | Claude Code (Pro)           | 20 $/mo                              | 5h + hebdomadaire             | Déjà abonné(e)                                 |
|                  | Codex (Plus/Pro)            | 20 $-200 $/mo                        | 5h + hebdomadaire             | Utilisateurs d'OpenAI                          |
|                  | Gemini CLI                  | **GRATUIT**                          | 180K/mo + 1K/jour             | Pour tout le monde !                           |
|                  | Copilote GitHub             | 10 $-19 $/mo                         | Mensuel                       | Utilisateurs GitHub                            |
| **🔑 CODE API**   | NVIDIA NIM                  | **GRATUIT** (dev pour toujours)      | ~40 t.p.m                     | 70+ modèles ouverts                            |
|                  | Cerebras                    | **GRATUIT** (1 M tok/jour)           | 60 000 TPM / 30 t.p.m         | Le plus rapide au monde                        |
|                  | Groq                        | **GRATUIT** (30 t.p.m)               | 14.400 R.p.d                  | Llama/Gemma de très rapide                     |
|                  | DeepSeek V3.2               | 0,27 $ / 1,10 $ par 1 M              | Aucun                         | Meilleure raison / meilleurs prix              |
|                  | xAI Grok-4 Fast             | **0,20 $/0,50 $ par 1 M** 🆕          | Aucun                         | Le plus rapide + appel de l'outil, ultralow    |
|                  | xAI Grok-4 (standard)       | 0,20 $/1,50 $ par 1 M 🆕              | Aucun                         | L'emblème de la prise de décision de xAI       |
|                  | Mistral                     | Essai gratuit + rémunéré             | Tarif limité                  | Intelligence artificielle européenne           |
|                  | OpenRouter                  | Paiement pour utilisation            | Aucun                         | 100+ modèles de rassembler                     |
| ** 💰 CHÈRE **    | GLM-5 (via Z.AI) 🆕          | 0,50 $/1M                            | Journalement 10 AM            | 128 Ko sortie, plus récentement prestige       |
|                  | GLM-4.7                     | 0,60 $/1M                            | Journalement 10 AM            | Sous-traitance budgétaire                      |
|                  | MiniMax M2.5  🆕             | 0,30 $/1M entrée                     | 5 heures de roulement         | Raisonnement + tâches agentiques               |
|                  | MiniMax M2.1                | 0,20 $/1 000 000                     | 5 heures de roulement         | Option la moins chère                          |
|                  | Kimi K2,5 (API Moonshot) 🆕  | Paiement pour utilisation            | Aucun                         | Accès direct à l'API Moonshot                  |
|                  | Kimi K2                     | 0,09 $/moitie fixe                   | 10 000 000 de jetons/mois     | Prix prévisible                                |
| **🆓 Gratuit**    | iFlow                       | **$0**                               | Sans limites                  | 5 modèles sans limites                         |
|                  | Qwen                        | **$0**                               | Sans limites                  | 4 modèles sans limites                         |
|                  | Kiro                        | **$0**                               | Sans limites                  | Claude Sonnet/Haïku (AWS Builder)              |
|                  | LongCat Flash-Lite 🆕        | **$0** (50 000 000 de jetons/jour 🔥) | 1 demande par seconde         | Le quota gratuit le plus important de la Terre |
|                  | Mises en pollinisation IA 🆕 | **$0** (aucune clé nécessaire)       | 1 req/15s                     | GPT-5, Claude, DeepSeek, Llama 4               |
|                  | Cloudflare Workers IA 🆕     | **$0** (10K Neurons/jour)            | ~150 resp/jour                | 50+ modèles, bordure mondiale                  |
|                  | Scaleway IA 🆕               | **$0** (1M jetons totaux)            | Tarif limité                  | UE/RGPD, Qwen3 235B, Llama 70B                 |

> 🆕 **Nouveaux modèles ajoutés (mars 2026):** Grok-4 Fast famille au
> $0,20/$0,50/M (évalué à 1143ms — 30% plus rapide que Gemini 2,5 Flash), GLM-5
> via Z.AI avec 128K de sortie, MiniMax M2,5 raison, DeepSeek V3,2 mises à jour
> de tarification, Kimi K2,5 via Moonshot API direct.

**💡 $0 Pilote Combo — L'ensemble gratuit complet:**

```
# 🆓 Échelle gratuite ultime 2026 — 11 prestataires, $0 à vie
Kiro (kr/)             → Claude Sonnet/Haïku INFINI
iFlow (if/)            → kimik2-penser, qwen3-coder-plus, deepseek-r1 INFINI
LongCat Lite (lc/)     → LongCat-Flash-Lite — 50M de jetons/jour 🔥
Mises en pollinisation (pol/)    → GPT-5, Claude, DeepSeek, Llama 4 — aucune clé nécessaire
Qwen (qw/)             → qwen3-coder-plus, qwen3-coder-Flash, qwen3-coder-suivant INFINI
Gemini (gemini/)       → Gemini 2,5 Flash — 1 500 req/jour clé gratuit d'API
Cloudflare IA (cf/)    → Llama 70B, Gemma 3, Mistral — 10K Neurons/jour
Scaleway (scw/)        → Qwen3 235B, Llama 70B — 1M de jetons gratuits (UE)
Groq (groq/)           → Llama/Gemma ultra-rapide — 14,4K req/jour
NVIDIA NIM (nvidia/)   → 70+ modèles ouverts — 40 RPM à vie
Cerebras (cerebras/)   → Llama/Qwen monde-le plus rapide — 1M tok/jour
```

**Ne coûte rien. Ne s'arrête jamais à coder.** Configurez ceci comme un pilote
combo OmniRoute et tous les redressements se produisent automatiquement — aucune
passerelle manuelle n'est jamais nécessaire.

---

---

## 🆓 Modèles gratuits — Ce que vous obtenez effectivement

> Tous les modèles ci-dessous sont **100% gratuits sans carte de crédit
> exigée**. OmniRoute passe automatiquement entre eux lorsque l'un des quotas
> s'épuise — combinez-les tous pour un combo inébranlable de $0.

### 🔵 MODELES DE CLAUDE (via Kiro — ID de constructeur AWS)

| Modèle              | Préfixe | limit               | Limite de taux                  |
| ------------------- | ------- | ------------------- | ------------------------------- |
| `claude-sonnet-4.5` | `kr/`   | [Tarif illimité] ** | Aucun plafond quotidien signalé |
| `claude-haiku-4.5`  | `kr/`   | [Tarif illimité] ** | Aucun plafond quotidien signalé |
| `claude-opus-4.6`   | `kr/`   | [Tarif illimité] ** | Dernier Opus par Kiro           |

### IFLOW MODELS (OAuth gratuit — Aucune carte de crédit requise) 🟢

| Modèle                       | Préfixe | limit               | Limite de taux        |
| ---------------------------- | ------- | ------------------- | --------------------- |
| `kimi-k2-thinking`           | `if/`   | [Tarif illimité] ** | Aucun plafond signalé |
| `qwen3-coder-plus`           | `if/`   | [Tarif illimité] ** | Aucun plafond signalé |
| [ behaviours_chercheur-r1` ] | `if/`   | [Tarif illimité] ** | Aucun plafond signalé |
| `mode minimax-m2.1`          | `if/`   | [Tarif illimité] ** | Aucun plafond signalé |
| `kimi-k2`                    | `if/`   | [Tarif illimité] ** | Aucun plafond signalé |

### 🟡 MODEL QWEN (Code d'appareil Auth.)

| Modèle                  | Préfixe | limit               | Limite de taux        |
| ----------------------- | ------- | ------------------- | --------------------- |
| `qwen3-coder-plus`      | `qw/`   | [Tarif illimité] ** | Aucun plafond signalé |
| `qwen3-dev-coder-flash` | `qw/`   | [Tarif illimité] ** | Aucun plafond signalé |
| `qwen3-dev-coder-next`  | `qw/`   | [Tarif illimité] ** | Aucun plafond signalé |
| `modèle de vision`      | `qw/`   | [Tarif illimité] ** | Multimodal (images)   |

### 🟣 CLI GEMINI (Authentification Google)

| Modèle                                                | Préfixe | limit                          | Limite de taux             |
| ----------------------------------------------------- | ------- | ------------------------------ | -------------------------- |
| `présentateur de l'arc-en-ciel-gemini-3-flash-aperçu` | `gc/`   | **180 K tok/month** + 1 K/jour | Réinitialisation mensuelle |
| `présentateur de l'arc-en-ciel-2.5-pro`               | `gc/`   | 180 K/month (pool partagé)     | Qualité élevée             |

### ⚫ NVIDIA NIM (Clé d'API gratuite — build.nvidia.com)

| Niveau        | Limite quotidienne         | Limite de taux | Remarques                                                           |
| ------------- | -------------------------- | -------------- | ------------------------------------------------------------------- |
| Gratuit (Dev) | Pas de débouchage de jeton | **~40 RPM**    | 70+ modèles ; passage à des limites de taux purement au milieu 2025 |

Modèles gratuits populaires : `moonshotai/kimi-k2.5` (Kimi K2.5), `z-ai/glm4.7`
(GLM 4.7), `deepseek-ai/deepseek-v3.2` (DeepSeek V3.2),
`nvidia/llama-3.3-70b-instruct`, `deepseek/deepseek-r1`

### ⚪ CEREBRAS (Clé d'API gratuite — inference.cerebras.ai)

| Niveau  | Limite quotidienne | Limite de taux        | Remarques                                                       |
| ------- | ------------------ | --------------------- | --------------------------------------------------------------- |
| Gratuit | **1M tokens/jour** | 60 000 TPM / 30 t.p.m | LLM d'inference le plus rapide au monde ; redéfinit chaque jour |

Disponible gratuitement : `llama-3.3-70b`, `llama-3.1-8b`,
`deepseek-r1-distill-llama-70b`

### 🔴 GROQ (Clé API gratuite — console.groq.com)

| Niveau  | Limite quotidienne | Limite de taux                    | Remarques                                                  |
| ------- | ------------------ | --------------------------------- | ---------------------------------------------------------- |
| Gratuit | **14,4 K RPD**     | 30 requêtes par minute par modèle | Pas de carte de crédit ; 429 en cas de limite, non facturé |

Disponible gratuitement : `llama-3.3-70b-versatile`, `gemma2-9b-it`,
`mixtral-8x7b`, `whisper-large-v3`

### 🔴 LONGCAT AI (Clé API gratuite — longcat.chat) 🆕

| Modèle                        | Préfixe | Quota quotidienne gratuite | Remarques                       |
| ----------------------------- | ------- | -------------------------- | ------------------------------- |
| `LongCat-Flash-Lite`          | `lc/`   | **50M jetons**  💥          | Meilleure quota gratuite jamais |
| `LongCat-Flash-Chat`          | `lc/`   | 500K jetons                | Dialogue multi-tour             |
| `LongCat-Flash-Thinking`      | `lc/`   | 500K jetons                | Raisonnement / CoT              |
| `LongCat-Flash-Thinking-2601` | `lc/`   | 500K jetons                | Version janvier 2026            |
| `LongCat-Flash-Omni-2603`     | `lc/`   | 500K jetons                | Multimodal                      |

> Gratuit à 100 % pendant la bêta publique. Inscrivez-vous à
> [longcat.chat](https://longcat.chat) avec un email ou un téléphone. Résilie
> quotidien à 00:00 UTC.

### 🟢 AI POLLINATIONS ( Pas de clé API nécessaire ) 🆕

| Modèle     | Préfixe | Limite de taux | Fournisseur à l'arrière-plan |
| ---------- | ------- | -------------- | ---------------------------- |
| `openai`   | `pol/`  | 1 req/15s      | GPT-5                        |
| `claude`   | `pol/`  | 1 req/15s      | Anthropic Claude             |
| `gemini`   | `pol/`  | 1 req/15s      | Google Gemini                |
| `deepseek` | `pol/`  | 1 req/15s      | DeepSeek V3                  |
| `llama`    | `pol/`  | 1 req/15s      | Meta Llama 4 Scout           |
| `mistral`  | `pol/`  | 1 req/15s      | Mistral AI                   |

> ✨ **Zéro fric:** Pas d'inscription, ni de clé API. Ajoutez le fournisseur
> Pollinations avec un champ clé vide et cela fonctionne immédiatement.

### 🟠 CLOUDFLARE WORKERS AI (Clé API gratuite - cloudflare.com) 🆕

| Niveau  | Neurones quotidiens | Équivalent d'utilisation                        | Remarques                     |
| ------- | ------------------- | ----------------------------------------------- | ----------------------------- |
| Gratuit | [0X]10,000[8X]      | ~ 150 LLM par rapport / 500s audio / 15K embeds | Paysage mondial, 50 + modèles |

Modèles gratuits populaires : [21X]@cf/meta/llama-3.3-70b-instruct[53X],
[56X]@cf/google/gemma-3-12b-it[82X],
[85X]@cf/openai/whisper-large-v3-turbo[119X] (audio gratuit !),
[136X]@cf/qwen/qwen2.5-coder-15b-instruct[172X]

> Requiert un jeton d'API + ID de compte à partir
> [dash.cloudflare.com](https://dash.cloudflare.com). Stockez l'ID de compte
> dans les paramètres fournisseur.

### 🟣 SCALEWAY AI (1M Jetons gratuit — scaleway.com) 🆕

| Niveau  | Quota gratuit      | Emplacement  | Remarques                                           |
| ------- | ------------------ | ------------ | --------------------------------------------------- |
| Gratuit | [0X]1M jetons[11X] | Paris, UE 🇫🇷 | Aucune carte de crédit nécessairie dans les limites |

Disponibles gratuitement: [16X]qwen3-235b-a22b-instruct-2507[46X] (Qwen3 235B
!), [63X]llama-3.1-70b-instruct[86X],
[89X]mistral-small-3.2-24b-instruct-2506[125X], [128X]deepseek-v3-0324[145X]

> Conformités UE / RGPD. Obtenez la clé API à
> [console.scaleway.com](https://console.scaleway.com).

> [0X] 💡 La stack ultime gratuite (11 fournisseurs, 0 $ pour toujours) : [55X]
> 
> ```
> Kiro (kr/)             → Claude Sonnet/Haiku illimité
> iFlow (if/)            → kimi-k2-thinking, qwen3-coder-plus, deepseek-r1 illimité
> LongCat Lite (lc/)     → LongCat-Flash-Lite — 50M tokens/jour
> Pollinations (pol/)    → GPT-5, Claude, DeepSeek, Llama 4 — aucune clé nécessaire
> Qwen (qw/)             → qwen3-coder modèles illimités
> Gemini (gemini/)       → Gemini 2.5 Flash — 1 500 requêtes/jour gratuites
> Cloudflare AI (cf/)    → 50+ modèles — 10K Neurons/jour
> Scaleway (scw/)        → Qwen3 235B, Llama 70B — 1M jetons gratuits (UE)
> Groq (groq/)           → Llama/Gemma — 14.4K requêtes/jour ultra-rapides
> NVIDIA NIM (nvidia/)   → 70+ modèles ouverts — 40 RPM permanent
> Cerebras (cerebras/)   → Llama/Qwen le plus rapide au monde — 1M tok/jour
> ```

## 🎙️ Combinaison de transcription gratuite

> Transcrit tout audio/vidéo pour **0** — Deepgram commence avec 200 $ gratuits,
> AssemblyAI 50 $ de remplacement, Groq Whisper comme sauvegarde d'urgence
> illimitée.

| Fournisseur      | Crédits Gratuits                 | Meilleur Modèle                               | Limite de taux                                 |
| ---------------- | -------------------------------- | --------------------------------------------- | ---------------------------------------------- |
| 🟢 **Deepgram**   | **200 $ gratuits** (inscription) | `nova-3` — meilleure précision, 30+ langues   | Aucune limite de RPM pour les crédits gratuits |
| 🔵 **AssemblyAI** | **50 $ gratuits** (inscription)  | `universal-3-pro` — chapitres, sentiment, PII | Aucune limite de RPM pour les crédits gratuits |
| 🔴 **Groq**       | **Gratuit pour toujours**        | `whisper-large-v3` — OpenAI Whisper           | 30 RPM (limité à la vitesse)                   |

**Combinaison suggérée dans `/dashboard/combos`:**

```
Nom : free-transcription
Stratégie : Priorité
Nœuds :
  [1] deepgram/nova-3          → utilise les 200 $ gratuits d'abord
  [2] assemblyai/universal-3-pro → remplacement lorsque les crédits Deepgram s'épuisent
  [3] groq/whisper-large-v3    → gratuit pour toujours, sauvegarde d'urgence
```

En ce point `/tableau média` → **Transcription** : télécharger tout fichier
audio ou vidéo → sélectionnez votre point d'axe d'endpoint → obtenir une
transcription dans les formats supportés.

## 💡 Fonctionnalités clefs

OmniRoute v2.0 est conçu comme une plate-forme opérationnelle et non seulement
un relay proxy.

### 🆕 Nouveau - Améliorations inspirées de ClawRouter (mars 2026)

| Fonctionnalité                                | Ce qu'elle fait                                                                                                                       |
| --------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| ⚡ **Grok-4 Fast Family**                      | Modèles A.I. au prix de 0,20/0,50/M — mis au calage 1143ms (30 % plus rapide que Gemini 2.5 Flash)                                    |
| 🧠 ** GLM-5 via Z.AI**                         | Contexte d'output de 128K, 0,5/1M — dernier modèle de la famille GLM                                                                  |
| 🔮 **MiniMax M2.5**                            | Tâches de raisonnement + agencieuses au prix de 0,30/1M — majeur passage à la version M2.1                                            |
| 🎯 **Lancement par modèle de flag par modèle** | Par modèle `lancement par modèle : vrai/faux` dans le registre — AutoCombo manque les modèles non capables de lancement               |
| 🌍 **Détection d'intention multilingue**       | Mots clés PT/ZH/ES/AR dans la notation de score pour AutoCombo — sélection de modèle au meilleur pour le contenu non anglophone       |
| 📊 **Chute de performances bariolée**          | Latence réelle p95 des requêtes en direct alimente le calcul de score pour AutoCombo — AutoCombo apprend à partir des données réelles |
| 🔁 **Suppression de requête dupliquée**        | Fenêtre de suppression basée sur hash du contenu — sécurisé pour les agents multi, prévient les frais de dédoublement                 |
| 🔌 ** Routage de Stratégie Router**            | Extension de l'interface de `Routage de Stratégie` — ajoutez une logique de routage personnalisée en tant que plugins                 |

### 🚀 Précédent v2.0.9+ — Playground, CLI Fingerprints et ACP

| Fonctionnalité                                    | Ce qu'elle fait                                                                                                                                                                                                                                                                                                         |
| ------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🎮 ** Zone de jeu de modèle**                      | Page de tableau de bord pour tester n'importe quel modèle directement — sélectionneurs de fournisseur/Modèle/endpoint, Monaco Editor, streaming, arrêt, temps                                                                                                                                                           |
| 🔏 ** Étiquetage de match de CLI Fingerprints**    | Ordre de header/bandeau par fournisseur pour correspondre aux signatures CLI natives — basculez par fournisseur dans Sécurité > Paramètres. **Votre IP proxy est préservée**                                                                                                                                            |
| 🤝 ** Support de ACP (Protocole d'Agent Client)**  | Découverte d'agent CLI (Codex, Claude, Goose, Gemini CLI, OpenClaw + 9 autres), lancement de processus, `/api/acp/agents` point de terminaison                                                                                                                                                                          |
| 🤖 ** Tableau de bord des agents ACP**             | Détenteurs › Agents page — grille des 14 agents avec statut d'installation, version, formulaire d'agent personnalisé pour tout outil CLI. **Utilisateurs d'OpenCode** obtiennent un bouton "Téléchargez opencode.json" qui génère automatiquement une configuration prête à l'emploi avec tous les modèles disponibles. |
| 🔧 ** Routage personnalisé `apiFormat` de modèle** | Les modèles personnalisés avec `apiFormat: "réponses"` routent maintenant correctement vers le traducteur de API de réponse                                                                                                                                                                                             |
| 🏢 ** Isolation de l'espace de travail Codex**     | Plusieurs espaces de travail Codex par email — OAuth sépare correctement les connections par ID de workspace                                                                                                                                                                                                            |
| 🔄 ** Mise à jour automatique d'Electron**         | L'application bureau vérifie les mises à jour + installe automatiquement à la réinitialisation                                                                                                                                                                                                                          |

### 🤖 Opérations d'agent et de protocole (v2.0)

| Fonctionnalité                                            | Ce qu'elle fait                                                                                                                |
| --------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| 🔧 **Serveur MCP (16 outils)**                             | IDE/agent tools via 3 transports: stdio, SSE (`/api/mcp/sse`), Streamable HTTP (`/api/mcp/stream`)                             |
| 🤝 **Serveur A2A (JSON-RPC + SSE)**                        | Exécution de tâches agent à agent avec des flux synchrones et en streaming                                                     |
| 🧭 **Page de points de terminaison consolidés**            | Page de gestion multiprise avec les boutons Proxy de point de terminaison, MCP, A2A et API                                     |
| 🎚️ **Alternateurs d'activation/désactivation de service** | Vérrous ON/OFF pour MCP et A2A avec persistance des paramètres (par défaut : OFF)                                              |
| 🛰️ **Pulse de cœur du runtime MCP**                       | Statut réel du processus (pid, uptime, âge de la pulsation, transport et mode de portée)                                       |
| 📋 **Fichier de journal de connexion MCP**                 | Filtres les journaux de connexion avec succès/échec et attribution du clé                                                      |
| 🔐 **Application du droit de portée MCP**                  | 9 droits de portée granulaires pour un accès contrôlé aux outils                                                               |
| 📡 **Gestion du cycle de vie de la tâche A2A**             | Affichez et réglez les tâches, inspectez les événements/artéfacts, annulez les tâches en cours                                 |
| 📋 **Découverte de la carte agent**                        | `/.well-known/agent.json` pour une découverte client automatique                                                               |
| 🧪 Protocole E2E Test Harness**                            | Vraies SDK MCP + clients A2A flux dans `test:protocols:e2e`                                                                    |
| ⚙️ **Commandes Opérationnelles**                          | Combo de commutateurs, mise en œuvre de profils de résilience, réinitialisation de breakers à partir d'une surface de contrôle |

### 🧠 Intelligence & Routage

| Fonctionnalité                              | Ce qu'elle fait                                                                                |
| ------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| 🎯 **Smart Echelonner à 4 Niveaux**          | Route automatique : Abonnement → Clé API → Chèque → Gratuit                                    |
| 📊 **Suivi de Quotas en Temps Réel**         | Comptage de jetons en direct + compteur de réinitialisation par fournisseur                    |
| 🔄 **Traduction de Format**                  | OpenAI ↔ Claude ↔ Gemini ↔ Conversions avec conversions sécurisées sous schéma                 |
| 👥 **Support Multi-Compte**                  | Plusieurs comptes par fournisseur avec sélection intelligente                                  |
| 🔄 **Rafraîchissement Automatique du Jeton** | Les jetons OAuth se rafraîchissent automatiquement avec redémarrage                            |
| 🎨 **Combos Personalisés**                   | 6 stratégies de rodage équilibrées + contrôle de la chaîne de fallback                         |
| 🌐 **Routeur Wildcard**                      | `fournisseur/*` routage dynamique                                                              |
| 🧠 **Pensée Gestion budgetaire**             | Acheminement libre, automatique, personnalisé, et limite de raisonnement adaptatif             |
| 🔀 **Ébauches de modèle**                    | Ébauches de modèle intégrées et personnalisées ainsi que la sécurité de migration              |
| ⚡ **Dégradation de fond d'écran**           | Acheminement des tâches de fond de priorité basse vers des modèles moins chers                 |
| 🧪 **Routage intelligent tâche-conscience**  | Sélection automatisée du modèle en fonction du type de contenu (codage/vision/analyse/summary) |
| 💬 **Injection de prompt systéme**           | Contrôles de comportement globaux appliqués de manière cohérente                               |
| 📄 **Compatibilité des API de réponse**      | Soutien complet `/v1/responses` pour Codex et flux de travail avancés agentiques               |

### 🎵 APIs multi-modal

| Fonctionnalité              | Ce qu'elle fait                                                                                                                                                                        |
| --------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🖼️ **Génération d'images**  | `/v1/images/generations` en arrière-plan cloud et local                                                                                                                                |
| 📐 **Inséquences**           | `/v1/embeddings` pour les pipelines de recherche et RAG                                                                                                                                |
| 🎤 **Transcription Audio**   | `/v1/audio/transcriptions` — 7 fournisseurs (Deepgram Nova 3, AssemblyAI, Groq Whisper, HuggingFace, ElevenLabs, OpenAI, Azure), détection automatique de langage, support MP4/MP3/WAV |
| 🔊 **Parole en texte**       | `/v1/audio/speech` — 10 fournisseurs (ElevenLabs, OpenAI, Deepgram, Cartesia, PlayHT, HuggingFace, Nvidia NIM, Inworld, Coqui, Tortoise) avec des messages d'erreur corrects           |
| 🎬 **Génération de vidéos**  | `/v1/videos/generations` (ComfyUI + SD WebUI workflows)                                                                                                                                |
| 🎵 **Génération de musique** | `/v1/music/generations` (ComfyUI workflows)                                                                                                                                            |
| 🛡️ **Médications**          | `/v1/moderations` contrôles de sécurité                                                                                                                                                |
| 🔀 **Reranking**             | `/v1/rerank` pour la notation de pertinence                                                                                                                                            |
| 🔍 **Recherche web** 🆕       | `/v1/search` — 5 fournisseurs (Serper, Brave, Perplexity, Exa, Tavily), 6 500 + gratuit / mois, redondance automatique, cache                                                          |

### 🛡️ Résilience, Sécurité & Gouvernance

| Fonctionnalité                                                                          | Ce qu'elle fait                                                                                                                   |
| --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| 🔌 **Coupe de circuit**                                                                  | La reprise modèle / par voyage avec des contrôles de seuil                                                                        |
| 🎯 **Modèles conscients des points de terminaison**                                      | 🛡️ [X3X]Défense contre l'hébédomadaire de tempête[X25X]                                                                           |
| Synchronisation + protection des sémaphores lors des événements de réessai/tarification | Réduction des coûts/teneur avec deux couches de cache                                                                             |
| 🧠 **Caching sémantique + signature**                                                    | Réduction de l'effort/latence avec deux couches de cache                                                                          |
| ⚡ **Idempotence de la demande**                                                         | Fenêtre de protection contre les doublons                                                                                         |
| 🔒 **Empoisonnement de l'empreinte TLS**                                                 | Empreinte d'empreinte du client natif TLS — **réduit la détection des bots et le rappel du compte**                               |
| 🔏 ** Étiquetage de match de CLI Fingerprints**                                          | Correspond au signature du requêtage natif du CLI — **réduit le risque de bannissement tout en préservant l'adresse IP du proxy** |
| 🌐 **Filtrage IP**                                                                       | Contrôle permettant/déclaratif des déploiements exposés                                                                           |
| 📊 **Plafonds de débit éditable**                                                        | Limites globales/définies par fournisseur avec persistance                                                                        |
| 🔑 **Gestion + scoping de la clé API**                                                   | Déploiement sécurisé de l'émission/rotation de clés et de contrôles du modèle/fournisseur                                         |
| 🛡️ **Modèles protégés `/`**                                                             | Garding d'authentification optionnelle et masquage des fournisseurs pour le catalogue de modèles                                  |

### 📊 Observation et Analytique &

| Fonctionnalité                             | Ce qu'elle fait                                                        |
| ------------------------------------------ | ---------------------------------------------------------------------- |
| 📝 Demande + Journalisation Proxy**         | Journalage complet de demande/réponse et journalisation proxy          |
| 📋 Tableau de bord de journaux unifié**     | Vues demande, proxy, audit et console sur une page                     |
| 🔍 **Analyse de Temps de Requête**          | Latence p50/p95/p99 et suivi de demande                                |
| 🏥 Tableau de bord d'Etat de santé**        | Disponibilité, états Breaker, blocages, statistiques cache             |
| 💰 Suivi des Frais**                        | Contrôle de budget et visibilité des tarifs par modèle                 |
| 📈 **Visualisations des Données d'Analyse** | Connaissances d'utilisation du modèle/ FOURNISSEUR et vues de tendance |
| 🧪 **Cadre d'Evaluation**                   | Tests de jeu doré avec des stratégies de correspondance configurables  |

### ☁️ Déploiement et Plateforme

| Fonctionnalité                                    | Ce qu'elle fait                                                                        |
| ------------------------------------------------- | -------------------------------------------------------------------------------------- |
| 🌐 **Déployer Partout**\                           | Localhost, VPS, Docker, Environnements Cloud                                           |
| 💾 **Cloud Sync**                                  | Synchronisation de configuration via travailleur cloud                                 |
| 🔄 **Backup/Restore**                              | Flux d'exportation/importation et de récupération après sinistre                       |
| 🧙 ** Assistant de démarrage gui**                 | Configuration guidée de démarrage                                                      |
| 🔧 **Outil de ligne de commande  Tableau de bord** | Configuration facile pour les outils de codage populaires                              |
| 🎮 ** Zone de jeu de modèle**                      | Tester tout fournisseur/modèle/point de terminaison depuis le tableau de bord          |
| 🔏 ** Tiroir d'empreinte CLI (afficher)**          | Correspondance d'empreinte au niveau des fournisseurs dans le menu Sécurité > Sécurité |
| 🌐 ** Traduction i18n (30 langages)**              | Support de langages complet pour l'interface utilisateur + docs avec couverture RTL    |
| 🧹 ** Effacer tous les modèles**                   | Effacer la liste de modèles en un clic dans les détails du fournisseur                 |
| 📋 ** Modèles de problème**                        | Modèles GitHub standardisés pour les bugs et les fonctionnalités                       |
| 📂 ** Répertoire de données personnalisé**         | `Répertoire des données` takeover pour emplacement de stockage                         |

### Fonctionnement en profondeur

#### Changement automatique avec contrôle des coûts pratiques

```txt
Combinaison : "ma pile de codage"
  1. cc/claude-opus-4-6
  2. nvidia/llama-3.3-70b
  3. glm/glm-4.7
  4. if/kimi-k2-thinking
```

Lorsque la quote, le taux ou l'état de santé échoue, OmniRoute passe
automatiquement au candidat suivant sans avoir besoin d'une opération manuelle.

#### Gestion des protocoles visible et opérationnel

- MCP + A2A sont décrits dans l'interface Utilisateur et dans le rapport (ne
  sont pas cachés)
- Les APIs de statut des protocoles exposent des données opérationnelles en
  temps réel (`/api/mcp/*`, `/api/a2a/*`)
- Les Tableaux de bord comprennent des actions pour les opérations jour 2
  (maillage à bascule, reinitialisation des bris, annulation de la tâche)

#### Découpe de l'écrivant + flux de validation

La zone Écrivain comprend :

- **Terrain de jeu** : contrôle des vérifications de transformation
- **Testeur de Chat** : ronds-trip demande/réponse en un seul passage
- **Banc d'essai** : plusieurs cas en un seul passage
- **Surveiller en temps réel** : vue de flux trafic en temps réel

Plus validation de procotol avec clients réels via `npm run test:protocols:e2e`.

> 📖 **Lecture Matérielle du Serveur MCP(open-sse/mcp-server/README.md)** —
> Référence de l'outil, configurations IDE et exemples de clients
> 
> 📖 **Lecture Matérielle du Serveur A2A(src/lib/a2a/README.md)** — Compétences,
> méthodes JSON-RPC, streaming, et cycle de vie de tâche

## 🧪 Évaluations (Évals)

OmniRoute inclut un cadre d'évaluation intégré pour tester la qualité des
réponses des LLM par rapport à un ensemble d'or. Accédez-y via **Analyses →
Évals** sur le tableau de bord.

### Enregistrement intégré de l'ensemble d'or

L'ensemble prédéfini "OmniRoute d'or intégré" contient des cas de test pour :

- Bonjour, mathématiques, géographie, génération de code
- Compatibilité avec la norme JSON, traduction, génération de markdown
- Refus de sécurité (contenu nuisible), comptage, logique booléenne

### Stratégies d'évaluation

| Stratégie  | Description                                                   | Exemple                                |
| ---------- | ------------------------------------------------------------- | -------------------------------------- |
| `exacts`   | La sortie doit corresponder exactement                        | `"4"`                                  |
| `contient` | La sortie doit contenir une sous-zone (insensible à la casse) | `"Paris"`                              |
| `regex`    | La sortie doit correspondre à un modèle regex                 | `"1.*2.*3"`                            |
| `custom`   | La fonction JS personnalisée renvoie vrai/faux                | `(sortie) =&gt; sortie.length &gt; 10` |

---

## 📖 Guide de configuration

### Modes de configuration du protocole (MCP + A2A)

<details>
<summary><b>🧩 MCP Setup (Model Context Protocol)</b></summary>

Démarrer le transport MCP sous mode stdio :

```bash
omniroute --mcp
```

Recommandé flux de validation :

1. Connectez votre client MCP sur stdio.
2. Exécutez `omniroute_get_health`.
3. Exécutez `omniroute_list_combos`.
4. Ouvrez `/dashboard/mcp` pour confirmer le signal d’activité, l’activité et
   l’audit.

_APIs utiles pour l'automatisation :

- `GET /api/mcp/statut`
- `GET /api/mcp/outils`
- `GET /api/mcp/audit`
- `GET /api/mcp/audit/stats`

</details>

<details>
<summary><b>🤝 A2A Setup (Agent2Agent)</b></summary>

Découvrez l'agent :

```bash
curl http://localhost:20128/.well-known/agent.json
```

Envoyez une tâche :

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"setup-a2a","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"Résumer le statut des quotas."}]}}'
```

Gérer le cycle de vie :

- `GET /api/a2a/status`
- `GET /api/a2a/tâches`
- `GET /api/a2a/tâches/:id`
- `POST /api/a2a/tâches/:id/annuler`

Interface de synthèse opérationnelle :

- `/plateforme_dashboard/a2a` pour l'observabilité et les actions de fumée des
  tâches/états/flux

</details>

<details>
<summary><b>🧪 End-to-end protocol validation</b></summary>

Validez les deux protocoles avec des clients réels :

```bash
npm run test:protocols:e2e
```

Cela vérfie :

- Client MCP SDK connect/list/call
- Découverte A2A/envoyer/flot/ obtenir/annuler
- Vérifiez les données dans les API de contrôle d'accès et de gestion des tâches
  A2A

</details>

<details>
<summary><b>💳 Subscription Providers</b></summary>

### Claude Code (Pro/Max)

```bash
Plateforme → Fournisseurs → Connectez-vous à Claude Code
→ Connexion OAuth → Rafraîchissement automatique de l'application
→ Suivi de la limite de 5 heures + hebdomadaire

Modèles:
  cc/claude-opus-4-6
  cc/claude-sonnet-4-5-20250929
  cc/claude-haiku-4-5-20251001
```

**Conseil Pro : ** Utilisez Opus pour les tâches complexes, Sonnet pour la
vitesse. OmniRoute suit les limites par modèle !

### OpenAI Codex (Plus/Pro)

```bash
Plateforme → Fournisseurs → Connectez-vous à Codex
→ Connexion OAuth (port 1455)
→ Réinitialisation hebdomadaire + 5 heures

Modèles:
  cx/gpt-5.2-codex
  cx/gpt-5.1-codex-max
```

#### Gestion des limites du compte Codex (5h + Hebdomadaire)

Chaque compte Codex est désormais équipé de boutons de paramètres de politique
dans `Plateforme -&gt; Fournisseurs` :

- `5h` (ACTIVER/DÉACTIVER) : appliquer la politique de plage de 5 heures
  Threshold.\
  ==WEBLATE_PART==
- `Sélective` (ALL/ARRETER): fait appliquer la politique de seuil de fenêtre
  hebdomadaire.
- Comportement de seuil : lorsqu'une fenêtre activée atteint ≥ 90 %
  d'utilisation, le compte est sauté.
- Comportement de rotation : OmniRoute route automatiquement vers le prochain
  compte Codex éligible.
- Comportement de réinitialisation : lorsqu'il passe le temps de
  réinitialisation fourni `resetAt`, le compte devient éligible à nouveau
  automatiquement.

Scénarios :

- `5h ON` + `Hebdo ON` : le compte est sauté lorsqu'une fenêtre atteint le
  seuil.
- `5h OFF` + `Hebdo ON` : la seule utilisation hebdomadaire peut bloquer le
  compte.
- `5h ON` + `Hebdo OFF` : la seule utilisation de 5 heures peut bloquer le
  compte.
- `resetAt` dépassé : le compte repasse automatiquement dans la rotation (aucune
  réactivation manuelle nécessaire).

### CLI Gemini (GRATUIT 180K/mois !)

```bash
Tableau de bord → Fournisseurs → Connectez-vous au CLI Gemini
→ Google OAuth
→ 180K compléments de vocabulaire/mois + 1K/jour

Modèles :
  gc/gemini-3-preview-avec-imagination
  gc/gemini-2.5-pro
```

**Meilleure valeur :** Huge niveau de gratification gratuit ! Utilisez ceci
avant les niveaux payants.

### Copilote GitHub

```bash
Tableau de bord → Fournisseurs → Connect GitHub
→ OAuth via GitHub
→ Réinitialisation mensuelle (1er jour du mois)

Modèles :
  gh/gpt-5
  gh/claude-4.5-sonnet
  gh/gemini-3-pro
```

</details>

<details>
<summary><b>🔑 API Key Providers</b></summary>

### NVIDIA NIM (GRATUIT accès en tant qu'éditeur — 70+ modèles)

1. S'inscrire : [build.nvidia.com](https://build.nvidia.com)
2. Obtenez le clé API gratuite (1 000 crédits d'inférence inclus)
3. Tableau de bord → Ajouter un fournisseur → NVIDIA NIM :
   - Clé API : ` nvapi-votre-clé `

**Modèles:** ` nvidia/llama-3.3-70b-instruct`, ` nvidia/mistral-7b-instruct` et
50+ plus

**Conseil EXPERT : ** L'API compatible avec OpenAI fonctionne en toute
transparence avec la traduction de format OmniRoute !

### DeepSeek

1. Inscription : [platform.deepseek.com](https://platform.deepseek.com)
2. Obtenez une clé API
3. Tableau de bord → Ajouter un fournisseur → DeepSeek

**Modèles : ** ` deepseek/deepseek-chat`, ` deepseek/deepseek-coder`

### Groq (Tarif gratuit disponible !)

1. Inscription : [console.groq.com](https://console.groq.com)
2. Obtenir une clé API (tarif gratuit inclus)
3. Tableau de bord → Ajouter un fournisseur → Groq

**Modèles : ** ` groq/llama-3.3-70b`, ` groq/mixtral-8x7b`

**Conseil EXPERT : ** Inférence ultra-rapide — idéal pour un codage en temps
réel !

### OpenRouter (100+ Modèles)

1. Inscription : [openrouter.ai](https://openrouter.ai)
2. Obtenez une clé API
3. Tableau de bord → Ajouter un fournisseur → OpenRouter

**Modèles : ** Accès à 100+ modèles de tous les principaux fournisseurs via une
seule clé API.

</details>

<details>
<summary><b>💰 Cheap Providers (Backup)</b></summary>

### GLM-4.7 (Réinitialisation quotidienne, 0,6 $/1 000 000)

1. Inscription : [Zhipu AI](https://open.bigmodel.cn/)
2. Obtenir une clé API du Plan de codage
3. Panneau de commande → Ajouter une clé API :
   - Fournisseur : `glm`
   - Clé API : `votre-clé`

**Utilisez:** `glm/glm-4.7`

**Conseil avancé:** Le Plan de développement offre 3 x quota au 1/7ème coût !
Réinitialisation quotidienne 10h00.

### MiniMax M2.1 (5h de réinitialisation, 0,20 $ / 1 M)

1. Inscrivez-vous: [MiniMax](https://www.minimax.io/)
2. Obtenez une clé API
3. Panneau de commande → Ajouter une clé API

**Utilisez:** `minimax/MiniMax-M2.1`

**Conseil avancé:** La meilleure option pour un grand contexte (1 million de
jetons)!

### Kimi K2 (9,00 $ par mois de manière flat)

1. Abonnez-vous: [Moonshot AI](https://platform.moonshot.ai/)
2. Obtenez une clé API
3. Panneau de commande → Ajouter une clé API

**Utilisez:** `kimi/kimi-latest`

**Conseil avancé:** Coût effectif de 0,90 $ par million de jetons pour une
fixation de 9,00 $ par mois pour 10 millions de jetons!

</details>

<details>
<summary><b>🆓 FREE Providers (Emergency Backup)</b></summary>

### iFlow (5 modèles gratuits via OAuth)

```bash
Panneau de commande → Se connecter à iFlow
→ S'authentifier avec iFlow via OAuth
→ Utilisation illimitée

Modèles :
  if/kimi-k2-étiquette
  if/qwen3-coder-plus
  if/glm-4.7
  if/minimax-m2
  if/deepseek-r1
```

### Qwen (4 Modèles gratuits via Code de dispositif)

```bash
Écran de tableau de bord → Connectez-vous à Qwen
→ Autorisation du code de l'appareil
→ Utilisation illimitée

Modèles :
  qw/qwen3-coder-plus
  qw/qwen3-coder-flash
```

### Kiro (Claude GRATUIT)

```bash
Écran de tableau de bord → Connectez-vous à Kiro
→ ID du bâtisseur AWS ou Google/GitHub
→ Utilisation illimitée

Modèles :
  kr/claude-sonnet-4.5
  kr/claude-haiku-4.5
```

</details>

<details>
<summary><b>🎨 Create Combos</b></summary>

### Exemple 1 : Maximize Subscription → Ligne de défense peu coûteuse

```
Écran de tableau de bord → Combinations → Créez un nouveau

Nom : codage premium
Modèles :
  1. cc/claude-opus-4-6 (Principal par abonnement)
  2. glm/glm-4.7 (Ligne de défense peu coûteuse, 0,6 $/1 000 000)
  3. minimax/MiniMax-M2.1 (Champion le moins cher, 0,2 $/1 000 000)

Utilisation dans CLI : codage premium
```

### Exemple 2 : Gratuit (Coût : 0 $)

```
Nom : combinaison gratuite
Modèles :
  1. gc/gemini-3-flash-preview (180 000 gratuit/mois)
  2. if/kimi-k2-thinking (illimité)
  3. qw/qwen3-coder-plus (illimité)

Coût : 0 $ toute la vie !
```

</details>

<details>
<summary><b>🔧 CLI Integration</b></summary>

### Curseur IDE

```
Paramètres → Modèles → Avancé :
  URL de base de l'API OpenAI : http://localhost:20128/v1
  Clé d'API OpenAI : [clé définie dans l'interface OmniRoute]
  Modèle : cc/claude-opus-4-6
```

### Claude Code

Utilisez l'interface **Outil de ligne de commande** dans l'écran de tableau de
bord pour une configuration rapide, ou éditez `~/.claude/settings.json`
manuellement.

### Outil de ligne de commande Codex

```bash
export OPENAI_BASE_URL="http://localhost:20128"
export OPENAI_API_KEY="votre-clé-api-omniroute"

codex "votre requête"
```

### OpenClaw

**Option 1 — Écran de tableau de bord (recommandé) : **

```
Écran de tableau de bord → Outils de ligne de commande → OpenClaw → Sélectionner le modèle → Appliquer
```

**Option 2 — Manuel : ** Éditez `~/.openclaw/openclaw.json` :

```json
{
  "models": {
    "fournisseurs": {
      "omniroute": {
        "baseUrl": "http://127.0.0.1:20128/v1",
        "apiKey": "sk_omniroute",
        "api": "openai-completions"
      }
    }
  }
}
```

> **Remarque : ** OpenClaw ne fonctionne qu'avec OmniRoute local. Utilisez
> `127.0.0.1` au lieu de `localhost` pour éviter les problèmes de résolution
> IPv6.

### Ligne de commande Cline / Continue / RooCode

```
Paramètres → Configuration de l'API :
  Fournisseur : OpenAI Compatible
  URL de base : http://localhost:20128/v1
  Clé API : [clé obtenue à partir de OmniRoute]
  Modèle : if/kimi-k2-thinking
```

### OpenCode

**Étape 1 :** Ajoutez OmniRoute comme fournisseur personnalisé :

```bash
opencode
/connect
# Sélectionnez "Autre" → Entrez l'ID : "omniroute" → Entrez votre clé API OmniRoute
```

**Étape 2 :** Créez/modifiez `opencode.json` dans le répertoire root de votre
projet :

```json
{
  "$schema": "https://opencode.ai/config.json",
  "fournisseur": {
    "omniroute": {
      "npm": "@ai-sdk/openai-compatible",
      "nom": "OmniRoute",
      "options": {
        "baseURL": "http://localhost:20128/v1"
      },
      "modèles": {
        "cc/claude-sonnet-4-20250514": { "nom": "Claude Sonnet 4" },
        "gg/gemini-2.5-pro": { "nom": "Gemini 2.5 Pro" },
        "if/kimi-k2-thinking": { "nom": "Kimi K2 ( Gratuit)" }
      }
    }
  }
}
```

**Étape 3 :** Sélectionnez le modèle dans OpenCode :

```bash
/models
# Sélectionnez n'importe quel modèle d'OmniRoute proposé dans la liste
```

> **Conseil :** Ajoutez tout modèle disponible à votre point d'extrémité
> `/v1/models` dans la section `modèles`. Utilisez la mise en forme
> `fournisseur/model-id` à partir de votre tableaux de bord d'OmniRoute.

</details>

---

## Dépannage

<details>
<summary><b>Click to expand troubleshooting guide</b></summary>

**"Le modèle de langage n'a pas fourni d'informations"**

- Le quota du fournisseur est épuisé → Vérifiez la table d'état de la limite de
  quota
- Solution : Utilisez un retournement de combinaison ou basculer dans un niveau
  tarifaire moins cher

**Limitation de taux**

- Le quota de l'abonnement est épuisé → Recourir à GLM/MiniMax
- Ajoutez un combo : `cc/claude-opus-4-6 → glm/glm-4.7 → if/kimi-k2-thinking`

**"Le jeton OAuth s'est expiré"**

- Renouvelé automatiquement par OmniRoute
- Si les problèmes persistent : Tableau de bord → Fournisseur → Reconnecter

**Coûts élevés**

- Vérifiez les statistiques d'utilisation sur Tableau de bord → Coûts
- Switcher le modèle primaire en GLM/MiniMax
- Utilisez la version gratuite (Gemini CLI, iFlow) pour les tâches critiques

Tableau de bord/[API ports][31X] sont incorrects

- La port[5X] est le port basique canonique (et par défaut la port[9X] API
  seulement en cas d'open-api)
- La port[9X] API override uniquement la listeeneur [open-AI]-compatible.
- La port[15X] Dashboard override uniquement le listener Dashboard/next.js
- Définissez [NEXT_PUBLIC_BASE_URL][25X] sur la URL du public de votre tableau
  de bord (pour les redirections OAuth)

Erreurs Cloud sync

- Vérifiez que [BASE_URL][16X] pointe vers votre instance en cours d'exécution
- Vérifiez que [CLOUD_URL][17X] pointe vers votre point finale de cloud attendu
- Gardez les valeurs [NEXT_PUBLIC_*][19X] alignées sur les valeurs côté serveur

Premier login ne fonctionne pas

- Vérifiez [INITIAL_PASSWORD][23X] dans .env[33X]
- Si non défini, le mot de passe par défaut de fallback est [123456][38X]

Pas de journaux de requête

- Définissez [ENABLE_REQUEST_LOGS=true][29X] dans .env[39X]

Test de connexion montre "Invalid" pour les fournisseurs OpenAI-compatible

- De nombreuses fournisseurs ne publient pas un endpoint /models [38X]
- OmniRoute v1.0.6+ inclut la validation de fallback via les terminaisons de
  dialogue.
- Assurez-vous que l'URL de base inclut la sous-mention `/v1` suffixe

### Authentification OAuth sur un Serveur Régional 🔐

<a name="oauth-on-a-remote-server"></a> <a name="oauth-em-servidor-remoto"></a>

> **⚠️ Important pour les utilisateurs exécutant OmniRoute sur un VPS, Docker ou
> tout serveur distant **

#### Pourquoi l'authentification OAuth Antigravity / Gemini CLI échoue sur les serveurs distants ?

Les fournisseurs **Antigravity** et **Gemini CLI** utilisent **Google OAuth
2.0**. Google exige que l'URI de redirection ` dans le flux d'authentification
OAuth corresponde exactement à une des URIs enregistrées dans la console Google
Cloud.

Les credentials d'authentification OAuth embarqués dans OmniRoute sont
enregistrés **pour `localhost` seulement**. Lorsque vous accédez à OmniRoute sur
un serveur distant (par exemple `https://omniroute.myserver.com`), Google
rejette l'authentification avec :

```
Erreur 400 : redirect_uri_mismatch
```

#### Solution : Configurez vos propres credentials d'authentification OAuth

Vous devez créer un **Client ID OAuth 2.0** dans la console Google Cloud avec
l'URI de votre serveur.

#### Étape par étape

**1. Ouvrez la console Google Cloud **

Allez à :
[https://console.cloud.google.com/apis/credentials](https://console.cloud.google.com/apis/credentials)

**2. Créez un nouveau Client ID OAuth 2.0 **

- Cliquez sur **"+ Créer des credentials"** → **"Client ID OAuth"**
- Type d'application : **"Application web"**
- Nom : N'importe quoi que vous lisez (par exemple `OmniRoute distant`)

**3. Ajoutez les URI de redirection autorisées **

Dans le **champ "URI de redirection autorisées" **, ajoutez :

```
https://votre-server.com/callback
```

> Remplacez `votre-server.com` par le domaine ou l'adresse IP de votre serveur
> (y compris le port si nécessaire, par exemple
> `http://45.33.32.156:20128/callback`).

**4. Sauvegarder et copier les informations d'identification**

Après avoir créé le client, Google affichera l' **ID du client** et **Le Secret
du client**.

**5. Définir les variables d'environnement**

Dans votre `.env` (ou variables d'environnement Docker) :

```bash
# Pour Antigravity :
ANTIGRAVITY_OAUTH_CLIENT_ID = votre-client-id.apps.googleusercontent.com
ANTIGRAVITY_OAUTH_CLIENT_SECRET = GOCSPX- votre-secret

# Pour Gemini CLI :
GEMINI_OAUTH_CLIENT_ID = votre-client-id.apps.googleusercontent.com
GEMINI_OAUTH_CLIENT_SECRET = GOCSPX- votre-secret
GEMINI_CLI_OAUTH_CLIENT_SECRET = GOCSPX- votre-secret
```

**6. Redémarrer OmniRoute**

```bash
# npm :
npm run dev

# Docker :
docker restart omniroute
```

**7. Essayer à nouveau de se connecter**

Panneau de commande → Preneurs → Antigravity (ou Gemini CLI) → OAuth

Google redirigera maintenant correctement vers `https://
votre-serveur.com/callback`.

---

#### Raccourci temporaire (sans paramètres personnalisés)

Si vous ne voulez pas configurer vos propres informations d'identification pour
le moment, vous pouvez toujours utiliser la **flux de URL manuel** :

1. OmniRoute ouvre l'URL de l'autorisation Google
2. Après avoir autorisé, Google essaie de rediriger vers `localhost` (ce qui
   échoue sur le serveur distant)
3. **Copier l'URL complète** provenant de la barre d'adresse de votre navigateur
   (même si la page ne s'affiche pas)
4. Collez cette URL dans le champ affiché dans le médiat de connexion OmniRoute
5. Cliquez sur **"Connecter "**

> Cela fonctionne parce que le code d'autorisation dans l'URL est valide quel
> que soit si la page de redirection s'est chargée.

---

<details>
<summary><b>🇧🇷 Versão em Português</b></summary>

#### Pourquoi le OAuth de Antigravity / Gemini CLI échoue-t-il sur les serveurs distants ?

Les fournisseurs **Antigravity** et **Gemini CLI** utilisent **Google OAuth
2.0** pour l'authentification. Le Google exige que la `redirect_uri` utilisée
dans le flux OAuth soit **exactement** une des URIs enregistrées dans le Google
Cloud Console de l'application.

Como **seu identificador** de aplicação OAuth embutido no OmniRoute é registrado
**seu identificador** apenas para `localhost`, lembre-se de que o Google não
autorizará a autenticação de `https://omniroute.meuservidor.com` :

```
Erreur 400 : redirect_uri_mismatch
```

#### Solução : Configurez vos propres credenciales OAuth

Vous devez créer un ** identifiant client OAuth 2.0** dans le Console Google
Cloud avec l'URI de vos serveurs.

#### Étape par étape

**1. Connectez-vous à la Console Google Cloud**

Ouvrez:
[https://console.cloud.google.com/apis/credentials](https://console.cloud.google.com/apis/credentials)

**2. Créez un nouvel identifiant client OAuth 2.0**

- Cliquez sur ** « Nouveau »** → ** « Nouvel identifiant client OAuth 2.0 »**
- Le type d'application : ** « Application Web »**
- Nom: choisissez un nom (par exemple, ` OmniRoute distant`)

**3. Ajoutez les adresses de redirection autorisées**

Dans le champ ** « Adresses de redirection autorisées »**, ajoutez :

```
https://seu-servidor.com/callback
```

> Remplacez ` votre domäne ou adresse IP serveur` par le domäne ou adresse IP de
> votre serveur (y compris la porte si nécessaire, exemple
> `http://45.33.32.156:20128/callback`).

**4. Enregistrez et copiez les informations de connectivité**

Après création, Google affichera le ** Client ID** et le ** Client Secret**.

**5. Configurez les variables d'environnement**

Dans votre ` fichier de configuration [.env` (ou dans les variables
d'environnement de la passerelle) :

```bash
# Pour Antigravity :
ANTIGRAVITY_OAUTH_CLIENT_ID=votre-client-id.apps.googleusercontent.com
ANTIGRAVITY_OAUTH_CLIENT_SECRET=GOCSPX-votre-secret

# Pour CLI Gemini:
GEMINI_OAUTH_CLIENT_ID=votre-client-id.apps.googleusercontent.com
GEMINI_OAUTH_CLIENT_SECRET=GOCSPX-votre-secret
GEMINI_CLI_OAUTH_CLIENT_SECRET=GOCSPX-votre-secret
```

**6. Réinitialisez OmniRoute**

```bash
# Si vous utilisez npm :
npm run dev

# Si vous utilisez Docker :
docker restart omniroute
```

**7. Réessayez de vous connecter**

tableau de bord → Fournisseurs → Antigravité (ou Gemini CLI) → OAuth

Google redirigera maintenant correctement vers
`https://seu-servidor.com/callback` et authentification fonctionnera.

---

#### Solution temporaire (sans configurer des identifiants propriétaires)

Si vous ne souhaitez pas créer des identifiants propriétaires maintenant, vous
pouvez toujours utiliser le flux **manuel de URL** :

1. Le OmniRoute ouvrira l'URL d'autorisation Google
2. Après avoir autorisé, Google tentera de rediriger vers `localhost` (qui
   échoue sur le serveur distant)
3. **Copiez l'URL complète** de la barre d'adresse de votre navigateur (même si
   la page ne s'affiche pas)
4. Collez cette URL dans le champ qui apparaît dans le modèle de connexion
   OmniRoute
5. Cliquez sur **"Connect"**

> Cette solution temporaire fonctionne car le code d'autorisation dans l'URL est
> valide, quel que soit le redirigeant qui ait chargé ou pas.

</details>

---

</details>

## 🛠️ Tech Stack

<details>
<summary><b>Click to expand tech stack details</b></summary>

- **Runtime**: Node.js 18–22 LTS (⚠️ Node.js 24+ is **ne prend pas en charge** —
  `binaires natives better-sqlite3` incompatibles)
- **Langage**: TypeScript 5.9 — **100% TypeScript** dans `src/` et `open-sse/`
  (pas de `any` dans les modules de base depuis v2.0)
- **Framework**: Next.js 16 + React 19 + Tailwind CSS 4
- **Base de données**: LowDB (JSON) + SQLite (état de la domaine + journaux de
  proxy + audit MCP + décisions de routage)
- **Schémas**: Zod (outil I/O de validation MCP, contrats d'API)
- **Protocoles**: MCP (stdio/HTTP) + A2A v0.3 (JSON-RPC 2.0 + SSE)
- **Diffusion** : événements envoyés par le serveur (SSE)
- **Auth** : OAuth 2.0 (PKCE) + JWT + API clés + autorisation étendue MCP
- **Testing** : exécuteur de tests Node.js + Vitest (900+ de tests, dont
  unitaires, d'intégration, E2E)
- **CI/CD** : GitHub Actions (auto publication npm + Docker Hub lors de la mise
  en production)
- **Site Web** : [omniroute.online](https://omniroute.online)
- **Package** :
  [npmjs.com/package/omniroute](https://www.npmjs.com/package/omniroute)
- **Docker** :
  [hub.docker.com/r/diegosouzapw/omniroute](https://hub.docker.com/r/diegosouzapw/omniroute)
- **Resilience** : circuit briseur, retrait exponentiel, anti-embryage
  foudroyant, simulacre de spoofing TLS, auto-mise en scène du self-healing

</details>

---

## Documentation

| Documenter                                                | Description                                                             |
| --------------------------------------------------------- | ----------------------------------------------------------------------- |
| [Répertoire de l'utilisateur](docs/USER_GUIDE.md)         | Fournisseurs, combinaisons, intégration CLI, déploiement                |
| [Recommandations de l'API](docs/API_REFERENCE.md)         | Tous les points de terminaison avec des exemples                        |
| [ Serveur MCP](open-sse/mcp-server/README.md)             | 16 outils MCP, configurations IDE, clients Python/TS/Go                 |
| [ Serveur A2A](src/lib/a2a/README.md)                     | protocole JSON-RPC 2.0, compétences, diffusion, gestion de tâches       |
| [Moteur de combinaison automatique](docs/auto-combo.md)   | Système de notation à 6 facteurs, packs de mode, réparation automatique |
| [Troubleshooting](docs/TROUBLESHOOTING.md)                | Problèmes courants et solutions                                         |
| [Architecture](docs/ARCHITECTURE.md)                      | Architecture et intérieurs du système                                   |
| [Contributing](CONTRIBUTING.md)                           | Paramètres de configuration et lignes directrices de développement      |
| [OpenAPI Spec](docs/openapi.yaml)                         | Spécification OpenAPI 3.0                                               |
| [Politique de sécurité](SECURITY.md)                      | Rapports de vulnérabilité et pratiques de sécurité                      |
| [Déploiement de la VM](docs/VM_DEPLOYMENT_GUIDE.md)       | Guide complet : déploiement de la VM + nginx + Cloudflare               |
| [Galérie des fonctionnalités](docs/FEATURES.md)           | Tour guidée du tableau de bord avec captures d'écran                    |
| [Tableau de bord des versions](docs/RELEASE_CHECKLIST.md) | Étapes de validation pré-sortie                                         |

---

## 🗺️ Carte des routes

OmniRoute prévoit **210+ fonctionnalités** au cours de multiples phases de
développement. Voici les principales domaines :

| Catégorie                                                      | Fonctionnalités prévues | Mis en avant                                                                                                                     |
| -------------------------------------------------------------- | ----------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| 🧠 Gestion Routée & Intelligence[2X]Routing & Intelligence[26X] | 25+                     | Routage de basse latence, routage basé sur un tag, évaluation préalable des quotas, sélection du compte P2C                      |
| 🔒 [2X] Sécurité & Normes**                                     | 20+                     | Renforcement anti-SSRF, dissimulation des identifiants, limiteur de débit par point de terminaison, écranage des clés de gestion |
| 📊 [2X] Observabilité**                                         | 15+                     | Intégration OpenTelemetry, suivi en temps réel des quotas, suivi des coûts par modèle                                            |
| 🔄 [2X] Intégrations de Fournisseurs**                          | 20+                     | Registre de modèles dynamique, temps de refroidissement des fournisseurs, comptes multiples Codex, analyse des quotas de Copilot |
| ⚡ [2X] Performance**                                           | 15+                     | Dual couche de cache, cache des suggestions, cache de réponse, streaming keepalive, Batch API                                    |
| 🌐 [2X] Écosystème**                                            | 10+                     | API WebSocket, rechargement de la configuration, stockage distribué de configuration, mode commercial                            |

### Bientôt disponible

- 🔗 [2X] Intégration OpenCode** — Support natif du fournisseur pour
  l'intégration d'IDÉ AI de codage OpenCode
- 🔗 **INTÉGRATION TRAE** — Support complet pour le framework de développement
  d'intelligence artificielle TRAE
- 📦 **API en lot** — Traitement en lot asynchrone pour les demandes de grande
  envergure
- 🎯 **Affichage de la routage sur la base de balises** — Routage des requêtes
  sur la base de balises personnalisées et de métadonnées
- 💰 **Stratégie de coût le plus bas** — Sélection automatique du fournisseur le
  moins cher disponible

> 📝 Les spécifications des fonctionnalités complètes sont disponibles dans
> [`docs/nouveautés-des-fonctionnalités/`](docs/new-features/) (217
> spécifications détaillées)

---

## 👥 Contribuant

[![Contributants](https://contrib.rocks/image?repo=diegosouzapw/OmniRoute&max=100&columns=20&anon=1)](https://github.com/diegosouzapw/OmniRoute/graphs/contributors)

### Comment contribuer

1. Fork le référentiel
2. Créer une branche de fonctionnalité (`git checkout -b
   feature/amazing-feature`)
3. Commitez vos modifications (`git commit -m 'Ajoutez la fonctionnalité
   incroyable'`)
4. Poussez la branche (`git push origin feature/amazing-feature`)
5. Ouvrez une demande de tirage

Consultez [CONTRIBUTING.md](CONTRIBUTING.md) pour des guides détaillés.

### Sortie d'une nouvelle version

```bash
# Créez une sortie — npm publish se déclenche automatiquement
gh release creo v2.0.0 --title "v2.0.0" --generate-notes
```

---

## 📊 Historique des étoiles

## Les étoiles sur le temps

## [![Étoiles sur le temps](https://starchart.cc/diegosouzapw/OmniRoute.svg?variant=adaptive)](https://starchart.cc/diegosouzapw/OmniRoute)

## 🙏 Remerciements

Merci spéciale à **[X(https://github.com/decolua/9router)] — le projet d'origine
qui a inspiré cette branche. OmniRoute se base sur cette merveilleuse fondation
avec d'autres fonctionnalités, des APIs multimodaux et une réécriture complète
en TypeScript.

Merci spéciale à **[CLIProxyAPI](https://github.com/router-for-me/CLIProxyAPI)**
— la mise en œuvre Go d'origine qui a inspiré cette version JavaScript.

---

## 📄 Licencia

LICENCE MIT - voir [LICENSE](LICENSE) pour plus de détails.

---

<div align="center">
  <sub>Built with ❤️ for developers who code 24/7</sub>
  <br/>
  <sub><a href="https://omniroute.online">omniroute.online</a></sub>
</div>
<!-- GitHub Discussions enabled for community Q&A -->
