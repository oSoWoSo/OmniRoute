# 🚀 OmniRoute — The Free AI Gateway

### 常にカスタム化を続けろ。 **FREE & 低コストのAIモデルのスマートルーティング** に、自動フェールバックが付く。

_ユニバーサルAPIプロキシ − 一つのエンドポイント、67 + 提供者、アプリケーションドウンタイムなし。 MEC & A2A
エージェントオーケストレーションで更新済み。_

**会話の完了 • 画像生成 • ビデオ • 音楽 • オーディオ • 再排列 •**Web 検索 • MCP サーバー • A2A プロトコル • 100%
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
[![License](https://img.shields.io/github/license/diegosouzapw/OmniRoute)](https://github.com/diegosouzapw/OmniRoute/blob/main/LICENSE)
[![Website](https://img.shields.io/badge/Website-omniroute.online-blue?logo=google-chrome&logoColor=white)](https://omniroute.online)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-Community-25D366?logo=whatsapp&logoColor=white)](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

[🌐 ウェブサイト](https://omniroute.online) • [🚀 Quick Start](#-quick-start) • [💡
フィーチャー](#-key-features) • [📖 ドキュメント](#-documentation) • [💰
プライシング](#-pricing-at-a-glance) • [💬
WhatsApp](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)

</div>

🌐 **利用可能な言語: ** 🇯🇵 [日本語](README.md) | 🇧🇷
[ポルトガル語(ブラジル)](docs/i18n/pt-BR/README.md) | 🇪🇸 [スペイン語](docs/i18n/es/README.md) |
🇫🇷 [フランス語](docs/i18n/fr/README.md) | 🇮🇹 [イタリア語](docs/i18n/it/README.md) | 🇷🇺
[ロシア語](docs/i18n/ru/README.md) | 🇨🇳 [中国語(簡体字)](docs/i18n/zh-CN/README.md) | 🇩🇪
[ドイツ語](docs/i18n/de/README.md) | 🇮🇳 [ヒンディー語](docs/i18n/in/README.md) | 🇹🇭
[タイ語](docs/i18n/th/README.md) | 🇺🇦 [ウクライナ語](docs/i18n/uk-UA/README.md) | 🇸🇦
[アラビア語](docs/i18n/ar/README.md) | 🇯🇵 [日本語](docs/i18n/ja/README.md) | 🇻🇳
[ベトナム語](docs/i18n/vi/README.md) | 🇧🇬 [ブルガリア語](docs/i18n/bg/README.md) | 🇩🇰
[デンマーク語](docs/i18n/da/README.md) | 🇫🇮 [フィンランド語](docs/i18n/fi/README.md) | 🇮🇱
[ヘブライ語](docs/i18n/he/README.md) | 🇭🇺 [ハンガリー語](docs/i18n/hu/README.md) | 🇮🇩
[インドネシア語](docs/i18n/id/README.md) | 🇰🇷 [韓国語](docs/i18n/ko/README.md) | 🇲🇾
[マレー語](docs/i18n/ms/README.md) | 🇳🇱 [オランダ語](docs/i18n/nl/README.md) | 🇳🇴
[ノルウェー語](docs/i18n/no/README.md) | 🇵🇹 [ポートガル語(ポルトガル)](docs/i18n/pt/README.md) |
🇷🇴 [ルーマニア語](docs/i18n/ro/README.md) | 🇵🇱 [ポーランド語](docs/i18n/pl/README.md) | 🇸🇰
[スロバキア語](docs/i18n/sk/README.md) | 🇸🇪 [スウェーデン語](docs/i18n/sv/README.md) | 🇵🇭
[フィリピーノ語](docs/i18n/phi/README.md) | 🇨🇿 [チェコ語](docs/i18n/cs/README.md)

---

## 🆕 v3.0.0で新しい機能

> **v2.9.5からアップグレードする場合**? —
> 全ての変更を確認するためには、[完全なCHANGELOG](CHANGELOG.md#300--2026-03-22-release-candidate--not-yet-merged-to-main)を参照してください。

| エリア                         | 変更                                                                                                         |
| --------------------------- | ---------------------------------------------------------------------------------------------------------- |
| 🔒 **CodeQL Security**       | 10 を超える CodeQL アラートが修正されました: polynomial-redos、insecure-randomness、shell-injection remediation              |
| ✅ **Route  Validation**     | すべての 176 アプリケーション API ルートが Zod スキーマで検証され、`validateBody()` — CI `チェック:route-validation:t06` が通るように変更されました。  |
| 🐛 **omniModel タグ漏れ**        | 内部タグ `<omnimodel>` が、SSE ストリーミングレスポンスによってクライアントに流れなくなりました (#585)</omnimodel>                               |
| 🔑 **Registered Keys API**   | API キーを自動設定して、`POST /api/v1/registered-keys` を使用して各プロバイダーやアカウントに定期メトリクス制御された暗号化されたAPIキーを取得します。             |
| 🎨 **プロバイダーのアイコン**           | 130+ provider logos via `@lobehub/icons` (SVG) with PNG → generic fallback chain                           |
| 🔄 **Model Auto-Sync**       | 24h scheduler and manual UI toggle to sync model lists for built-in and custom OpenAI-compatible providers |
| 🌐 **OpenCode Zen/Go**       | Two new providers from @kang-heewon via PR #530: free tier + subscription tier via `OpencodeExecutor`      |
| 🐛 **Gemini CLI OAuth**      | Actionable error when `GEMINI_OAUTH_CLIENT_SECRET` is missing in Docker (was cryptic Google error)         |
| 🐛 **OpenCode config**       | `saveOpenCodeConfig()` now correctly writes TOML to `XDG_CONFIG_HOME`                                      |
| 🐛 **Pinned model override** | `body.model` correctly set to `pinnedModel` on context-cache protection                                    |
| 🐛 **Codex/Claude loop**     | `tool_result` blocks now converted to text to stop infinite loops                                          |
| 🐛 **Login redirect**        | Login no longer freezes after skipping password setup                                                      |
| 🐛 **Windows paths**         | MSYS2/Git-Bash paths (`/c/...`) normalized to `C:\...` automatically                                       |

---

## 🖼️ Main Dashboard

<div align="center">
  <img src="./docs/screenshots/MainOmniRoute.png" alt="OmniRoute Dashboard" width="800"/>
</div>

---

## 📸 Dashboard Preview

<details>
<summary><b>Click to see dashboard screenshots</b></summary>

| Page         | スクリーンショット                                     |
| ------------ | --------------------------------------------- |
| **プロバイダー**   | ![プロバイダー](docs/screenshots/01-providers.png)  |
| **組み合わせ**    | ![組み合わせ](docs/screenshots/02-combos.png)      |
| ** アナリティクス** | ![アナリティクス](docs/screenshots/03-analytics.png) |
| **ヘルス**      | ![ヘルス](docs/screenshots/04-health.png)        |
| **翻訳機**      | ![翻訳機](docs/screenshots/05-translator.png)    |
| **設定**       | ![設定](docs/screenshots/06-settings.png)       |
| **CLIツール**   | ![CLIツール](docs/screenshots/07-cli-tools.png)  |
| **使い方ログ**    | ![使い方](docs/screenshots/08-usage.png)         |
| **エンドポイント**  | ![エンドポイント](docs/screenshots/09-endpoint.png)  |

</details>

---

### 🤖 お気に入りのコード実行エージェントのために、フリーのAI プロバイダーです

_AIエクスペリエンスをサポートするIDEやCLIツールとOmniRouteを繋げて—無料のAPIゲートウェイ—無制限のコードに。_

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

<sub>📡 すべてのエージェントは <code>http://localhost:20128/v1</code> または
<code>http://cloud.omniroute.online/v1</code> — 1 つの設定、無制限のモデルとクォーターのため、1
つの設定</sub>

---

## 🤔 为何OmniRoute？

**お金を無駄にしないでください、制限を超えます:**

- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  有効期限切れの申請は毎月残ります
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  制限したときの制限時に制限されます
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  高額なAPI（每月20〜50ドル/提供者）)
- <img src="https://img.shields.io/badge/✗-e74c3c?style=flat-square" height="16"/>
  プロバイダー間で自動的に変更する必要がある

**OmniRouteが解決します:**

- ✅ **最大のサブスクリプションを実現** - クォータをトラッキングして、リセットされる前に利用する
- ✅ **自動のフェールバック** - サブスクリプション→ API キー → 安価な → 費用を負う、0 のダウンタイム
- ✅ **マルチアカウント** - プロバイダーごとにアカウントを回転させる
- ✅ **ユニバーサル** - Claude Code、Codex、Gemini
  CLI、Cursor、Cline、OpenClaw、どのCLIツールとも、どのCLIツールとも

---

## 📧 サポート

> 💬
> **コミュニティに参加**！[Whatsappグループ](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)
> — ヘルプ、ヒント、そしてアップデートを共有してください。

- **ウェブサイト**:[omniroute.online](https://omniroute.online)
- **GitHub**:[github.com/diegosouzapw/OmniRoute](https://github.com/diegosouzapw/OmniRoute)
- **問題**:[github.com/diegosouzapw/OmniRoute/issues](https://github.com/diegosouzapw/OmniRoute/issues)
- **Whatsapp**:[コミュニティグループ](https://chat.whatsapp.com/JI7cDQ1GyaiDHhVBpLxf8b?mode=gi_t)
- **貢献**:[CONTRIBUTING.md](CONTRIBUTING.md)を参照してください、PRを開いてください、または`おおい初心者の問題`を開いてください。
- **オリジナルのプロジェクト**: [9router by decolua](https://github.com/decolua/9router)

### 🐛 バグを報告する?

問題を提出する際に、システム情報コマンドを実行し、生成されたファイルを追加してください：

```bash
npm run system-info
```

これにより、Node.js のバージョン、OmniRoute のバージョン、OS の詳細、インストール済み CI ツール (iflow、Gemini
CLI、Claude、Codex、Antigravity、Droid など)、docker/PM2
状態、およびシステムパッケージも含め、すべてを生成します。これで、問題を迅速に再現できるようになります。\
ファイルを直接 GitHub の問題に接続してください。

---

## 仕組み

```
┌─────────────┐
│  Your CLI   │  (Claude Code、Codex、Gemini CLI、OpenClaw、Cursor、Cline...)
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
       ├─→ [Tier 1: サブスクリプション] Claude Code、Codex、Gemini CLI
       │   ↓ 実行回数枯渇
       ├─→ [Tier 2: API キー] DeepSeek、Groq、xAI、Mistral、NVIDIA NIM、など
       │   ↓ 資金枯渇
       ├─→ [Tier 3:安さ] GLM ($0.6/1M)、MiniMax ($0.2/1M)
       │   ↓ 資金枯渇
       └─→ [Tier 4: 無料] iFlow、Qwen、Kiro (無限)

結果：常にコーディングを続け、コスト最小化
```

---

## 🎯 OmniRoute が解決すること — 30 の実際の苦手な部分と使用例

> **開発者は、AI ツールを使用する場合に何度か日常的にそれなどの問題を遭遇するだろう.** OmniRoute
> は、コストオーバーランから地域のブロック、ブロークンな OAuth
> フローからプロトコルオペレーションまで、エンタープライズのオブザーブアビリティまで、すべてのことに解決策があることを目的としている。

<details>
<summary><b>💸 1. "I pay for an expensive subscription but still get interrupted by limits"</b></summary>

開発者が Claude Pro、Codex Pro、GitHub Copilot の 1 か月ごとの費用に相当する
$20–200/月を支払う場合、クォーターは上限がある — 5 時間 (h) の使用、週ごとの制限、1 分あたりの料金制限。mid-coding
セッションのある時、提供者が応答してくるところが終わり、開発者はフローと有効性を落とすことになります。

**OmniRoute がそれを解決する方法:**

- **優秀な 4 層分散[Fallback** — サブスクリプションを使用するクォーターを枯渇すると、自動的に
  APIキーや安さ、無料のそれや、人為的な措置のないようにする。
- **リアルタイムクォーター追跡[追跡] — 実況中のトークン消費をリアルタイムに表示するためのリセットカウントダウン (5 時間、毎日または毎週)
- **複数アカウントのサポート[アカウント] — サービス提供者の特定のアカウント毎に並べ替えられる。\
  もしくは、実行が完了した最初のものに。
- **カスタムコンボ[カスタマイズ] — カスタマイズできる fallback チェーンにつき、6 通りのバランス付け方
  (fill-first、round-robin、P2C、random、least-used、cost-optimized) を選択できます。
- ** Codex ビジネスクォータ監視[ビジネス] — ビジネス/チーム ワークスペースクォータ監視をダッシュボード上で直接見ることができます。

</details>

<details>
<summary><b>🔌 2. "I need to use multiple providers but each has a different API"</b></summary>

OpenAI は一つのフォーマットを、Claude (Anthropic) は別のもの (Gemini にはまた別)
を使っている。開発者は、モデルを試すときは、SDK
に手動で設定するだけでは、モデルが別のサービスでしか動作しないなど、各サービスを手動で設定して、フォーマットを変えて、サービスを変更しなければならない。カスタムのサービス
(FriendL）, NVIDIA NIM) は非標準のモデルエンドポイントを持っている。

**OmniRoute がそれを解決する方法:**

- **統合エンドポイント[統合] — 67 以上のサービスのエンドポイントとして使う、単一の `http://localhost:20128/v1`
  があれば、すべてのことが解決する。
- **フォーマットの置換[置換] — オープンAI ↔ クラウド ↔ ギミニ ↔ レスポンス API の間で、自動でフォーマットを変える。
- **リスポンス消毒** — 非標準フィールドが削除されます ([X56X)x_groq`, `usage_breakdown`,
  `service_tier`) でOpenAI SDK v1.83+のバージョンを破壊します
- **ロール正常化** — 非OpenAI プロバイダー用に`developer` → `system` に変換します;
  GLM/ERNIE用に`system` → `user`
- **Think Tag抽出** — DeepSeek R1などのモデルから標準化された`reasoning_content` の抽出に`<think>`
  ブロックを使用します</think>
- **Geminiへの構造化出力** — `json_schema` → `responseMimeType`/`responseSchema` の自動変換
- **`stream`はデフォルトでは`false`に設定されます** — OpenAI仕様に合わせ、Python/Rust/Go
  SDKで予期しないSSEを回避します

</details>

<details>
<summary><b>🌐 3. "My AI provider blocks my region/country"</b></summary>

オープンAI/Codexなどのプロバイダーは、特定の地理的地域からアクセスをブロックしています。ユーザーは、OAuthとAPI接続で[XL96X]unsupported_country_region_territory`
のエラーが発生します。

**OmniRoute がそれを解決する方法:**

- **3レベルプロキシ設定** — プロキシ設定は3レベルで構成され、グローバル(すべてのトラフィック)、プロバイダ(一つだけ)、接続/鍵ごとに設定できます
- **カラーコードプロキシビード** — Visaulの指標: 🟢 グローバルプロキシ、🟡 プロバイダプロキシ、🔵 接続プロキシ
- **OAuthトークン交換プロキシ** —
  OAuthフローもプロキシを通じて実行されます。これで[XL89X]unsupported_country_region_territory`
  は解決されます
- **接続テストプロキシ** — 接続テストでは、設定されたプロキシを使用します
- **SOCKS5サポート** — アウトバウンドルーティングにフルSOCKS5プロキシをサポートします
- **TLSフィンガープリントスニフ** — browser-like TLSフィンガープリントをwreq-jsで使用してbot検知を回避
- **CLIフィンガープリントマッチング** — 本来のCLIバイナリのシグネチャにマッチするようにヘッダーとボディフィールドを並べ替えます

</details>

<details>
<summary><b>🆓 4. "I want to use AI for coding but I have no money"</b></summary>

全てのユーザーがAIサブスクリプションに20～200ドルの費用を支払う必要があるわけではありません。教育者、エーテミング国からの開発者、趣味者、自由契約者には、0に費用の質の高いモデルにアクセスできます

**OmniRoute がそれを解決する方法:**

- **FreeTierプロバイダ内部** — 100％の無料プロバイダを取り入れる: iFlow
  (5限ずつのモデルはOAuth:kimi-k2-想像、qwen3-coder-plus、deepseek-r1、最適化2、kimi-k2)、Qwen
  (4限無制限モデル：qwen3-coder-plus、qwen3-coder-フラッシュ、qwen3-coder-nex、ビジョンモデル)、Kiro
  (クラウド+AWSビルダーID、自由)、Gemini CLI (1月18Kトークン、無料)
- **Ollama Cloud** — API.ollama.comのクラウドホスティングでOllamaモデルを[XL49X]api.ollama.com`
  で提供しています
- **フリーオンリー組み合わせ** —
  低価格の組み合わせが可能です：gc、gemin-3フラッシュ→if、kimi-k2-think→qw、qwen3-coder-plus=0/月の料金に耐えられない
- **nVIDIA NIM無料アクセス** — 70+モデルにアクセスすることができます。build.nvidia.comから40
  RPMの無料アクセスが可能です（クレジット制度から純粋な制限時間になります）
- **コスト最適化戦略** — ルーティング戦略が自動的に最安手の利用可能なプロバイダーを選択します。

</details>

<details>
<summary><b>🔒 5. "I need to protect my AI gateway from unauthorized access"</b></summary>

AIゲートウェイをLAN、VPS、Dockerで公開する場合、それにはアドレスだけが必要です。開発者のトークン/クォータも、プロテクションなしでどのユーザでも消費することができます。このため、APIは、誤用、プレンプト注入、および濫用に対して脆弱になります。

**OmniRoute がそれを解決する方法:**

- **APIキー管理** — `/ダッシュボード/セキュリティ(APIマネージャー`)ページ上で、プロバイダーごとに、キーを生成、回転、およびスコープします。
- **モデルレベルの権限** —
  APIキーの制限を特定のモデル(`openai/*`、ワイルドカードパターン）にします。許可するアクション/制限を切り替えます
- **APIエンドポイント保護** — `/v1/models`のAPIキーを必要です。また、特定のプロバイダーはリストからブロックされる
- **Auth Guard + CSRF保護** — `withAuth`ミドルウェアで保護されたすべてのダッシュボードルート + CSRF トークン
- **リートリミッター** — 可変期間のパーIPリートリミッター
- **IPフィルタリング** — アクセス制御用のホワイトリスト/ブラックリスト
- **プレンプト注入グアルード** — 害意のプレンプト パターンに対する汚物除去
- **AES-256-GCM暗号化** — 資格情報はロード中に暗号化される

</details>

<details>
<summary><b>🛑 6. "My provider went down and I lost my coding flow"</b></summary>

AIプロバイダーは不安定になることがあります。500番外信号、または一時的な率制限を返すことがあります。デベロッパーよりも1つのプロバイダーに依存する場合、停止します。特定のプロバイダーを保護するcircuit-breakerのない場合、反復試行はアプリケーションをクラッシュさせます。

**OmniRoute がそれを解決する方法:**

- **モデル毎のcircuit-breaker** —
  可変的な閾値とクールダウン（クローズド/オープン/ハイアウトド）のオートオープン/クローズ、モデル毎に実装されたクラスタリングを阻止します
- **指数バックオフ** — 進行的なリトライ時の遅延
- **アンチサンダーヘルド** — 並列リトライの対処用のミュエックスおよびセマフォ保護
- **ボンボールチェイン** — 正常なプロバイダが失敗した場合、複合ファルバックチェインを自動的に繊維します
- **組合circuit-breaker** — 生成されたプロビーダが複合チェイン内で自動でブロックされる
- **健康ダイジェスト** — 正常時間調査、断続器の状態、ブロック、キャッシュ統計、p50/p95/p99リトゥー遅延

</details>

<details>
<summary><b>🔧 7. "Configuring each AI tool is tedious and repetitive"</b></summary>

デベロッパーはCursor、Clude Code、Codex CLI、OpenCLaw、Gemini CLI、Kilo
Codeなどを使用しています。各ツールにはAPI
エンドポイント、キー、モデルごとに異なる設定が必要です。スイッチするプロバイダーやモデルごとに設定を再構成することは時間を無駄にかかることになります。

**OmniRoute がそれを解決する方法:**

- **CLIツールズ ダッシュボード** — Dedicated page with one-click setup for Claude Code,
  Codex CLI, OpenClaw, Kilo Code, Antigravity, Cline
- **GitHub Copilot Config Generator** — Generates `chatLanguageModels.json` for
  VS Code with bulk model selection
- **オンボーディング ウィザード** — Guided 4-step setup for first-time users
- **One endpoint, all models** — Configure `http://localhost:20128/v1` once,
  access 67+ providers

</details>

<details>
<summary><b>🔑 8. "Managing OAuth tokens from multiple providers is hell"</b></summary>

Claude Code, Codex, Gemini CLI, Copilot — all use OAuth 2.0 with expiring
tokens. Developers need to re-authenticate constantly, deal with `client_secret
is missing`, `redirect_uri_mismatch`, and failures on remote servers. OAuth on
LAN/VPS is particularly problematic.

**OmniRoute がそれを解決する方法:**

- **Auto Token Refresh** — OAuth tokens refresh in background before expiration
- **OAuth 2.0 (PKCE) Built-in** — Automatic flow for Claude Code, Codex, Gemini
  CLI, Copilot, Kiro, Qwen, iFlow
- **Multi-Account OAuth** — Multiple accounts per provider via JWT/ID token
  extraction
- **OAuth LAN/Remote Fix** — Private IP detection for `redirect_uri` + manual
  URL mode for remote servers
- **OAuth Behind Nginx** — Uses `window.location.origin` for reverse proxy
  compatibility
- **Remote OAuth Guide** — Step-by-step guide for Google Cloud credentials on
  VPS/Docker

</details>

<details>
<summary><b>📊 9. "I don't know how much I'm spending or where"</b></summary>

開発者は複数の有料プロバイダーを使用していますが、費用の統一された視覚化機能はありません。一部のプロバイダーには独自の請求ダッシュボードがあり、予想外の費用が累積する可能性があります。

**OmniRoute がそれを解決する方法:**

- **Cost Analytics Dashboard** — Per-token cost tracking and budget management
  per provider
- **Budget Limits per Tier** — Spending ceiling per tier that triggers automatic
  fallback
- **Per-Model Pricing Configuration** — Configurable prices per model
- **Usage Statistics Per API Key** — Request count and last-used timestamp per
  key
- **Analytics Dashboard** — Stat cards, model usage chart, provider table with
  success rates and latency

</details>

<details>
<summary><b>🐛 10. "I can't diagnose errors and problems in AI calls"</b></summary>

When a call fails, the dev doesn't know if it was a rate limit, expired token,
wrong format, or provider error. Fragmented logs across different terminals.
Without observability, debugging is trial-and-error.

**OmniRoute がそれを解決する方法:**

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

**OmniRoute がそれを解決する方法:**

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

**OmniRoute がそれを解決する方法:**

- **ダッシュボード i18n — 30 の言語** —
  Arabica、ブルガリア語、デンマーク語、ドイツ語、スペイン語、フィンランド語、フランス語、ヘブライ語、ヒンディ語、ハンガリー語、インドネシア語、イタリア語、日本語、韓国語、マレー語、オランダ語、ノルウェー語、ポーランド語、ポルトガル語
  (PT/BR)、ルーマニア語、ロシア語、スロバキア語、スウェーデン語、タイ語、ウクライナ語、ベトナム語、中国語、フィリピノ語、英語
- **RTL をサポートする** — 英語とアラビア語の右から左へ
- **多言語 README** — 30 の完全なドキュメント翻訳
- **言語シッター** — ヘッダーに実時間で切り替え用の球 icon

</details>

<details>
<summary><b>🔄 13. "I need more than chat — I need embeddings, images, audio"</b></summary>

AI の chat とは別にある。デベロッパーらは、画像を生成する、音を文字化する、RAG 用の埋め込みを作成する、文書を再度並べる、コンテンツを調整するなどの
API を使う。各 API は異なる終点とフォーマットを持つ。

**OmniRoute がそれを解決する方法:**

- **埋め込み** — `/v1/embeddings`、6 つのプロバイダー・9+ のモデル
- **画像生成** — `/v1/images/generations`、10 つのプロバイダー・20+
  のモデル（OpenAI、xAI、Together、Fireworks、Nebius、Hyperbolic、NanoBanana、アンチグラビティ、SD
  WebUI、ComfyUI）
- **テキスト映像** — `/v1/videos/generations`—ComfyUI（AnimateDiff、SVD）とSD WebUI
- **テキスト音楽** — `/v1/music/generations`—ComfyUI（Stable Audio Open、MusicGen）
- **音声録音** — `/v1/audio/transcriptions`—Whisper + Nvidia NIM、HuggingFace、Qwen3
- **テキスト読み上げ** — `/v1/audio/speech`—ElevenLabs、Nvidia
  NIM、HuggingFace、Coqui、Tortoise、Qwen3、**Inworld**、**Cartesia**、**PlayHT**、+
  existngプロバイダー
- **調整** — `/v1/moderations`—コンテンツセーフティチェック
- **再ランキング** — `/v1/rerank`—文書の関連度再ランキング
- **Response API** — Codex の完全な `/v1/responses` サポート

</details>

<details>
<summary><b>🧪 14. "I have no way to test and compare quality across models"</b></summary>

デベロッパーは、どのモデルが自分たちが使いたい場合を考慮したのが見つけたいが、そうして行うと遅すぎるので、このような比較機能は開発者にはない。

**OmniRoute がそれを解決する方法:**

- **LLM 評価** — 10
  個のプリロードされたケースで、挨拶、数学、地理、コード生成、JSON検証、翻訳、マークダウン、セーフティリフォーズを網羅したゴールデンセット。
- **4 つのマッチストラテジーズ** — `exact`、`contains`、`regex`、`custom`（JS関数）
- **翻訳プレイグランド テストベンチ** — 複数入力と期待した出力、クロスプロバイダーによる比較を行う
- **コンベンションテスター** — フォルクライド アラウンドトリップ機能とビジュアル レスポンス のルーティング
- **ライブモニター** — リクエストフローのリアルタイム ストリームでプロキシが作成します

</details>

<details>
<summary><b>📈 15. "I need to scale without losing performance"</b></summary>

リクエストが増えるほど、キャッシュせずに同じユースケースが複製されるためコストが生じます。
冗長リクエストは処理を無駄にしてしまいます。各プロバイダーのレート制限を尊重する必要があります。

**OmniRoute がそれを解決する方法:**

- **セマンティックキャッシュ** — 署名 + セマンティック 2 進キャッシュ (コスト削減および遅延低減)
- **リクエスト非重複要件** — 同一リクエストの 5 秒間の非重復化ウィンドウ
- **レート制限検出** — 各プロバイダーのリクエストマイナス 1 秒、最小間隔、最大並列数の追跡
- **エディタブルのレート制限** — スettings → 逸脱耐性の設定でエディタブルコマンドが実装されます。
- **API キー検証キャッシュ** — 製品パフォーマンス向上のための 3 レベルキャッシュ
- **ヘルスダッシュボード テレメトリー** — パ50 / パ95 / パ99 から遅延およびキャッシュ情報、オンライン時間

</details>

<details>
<summary><b>🤖 16. "I want to control model behavior globally"</b></summary>

開発者が各リクエストまたはツール内のリソースをすべて特定の言語に翻訳したい、特定のトーンに応えるようにしたい、またはロジカル
タークンを制限したい。すべてのツールやリクエストごとに設定することは実用的ではありません。

**OmniRoute がそれを解決する方法:**

- **システム パラメータの挿入** — 全体のリクエストにグローバル パラメータをアプレーションバーに適用します。
- **推論予算の検証** — リクエスト毎のパスソー トークンの制御を実装します。 (ポアススルー、オート、カスタム、アダプティブ)
- **6 の router ストラテジー** — 全体のパターンを決定するためのグローバル ストラテジー
- **ワイルドカード ルーター** — プロバイダー / *パターンは、ワイルドカード パターンが任意のプロバイダーにルーティングします
- **Combo 有効/無効のトグル** — ダッシュボードからコンボを有効/無効化できます
- **プロバイダーのtoggle** — 1つのクックですべての対応するプロバイダを有効/無効化します
- **ブロックしたプロバイダー** — スペフィックがブロックされたプロバイダは、`/v1/モデル / `のリストから排除することができます

</details>

<details>
<summary><b>🧰 17. "I need MCP tools as first-class product capabilities"</b></summary>

多くの AI ゲートウェイは MCP
を隠した実行部門のみで実装したり、隠さずには実現することができない場合もあり、その為、チームは一部を管理するため、操作の透明性を必要とします。

**OmniRoute がそれを解決する方法:**

- マスター コントロール プラーナ (MCP) はダッシュボード ナビゲーションとエンドポイント プロトコル タブに表示されます。
- MCP管理専用ページにプロセス、ツール、スコープ、監査が表示されます。
- [25]- omniroute コマンドのサーバー セットアップとクライアント オンボード ワークフロー

</details>

<details>
<summary><b>🧠 18. "I need A2A orchestration with sync + stream task paths"</b></summary>

エージェント ワークフローでは、直接応答と長時間ストリーミング実行の両方のライフサイクル制御機能が必要です。

**OmniRoute がそれを解決する方法:**

- A2A JSON-RPC エンド ポイント ( [23]- POST /a2a[x33]) には、[41]- メッセージを送信[x54] および [60]-
  メッセージをストリーミング[x75]機能が含まれます。
- SSE ストリーミングにステータス伝播機能があります。
- タスク ライフサイクル API には、[24]- タスクを取得[x34] および [40]- タスクをキャンセル[x53]機能が含まれます。

</details>

<details>
<summary><b>🛰️ 19. "I need real MCP process health, not guessed status"</b></summary>

オペレーショナル チームには、マスター コントロール プラーナが実際に稼動しているかどうかを知ることが必要です。

**OmniRoute がそれを解決する方法:**

- パフォーマンス カウンター ファイルに PID、タイムスタンプ、トランスポート、ツール カウント、スコープ モードが含まれます。
- MCP ステータス API には、ハートビートと最近の活動を組み合わせて読込になります。
- アクティビティ UI カードには、プロセス/稼動時間/ハートビートの新鮮さ機能が含まれます。

</details>

<details>
<summary><b>📋 20. "I need auditable MCP tool execution"</b></summary>

ツールが構成を変化させるときやオペレーションをトリガするときには、トレースアビリティが必要です。

**OmniRoute がそれを解決する方法:**

- MCP トール カール スタア ルギニ には、sqlite バッククド アウディア ラギニ機能が含まれます。
- フィルタリングには ツール、成功/失敗、API キー、ページネーションが必要です。
- ダッシュボード アウディア ラギニ テーブルと統計 エンド ポイントはオートメーション管理機能をサポートします。

</details>

<details>
<summary><b>🔐 21. "I need scoped MCP permissions per integration"</b></summary>

異なるクライアントがツール カテゴリに最低権限アクセスを要します。

**OmniRoute がそれを解決する方法:**

- 9 granular MCP スコープの制御されたツールアクセス
- スコープの取り入れと視覚化を含む MCP管理UI
- 安全なデフォルトポジティブフルオペレーションティングへの統制

</details>

<details>
<summary><b>⚙️ 22. "I need operational controls without redeploying"</b></summary>

インシデントまたはコストイベント中の、チームの迅速な実行時間の変更が必要です。

**OmniRoute がそれを解決する方法:**

- MCP ダッシュボードからコンビネータの直接アクティベーション
- 事前に定義されたポリシーパックからリジリエンス プロフィールの適用
- 同じオペレーションペナルからサーカイット ブレイカー ステートをリセット

</details>

<details>
<summary><b>🔄 23. "I need live A2A task lifecycle visibility and cancellation"</b></summary>

ライフサイクルビューがなく、タスクのインシデントをトリアージしたりすることは困難になります。

**OmniRoute がそれを解決する方法:**

- 状態/スキルでpaginateしてタスクの一覧/フィルタリング
- タスクのメタデータ/イベント/アーティファクトへのドリルダウン
- キャンセルタスクエンドポイントおよびUIアクションに対する確認

</details>

<details>
<summary><b>🌊 24. "I need active stream metrics for A2A load"</b></summary>

継続的 デリバリを必要とするストリーミング ワークフローは、活発な実行中の接続の視覚化が必要です。

**OmniRoute がそれを解決する方法:**

- A2A状態のアクティブ ストリーム カウントの統合
- 最後のタスク ステータス タイムスタンプとステートあたりのカウント
- A2A ダッシュボード カードをリアルタイム オペレーションモニタリング

</details>

<details>
<summary><b>🪪 25. "I need standard agent discovery for clients"</b></summary>

クライアントまたはオーシャレータに、ライブラリアクセス可能なメタデータを送信する必要があります。

**OmniRoute がそれを解決する方法:**

- Agent Card exposed at `/.well-known/agent.json`
- Capabilities and skills shown in management UI
- A2A status API includes discovery metadata for automation

</details>

<details>
<summary><b>🧭 26. "I need protocol discoverability in the product UX"</b></summary>

If users cannot discover protocol surfaces, adoption and support quality drop.

**OmniRoute がそれを解決する方法:**

- Consolidated **Endpoints** page with tabs for Proxy, MCP, A2A, and API
  Endpoints
- Inline service status toggles (Online/Offline) for MCP and A2A
- Links from overview to dedicated management tabs

</details>

<details>
<summary><b>🧪 27. "I need end-to-end protocol validation with real clients"</b></summary>

Mock tests are not enough to validate protocol compatibility before release.

**OmniRoute がそれを解決する方法:**

- E2E suite that boots app and uses real MCP SDK client transport
- A2A client tests for discovery, send, stream, get, and cancel flows
- Cross-check assertions against MCP audit and A2A tasks APIs

</details>

<details>
<summary><b>📡 28. "I need unified observability across all interfaces"</b></summary>

Splitting observability by protocol creates blind spots and longer MTTR.

**OmniRoute がそれを解決する方法:**

- Unified dashboards/logs/analytics in one product
- Health + audit + request telemetry across OpenAI, MCP, and A2A layers
- Operational APIs for status and automation

</details>

<details>
<summary><b>💼 29. "I need one runtime for proxy + tools + agent orchestration"</b></summary>

Running many separate services increases operational cost and failure modes.

**OmniRoute がそれを解決する方法:**

- オープンAI互換プロキシ、MCPサーバー、A2Aサーバーを1つのスタックに統合
- 共有認証、耐性、データストア、および可視性
- すべてのインタラクション上でのポリシーモデルを一元化

</details>

<details>
<summary><b>🚀 30. "I need to ship agentic workflows without glue-code sprawl"</b></summary>

チームのペースが遅くなるのは、複数のアドホックサービスコードを組み合わせることです

**OmniRoute がそれを解決する方法:**

- クライアントやエージェント向けの統一されたエンドポイント戦略
- 組みみたプロトコルマネジメントUIおよびスマック検証パス
- 生産環境に適した基盤(セキュリティ、ロギング、耐性、バックアップ)

</details>

### 例プレイブック (取り組み)

**プレイブックA：有料サブスクリプションを最大化＋低価格バックアップ**

```txt
組み合わせ:「maximize-claude」
  1. cc/claude-opus-4-6
  2. glm/glm-4.7
  3. if/kimi-k2-thinking

月額費用: $20 + バックアップスペンド
結果: 高品質、ゼロの遮断
```

**プレイブックB：コストゼロのコーディングスタック**

```txt
組み合わせ:「free-forever」
  1. gc/gemini-3-flash
  2. if/kimi-k2-thinking
  3. qw/qwen3-coder-plus

月額費用: $0
結果: 安定した無料コーディングワークフロー
```

**プレイブックC：24/7常時オンのフェールバックチェーン**

```txt
組み合わせ:「always-on」
  1. cc/claude-opus-4-6
  2. cx/gpt-5.2-codex
  3. glm/glm-4.7
  4. minimax/MiniMax-M2.1
  5. if/kimi-k2-thinking

結果: 重要なタスクの間に深いフェールバックの奥行きを実現
```

**プレイブックD：エージェントOPス・マCP + A2A**

```txt
1) MCPトランスポートを開始する (`omniroute --mcp`) をツールドライブ オペレーション
2) A2Aタスクを実行する (メッセージ/送信`と`、メッセージ/ストリーム`と`)
3) /ダッシュボード/エンドポイント (MCPおよびA2Aタブ) で観察する
4) inlineステータス制御でサービスを切り替える
```

---

## 🆓_start Free — Zero_Configuration Cost

> $0/月の**AI コーディングをセットアップせずに[30X]分で[X36X] $0 **月の月額構成 コネクト
> これらの無料アカウントを使用して、組みみた**Free Stack** 組み合わせの組み合わせ。

| Step | アクション                                     | プロバイダーロック                                                    |
| ---- | ----------------------------------------- | ------------------------------------------------------------ |
| 1    | [Kiro]を接続 (AWS メンバー ID OAuth)             | クーロンソネット 4.5、ハイキュー 4.5 — [unlimited]                         |
| 2    | [iFlow]を接続 (Google OAuth)                 | kimi-k2-thinking、qwen3-coder-plus、deepseek-r1… — [unlimited] |
| 3    | [Qwen]を接続 (デバイス コード)                      | qwen3-coder-plus、qwen3-coder-flash… — [unlimited]            |
| 4    | Gemini CLIを接続 (Google OAuth)              | gemini-3-flash、gemini-2.5-pro — [180K/mo free]               |
| 5    | dashboard/combos → Free Stack ($0) テンプレート | すべての無料プロバイダを自動で転送する                                          |

任意のIDE/CLIにアクセス:「http://localhost:20128/v1」 · API キー: 「あらゆる文字」 ·完了。

> Optional追加のカバレージ(無料)(カバレージ): [Groq API キー (30 RPM,無料)、NVIDIA NIM (40
> RPM,無料、70+モデル)、Cerebras (1M tok/ day)、LongCat API キー (50M トークン/日!) 、Cloudflare
> Workers AI (10Kニューロン/日、50+モデル)。

## クイックスタート

### 1. インストールして実行する

```bash
npm install -g omniroute
omniroute
```

> **omnirmnpm users:** Run `omnirmnpm approve-builds -g` after install to enable
> native build scripts required by `better-sqlite3` and `@swc/core`:
> 
> ```bash
> omnirmpnm install -g omniroute
> omnirmnpm approve-builds -g   # Select all packages → approve
> omniroutem
> ```

ダッシュボードは `http://localhost:20128` でオープンされ、アウトレットベースURLは
`http://localhost:20128/v1` になります。

| コマンド                 | 説明                                           |
| -------------------- | -------------------------------------------- |
| `omnirm`             | サーバーを起動（`PORT=20128`を指定する、APIとダッシュボードは同一ポート） |
| `omnirm --port 3000` | APIとダッシュボードのポートを別個にする                        |
| `omnirm --mcp`       | MCPサーバーを起動（stdioトランスポート）                     |
| `omnirm --no-open`   | ブラウザを自動で開かない                                 |
| `omnirm --help`      | ヘルプを表示                                       |

オプションのポート分割モード：

```bash
PORT=20128 DASHBOARD_PORT=20129 omnirm
# アウトレット: http://localhost:20128/v1
# ダッシュボード: http://localhost:20129
```

### 2) Connect providers and create your API key

1. Open Dashboard → `Providers` and connect at least one provider (OAuth or API
   key).
2. Open Dashboard → `Endpoints` and create an API key.
3. (Optional) Open Dashboard → `Combos` and set your fallback chain.

### 3) Point your coding tool to OmniRoute

```txt
Base URL: http://localhost:20128/v1
API Key:  [copy from Endpoint page]
Model:    if/kimi-k2-thinking (or any provider/model prefix)
```

Works with Claude Code, Codex CLI, Gemini CLI, Cursor, Cline, OpenClaw,
OpenCode, and OpenAI-compatible SDKs.

### 4) Enable and validate protocols (v2.0)

**MCP (for tool-driven operations):**

```bash
omniroute --mcp
```

Then connect your MCP client over `stdio` and test tools like:

- `omniroute_get_health`
- `omniroute_list_combos`

**A2A (for agent-to-agent workflows):**

```bash
curl http://localhost:20128/.well-known/agent.json
```

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"quickstart","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"Give me a short quota summary."}]}}'
```

### 5) Validate everything end-to-end (recommended)

```bash
npm run test:protocols:e2e
```

This suite validates real MCP and A2A client flows against a running app.

### Alternative: run from source

```bash
cp .env.example .env
npm install
ポート番号20128 がDASHBOARD_PORT 20129としてNEXT_PUBLIC_BASE_URL=http://localhost:20129 に設定されています。 npm run dev
```

---

## 🐳 Docker

OmniRoute は、[Docker
Hub](https://hub.docker.com/r/diegosouzapw/omniroute)上で公共のDocker イメージとして利用可能です。

**Quick run:**

```bash
docker run -d \
  --name omniroute \
  --restart unless-stopped \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:latest
```

**エンドポイントファイルを指定:**

```bash
# .envファイルをコピーして編集してください
cp .env.example .env

docker run -d \
  --name omniroute \
  --restart unless-stopped \
  --env-file .env \
  -p 20128:20128 \
  -v omniroute-data:/app/data \
  diegosouzapw/omniroute:latest
```

**Docker Composeを使用:**

```bash
# 基準プロファイル（CLIツールが付属していない）
docker compose --profile base up -d

# CLIプロファイル（Claude Code、Codex、OpenClaw組み込み）
docker compose --profile cli up -d
```

| 画像                       | タグ       | サイズ    | 説明          |
| ------------------------ | -------- | ------ | ----------- |
| `diegosouzapw/omniroute` | `latest` | 約250MB | 最新の安定したリリース |
| `diegosouzapw/omniroute` | `1.0.3`  | 約250MB | 現在のバージョン    |

---

## 🖥️ デスクトップ アプリ — オフライン & 常にオンライン

> 🆕 **NEW!** オミニルートは、Windows、macOS、Linux用の **ナティブ デスクトップアプリケーション**として利用可能になりました。

オミニルートをスタンドアロンとして実行することができます —
ローカルモデルの場合、任意のインターネット接続無しで。エレクトロンベースのアプリケーションには以下のような機能があります。

- 🖥️ **ネイティブ ウインドウ** — システムトレイ統合を含む専用アプリケーションウィンドウ
- 🔄 **オートスタート** — システムログイン時にオミニルートを起動する
- 🔔 **ネイティブ ノーティフィケーション** — クォータ枯渇またはサービスの問題の際に警告される
- ⚡ **ワンクリック インストール** — NSIS（Windows）、DMG（macOS）、AppImage（Linux）
- 🌐 **オフライン モード** — サーバーをプаковして、完全にオフラインで動作します

### クイックスタート

```bash
# デバッグモード
npm run electron:dev

# バイルトのためのビルド
npm run electron:build         # カレント プラットフォーム
npm run electron:build:win     # Windows (.exe)
npm run electron:build:mac     # macOS (.dmg) — x64 &amp; arm64
npm run electron:build:linux   # Linux (.AppImage)
```

### System Tray

オミニルートを最小化すると、システムトレイに表示され、以下のようなアクションが可能です。

- ダッシュボードを開く
- サーバー ポートを変更する
- アプリケーションを終了する

📖 フル ドキュメント: [`electron/README.md`](electron/README.md)

---

## 💰 プライシング アット グラムス

| レイヤ             | Provider                   | コスト                      | クォータ リセット                 | ベストプラン                            |
| --------------- | -------------------------- | ------------------------ | ------------------------- | --------------------------------- |
| **💳 契約**        | クロード コード (プロ)              | $20/月                    | 1週間あたり5時間                 | すでに契約済み                           |
|                 | コドックス（プラス/プロ）              | $20-$200/月               | 1週間あたり5時間                 | OpenAI ユーザー                       |
|                 | ジェミニ CLI                   | **FREE**                 | 月あたり180,000回 + 日あたり1,000回 | 誰でも使える！                           |
|                 | GitHub コパイロット              | $10-$19/月                | 毎月                        | GitHub ユーザー                       |
| **🔑 API キー**    | NVIDIA NIM                 | **FREE** (開発者だけ永遠に)      | 40 RPM                    | 70名以上のモデルが開放中                     |
|                 | Cerebras                   | ** 無料 ** (1M 単位/日)       | 60万 TPM / 40 RPM          | 世界最速                              |
|                 | Groq                       | ** 無料 ** (40 RPM)        | 14.4K RPD                 | 超高速のLlama/Gemma                   |
|                 | DeepSeek V3.2              | $0.27/$1.10 per 1M       | なし                        | 最高の価格経済的な考慮                       |
|                 | xAI Grok-4 Fast            | **$0.20/$0.50 per 1M** 🆕 | なし                        | 最速 + 工具コール、超低コスト                  |
|                 | xAI Grok-4 (標準)            | $0.20/$1.50 per 1M 🆕     | なし                        | xAIから生まれた推論の最高峰                   |
|                 | ミストラル                      | フリートライアル＋有料              | レート制限あり                   | ヨーロッパAI                           |
|                 | OpenRouter                 | 使用者ごみコスト                 | なし                        | 100+モデル集約                         |
| **💰  安い**       | GLM-5（via Z.AI） 🆕          | $0.5/1,000万              | 毎日10時                     | 128K出力、最新フラッグシップ                  |
|                 | GLM-4.7                    | $0.6/1,000万              | 毎日10時                     | 予備費用                              |
|                 | ミニマックス M2.5 🆕              | $0.3/1,000万入力            | 5時間ローリング                  | 推論+行動タスク                          |
|                 | ミニマックス M2.1                | 0.2/100万                 | 5時間ローリング                  | きついオプション                          |
|                 | Kimi K2.5 (Moonshot API) 🆕 | 使用者ごみコスト                 | なし                        | Direct Moonshot APIアクセス           |
|                 | Kimi K2                    | $9/moフラット                | 10,000万トークン/mo            | 予想のコスト                            |
| **🆓 бесплатно** | iFlow                      | **$0**                   | 無制限                       | 5モデル無制限                           |
|                 | Qwen                       | **$0**                   | 無制限                       | 4モデル無制限                           |
|                 | Kiro                       | **$0**                   | 無制限                       | Claude Sonnet/Haiku (AWS Builder) |
|                 | LongCat Flash-Lite 🆕       | **$0** (50M tok/day 🔥)   | 1 RPS                     | 世界最大のフリクォータ                       |
|                 | Pollinations AI            | **$0** (no key needed)   | 1 req/15s                 | GPT-5, Claude, DeepSeek, Llama 4  |
|                 | Cloudflare Workers AI      | **$0** (10K Neurons/day) | ~150 resp/day             | 50+ models, global edge           |
|                 | Scaleway AI                | **$0** (1M tokens total) | レート制限あり                   | EU/GDPR, Qwen3 235B, Llama 70B    |

> 🆕 **New models added (Mar 2026):** Grok-4 Fast family at $0.20/$0.50/M
> (benchmarked at 1143ms — 30% faster than Gemini 2.5 Flash), GLM-5 via Z.AI
> with 128K output, MiniMax M2.5 reasoning, DeepSeek V3.2 updated pricing, Kimi
> K2.5 via Moonshot direct API.

**💡 $0 Combo Stack — The Complete Free Setup:**

```
🆓 最終的フリースタック 2026 — 11 のプロバイダー、 $0 である
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

**Zero cost. Never stops coding.** このオミンモードを組み合わせて、すべてのフォールバックが自動で発生 —
マニュアルでswicthする必要はありません。

---

---

## 🆓 Free Models — What You Actually Get

> 以下のすべてのモデルは **%100フリーワザーケード、クレジットカードなし必要** All OmniRoute
> modelsがローターベータインを使って、すべて同じクオーターが終わったとき。 Omirmodeをまとめて組み合わせてアンブレイクな$0 combo

### 🔵 CLAUDE MODELS (Kiro — AWS Builder ID)

| Model               | プレフィックス | limit   | レート制限            |
| ------------------- | ------- | ------- | ---------------- |
| `claude-sonnet-4.5` | `kr/`   | **無制限** | 日間制限なし           |
| `claude-haiku-4.5`  | `kr/`   | **無制限** | 日間制限なし           |
| `claude-opus-4.6`   | `kr/`   | **無制限** | 最新のオーピュスvia kiro |

### 🟢IFLOW MODELS(フリーOAuth — クレジットカードなし)

| Model              | プレフィックス | limit   | レート制限    |
| ------------------ | ------- | ------- | -------- |
| `kimi-k2-thinking` | `if/`   | **無制限** | 未報告の制限なし |
| `qwen3-coder-plus` | `if/`   | **無制限** | 未報告の制限なし |
| `デープシーク-r1`        | `if/`   | **無制限** | 未報告の制限なし |
| `ミニマックス-m2.1`      | `if/`   | **無制限** | 未報告の制限なし |
| `キミ-k2`            | `if/`   | **無制限** | 未報告の制限なし |

### 🟡 QWEN モデル (機器 ID 認証)

| Model              | プレフィックス | limit   | レート制限        |
| ------------------ | ------- | ------- | ------------ |
| `qwen3-coder-plus` | `qw/`   | **無制限** | 未報告の制限なし     |
| `KWEN3 コーダー フラッシュ` | `qw/`   | **無制限** | 未報告の制限なし     |
| `KWEN3 コーダー ネクスト`  | `qw/`   | **無制限** | 未報告の制限なし     |
| `ビジョンモデル`          | `qw/`   | **無制限** | マルチモーダル (画像) |

### 🟣 ジェミニ CLI (Google OAuth)

| Model                    | プレフィックス | limit                       | レート制限  |
| ------------------------ | ------- | --------------------------- | ------ |
| `gemini-3-flash-preview` | `gc/`   | **180K tok/month** + 1K/day | 월초 리셋  |
| `gemini-2.5-pro`         | `gc/`   | 180K/month (shared pool)    | 고객 만족度 |

### ⚫ NVIDIA NIM (Free API Key — build.nvidia.com)

| レイヤ        | 1日あたりの制限 | レート制限       | 注意事項                                      |
| ---------- | -------- | ----------- | ----------------------------------------- |
| Free (Dev) | 토큰 제한 없음 | **~40 RPM** | 2025년 중반 pure rate limits 전환 중입니다: 70+ 모델 |

인기있는 무료 모델: `moonshotai/kimi-k2.5` (Kimi K2.5), `z-ai/glm4.7` (GLM 4.7),
`deepseek-ai/deepseek-v3.2` (DeepSeek V3.2), `nvidia/llama-3.3-70b-instruct`,
`deepseek/deepseek-r1`

### ⚪ CEREBRAS (Free API Key — inference.cerebras.ai)

| レイヤ | 1日あたりの制限          | レート制限            | 注意事項                     |
| --- | ----------------- | ---------------- | ------------------------ |
| 無料  | **1M tokens/day** | 60万 TPM / 40 RPM | 世界最速のLLMインフェランス; 日毎にリセット |

無料で利用可能: `llama-3.3-70b`, `llama-3.1-8b`, `deepseek-r1-distill-llama-70b`

### 🔴 GROQ (無料API Key — console.groq.com)

| レイヤ | 1日あたりの制限      | レート制限       | 注意事項                          |
| --- | ------------- | ----------- | ----------------------------- |
| 無料  | **14.4K RPD** | モデルごとに30RPM | クレジットカードなし; 限界を超えると429発生、請求なし |

利用可能: `llama-3.3-70b-versatile`, `gemma2-9b-it`, `mixtral-8x7b`,
`whisper-large-v3`

### 🔴 LONGCAT AI (無料 API Key — longcat.chat) 🆕

| Model                         | プレフィックス      | 毎日無料クオタ          | 注意事項          |
| ----------------------------- | ------------ | ---------------- | ------------- |
| `LongCat-Flash-Lite`          | [カスタマーのID]/` | **50M tokens** 💥 | 歴史的最も大きい無料クオタ |
| `LongCat-Flash-Chat`          | [カスタマーのID]/` | 500K tokens      | マルチターンの会話     |
| `LongCat-Flash-Thinking`      | [カスタマーのID]/` | 500K tokens      | 推論 / CoT      |
| `LongCat-Flash-Thinking-2601` | [カスタマーのID]/` | 500K tokens      | 2026年1月版      |
| `LongCat-Flash-Omni-2603`     | [カスタマーのID]/` | 500K tokens      | マルチモーダル       |

> パブリックベータ中は完全無料。 EMAILまたは電話で[longcat.chat](https://longcat.chat)に登録してください。
> 00:00 UTCで毎日リセットされます。

### 🟢 POLLINATIONS AI (APIキーなし) 🆕

| Model      | プレフィックス | レート制限     | プロバイダー 後ろ          |
| ---------- | ------- | --------- | ------------------ |
| `openai`   | `pol/`  | 1 req/15s | GPT-5              |
| `claude`   | `pol/`  | 1 req/15s | Anthropic Claude   |
| `gemini`   | `pol/`  | 1 req/15s | Google Gemini      |
| `deepseek` | `pol/`  | 1 req/15s | DeepSeek V3        |
| `llama`    | `pol/`  | 1 req/15s | Meta Llama 4 Scout |
| `mistral`  | `pol/`  | 1 req/15s | Mistral AI         |

> ✨ **ゼロ抵抗:** 無料登録、API キーなし。空のキー フィールドで Pollinations プロバイダーを追加すれば即効。

### 🟠 CLOUDFLARE WORKERS AI (無料 API キー — cloudflare.com) 🆕

| レイヤ | 毎日ニューロン  | 使用例                               | 注意事項              |
| --- | -------- | --------------------------------- | ----------------- |
| 無料  | 10,000** | ~150 LLM 導入量 / 500秒音声 / 15K エンバेड | グローバル エッジ、50+ モデル |

人気のフリーモデル: `cf/meta/llama-3.3-70b-instruct`, `cf/google/gemma-3-12b-it`,
`cf/openai/whisper-large-v3-turbo` (フリーアコースティック!),
`cf/qwen/qwen2.5-coder-15b-instruct`

> API トークン + アカウント ID を [dash.cloudflare.com](https://dash.cloudflare.com)
> から求めます。アカウント ID をサービス設定に保存してください。

### 🟣 SCALEWAY AI (1,000,000 フリータウン_tokens — scaleway.com) 🆕

| レイヤ | フリーコロタ           | ロケーション   | 注意事項                          |
| --- | ---------------- | -------- | ----------------------------- |
| 無料  | 1,000,000** トークン | 🇫🇷 パリ、EU | クレジットカードが必要なく、一定額以内でサポートされます。 |

利用可能な無料: `qwen3-235b-a22b-instruct-2507` (Qwen3 235B!),
`llama-3.1-70b-instruct`, `mistral-small-3.2-24b-instruct-2506`,
`deepseek-v3-0324`

> EU/GDPR 規制に適合しています。 API キーは
> [console.scaleway.com](https://console.scaleway.com) から取得してください。

> **💡 最高のフリースタック (11 サービス、$0 永久):**
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

| Provider         | Free Credits           | Best Model                                   | レート制限                        |
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

🎉 [X0X]/ダッシュボード/メディア` → **トランスクリプション** タブ：音声または動画ファイルをアップロード → 組み込みエンドポイントを選択 →
対応する形式でトランスクリプションを取得。

## 💡 重要機能

OmniRoute v2.0は、リレー プロキシだけではなく、運用プラットフォームとして構築されています。

### 🆕新規 — 怪力ルーターインスピレーションの改良（2026年3月）

| 機能                          | 機能概要                                                                         |
| --------------------------- | ---------------------------------------------------------------------------- |
| ⚡ ** Grok-4 ファストファミリー**     | xBenchmark$0.20/ $0.50/M — 1143ms (Gemini 2.5 Flashより30%速い)                  |
| 🧠 ** GLM-5 via Z.AI**       | 128K 出力コンテキスト、 $0.5/1M — 最新旗艦モデルはGLM ファミリー                                   |
| 🔮 **MiniMax M2.5**          | 推論 + 代理タスク、 $0.30/1M —  M2.1 と比較し、著しいアップグレード                                 |
| 🎯 **toolCalling フラグごとにモデル** | モデルごとの `toolCalling: true/false` レジストリ — AutoCombo は、ツールでないモデルをスキップします       |
| 🌍 ** マルチ言語の意図検出**           | PT/ZH/ES/AR キーワードはAutoCombo スコアリングで使用 —  非英語コンテンツのためのモデル選択には、より適切なモデルが選択されます |
| 📊 ** ベンチマークドライブでフォールバック**   | リアル リクエストの p95 ラテンシティが、カンバス スコアリングに反映されます — AutoCombo は実際のデータを基にして学習します      |
| 🔁 ** リクエスト ディープリケーション**     | コンテンツハッシュベースのデプロイ ウィンドウ — マルチエージェント向けに安全で、複製料金を防止                            |
| 🔌 **プラグナブル ルータースタレジー**      | カスタムルーティングロジックをプラグインとして追加できる拡張可能な `ルータースタレジー` インターフェース                       |

### 🚀 Previous v2.0.9+ — Playground、CLI Fingerprints & ACP

| 機能                                   | 機能概要                                                                                                                                                                   |
| ------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🎮 **モデル プレイグラウンド**                   | モデルを直接テストできるダッシュボードページ — プロバイダー/モデル/エンドポイント セレクタ、モナコ エディター、ストリーミング、アボート、タイミング                                                                                          |
| 🔏 **CLI フィンガープリント マッチング**            | ネイティブ CLIサインチャをマッチングするためのプロバイダー毎のヘッダ/ボディの並べ替え — セキュリティ > セキュリティ設定でプロバイダー毎にトグル **あなたのプロキシ IPは保存されます**                                                                   |
| 🤝 **ACP サポート (エージェント クライアント プロトコル)** | Codex、Claude、Goose、Gemini CLI、OpenClaw + 9 以上のCLIツールのエージェント検出 (アジャイル)、プロセス スパウナー、`/api/acp/エージェント` エンドポイント                                                             |
| 🤖 **ACP エージェント ダッシュボード**             | デバッグ › エージェント タブ — 14 つのエージェントのグリッド、インストール状態、バージョン、カスタム エージェント フォームが表示される。 **オープンコード** ユーザーには「ダウンロード opencode.json」ボタンが表示されるのが特徴で、自動生成された設定ファイルにはすべての利用可能なモデルが含まれています。 |
| 🔧 **カスタム モデル `apiFormat` ルーティング**    | カスタム モデルに `apiFormat : "responses"` が指定されている場合、正しく Responses API トランスレータに向かいます。                                                                                        |
| 🏢 **コデックス ワーク スペース アイザベーション**        | オーサスを使用して複数のワーク スペースがあれば、ワーク スペース IDごとに接続を正しく分離するOAuth                                                                                                                 |
| 🔄 **電子 オートアップデート**                   | デスクトップ アプリケーションはアップデートのチェック & アプリケーションの自動インストール                                                                                                                        |

### 🤖 エージェント & プロトコル オペレーション (v2.0)

| 機能                                    | 機能概要                                                                                               |
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
| 🧪 **プロトコル E2E テストハーネス**               | リアル MCP SDK + A2A クライアント フローの方程式 in `test:protocols:e2e`                                           |
| ⚙️ **実稼働操作管理**                        | スイッチ組み合わせ、適用される耐性プロファイルと、1 つの制御表面から破壊される機能                                                         |

### 🧠 ルーティング & 知能

| 機能                       | 機能概要                                                  |
| ------------------------ | ----------------------------------------------------- |
| 🎯 **スマート 4 層ファールバック**    | 自動ルーティング: セールス システム → API キー → 有料 → 無償                |
| 📊 **リアルタイムクォータ追跡**       | ライブトークン数 + リセットカウント ダウタイマーあらわす                        |
| 🔄 **フォーマット変換**           | OpenAI ↔ Claude ↔ Gemini ↔ レスポンスとスキーマセーフな変換           |
| 👥 **マルチアカウントサポート**       | プロバイダあらわす、複数のアカウントあらわす                                |
| 🔄 **自動トークンリフレッシュ**       | OAuth トークンが自動リフレッシュする機能のあるリトライ                        |
| 🎨 **カスタム組み合わせ**          | 6 バランス戦略 + 併用チェーン制御                                   |
| 🌐 **ワイルドカードルーター**        | `サービスのプロバイダー /*`ダイナミックルーティング                          |
| ✨ **思考と予算管理              | 自動、カスタム、そして適応可能な推論制限                                  |
| ✨ **モデルエイリアス**           | ユーザー定義のモデルエイリアスと安全なマイグレーション                           |
| ⚡ **バックグラウンドの劣化**        | 低優先度のバックグラウンドタスクを安価なモデルにrerouteする                     |
| 🧪 **タスクで意識したスマートルーティング** | 自動でコンテンツのタイプ（コード/シーム/分析/要約）でモデルを選択                    |
| 💬 **システムプロンプトの投射**       | 汎用的な動作制御を統一的に適用                                       |
| 📄 **レスポンスAPIの互換性**       | Codexと高度なアジエンティーフローのために[full /v1/responses` サポートがあります |

### 🎵 マルチモーダルAPI

| 機能                  | 機能概要                                                                                                                                                  |
| ------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
| 🖼️ **イメージジェネレーション** | `/v1/images/generations` のクラウド基盤とローカル基盤                                                                                                               |
| 📐 **埋め込みデータ**       | `/v1/embeddings` の検索とRAGパイプライン                                                                                                                        |
| 🎤 **オーディオ断片録音**     | `/v1/audio/transcriptions` — 7 providers (Deepgram Nova 3, AssemblyAI, Groq Whisper, HuggingFace, ElevenLabs, OpenAI, Azure), 自動言語検出、MP4/MP3/WAV サポート |
| 🔊 **音声合成**          | `/v1/audio/speech` — 10 providers (ElevenLabs, OpenAI, Deepgram, Cartesia, PlayHT, HuggingFace, Nvidia NIM, Inworld, Coqui, Tortoise) に正しいエラーコードを持つ   |
| 🎬 **ビデオ生成**         | `/v1/videos/generations` (ComfyUI + SD WebUI ワークフロー)                                                                                                  |
| 🎵 **楽曲生成**          | `/v1/music/generations` (ComfyUI ワークフロー)                                                                                                              |
| 🛡️ **モデレーション**      | `/v1/moderations` セーフティ チェック                                                                                                                          |
| 🔀 **再ランキング**        | `/v1/rerank` に関する関連度スコアリングのために                                                                                                                        |
| 🔍 **ウェブ検索** 🆕       | `/v1/search` — 5 providers (Serper, Brave, Perplexity, Exa, Tavily), 6,500+ free/month、自動フェイルオーバー、キャッシュ                                               |

### 🛡️ リズム、セキュリティ & ゴバナンス

| 機能                        | 機能概要                                                      |
| ------------------------- | --------------------------------------------------------- |
| 🔌 **サーキットブレイカー**          | マス目式リリース/復元ウィズ ユーザー定義のしきい値コントロール                          |
| 🎯 **エンドポイント認識モデル**        | カスタムモデルによってサポートされているエンドポイント + API フォーマット                  |
| 🛡️ **嵐を防ぐ羊**              | リトライ/レートイベントにおけるミューテックス + セマフォ保護                          |
| 🧠 **意味的 + 署名キャッシュ**       | 2 つのキャッシュレイヤを使用したコスト/遅延の削減                                |
| ⚡ **要求の恒等性**              | 重複保護期間                                                    |
| 🔒 **TLS の指紋の偽似**          | ボットの検出とアカウントのフラグの削減のためにブラウザ_like の TLS 指紋 — **のアセスを低減する** |
| 🔏 **CLI フィンガープリント マッチング** | 起源のCLI要求の署名にマッチする — **のバンリスクを低減しつつプロキシIPを保存する**           |
| 🌐 **IP 判別**               | 公開配布する暴露された設定でアロールリスト/ブロックリストの制御                          |
| 📊 **編集可能な速度制限**           | グローバル/プロバイダーレベルにパーミテンス付きで調整可能な制限設定                        |
| 🔑 **API キー の管理 + スコープ**   | 安全なキー発行/回転とモデル/プロバイダの制御                                   |
| 🛡️ **保護された `/models`**    | モデルカタログの為のオプショナルな認証入力とプロバイダの非表示                           |

### 📊 オブザーブリティ & 分析

| 機能                      | 機能概要                                   |
| ----------------------- | -------------------------------------- |
| 📝 **リクエスト + プロキシ ロギング** | フル リクエスト レスポンス および プロキシ ロギング           |
| 📋 **統合ログ ダッシュボード**      | 1 ページ内でリクエスト 、プロキシ 、監査 、コンソール ビュー      |
| 🔍 **リクエスト テレメトリ**       | p50/p95/p99 ラティエンス および リクエスト トレース      |
| 🏥 **ヘルス ダッシュボード**       | アップタイム 、ブレーカー ステート 、ロックアウト 、キャッシュ スタッツ |
| 💰 **コスト トラッキング**        | バジェット コントロール および パーミデル プライシング 可視性      |
| 📈 **分析可視化**             | モデル プロバイダー 使用状況の洞察とトレンド ビュー            |
| 🧪 **評価 フレームワーク**        | ゴールデン セット テスト に関する可変マッチ ストリーエス         |

### ☁️ デプロイメント & プラットフォーム

| 機能                    | 機能概要                                           |
| --------------------- | ---------------------------------------------- |
| 🌐 **どこでもデプロイ**        | ローカルホスト, VPS, Docker, クラウド環境                   |
| 💾 **クラウド同期**          | クラウドワーカーを介した構成の同期                              |
| 🔄 **バックアップ/リストア**     | エクスポート/インポートとディザスターリカバーフローのフロー                 |
| 🧙 **セットアップ ウィザード**    | 初回実行ガイド付きセットアップ                                |
| 🔧 **CLI ツール ダッシュボード** | コーディングツールに対するポピュラーなワンクリックセットアップ                |
| 🎮 **モデル プレイグラウンド**    | ダッシュボード上からプロバイダー/モデル/エンドポイントをテスト               |
| 🔏 **CLI 指紋切替**        | デバイス > セキュリティ > セットアップ > プロバイダーごとに指紋情報を一致させる設定 |
| 🌐 **地域化 (30 言語)**     | ダッシュボード + 手冊の言語サポートと RTL カバレッジ                 |
| 🧹 **モデルをすべて消去**       | プロバイダー詳細でモデルの一覧を一括削除                           |
| 📋 **問題テンプレート**        | プルリクエストと新機能のための標準化されたGitHub テンプレート             |
| 📂 **カスタムデータの保存先**     | `データディレクトリ`のセッティング                             |

### 機能の深みにあたる解説

#### 実用的コストの管理を伴うスマートフォールバック

```txt
Combo:"my-coding-stack"
  1. cc/claude-opus-4-6
  2. nvidia/llama-3.3-70b
  3. glm/glm-4.7
  4. if/kimi-k2-thinking
```

クォタ,レート,またはヘルスが落ちてくると、OmniRouteは自動的に次の候補に切り替える。

#### プロトコルの組み込み管理は、操作可能で実行用のビジュアル形式。

- MCP + A2AはUI/ドキュメント上で見つけることができる。
- APIはリアルタイムで実行中のメトロポリタンデータを公開する(`/api/mcp/*`, `/api/a2a/*`)
- ダッシュボードでは、day2オペのアクションが含まれている(Comboの切り替え、ブレイカーのリセット、アクティビティのキャンセル)

#### 翻訳者のワークフローの検証者

翻訳者エリアには次の機能がある。

- **Playground**:要求の式化のチェック
- **Chat Tester**:要求と応答の全ワークロードの一巡
- **Test Bench**:複数のケースを一度の実行でテスト
- **Live Monitor**:リアルタイムのトラフィックビュー

＋プロトコルの検証もnpm run test:protocols:e2e`というユーザーを通じて行う。

> 📖 **[MCPサーバーのREADME](open-sse/mcp-server/README.md)** —ツールのルール、IDEの設定、クライアントの例
> 
> 📖 **[A2AサーバーのREADME](src/lib/a2a/README.md)**
> —スキル、JSON-RPCのメソッド、ストリーミング、アクティビティのライフサイクル

## 🧪Evaluations (Evals)

OmniRouteには、金色のセットを使用してLLMのレスポンスの品質を検証できる、組み込まれた評価フレームワークがある。アナリティクス⇒Evalsのダッシュボード上でアクセスしてください。

### Built-in Golden Set

「標準セットのオムニルート」には、次のテストケースが含まれています。

- 挨拶、数学、地理、コード生成
- JSON形式の連携、翻訳、Markdown生成
- 害になるコンテンツの拒絶、数え上げ、論理演算

### 評価戦略

| 戦略         | 説明                        | 例                                    |
| ---------- | ------------------------- | ------------------------------------ |
| `exact`    | Exactly の値が完全に一致する必要があります | `"4"`                                |
| `contains` | 含まれる値の一部が存在する             | `"Paris"`                            |
| `regex`    | 正規表現の形式の値が一致する            | `"1.*2.*3"`                          |
| `custom`   | カスタムJS関数がtrue値を返す         | `(sekai) =&gt; sekai.length &gt; 10` |

---

## 📖 セットアップ ガイド

### プロトコルセットアップ (MCP + A2A)

<details>
<summary><b>🧩 MCP Setup (Model Context Protocol)</b></summary>

MCP トランスポートを標準入力モードで開始する:

```bash
omniroute --mcp
```

推奨検証フロー:

1. 標準入力でMCPクライアントに接続する。
2. omniroute_get_health を実行する `。
3. omniroute_list_combos を実行する `。
4. ['X5X']/dashboard/mcp` を開いて、ハートビート、アクティビティ、オーディットを確認する。

自動化に便利なAPI:

- ['X0X']GET /api/mcp/status`.
- ['X0X']GET /api/mcp/tools`.
- ['X0X']GET /api/mcp/audit`.
- ['X0X']GET /api/mcp/audit/stats`.

</details>

<details>
<summary><b>🤝 A2A Setup (Agent2Agent)</b></summary>

エージェントを発見する:

```bash
curl http://localhost:20128/.well-known/agent.json
```

タスクを送信する:

```bash
curl -X POST http://localhost:20128/a2a \
  -H 'content-type: application/json' \
  -d '{"jsonrpc":"2.0","id":"setup-a2a","method":"message/send","params":{"skill":"quota-management","messages":[{"role":"user","content":"quota 利用状況を要約する。"}}]}}'
```

ライフサイクルを管理する:

- `GET /api/a2a/[[status]]X20X]
- `GET /api/a2a/tasksX19X]
- `GET /api/a2a/tasks/[id]X23X]
- `POST /api/a2a/tasks/[id]/cancelX31X]

[[Operational UI]]:

- `/{{dashboard}}/a2aX15X] for task/state/stream observability and smoke actions

</details>

<details>
<summary><b>🧪 End-to-end protocol validation</b></summary>

[X0X][X0X]プルートコールの両方を、実際のクライアントで検証する[[X15X]]X15X]

```bash
npm run test:protocols:e2e
```

[[verifies]]:

- MCP SDK クライアントの接続・リスト・コール
- A2A discovery/send/stream/get/cancel
- MCP アウディットと A2A タスク マネジメント API のデータをクロスチェック

</details>

<details>
<summary><b>💳 Subscription Providers</b></summary>

### [[Claude Code]]:

```bash
ダッシュボード→プロバイダー→Claude Codeを接続→オーソチックローカン→自動トークン リフレッシュ→5時間以上の+週間のクォータトラッキング

モデルの種類:
  cc/claude-opus-4-6
  cc/claude-sonnet-4-5-20250929
  cc/claude-haiku-4-5-20251001
```

**Pro Tip:**Opusを複雑なタスクに、Sonnetを速度で使用する[**]X10X]
OmniRouteはモデルごとにクォータをトラッキングしています

### [[OpenAI Codex]]:

```bash
ダッシュボード → プロバイダー → OpenAI Codex の接続
→ オーソチック ローカン (ポート 1455)
→ 5時間 + 週次リセット

モデルの種類:
  cx/gpt-5.2-codex
  cx/gpt-5.1-codex-max
```

#### [[Codex Account Limit]],

各 Codex アカウントには、[`]ダッシュボード-&gt;プロバイダー[`]でポリシーのトグルが用意されています:

- [[5h]] [[threshold]] (ON/OFF): 5時間のドロワーpolicyが効かないオフにすることができます。
- `週間` (オン/オフ): 週間ウィンドウしきい値ポリシーを強制します。
- しきい値の挙動: 有効なウィンドウが >=90% 使用されると、そのアカウントはスキップします。
- ローテーション挙動: OmniRoute は自動的に次のエリジブルなCodexアカウントにルーティングします。
- リセット挙動: プロバイダー `resetAt` 時間が経過すると、アカウントは再度エリジブルになります。

シナリオ:

- `5h ON` + `週期ON`: 両方のウィンドウのいずれかがしきい値に到達すると、アカウントはスキップされます。
- `5h OFF` + `週期ON`: ただし、週期の使用率がアカウントをブロックする唯一の要因となります。
- `5h ON` + `週期OFF`: ただし、5時間の使用率がアカウントをブロックする唯一の要因となります。
- `resetAt` that has passed: アカウントは自動的に再入轮询 (手動の再有効化なし)。

### ガンマ CLI (無料 180K/月!)

```bash
ドASHBOARD → プロバイダー → ガンマ CLI への 接続 →
Google OAuth
→ 1月に 180K 完成度/月 + 1K/日

モデル:
 gc / gemini-3 - Flash 予告
 gc / gemini-2.5 - プロ
```

**ベスト バリュー:** 巨大な無料枠内!. 有料枠前に使用するものです。

### GitHub コパイロット

```bash
ドシュボード → プロバイダー → GitHub への接続
→ GitHub による OAuth
→ 毎月リセット (1月月号)

モデル:
  gh / gpt-5
  gh / claude - 4.5 - sonnet
  gh / gemini - 3 - pro
```

</details>

<details>
<summary><b>🔑 API Key Providers</b></summary>

### NVIDIA NIM (無料の開発者用アクセス — 70+ モデル)

1. サインアッ : [build.nvidia.com](https://build.nvidia.com)
2. フリーア APIキーを取得する ( 1000 インフェレンシーセド内の)
3. ドシュボード → プロバイダー → NVIDIA NIM を追加 :
   - APIキー: ` nvapi-your -キー`

**モデル:** ` nvidia / llama - 3 - 70 B - 指示` 、` nvidia / mistral - 7 B - 指示` 等、50
モード以上

プロチップ：**オープンAIの互換性あるAPI — オムニルートのフォーマット翻訳と最大限に統合されます

### ディープシーク

1. 新規登録：[platform.deepseek.com](https://platform.deepseek.com)
2. APIキー取得
3. パネル → プロバイダー追加 → ディープシーク

**モデル：** `ディープシーク/deepseek-chat`, `ディープシーク/deepseek-coder`

### グロック（フリータイヤ利用可能）

1. 新規登録：[console.groq.com](https://console.groq.com)
2. APIキー取得（フリータイヤ含む）
3. パネル → プロバイダー追加 → グロック

**モデル：** `groq/llama-3.3-70b`, `groq/mixtral-8x7b`

**プロチップ：**リアルタイムコーディングに最適！超高速推論。

### オープンルーター（100+モデル）

1. 新規登録：[openrouter.ai](https://openrouter.ai)
2. APIキー取得
3. パネル → プロバイダー追加 → オープンルーター

**モデル：** オープンルーターを介して1つのAPI キーを使用して、マJORプロバイダーの100以上のモデルにアクセスできます。

</details>

<details>
<summary><b>💰 Cheap Providers (Backup)</b></summary>

### GLM-4.7 (毎日リセット、0.6 ドル/1000万)

1. 新規登録：[Zhipu AI](https://open.bigmodel.cn/)
2. コードプランからAPIキーを取得
3. ダッシュボード → API キー追加:
   - プロバイダー: `glm`
   - API キー: `your-key`

**使用:** `glm/glm-4.7`

**プロチップ:** クオタは3倍、7割のコスト! 日替わり10:00 AMでリセット。

### MiniMax M2.1 (5h リセット、$0.20/1M)

1. 申し込み： [MiniMax] (https://www.minimax.io/)
2. APIキー取得
3. ダッシュボード → API キー追加

**使用:** `minimax/MiniMax-M2.1`

**プロチップ:** 枚続の長いコンテキストの最安オプション（1M トークン！）

### Kimi K2 ($9/月フラット)

1. サブスクライブ： [Moonshot AI] (https://platform.moonshot.ai/)
2. APIキー取得
3. ダッシュボード → API キー追加

**使用:** `kimi/kimi-latest`

**プロチップ:** 10Mトークン= $0.90/1M の効果的なコスト= $9/月の定額

</details>

<details>
<summary><b>🆓 FREE Providers (Emergency Backup)</b></summary>

### iFlow (5フリーでOAuth)

```bash
ダッシュボード → iFlow接続
→ iFlow OAuthログイン
→ 無制限使用

モデル：
  if/kimi-k2-thinking
  if/qwen3-coder-plus
  if/glm-4.7
  if/minimax-m2
  if/deepseek-r1
```

### Qwen (4フリーモデルデバイスコード)

```bash
ダッシュボード → Connect Qwen
→ デバイスコード 認証
→ 無制限利用

モデル:
  qw/qwen3-coder-plus
  qw/qwen3-coder-flash
```

### キロ (クラウド フリー)

```bash
ダッシュボード → Connect Kiro
→ AWS ビルダー ID または Google/GitHub
→ 無制限利用

モデル:
  kr/claude-sonnet-4.5
  kr/claude-haiku-4.5
```

</details>

<details>
<summary><b>🎨 Create Combos</b></summary>

### 例 1: サブスキピングの最大化 → Cheap Backup

```
ダッシュボード → COMBOS → 新規作成

名称: プレミアム コーディング
モデル:
  1. cc/claude-opus-4-6 (サブスクリプション プライマリ)
  2. glm/glm-4.7 (安cheap ため、backup、$0.6/1M)
  3. minimax/MiniMax-M2.1 (最低費用回避、$0.20/1M)

CLI で使用: premium-coding
```

### 例 2: 無料のみ (ゼロコスト)

```
名称: 無料 COMBO
モデル:
  1. gc/gemini-3-flash-preview (180k 無料月)
  2. if/kimi-k2-thinking (無制限)
  3. qw/qwen3-coder-plus (無制限)

コスト: $0 いつまでも!
```

</details>

<details>
<summary><b>🔧 CLI Integration</b></summary>

### カーソルIDE

```
設定 → モデル → 開発者:
  OpenAI APIBase URL: http://localhost:20128/v1
  OpenAI API Key: [から OmniRoute ダッシュボード]
  モデル: cc/claude-opus-4-6
```

### クロード・コード

[CLAUSE]** CLI ツール** ポेजを開くダッシュボードで一括設定、または[81X]~/.claude/settings.json`
編集して手動で設定を変更します。

### コデックス CLI

```bash
export OPENAI_BASE_URL="http://localhost:20128"
export OPENAI_API_KEY="あなたのomniroute-api-key"

コデックス "あなたのプロンプト"
```

### オープンクロー

**オプション 1 —ダッシュボード（推奨）：**

```
ダッシュボード → CLI Tools → OpenClaw → 選択モデル → 適用
```

**オプション 2 —手動：** `~/.openclaw/openclaw.json`: 編集して下さい：

```json
{
  "モデル":
  "プロバイダー" :
  "Open AI API" :
  "omniroute" :
    "baseUrl": "http://127.0.0.1:20128/v1",
    "apiKey": "sk_omniroute",
    "api": "openai-completions"
}
```

> **ノート：** OpenClaw はアクセスすることができるオーキルートのローカルのみで使用することができます。`127.0.0.1`
> を[79X]localhost` の代わりに使用するため IPv6 解決の問題を回避します。

### ライン / クローズ / ルーコード

```
設定 → API 設定：
  プロバイダー: OpenAI 準拠
  ベース URL: http://localhost:20128/v1
  API キー: [OmniRoute ダッシュボードから]
  モデル: if/kimi-k2-thinking
```

### OpenCode

**ステップ 1:** OmniRoute をカスタム プロバイダーとして追加する:

```bash
opencode
/connect
# "他の" を選択 → ID: "omniroute" → OmniRoute API キーを入力
```

**ステップ 2:** `opencode.json` をプロジェクトルートで作成/編集する:

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

**ステップ 3:** OpenCode でモデルを選択する:

```bash
/models
# OmniRoute からリストでモデルを選ぶ
```

> **ヒント:** Omniroute [`/v1/models` エンドポイントにあるモデルを OmniRoute ドASH
> ドックボードから取得できます。] models を追加して、次のフォーマットを使用できます。`プロバイダー/model-id`

</details>

---

## トラブルシューティング

<details>
<summary><b>Click to expand troubleshooting guide</b></summary>

**"language model はメッセージを生成しませんでした"**

- プロバイダクォタ切れ → ダッシュボードのクォタトラッカーを確認
- ソリューション: コンボフォールバックまたは値段が安いプランに変更する

**レート制限**

- サブスクリプションクォタ切れ → GLM/MiniMax にフォールバックする
- コンビネーションを追加:`cc/claude-opus-4-6 → glm/glm-4.7 → if/kimi-k2-thinking`

**OAuth テークンが期限切れ**

- 自動で OmniRoute によって再接続されます
- トラブルが続いて場合は: ダッシュボード → プロバイダー → 再接続を実行する

**コストが高すぎる**

- 総合使用状況をダッシュボード → コストにチェック
- 主なモデルをGLM/MiniMaxに切り替え
- 非臨界タスクはフリータイヤ（Gemini CLI、iFlow）をご利用ください

**ダシュボード/API ポータルが間違っています**

- `PORT`は標準的なベースポート（とAPI ポートとしてデフォルトです）
- `API_PORT`は、OpenAI互換性APIリスナをのみオーバライド
- `DASHBOARD_PORT`はダッシュボード/Next.jsリスナをのみオーバライドします
- [X0X]基準となるベースURL`には、OAuth回呼URLにあたるダッシュボード/パブリックURLを設定してください

**クラウド同期エラー**

- [X0X]BASE_URL`が実行中のインスタンスにポイントしていることを確認してください
- [X0X]CLOUD_URL`が予期されるクラウドエンドポイントにポイントしていることを確認してください
- [X0X]NEXT_PUBLIC_*`の値をサーバー側の値と同期してください

**初回ログインが動作せず**

- [X0X]INITIAL_PASSWORD`を`.env`の値を確認してください
- 未セットの場合、デフォルトパスワードは`123456`です

**リクエストログが利用できないようです**

- [X0X]ENABLE_REQUEST_LOGS=true`を`.env`の値に設定してください

**OpenAI互換のプロバイダーに対して接続テストが「無効」であることが示唆され**

- manyプロバイダーはモデルエンドポイントを公開していません
- OmniRoute v1.0.6+では、チャットコンプリションを利用したフォールバックバリデーションが含まれます。
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

**4. 保存およびコピーするための資格情報**

Googleで作成すると、**クライアントID**と[ X55X]クライアントシークレット** が表示されます。

**5. 環境変数を設定**

あなたの[ X8X].env` (or Docker environment variables):

```bash
# Antigravity:
ANTIGRAVITY_OAUTH_CLIENT_ID=your-client-id.apps.googleusercontent.com
ANTIGRAVITY_OAUTH_CLIENT_SECRET=GOCSPX-your-secret

# Gemini CLI:
GEMINI_OAUTH_CLIENT_ID=your-client-id.apps.googleusercontent.com
GEMINI_OAUTH_CLIENT_SECRET=GOCSPX-your-secret
GEMINI_CLI_OAUTH_CLIENT_SECRET=GOCSPX-your-secret
```

**6. OmniRouteを再起動**

```bash
# npm:
npm run dev

# Docker:
docker restart omniroute
```

**7. 再び接続を試してみる**

Dashboard → Providers → Antigravity (or Gemini CLI) → OAuth

Googleは、現在コールバックされるべき[ X38X]https://your-server.com/callback`
に直接リダイレクトするようになります。

---

#### 一時的なワークアラウンド (カスタム資格情報の設定なし)

資格情報を自分で設定しない場合は、この[ X82X]アプリケーション設定フロー** を使用できます :

1. OmniRouteは、Google認証プロバイダーURLを開きます
2. 認証後に、Googleは[ X47X]ローカルホスト` (ローカルホストにアップデートされ、リモートサーバーでは失敗します) へのリダイレクトを実行します
3. **このURLをコピーしてください** をブラウザーのアドレスバーから (ページがロードされない場合でも)
4. このURLをOmniRoute接続モーダルにペーストしてください
5. [ X6X]"接続**"

> これは、URLの認証コードがロードされていない場合であっても有効であるためです。

---

<details>
<summary><b>🇧🇷 Versão em Português</b></summary>

#### Antigravity / Gemini CLI OAuthがサーバー上でうまくいかない理由ですか?

サービス提供者 **Antigravity** および **Gemini CLI** は、**Google OAuth 2.0**
を使用して認証します。Googleは、OAuthフローで使用される[ X113X]リダイレクトURI` が、Google Cloud
Consoleでアプリケーションに事前登録されたURIと一致しているかどうかをチェックします。

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

**6. OmniRouteを再起動**

```bash
# npmを使用する場合:
npm run dev

# Dockerを使用する場合:
docker restart omniroute
```

**7. 再接続を試めよう**

Dashboard → Providers → Antigravity (またはGemini CLI) → OAuth

Gooleのredirecionará 正しく今
`https://%E3%82%BB%E3%82%AD%E3%82%B9%E3%83%88%E3%82%92%E3%82%B3%E3%83%BC%E3%83%95%E3%82%99%E3%82%99`
へ、 認証が機能します。

---

#### 一時的なワークアラウンド (資格情報を自作する)

資格情報自作を今しばしは行わなくても、まだ使用可能なフロー **URLマニュアル** です：

1. OmniRouteはGoogleの認可URLを開く
2. あなたが認証すると、Gooleは `localhost` (セキュリティサーバに失敗) へredirecionará
3. **URLのコピー** を Webブラウザインディペネンのバーから
4. コピしたURLをOmniRouteの接続モダルの欄で貼る
5. 「**Connect**」とクリックしてください

> このワークアラウンドは、redirecionが読み込まれたかどうかに関係なく、認可のコードがURL上で有効であるため機能します。

</details>

---

</details>

## 🛠️ Tech Stack

<details>
<summary><b>Click to expand tech stack details</b></summary>

- **Runtime**: Node.js 18 - 22 LTS (注意: Node.js 24+は**未サポート** です —
  `better-sqlite3` 自然バイナリーズは互換性が無い)
- **言語**: TypeScript 5.9 - **%100TypeScript**全 `src/` と `open-sse/`
  (v2.0より後、コアモジュールに[ ]any[ ]ゼロあります)
- **フレームワーク**: Next.js 16 + React 19 + Tailwind CSS 4
- **データベース**: LowDB (JSON) + SQLite (ドメインステート+プロキシログ+MCP経済観測+ルーティング決定)
- **スキーマ**: Zod (MCPツールI/O検証、API契約)
- **プロトコル**: MCP (stdio/HTTP) + A2A v0.3 (JSON-RPC 2.0 + SSE)
- **ストリーミング**: Server-Sent Events (SSE)
- **認証**: OAuth 2.0 (PKCE) + JWT + API Keys + MCP スコープ 認可
- **テスト**: Node.jsテスト ランナー + Vitest (900+ ユニットテスト、統合テスト、E2Eテストを含む)
- **CI/CD**: GitHub Actions (auto npm publish + Docker Hub on release)
- **ウェブサイト**:[omniroute.online](https://omniroute.online)
- **パッケージ**:
  [npmjs.com/package/omniroute](https://www.npmjs.com/package/omniroute)
- **Docker**:
  [hub.docker.com/r/diegosouzapw/omniroute](https://hub.docker.com/r/diegosouzapw/omniroute)
- **備災**: 回路ブレーカー、指数バックオフ、反トハーディーン、TLS スポッフ、自動組み合わせ自己修復

</details>

---

## ドキュメント

| ドキュメント                                     | 説明                                      |
| ------------------------------------------ | --------------------------------------- |
| [ユーザー ガイド](docs/USER_GUIDE.md)             | プロバイダー、組み合わせ、CLI統合、デプロイ                 |
| [API リファレンス](docs/API_REFERENCE.md)        | すべてのエンドポイントと例                           |
| [MCP サーバー](open-sse/mcp-server/README.md)  | 16 MCP � ツール、IDE 設定、Python/TS/Go クライアント |
| [A2A サーバー](src/lib/a2a/README.md)          | JSON-RPC 2.0 プロトコル、スキル、ストリーミング、タスク管理    |
| [自動組み合わせエンジン](docs/auto-combo.md)          | Scoring 6つの要素評価, モード パック, 自己診断          |
| [Troubleshooting](docs/TROUBLESHOOTING.md) | よくある問題と解決方法                             |
| [設計](docs/ARCHITECTURE.md)                 | システム アーキテクチャと内部構造                       |
| [貢献](CONTRIBUTING.md)                      | 開発環境セットアップとガイドライン                       |
| [OpenAPI Spec](docs/openapi.yaml)          | OpenAPI 3.0仕様                           |
| [セキュリティ ポリシー](SECURITY.md)                 | 脆弱性の報告とセキュリティ プラクティス                    |
| [VM インストール](docs/VM_DEPLOYMENT_GUIDE.md)   | VM + nginx + Cloudflare セットアップの完全ガイド    |
| [要素ギャラリー](docs/FEATURES.md)                | スクリーンショット付きビジュアル ダッシュボードツアー             |
| [リリース チェックリスト](docs/RELEASE_CHECKLIST.md)  | 前リリースの確認ステップ                            |

---

## 🗺️ ROADMAP

OmniRouteには**210+の機能が計画されています**、複数の開発フェーズを通じて。次の主な分野があります。

| カテゴリ                  | 予定されている機能 | ハイライト                                                     |
| --------------------- | --------- | --------------------------------------------------------- |
| 🧠 **ルーティング・インテリジェンス** | 25+       | 最短経路ルーティング、タグベースルーティング、クォータプレフライト、P2Cアカウント選択              |
| 🔒 **セキュリティ・コンプライアンス** | 20+       | SSRF強化、クレデンシャルクローク、エンドポイントあたりレート制限、管理鍵スコーピング              |
| 📊 **オブザーブレティビリティ**    | 15+       | オープンテレメトリー統合、リアルタイムクォータ監視、モデルあたりコストトラッキング                 |
| 🔄 **プロバイダー統合**        | 20+       | ダイナミックモデルレジストリ、プロバイダーダウンタイム、複数アカウントCodex、コピロットクォータパーシング   |
| ⚡ **パフォーマンス**         | 15+       | Dualキャッシュレイヤー、プログラムキャッシュ、レスポンスキャッシュ、ストリーミングキープアライブ、バッチAPI |
| 🌐 **エコシステム**          | 10+       | WebSocketAPI、構成ホットロード、分散構成ストア、商用モード                       |

### 近日公開

- 🔗 **OpenCode統合** — OpenCode AIコーディングIDE向けネイティブプロバイダー対応
- 🔗 ** TraE 連携** — TraE AI 開発フレームワーク全面サポート
- 📦 ** バッチAPI** —Bulkリクエスト用非同期バッチ処理
- 🎯 ** タグベースルーティング** —カスタムタグやメタデータに基づくリクエストルーティング
- 💰 ** 最小コスト戦略 ** —最安値の利用可能なサービスを自動的に選択

> 📝 フル特徴仕様は[`docs/new-features/`](docs/new-features/)(217の詳細仕様)に詳細に記載されています

---

## 👥 コントリビューター

[![Contributors](https://contrib.rocks/image?repo=diegosouzapw/OmniRoute&max=100&columns=20&anon=1)](https://github.com/diegosouzapw/OmniRoute/graphs/contributors)

### コントリビュートする方法

1. リポジトリをフォークする
2. 特性ブランチを作成する (`git checkout -b feature/amazing-feature`)
3. 変更をコミットする (`git commit -m 'Add amazing feature'`)
4. ブランチをプッシュする (`git push origin feature/amazing-feature`)
5. プルリクエストを開く

詳細なガイドラインについては[CONTRIBUTING.md](CONTRIBUTING.md)を参照

### 新バージョンのリリース

```bash
# リリース用コマンドを実行 —npm publishは自動的に実行される
gh release create v2.0.0 --title "v2.0.0" --generate-notes
```

---

## 📊 スターコードの履歴

## 時間の経過に伴うスター数の推移

## [![Stargazers over time](https://starchart.cc/diegosouzapw/OmniRoute.svg?variant=adaptive)](https://starchart.cc/diegosouzapw/OmniRoute)

## 🙏 誠意の表現

乙覧の感謝は**(https://github.com/decolua/9router)**の**(https://github.com/decolua)**さんにある。OmniRouteはその巨大な礎に新たな機能、多モードAPI、
TypeScriptの完全リライトで成長させた。

**(https://github.com/router-for-me/CLIProxyAPI)**のGo実装がこのJavaScript版を刺激した。

---

## 📄 ライセンス

MITライセンス - 詳細は[LICENSE](LICENSE)のファイルを参照してください。

---

<div align="center">
  <sub>Built with ❤️ for developers who code 24/7</sub>
  <br/>
  <sub><a href="https://omniroute.online">omniroute.online</a></sub>
</div>
<!-- GitHub Discussions enabled for community Q&A -->
