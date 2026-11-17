# ピンログ(試作版)

訪れた場所をGPSで記録し、名前・カテゴリ・備考を付けて、Googleマイマップ用のKML(CSV/GPXも可)を出力するスマホ向けWebアプリ(PWA)です。

## スマホに入れる手順(GitHub Pages・無料)

1. GitHubのアカウントを作る(https://github.com)。
2. 右上の「+」→「New repository」。名前は `pinlog` などにして、Publicのまま作成。
3. 「uploading an existing file」から、このフォルダの中身(index.html、sw.js、manifest.webmanifest、icon-192.png、icon-512.png)をアップロードして「Commit changes」。
4. リポジトリの「Settings」→「Pages」→ Branch を `main` / `/(root)` にして「Save」。
5. 数分後に表示されるURL(`https://ユーザー名.github.io/pinlog/`)をAndroidのChromeで開く。
6. 位置情報を「許可」し、Chromeのメニュー →「ホーム画面に追加」(または「アプリをインストール」)。

公開されるのはアプリ本体だけです。記録した地点はスマホの中にだけ保存され、GitHubには送られません。

## Googleマップに表示する手順

1. アプリの「出力」→ KML →「共有・保存」で、Googleドライブかスマホ本体に保存。
2. PCで https://www.google.com/mymaps を開き、地図を作成 →「インポート」でKMLを選ぶ。
3. Googleマップアプリの「保存済み」→「マイマップ」に表示されます。ピンの説明欄にあるナビ用URLをタップすると案内が始まります。

更新するときは、マイマップの古いレイヤを削除してから新しいKMLを取り込んでください。

## 注意

- データはブラウザの中に保存されます。Chromeの「サイトデータを削除」をすると消えるので、「出力」→「バックアップ」で定期的に書き出してください。
- 運転中の操作は避け、停車中に記録してください。
