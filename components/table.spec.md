# Table — 仕様
表（Web-Admin 中核）。
- **実装**: `.fig-table`（`th`/`td`、ソート/選択は消費側）
- **States**: 既定/Hover行/選択行/ソート列
- **a11y**: ネイティブ `<table>` 構造、`<th scope>`、ソートは `aria-sort`、キャプション推奨
- **Profiles**: 3プロファイル成立（行高/余白プロファイル変動。Admin で密）
- **Tokens**: `--color-border-default` / `--color-surface-container-low` / `--fig-density-row-padding-y` / `--fig-size-body`
- **Preview**: `preview/components-list-rows.html`（要整備）
