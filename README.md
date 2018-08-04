
# Docker
1. dockerをインストール
2. MySQL接続用パスはローカル上に.envを作成してください

```
設定例
        WORDPRESS_DB_NAME=wordpress
        WORDPRESS_DB_USER=wp_user
        WORDPRESS_DB_PASSWORD=password

        MYSQL_RANDOM_ROOT_PASSWORD=yes
        MYSQL_DATABASE=wordpress
        MYSQL_USER=wp_user
        MYSQL_PASSWORD=password
```

3. `docker-compose up` でコンテナ起動
4. `http://localhost:1002` でアクセス
5. 作業を終えたら `docker-compose stop` 
6. また作業するときは `docker-compose start` もしくは `docker-compose up -d` で開始