# Claude Code スキル

Claude Code のツール実行・ファイル操作が必要なスキルです。

**出所**: [anthropics/skills](https://github.com/anthropics/skills)

---

## skill-creator

新しいスキルの作成・改善・評価を行うメタスキルです。

- **用途**: スキルをゼロから作る、既存スキルを改善・最適化する
- **流れ**: 草案作成 → テスト実行 → 定性/定量評価 → 改善 → 繰り返し
- **ツール**: `scripts/run_eval.py` でバッチ評価、`eval-viewer/` で結果の可視化
- **場所**: `skills/claude-code/skill-creator/`

---

## webapp-testing

Playwright を使ってローカル Web アプリをテスト・デバッグするスキルです。

- **用途**: フロントエンドの動作確認・UI デバッグ・スクリーンショット取得・ブラウザログの確認
- **実装**: ネイティブ Python Playwright スクリプトで記述
- **ヘルパー**: `scripts/with_server.py` でサーバーライフサイクルを管理（複数サーバー対応）
- **場所**: `skills/claude-code/webapp-testing/`
