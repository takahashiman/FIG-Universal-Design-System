# Header — 仕様
画面ヘッダ（タイトル＋アクション）。
- **実装**: `.fig-header`（トークン経由）
- **States**: 既定/スクロール時の elevation（消費側）
- **a11y**: `role="banner"` または `<header>`、見出し階層を尊重
- **Profiles**: 3プロファイル成立（高さプロファイル変動）
- **Tokens**: `--color-surface-default` / `--color-border-default` / `--fig-target-comfortable` / `--elevation-z-header`
- **Preview**: `preview/device-profiles.html`（要整備）
