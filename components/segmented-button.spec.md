# Segmented Button — 仕様
排他選択（画面内の表示切替等）。Tab と責務分離（Segmented=値選択、Tab=ビュー切替）。
- **実装**: `.fig-segmented`（`__item`、選択は `aria-selected="true"`）
- **States**: 各 item の 選択/非選択/Hover/Focus/Disabled
- **a11y**: `role="group"`、各 item は `role="button"` ＋ `aria-pressed`/`aria-selected`、キーボード操作
- **Profiles**: 3プロファイル成立
- **Tokens**: `--color-surface-container-low` / `--color-surface-default` / `--color-text-brand` / `--fig-radius-control`
- **Preview**: `preview/components-tabs.html`（要整備）
