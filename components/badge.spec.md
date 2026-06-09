# Badge — 仕様

数値・状態を示す小型インジケータ。アイコンやアバターに添える。

## 実装
- CSS クラス: `.fig-badge`（修飾: `--dot` でドット表示）
- トークン経由のみ（生値なし）。`tokens/components.css`

## 属性/修飾
| 修飾クラス | 用途 |
|---|---|
| `.fig-badge` | 数値/ラベル付き |
| `.fig-badge--dot` | 数なしのドット（新着等） |

## States
Default / 0件時は非表示推奨 / 99+ の上限表記

## a11y
- 数値は読み上げ対象（`aria-label="未読 3件"` 等）
- ドットのみは装飾。意味があれば代替テキスト
- コントラスト WCAG AA

## Profiles
Admin/Consumer/Terminal で成立（サイズはタイポトークン連動）

## Tokens（参照例）
`--color-surface-brand` / `--color-text-onBrand` / `--fig-radius-pill` / `--fig-size-{body,caption}` / `--fw-bold`

## Preview
`preview/components-status-pills.html`（badge も含め整備）
