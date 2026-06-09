# Breadcrumb — 仕様
階層位置のパンくず。
- **実装**: `.fig-breadcrumb`（`__sep` 区切り）
- **States**: 各リンク Default/Hover/Focus、現在地は非リンク
- **a11y**: `<nav aria-label="パンくず">` ＋ `<ol>`、現在地に `aria-current="page"`、区切りは装飾（`aria-hidden`）
- **Profiles**: 3プロファイル成立
- **Tokens**: `--color-text-secondary` / `--color-text-disabled` / `--fig-size-caption` / `--fig-spacing-xs`
- **Preview**: `preview/device-profiles.html`（要整備）
