# docs

## アプリの概要

一つの部屋の中で複数人でチャットできる。

![アプリのイメージ](img/アプリのイメージ.png)

<br>

## 全体

![ブロック図](img/ブロック図.png)

<br>

## チャットルームとチャット

topic は MQTT でも活用する部屋を識別するもの。C# の Dictionary を使って topic と chat room を結びつける<br>
あるトピックに複数人でコメント投げ合い、投げられたコメントは chat room 内の Collection で管理する。

commentは以下の情報を持つ。
- PostTime : 投稿時間
- Content  : 投稿内容
- UserName : ユーザー名

![チャットルームとチャット](img/チャットルームとチャット.png)

## チャットサーバーのアーキテクチャ

![チャットサーバーアーキテクチャ](img/サーバーアーキテクチャ.png)