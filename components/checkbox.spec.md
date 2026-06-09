# Checkbox — 仕様
複数選択。
- **実装**: `.fig-checkbox`（状態は `aria-checked`、`true`/`false`/`mixed`）
- **States**: 未選択/選択/不確定/Disabled/Focus
- **a11y**: `role="checkbox"` ＋ `aria-checked`、`<label>` 関連付け、キーボード（Space）
- **Profiles**: 3プロファイル成立
- **Tokens**: `--color-border-default` / `--color-surface-brand` / `--color-text-onBrand` / `--fig-radius-control` / `--color-border-focus`
- **Preview**: `preview/components-inputs.html`（要整備）
