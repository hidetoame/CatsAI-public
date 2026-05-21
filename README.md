# CatsAI

Macを、声で動かす。  
デスクトップ常駐型・音声AIアシスタントです。

CatsAI は、OpenAI GPT Realtime 2 を使い、音声でMacを操作できる実験アプリです。デスクトップに常駐するキャラクターに話しかけるだけで、フォルダを開いたり、メモを作ったり、調べ物をさせたりできます。

## ダウンロード

公証済みアプリは GitHub Releases からダウンロードしてください。

1. `CatsAI.app.zip` をダウンロード
2. ZIPを解凍
3. `CatsAI.app` を `アプリケーション` フォルダへ移動
4. 起動後、OpenAI APIキーを設定

## 主な機能

- 音声でアプリやフォルダを起動（例: 「Dropboxを開いて」「システム設定を開いて」）
- 音声でファイル作成（例: 「デスクトップにメモを作って」）
- 音声でWeb検索（例: 「今日のAIニュースを調べて」）
- 画面理解（例: 「これ見て」）
- メディア検索（YouTube / iTunes / Apple Music）
- タイマー / アラーム
- Googleカレンダー確認 / 予定追加
- メールチェック（IMAP / POP3）
- キャラクターは画像1枚から生成可能
- おまけ: スクリーンショット拡張（撮影後にその場で注釈、ON/OFF可）

## 使い方

デスクトップ上のキャラクターをダブルクリックすると、音声会話を開始または終了します。

話しかける例:

- 「ダウンロードフォルダを開いて」
- 「Notionを立ち上げて」
- 「デスクトップにメモを作って」
- 「今日のAIニュースを調べて」
- 「メール何件ある？」

返答中にスペースキーを押すと、音声を停止できます。

## 初期設定

CatsAI を使うには OpenAI APIキーが必要です。ChatGPTの有料プランとは別に、OpenAI APIの課金設定が必要です。トークン使用量は各自の負担となりますので、OpenAI Platformで適時確認してください。

- OpenAI Platform: https://platform.openai.com/
- Billing: https://platform.openai.com/settings/organization/billing/overview

Googleカレンダーやメールチェックは、設定画面でONにした場合だけ使います。

Googleカレンダー連携では、Google認証時に「このアプリは Google で確認されていません」といった警告が表示される場合があります。信頼できる場合だけ、詳細表示から続行して許可してください。

## 権限について

macOSの仕様により、マイク、アクセシビリティ、画面収録、自動化などの許可が必要になる場合があります。CatsAIは必要な時だけ権限を要求します。

## キャラクターについて

キャラクターは写真やイラスト1枚で自由に差し替えできます。デフォルトでは、猫キャラクターの「よもぎ」「あずき」「うめ」を同梱しています。

ねこキャラ: https://x.com/shakotanCats

## 開発者向け

```bash
cd HomeApp/Agent
npm install
cd ..
./build.sh
```

ビルドには macOS、Swift、Node.js、署名環境が必要です。配布用に公証する場合は Apple Developer ID が必要です。


## ソースコードについて

ソースコードは、反響があれば公開します。興味がある方はご連絡ください。

GitHubの仕様でReleaseには自動的に `Source code (zip)` / `Source code (tar.gz)` が表示されますが、これは公開リポジトリ内のREADME等をまとめたもので、CatsAI本体のソースコードではありません。

## Privacy Policy

- [Privacy Policy](PRIVACY.md)
- [Terms / Disclaimer](TERMS.md)

## 免責

本アプリは個人開発の実験アプリです。不具合やセキュリティ上の問題が含まれる可能性があります。本アプリの使用、PC操作、外部サービス連携によって発生した不都合や損害について、開発者は責任を負いません。利用者ご自身の責任で使用してください。

## 著作

Copyright (c) hidetoame

- https://x.com/hidetoame
- https://x.com/shakotanCats
