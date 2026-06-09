# Radio Button — 仕様
単一選択（グループ内排他）。
- **実装**: `.fig-radio`（状態は `aria-checked`）
- **States**: 未選択/選択/Disabled/Focus
- **a11y**: `role="radio"`、親に `role="radiogroup"`、矢印キーで移動、`<label>` 関連付け
- **Profiles**: 3プロファイル成立
- **Tokens**: `--color-border-default` / `--color-surface-brand` / `--fig-radius-pill` / `--color-border-focus`
- **Preview**: `preview/components-inputs.html`（要整備）
