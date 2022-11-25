# 100 Days Of Code - 学習ログ

### 0日目: 2022年11月24日

**今日の進捗**: 
「りあくと！」を読み始めた。
基本情報の試験も終わったのでやっとコードを書く時間が取れそう。
100DaysOfCodeの取り組みも始めてみた。

**思ったこと・わかったこと** 
- Node.jsとは
  -  PC のターミナル上で 実行できる環境を提供するソフトウェア
-  フロントエンド開発にNodeが必要な理由
  - パフォーマンス最適化のために JavaScript や CSS ファイルを少数のファイルにまとめる(=バンドル)
  - 新しいバージョンの JavaScript や AltJS12 のコードを古いバージョンの JavaScript コンパイルして、古いブラウザでも動作可能にする
  - 開発環境においてブラウザにローカルファイルを直接読み込ませるのではなく、ローカルに開発用のアプリ ケーションサーバを稼働させることで、動作を検証しやすくし開発効率を高める
  - テストツールを用いてユニットテストや E2E テスト 13 を記述・実行する
  - ソースコードの静的解析や自動整形を行う
- asdfを使って他の言語環境も管理する
  - brew install asdf
- `.default-npm-packages`の役割
  - 任意のNodeのバージョンをインストールしたときにデフォルトでインストールされるnpmパッケージを登録しておける

**リンク**
- [りあクト！ TypeScriptで始めるつらくないReact開発 第4版【① 言語・環境編】 - くるみ割り書房 ft. React - BOOTH](https://oukayuka.booth.pm/items/2368045)
- [#100DaysOfCode Official Website | #100DaysOfCode](https://www.100daysofcode.com/)

### 1日目: 2022年11月25日

**今日の進捗**: 2-1-2. 年々進化していく JavaScript まで

**思ったこと・わかったこと**
- Viteでプロジェクトを作成する
    - viteを使うことで面倒な設定不要でプロジェクトをつくることができる
      - `rails new`と似たやつ
    - `yarn create vite hello-world --template=react-ts`
    - `--template`でプロジェクトのテンプレートを指定する
    - 今回はReact+TypeScriptのテンプレートを選択している
    - viteはReactだけでなくVueなどの他のフレームワークのプロジェクトも作ることができる
    - yarn を実行
      - yarn install では, package.jsonに記述されている依存パッケージを`node_modules/`配下にインストールして, さらにイン ストールされたパッケージのバージョン情報を、その依存関係も含めて`yarn.lock`というファイルに出力する
      - yarn.lock
        - インストールしたパッケージの依存情報を保存しておくためのファイル
      - リポジトリには`node_modules/`は入れないけど、`yarn.lock`は必ず入れておく\
    - Hot Module Replacement
      - ソースコードを変更・保存するとアプリケーションに即座に反映される
      - Viteの機能のひとつ
    - npm と yarn
      - 後発のyarnがだんだん使われるようになってきた
      - 依存パッケージのバージョン固定ができるyarn.lockが最初から備わっていた
      - Workspace: 複数のプロジェクトを単一のリポジトリで管理するための機能もあった
    - package,json内のdependenciesとdevDependencies
    - devDependencies: 開発環境でしか有効にならない。開発ツールのパッケージを入れる
    - dependencies: 
  -  そもそもJavaScriptについて
    - ES2015以降をモダンJSという
