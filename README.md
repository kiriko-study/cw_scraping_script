## 使い方
# １．config.iniに必要項目を書き込んでください。
メールは自分から自分に送信します。
[CW Category ID]の欄は、チェックしたい仕事カテゴリの数字を登録してください。
例：「HTML・CSSコーディング」なら「16」、「ランディングページ（LP）制作」なら「17」

# ２．Googleの設定で安全性の低いアプリのアクセスを許可してください。
（アカウント管理→セキュリティ）

# ３．cw_scraping_script.exeを実行
初回起動時に「cw_job_log_category_XX.txt」といったファイルが生成され、新着メール通知が来ます。
2回目以降は新着があった時だけメール通知します。
新着を確認したい時に起動するか、後述のタスクスケジューラに登録して自動化してください。

# ※Chromeをインストールしていないと使えません。
またChromedriverとChrome本体のバージョンが一致していないとエラーになります。
もしエラーになったら両方を同じバージョンに合わせてください。

## Windowsタスクスケジューラ（Windows管理ツール）への登録
# １．「操作」→「タスクの作成」
# ２．「全般」タブで名前を入力
# ３．「操作」タブで新規追加
# ４．「プログラム/スクリプト」でcw_scraping_script.exeを指定
# ５．「トリガー」タブで新規追加
# ６．「設定」を「毎日」にして、「詳細設定」の「繰り返し間隔」にチェック
# ７．「繰り返し間隔」はお好みで、「継続時間」を無期限にして
# ８．OKを押していって登録を完了させる
