# github-portfolio

# CHATTING PROGRAME
> インフラ系(サーバー、ネットワーク)に興味を持つようになった理由は、チーム課題として制作していたゲームで
> 作業を担当したチャットプログラムの問題のためでした。
> 現在HITスクールの職業訓練コースで学んでいるpythonを利用して小さなプログラムを作ってみました。

# 使用した技術の説明

このコードは、マルチスレッドとソケットプログラミングを使用したマルチリンガルチャットサーバーを作成するためのものです。
以下に、このコードの主要な機能と使用されている技術を詳しく説明します。

マルチスレッド: Pythonのthreadingモジュールを使用して、各クライアント接続に対して個別のスレッドを作成します。
              これにより、複数のクライアントが同時にサーバーに接続し、メッセージを送受信することが可能になります。

ソケットプログラミング: Pythonのsocketモジュールを使用して、ネットワーク接続を確立し、データを送受信します。
                      このコードでは、TCP/IPソケットを使用しています。
マルチリンガルサポート: messagesという辞書を使用して、英語(en)、日本語(jp)、韓国語(kr)の3つの言語でのメッセージをサポートしています。
                      これにより、ユーザーは自分の好きな言語でチャットを楽しむことができます。

ユーザー管理: clientsとusers_idという2つのリストを使用して、接続中のすべてのクライアントとそのユーザーIDを管理します。
            これにより、ユーザーが接続または切断したときに、他のすべてのユーザーに通知することができます。

コマンド: /qまたは/quitでチャットから退出し、/ulまたは/userlistで接続中のユーザーのリストを取得することができます。

> [プロジェクトプログラム詳細](https://github.com/03kimu/github-portfolio/tree/main/Chatting)