# React スキル

React / Next.js 向けのスキルです。

---

## react-best-practices

**出所**: [vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills)

Vercel Engineering が提供する React / Next.js パフォーマンス最適化ガイドです。

- **用途**: React コンポーネントの作成・レビュー・リファクタリング・パフォーマンス改善
- **ルール数**: 62 ルール / 8 カテゴリ（優先度順）
- **場所**: `skills/react/react-best-practices/`

### カテゴリ

| 優先度 | カテゴリ | 影響度 | プレフィックス |
|---|---|---|---|
| 1 | ウォーターフォール排除 | CRITICAL | `async-` |
| 2 | バンドルサイズ最適化 | CRITICAL | `bundle-` |
| 3 | サーバーサイドパフォーマンス | HIGH | `server-` |
| 4 | クライアントサイドデータ取得 | MEDIUM-HIGH | `client-` |
| 5 | 再レンダリング最適化 | MEDIUM | `rerender-` |
| 6 | レンダリングパフォーマンス | MEDIUM | `rendering-` |
| 7 | JavaScript パフォーマンス | LOW-MEDIUM | `js-` |
| 8 | 高度なパターン | LOW | `advanced-` |

### 主なルール

**ウォーターフォール排除（CRITICAL）**
- `async-parallel` — 独立した操作には `Promise.all()` を使用
- `async-suspense-boundaries` — Suspense でコンテンツをストリーム配信

**バンドルサイズ最適化（CRITICAL）**
- `bundle-barrel-imports` — バレルファイルを避け直接インポート
- `bundle-dynamic-imports` — 重いコンポーネントには `next/dynamic` を使用

**サーバーサイドパフォーマンス（HIGH）**
- `server-cache-react` — `React.cache()` でリクエスト単位の重複排除
- `server-parallel-fetching` — フェッチの並列化のためにコンポーネントを再構成
