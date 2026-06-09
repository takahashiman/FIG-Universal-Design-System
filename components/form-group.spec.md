# Form Group — 仕様
ラベル＋コントロール＋ヘルプ/エラーの入力グループ。
- **実装**: `.fig-form-group`（`__label` / `__help` / `__error`）
- **States**: 既定/エラー（`__error` 表示）
- **a11y**: `<label for>` と入力の関連付け、`aria-describedby` でヘルプ/エラー、エラーは `aria-invalid`
- **Profiles**: 3プロファイル成立
- **Tokens**: `--fig-spacing-xs` / `--fig-size-body-strong` / `--color-text-error` / `--color-text-secondary`
- **Preview**: `preview/components-inputs.html`（要整備）
