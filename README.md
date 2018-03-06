# clickShussha
実行するとデスクネッツを開いて出社ボタンを押します。


## 使い方
  基本的にはWindowsのタスクスケジューラに登録し、自動実行される事を想定しています。タスクスケジューラに`backgroundRunner.vbs` を登録し、アンロック時、ログオン時に実行されるようにスケジュールしてください。。
  `_backgroundRunner.bat` のPythonのパスを、通るところに修正してください。

  手動で実行する場合は `python main.py` で実行してください。

## 設定ファイル
  credentials.template.yamlをcredentials.yamlとリネームし、desknet'sのログイン情報を書き込んでください。Slackのトークンを入れておくと、#zzz-slack-sandbox に実行結果が書き込まれます。




## Known issues
  以前は動いていたのに動かなくなった
  -  Windowsのパスワードを変更した場合は実行されなくなってしまいます。登録したタスクのプロパティを開き、何も変更せずにOKを押すとパスワード入力画面が出て新しいパスワードに更新されます。