# Web スキル

Web フロントエンド向けのスキルです。Claude Code・claude.ai どちらでも使えます。

**出所**: [anthropics/skills](https://github.com/anthropics/skills)

---

## frontend-design

ありきたりではない、高品質なフロントエンドを作成するためのスキルです。

- **用途**: Web コンポーネント・ページ・アプリケーションの実装
- **特徴**: デザイン方向性を先に決め、「AI っぽい無難な UI」を意識的に避ける
- **重視する点**: タイポグラフィ・配色・アニメーション・レイアウト・装飾
- **場所**: `skills/web/frontend-design/`

---

## web-artifacts-builder

React + Tailwind CSS + shadcn/ui を使って複雑な claude.ai HTML アーティファクトを構築するスキルです。

- **用途**: 状態管理・ルーティングが必要な複雑なアーティファクト作成
- **スタック**: React 18 + TypeScript + Vite + Parcel + Tailwind CSS + shadcn/ui
- **注意**: シンプルな単一ファイル HTML には不要。主に claude.ai 向け
- **場所**: `skills/web/web-artifacts-builder/`
