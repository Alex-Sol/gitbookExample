# gitbookExample

gitbook とgitlab-pages の例

[Gitlab リポジトリ](https://gitlab.com/Ouvill/gitbookexample)

[デモ](https://ouvill.gitlab.io/gitbookexample)

当リポジトリを Gitlab リポジトリに Push　すると自動的に gitlab-ci が走り、gitbook サイトが公開されます。

## 簡単な使い方

 1. Gitlab でフォークする。
 1. リポジトリをクローン
    ``` sh
    git clone ******(クローン先のURL)
    ```
 1. `SUMMARY.md` と `source` フォルダ内のファイルを編集する。
 1. git push する

## ローカルで動作させる。

 1. Node.js をインストールしてください
 1. Gitbook のインストール
    ```
    npm install -g gitbook-cli
    ```
 1. リポジトリをクローン
    ``` sh
    git clone https://gitlab.com/Ouvill/gitbookexample.git
    ```
 1. フォルダに移動
    ``` sh
    cd gitbookexample
    ```
1. 依存関係をインストール
    ``` sh
    npm install
    gitbook install
    ```
1. ファイルを編集する
1. ビルドする
    ```sh
    gitbook build . public
    ```
