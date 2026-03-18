# Web スキル

Web フロントエンド向けのスキルです。Claude Code・claude.ai どちらでも使えます。

---

## frontend-design

**出所**: [anthropics/skills](https://github.com/anthropics/skills)

ありきたりではない、高品質なフロントエンドを作成するためのスキルです。

- **用途**: Web コンポーネント・ページ・アプリケーションの実装
- **特徴**: デザイン方向性を先に決め、「AI っぽい無難な UI」を意識的に避ける
- **重視する点**: タイポグラフィ・配色・アニメーション・レイアウト・装飾
- **場所**: `skills/web/frontend-design/`

---

## web-artifacts-builder

**出所**: [anthropics/skills](https://github.com/anthropics/skills)

React + Tailwind CSS + shadcn/ui を使って複雑な claude.ai HTML アーティファクトを構築するスキルです。

- **用途**: 状態管理・ルーティングが必要な複雑なアーティファクト作成
- **スタック**: React 18 + TypeScript + Vite + Parcel + Tailwind CSS + shadcn/ui
- **注意**: シンプルな単一ファイル HTML には不要。主に claude.ai 向け
- **場所**: `skills/web/web-artifacts-builder/`

---

## composition-patterns

**出所**: [vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills)

スケーラブルな React コンポジションパターンのガイドです。

- **用途**: コンポーネント設計・リファクタリング・再利用可能な API 設計
- **特徴**: boolean prop の増殖を避け、compound component・状態リフト・合成パターンを活用
- **ルール数**: 8 ルール / 4 カテゴリ
- **場所**: `skills/web/composition-patterns/`

### カテゴリ

| 優先度 | カテゴリ | 影響度 |
|---|---|---|
| 1 | コンポーネントアーキテクチャ | HIGH |
| 2 | 状態管理 | MEDIUM |
| 3 | 実装パターン | MEDIUM |
| 4 | React 19 API | MEDIUM |
