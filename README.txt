セトリ帳（スマホのホーム画面アプリ版）

■ 中身
index.html            アプリ本体
manifest.webmanifest  アプリ名・アイコンの設定
sw.js                 電波がなくても開けるようにする仕組み
icons/                アイコン画像

■ 使えるようにする手順（GitHub Pages・無料）
1. GitHub（https://github.com）でアカウントを作る
2. 右上の「＋」→「New repository」で、名前を setlist などにして Public で作成
3. 「uploading an existing file」から、このフォルダの中身（index.html、manifest.webmanifest、sw.js、icons フォルダ）をまとめてドラッグして「Commit changes」
4. リポジトリの「Settings」→「Pages」で、Branch を「main」「/(root)」にして Save
5. 数分後に表示される https://ユーザー名.github.io/setlist/ がアプリのアドレス

■ ホーム画面に追加する
iPhone : Safariで上のアドレスを開く →（共有ボタン）→「ホーム画面に追加」
Android: Chromeで開く → 右上の︙ →「ホーム画面に追加」または「アプリをインストール」

■ データについて
・セトリはそれぞれのスマホの中に保存されます（メンバー同士では共有されません）
・機種変更や別の端末へ移すときは、「バックアップ」の「書き出す」→ 移した先で「読み込む」
・メンバーへは「LINEなどで送る」か「コピー」で文面を送ってください

■ アプリを更新したとき
index.html などを差し替えたら、sw.js の 1行目付近の VERSION（setlist-v1）を setlist-v2 のように変えてアップロードすると、各スマホで次に開いたときに新しい版になります。
