# symfony-test

Symfonyを使った会員登録、ログイン、投稿の作成、一覧、詳細のサンプル実装。  
PHP8.1以上、[composer](https://getcomposer.org/download/)が必要。

## Setup

### このリポジトリをクローン
```
git clone https://github.com/ezaki3/symfony-test.git
```

### 必要モジュールのインストール
```
cd symfony-test
composer install
```

### DB設定
.envを.env.localにコピーして編集する
```
cp .env .env.local
```
DATABASE_URLを自分の環境に合わせて変更する

#### DB作成
DBがまだ存在しない場合は作成することができる
```
php bin/console doctrine:database:create
```

### マイグレーション
```
php bin/console doctrine:migrations:migrate
```
