# Alert — 仕様

注意喚起バナー。情報・成功・警告・エラーを面で伝える。

## 実装
- CSS クラス: `.fig-alert`（severity 修飾: `--success` / `--warning` / `--error`）
- トークン経由のみ（生値なし）。`tokens/components.css`

## 属性/修飾
| 修飾クラス | 用途 |
|---|---|
| `.fig-alert` | 既定（中立・情報） |
| `.fig-alert--success` | 成功 |
| `.fig-alert--warning` | 警告 |
| `.fig-alert--error` | エラー |

## States
Default / （dismissible 時）Hover・Focus の閉じるボタン / 各 severity

## a11y
- `role="alert"`（重要）または `role="status"`（軽微）
- 色のみに依存しない（アイコン/テキスト併用）。コントラスト WCAG AA
- 閉じるボタンは `aria-label`・フォーカス可視

## Profiles
Admin/Consumer/Terminal すべてで成立（余白/文字はプロファイル変動）

## Tokens（参照例）
`--color-surface-{success,warning,error}` / `--color-text-{success,warning,error}` / `--color-border-{default,warning,error}` / `--fig-spacing-*` / `--fig-radius-control` / `--fig-size-body`

## Preview
`preview/feedback-patterns.html`（5状態以上を可視化・要整備）
