
## 概要

- 以下のフレームワーク･ライブラリを使ったテンプレートプロジェクト
  - Vue2.x
  - Laravel8.x

## 設定内容

- 実行コマンド
```
composer create-project laravel/laravel vue-laravel-template --prefer-dist`
composer require laravel/ui
php artisan ui vue
npm install
npm install --save-dev vue-router
npm audit fix
npm run dev
```

- カスタマイズ部分
  - `welcome.blade.php`、`ExampleComponent.vue`の削除
  - `app.blade.php`の追加、`HeaderComponent`と`router-view`のビューの構成
  - `HeaderComponent`,`DashboardComponent`,`HomeComponent`の追加
  - `web.php`にあらゆるURLについて`app.blade.php`のビューを返す設定
  - `vue-router`で`Dashboard`,`Home`をそれぞれ`router-view`で吐き出すように設定
  - `vue-loader`のインストール
  - `_variables.scss`に`$black`と`$white`を追加
  - `.gitignore`に`public/`を設定
  - `README.md`の編集
  
## 使い方
  - テンプレートリポジトリを元にリポジトリを作る
  - 以下のコマンドを叩く
  ```
  git clone https://github.com/{UserName}/{RepositoryName}
  npm install
  npm run dev
  php artisan serve
  ```
  - http://localhost:8000 へアクセス
  - カスタマイズ
