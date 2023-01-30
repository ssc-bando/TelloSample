# Tello操作サンプルやら

参考: https://ponkichi.blog/drone01/

## Tello挙動メモ

* コマンドを送信後、コマンドの実行を完了すると、応答を返してくるみたい
* なので、「コマンド送信＋応答受信」を同期して実行するほうが動作が安定する

## ファイル一覧

* [sample.py](./sample.py)
    * 参考サイトのコードのまま
    * **送受信を非同期に実行しているため**挙動が不安定
* [move.py](./move.py)
    * 参考サイトをベースにコマンドの送受信を同期処理に変更
    * コードをそれっぽいクラスにまとめる
    * 実行内容は移動系のコマンドのみ
