# wp-theme-template
WordPress テーマ開発用レポジトリです。
Docker を使って、 WordPress テーマの開発を簡単に始められるようになっています。

## 事前準備
`docker-compose` コマンドが使える必要があります。
大抵は Docker for Windows か Docker for Mac をインストールすれば良いはず。

- Windows の場合 https://docs.docker.com/docker-for-windows/
- mac の場合 https://docs.docker.com/docker-for-mac/

その後、ターミナルで `docker-compose -v` と入力して、 `docker-compose` コマンドを使える事を確認しましょう。

```
$ docker-compose -v
docker-compose version 1.9.0, build 2585387
```

## 開発の手順
1. ターミナルで `git clone https://github.com/fand/wp-theme-template && cd wp-theme-template` を実行
2. ターミナルで `docker-compose up` を実行
  - 手元のマシンで WordPress サーバーが起動します
3. ブラウザで `http://localhost:8080` にアクセス
4. `themes/` 以下にテーマを作成
5. 管理画面でテーマを設定

`themes/` にあるテーマを編集すると、手元の WordPress サイトに即反映されます。

## `themes/` について
`themes/` には WordPress のデフォルトテーマ twentyseventeen が入っています。
このディレクトリを参考にしたり、直接編集したりしてテーマを作成できます。

自作のテーマを既にお持ちの場合、 `themes/` 内にコピペすると良いでしょう。
