
# 模擬案件　_フリマアプリ

## 環境構築

### Docker ビルド

1. docker-compose up -d --build

### Laravel 環境構築

1.docker-compose exec php bash

2.composer install

3.『.env.example』をコピー名前変更し『.env』を作成。70行目あたりを以下のように編集

// 前略

DB_CONNECTION=mysql

DB_HOST=mysql

DB_PORT=3306

DB_DATABASE=laravel_db

DB_USERNAME=laravel_user

B_PASSWORD=laravel_pass

// 後略

5.アプリキーを作成

php artisan key:generate

6.マイグレーション実行

php artisan migrate

7.シーディング実行

php artisan db:seed

## 使用技術（実行環境）

+ PHP7.4.9-fpm
  
+ Laravel8.83.29
  
+ MySQL8.0.26

## ER 図

![furimaAppER net](https://github.com/user-attachments/assets/c4492b76-c1c3-499e-83f5-1f1fed9cc892)




## URL

+ 開発環境：http://localhost/

+ phpMyadmin：http://localhost:8080/
