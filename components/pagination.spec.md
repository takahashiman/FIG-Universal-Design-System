# Pagination — 仕様
ページ送り。
- **実装**: `.fig-pagination`（`__item`、現在は `aria-current="page"`）
- **States**: 各 item Default/Hover/Focus/現在/Disabled（端）
- **a11y**: `<nav aria-label="ページ送り">`、現在に `aria-current="page"`、前後ボタンに `aria-label`
- **Profiles**: 3プロファイル成立
- **Tokens**: `--color-border-default` / `--color-surface-brand` / `--color-text-onBrand` / `--fig-target-min` / `--fig-radius-control`
- **Preview**: `preview/components-list-rows.html`（要整備）
