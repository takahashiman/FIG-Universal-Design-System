# Bottom Sheet — 仕様
下部からせり出すシート（主に Consumer/Terminal）。
- **実装**: `.fig-bottom-sheet`（`tokens/components.css`、トークン経由）
- **States**: 閉/開/ドラッグ（実装は消費側）
- **a11y**: `role="dialog"` `aria-modal="true"`、フォーカストラップ、Esc で閉、背景 scrim
- **Profiles**: 3プロファイル成立（余白プロファイル変動）
- **Tokens**: `--color-surface-default` / `--fig-radius-card` / `--fig-elevation-floating` / `--color-surface-scrim` / `--elevation-z-modal`
- **Preview**: `preview/feedback-patterns.html`（要整備）
