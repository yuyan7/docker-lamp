## YAMLに「build:」があればそのイメージをまとめてビルド
docker-compose build
## YAMLに「image:」があればそのイメージをまとめてプル
docker-compose pull
## docker-compose build, docker-compose pullをした後にdocker run
docker-compose up -d
## 個別のサービスを指定することもできる。依存関係がある場合は関係するコンテナが全て起動される
docker-compose up -d php
## 関係するコンテナすべての出力を表示
docker-compose logs
## 関係するコンテナをまとめて終了
docker-compose stop
## 関係するコンテナをまとめて削除
docker-compose rm

## コンテナ内にホストのファイルをコピー
docker cp <ホストのコピー元> <コンテナID>:<コンテナ内のコピー先>

php/source内にドキュメントルートに配置したいソースコードを置く。
mysqlコンテナはphpコンテナからはホスト名「mysql」で見れる。
