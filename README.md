# Vue-Training

[English](./docs/lang/en.md) | 日本語

Vue.js 3 + Firebase + RESAS API を使用した都道府県データ可視化アプリケーション

## RESAS API

RESAS APIは2025年3月24日（月）をもって提供を終了いたしました。

現在、このアプリケーションはRESAS APIに依存しているため、システムとして機能していません。

参考: [RESAS APIの提供終了・新規利用申し込み停止について](https://opendata.resas-portal.go.jp/docs/api/v1/index.html)

## セットアップ

1. リポジトリをクローン

   ```bash
   git clone <repository-url>
   cd vue-training
   ```

2. 依存関係をインストール

   ```bash
   pnpm install
   ```

3. 環境変数を設定
   `.env`ファイルを作成し、以下の変数を設定してください：

   ```env
   # Firebase設定
   VUE_APP_FIREBASE_API_KEY=your_firebase_api_key
   VUE_APP_FIREBASE_AUTH_DOMAIN=your_project.firebaseapp.com
   VUE_APP_FIREBASE_PROJECT_ID=your_project_id
   VUE_APP_FIREBASE_STORAGE_BUCKET=your_project.appspot.com
   VUE_APP_FIREBASE_MESSAGING_SENDER_ID=your_sender_id
   VUE_APP_FIREBASE_APP_ID=your_app_id
   VUE_APP_FIREBASE_MEASUREMENT_ID=your_measurement_id

   # RESAS API設定
   VUE_APP_RESAS_API_KEY=your_resas_api_key
   ```

4. 開発サーバーを起動

   ```bash
   pnpm serve
   ```

## 技術スタック

- Vue.js 3
- Vuex
- Firebase
- RESAS API
- Chart.js
- SCSS
- ESLint + Prettier

## 機能

- 都道府県データの取得・表示
- チェックボックスによる都道府県選択
- 選択した都道府県のデータ可視化（チャート表示）
