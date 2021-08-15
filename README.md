# Laravel テンプレート
Docker環境でのLaravel開発用テンプレート。(バージョンは5.5)
mock用サーバーとしてjson-serverも設置済み。

## 環境構築
コンテナ起動
```sh
git clone git@github.com:yusuke0724/laravel-template.git
cd laravel-template
docker-compose up -d
```

マイグレーション
```sh
docker exec -it laravel bash
cd app
composer install
cp .env.local .env
php artisan migrate
```

下記へアクセス
```
http://localhost:8000/
```
