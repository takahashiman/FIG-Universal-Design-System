# Navigation Rail — 仕様
縦型ナビ（PC/Admin の主ナビ）。
- **実装**: `.fig-nav-rail`（`__item`、現在は `aria-current="page"`）
- **States**: 各 item Default/Hover/Focus/現在
- **a11y**: `<nav>` ＋ リスト、現在に `aria-current="page"`、アイコンのみは `aria-label`
- **Profiles**: 3プロファイル成立（Admin/Terminal 主用途）
- **Tokens**: `--color-surface-brand-subtle` / `--color-text-brand` / `--color-text-secondary` / `--fig-target-comfortable`
- **Preview**: `preview/device-profiles.html`（要整備）
