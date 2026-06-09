# Picker — 仕様
選択（候補/日付等）。トリガ＋ポップアップ。
- **実装**: `.fig-picker`（トリガ。ポップアップは消費側）
- **States**: 既定/開/選択済/Disabled/Focus
- **a11y**: `role="combobox"` ＋ `aria-expanded`/`aria-controls`、キーボード操作、選択は `aria-selected`
- **Profiles**: 3プロファイル成立
- **Tokens**: `--color-border-default` / `--color-surface-default` / `--fig-radius-control` / `--fig-target-min`
- **Preview**: `preview/components-inputs.html`（要整備）
