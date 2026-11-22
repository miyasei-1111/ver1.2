にょん姉貴が登場☆ v1.2

v1.1を改良してウィンドウ上を歩いたり、別のウィンドウへ飛び移ったりするようにしました。

## 起動

プロジェクト直下で実行してください。

```bash
python main.py
```

## 素材

画像・音声素材は `assets/` に同梱されています。画像は `assets/<状態名>/`、音声は `assets/voices/<イベント名>/` に配置されており、自由に差し替えられます。素材がない場合は、簡易キャラクターが表示されます。素材がない場合は、簡易的なキャラクターが生成されます。~~nyn姉貴の素材は容量が大きくアップロードできなかった~~ので以下のリンクから配布。assetsごと置き換えればnyn姉貴がデスクトップ上に現れるゾ。
https://41.gigafile.nu/1120-k42c1743e0c7f957ddebde5e9013fa555

## EXE化

PySide6を使用しています。`main.py` が起動ファイルで、EXE化する場合のエントリポイントです。
"python -m PyInstaller --noconsole --noconfirm main.py"でコンパイルしてください
アイコンを設定したい場合
"python -m PyInstaller --noconsole --noconfirm --icon=アイコンのファイル名.ico main.py"でコンパイルしてください
コンパイルすると、main.pyと同じ場所にdistフォルダが作成され、その中にmain.exeが作成されます。
exe化した場合、main.exeと同じ場所にassetsフォルダを再配置してください。

## OS対応について

Windowsでは他のアプリのウィンドウ上を歩く機能を実装しています。macOSとLinux X11にも同機能の実装がありますが、いずれも実機ではテストしていません。Windowsを含め、OSのウィンドウ取得処理は実機未検証です。Linux WaylandではOSの仕様により他アプリのウィンドウ上を歩く機能は使えず、画面下端のみ歩きます。

## 使用したNYN姉貴素材

sm30598781.mp4
sm31945874.mp4
sm30761410.mp4
sm32184120.mp4
sm33898287.mp4
https://www.axfc.net/u/3844454.zip
