# 開発環境手順

1. Python, Django のインストール
2. `django-admin startproject Django`
3. `py manage.py runserver` 開発環境の起動 >> [確認](http://127.0.0.1:8000/)

# ディレクトリ構成

-   外側の mysite/ ルートディレクトリは、プロジェクトのコンテナです。その名前は Django にとって重要ではありません。任意の名前に変更できます。
-   manage.py: Django プロジェクトに対する様々な操作を行うためのコマンドラインユーティリティです｡詳しくは django-admin と manage.py 内の manage.py を参照してください｡
-   内側の mysite/ ディレクトリは、このプロジェクトの実際の Python パッケージです。この名前が Python パッケージの名前であり、 import の際に 使用する名前です (例えば import mysite.urls) 。
-   mysite/\_\_init\_\_.py: このディレクトリが Python パッケージであることを Python に知らせるための空のファイルです。Python の初心者は、 Python の公式 ドキュメントの more about packages を読んで下さい。
-   mysite/settings.py: Django プロジェクトの設定ファイルです。 設定の仕組みは Django の設定 を参照してください。
-   mysite/urls.py: Django プロジェクトの URL 宣言、いうなれば Django サイトにおける「目次」に相当します。詳しくは URL ディスパッチャ を参照 してください。
-   mysite/asgi.py: プロジェクトを提供する ASGI 互換 Web サーバーのエントリポイント。詳細については ASGI でデプロイする を参照してください。
-   mysite/wsgi.py: プロジェクトをサーブするための WSGI 互換 Web サーバーとのエントリーポイントです。詳細は WSGI とともにデプロイするには を参照してください。
