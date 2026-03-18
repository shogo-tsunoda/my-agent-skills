# React Native / Expo スキル

React Native・Expo 向けのスキルです。

---

## expo プラグイン（公式）

**リポジトリ**: [expo/skills](https://github.com/expo/skills)

Expo チームが公式に提供するプラグインです。Claude Code へのインストールは以下のコマンドで行います。

```
/plugin marketplace add expo/skills
/plugin install expo
```

**場所**: `skills/react-native/expo/`

### 収録スキル

| スキル | 説明 |
|---|---|
| building-native-ui | Expo Router を使ったネイティブ UI 構築の完全ガイド（スタイリング・ナビゲーション・アニメーション） |
| native-data-fetching | fetch / React Query / SWR などのデータ取得・キャッシュ・オフライン対応 |
| expo-api-routes | Expo Router + EAS Hosting での API ルート作成ガイド |
| expo-deployment | iOS App Store / Android Play Store / Web へのデプロイ手順 |
| expo-dev-client | ローカルまたは TestFlight 経由での開発クライアントのビルド・配布 |
| expo-cicd-workflows | EAS ワークフロー YAML の作成・CI/CD パイプライン構築 |
| expo-tailwind-setup | Expo で Tailwind CSS v4 + NativeWind v5 をセットアップ |
| upgrading-expo | Expo SDK のバージョンアップと依存関係の修正 |
| expo-ui-swift-ui | `@expo/ui/swift-ui` を使って SwiftUI ビューをアプリに組み込む |
| expo-ui-jetpack-compose | `@expo/ui/jetpack-compose` を使って Jetpack Compose ビューをアプリに組み込む |
| use-dom | Expo DOM コンポーネントを使い、Web コードをネイティブに段階的に移行する |

---

## expo-mobile-app-skill

**リポジトリ**: [zaferayan/skills](https://github.com/zaferayan/skills)

RevenueCat・AdMob・i18n を含む、収益化対応のプロダクションレディな Expo アプリを構築するためのスキルです。

**場所**: `skills/react-native/expo-mobile-app-skill/`

```
/zafer-skills Create a water reminder app
```

### 主な機能

| 機能 | 内容 |
|---|---|
| **購読** | RevenueCat（週払い / 年払い、50% OFFバッジ付き） |
| **広告** | Google AdMob バナー（プレミアムユーザーは非表示） |
| **多言語** | i18next + react-i18next（日本語・英語・トルコ語等） |
| **オンボーディング** | フルスクリーン背景動画 + グラデーションオーバーレイ付きスワイプ画面 |
| **ナビゲーション** | NativeTabs（`expo-router/unstable-native-tabs`） |
| **テーマ** | Light / Dark / System 対応 |

### テックスタック

- Expo SDK + Expo Router（ファイルベースルーティング）
- NativeTabs ナビゲーション
- RevenueCat（`react-native-purchases`）
- AdMob（`react-native-google-mobile-ads`）
- expo-sqlite（localStorage ポリフィル）
- react-native-reanimated

### 主な制約

- `AsyncStorage` は使用禁止 → `expo-sqlite` の localStorage を使用
- `lineHeight` は使用禁止 → padding / margin で代替
- `Tabs`（expo-router）は使用禁止 → `NativeTabs` を使用
- `expo-av` は使用禁止 → 映像は `expo-video`、音声は `expo-audio`
