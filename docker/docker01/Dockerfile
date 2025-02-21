# 1. ベースとなるイメージを指定
FROM ubuntu:latest
# 2. 必要なパッケージをインストール
RUN apt update && apt install -y nginx
# 3. 環境変数を設定
ENV SERVER_NAME=konbusv
# 4. 作業ディレクトリを設定
WORKDIR /app
# 5. ファイルをコンテナにコピー
COPY index.html /var/www/html/index.html
# 6. ポートを開放
EXPOSE 80
# 7. コンテナ起動時にコマンドを実行
CMD ["nginx", "-g", "daemon off;"]