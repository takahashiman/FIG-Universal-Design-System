# Toggle Switch — 仕様
ON/OFF の即時切替。
- **実装**: `.fig-switch`（`__track` / `__thumb`、状態は `aria-checked`）
- **States**: OFF/ON/Disabled/Focus
- **a11y**: `role="switch"` ＋ `aria-checked`、キーボード（Space/Enter）、`aria-label`
- **Profiles**: 3プロファイル成立（固有寸法は最小 raw＝Lint allowlist）
- **Tokens**: `--color-surface-brand`（ON）/ `--color-text-disabled`（OFF）/ `--color-surface-default`（thumb）/ `--fig-radius-pill`
- **Preview**: `preview/state-tokens.html`（要整備）
