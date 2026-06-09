# FIG Core DS — FIG Universal Design System（中核）

FIG ブランドの**普遍的中核デザインシステム**。すべての製品（拡張プロジェクト）の親であり、三層アーキテクチャのトークンと 28 コンポーネントを提供します。本リポジトリの既定ブランチは **`core`** です。

> このリポジトリはマルチレポ構成の中核です。拡張プロジェクトは `fig-ext-<category>-<product>` として独立し、Core を **submodule で pin** して利用します。ポータル（閲覧）は最新 Core を **rolling** 参照します。

---

## アーキテクチャ（三層）
```
Primitive（生値 HEX/px）  →  Semantic（役割トークン）  →  Component（CSSクラス）
  primitives.css              semantic.css                  tokens/components.css
```
- **Component は Semantic のみ参照**。生値・Primitive の直参照は禁止（CI で検査）。
- **トークン命名（多接頭辞）**: `--color-*`（色役割）／ `--fig-*`（サイズ・余白・タイポ）／ `--fg-*`（スレート primitive）。

## デバイスプロファイル（3種）
`.fig-profile-*` を文書ルートに付与するとトークン値が上書きされます。
- **`.fig-profile-admin`** … Web-Admin（PC・情報密度優先）※既定
- **`.fig-profile-consumer`** … 一般ユーザー向けスマホ（操作性優先）
- **`.fig-profile-terminal`** … 業務端末（固定視認性）

## コンポーネント（CSS クラス方式・framework 非依存）
コンポーネントは **CSS クラス `.fig-<name>`**（`tokens/components.css`）。class を付与するだけで任意の framework から利用できます（React/JSX は各拡張の任意ラッパー）。

```html
<button class="fig-button">送信</button>
<span class="fig-status-pill fig-status-pill--success">有効</span>
<div class="fig-card"><h3 class="fig-card__title">...</h3></div>
```

提供コンポーネント（28＋）: button / card / input / list-item / modal / bottom-sheet / side-sheet / header / form-group / fab / icon-button / segmented / switch / checkbox / radio / picker / table / tabs / breadcrumb / pagination / nav-rail / bottom-nav / alert / toast / badge / status-pill / icon-bubble / sense ほか。各契約は `components/<name>.spec.md`、見た目は `preview/*.html`。

## ファイル
| パス | 役割 |
|---|---|
| `primitives.css` / `semantic.css` / `tokens/` | 三層トークン（base/components/profile-*） |
| `tokens/components.css` | コンポーネント CSS クラス |
| `components/*.spec.md` | コンポーネント契約 |
| `preview/*.html` | 状態プレビュー |
| `registry.json` / `taxonomy.json` | 拡張登録簿・分類階層（**単一正典**・Core Maintainer 管理） |
| `deprecated-aliases.css` | 後方互換エイリアス層 |
| `cliff.toml` / `CHANGELOG.md` / `.github/workflows/release.yml` | SemVer 自動リリース |

## バージョニング
- **SemVer** git タグ。**昇格・追加＝MINOR / 破壊的＝MAJOR / 修正＝PATCH**。
- タグ push で GitHub Actions＋git-cliff が CHANGELOG/Release を自動生成。
- 拡張は特定版に pin し `CORE-DS-VERSION` に明記。ポータルは rolling。

## 利用（拡張プロジェクト）
```bash
git submodule add -b core https://github.com/takahashiman/FIG-Universal-Design-System.git design-system
# CSS を読み込み、必要なら <body class="fig-profile-admin"> でプロファイル指定
```

## 貢献・Core 昇格
拡張で生まれた優れた部品は **Core 昇格フロー**（`core-promotion` ラベル → 3プロダクト基準 → 普遍化 → レビュー → 次 MINOR）で Core 化されます。詳細はポータルの「運用 > Contribution」を参照。

---
*本デザインシステムは AI-DLC で設計・構築されています（設計資料: ポータルリポジトリ `aidlc-docs/`）。*
