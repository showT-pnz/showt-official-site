# showT Official Site

このリポジトリは showT ブランドの公式サイトと、アプリ「VAULT.」の配布ページを含んでいます。

## 公開手順 (GitHub Pages)

1.  GitHub で新しいリポジトリを作成します（例: `showt-official`）。
2.  このローカルディレクトリで以下のコマンドを実行して、GitHub にプッシュします。
    ```bash
    git remote add origin https://github.com/あなたのユーザー名/showt-official.git
    git branch -M main
    git push -u origin main
    ```
3.  GitHub リポジトリの `Settings > Pages` を開きます。
4.  `Build and deployment > Source` で `Deploy from a branch` を選択し、`main` ブランチの `/ (root)` を指定して `Save` します。
5.  数分待つと、`https://あなたのユーザー名.github.io/showt-official/` でサイトが公開されます。

## VAULT. APKの配布手順

1.  Flutter プロジェクト (`collect_app`) で APK をビルドします:
    ```bash
    flutter build apk --release
    ```
2.  GitHub のリポジトリページ右側にある `Releases` から `Create a new release` をクリックします。
3.  ビルドした APK (`build/app/outputs/flutter-apk/app-release.apk`) を添付して公開します。
4.  公開後、APK の直リンク（`https://github.com/.../releases/download/.../app-release.apk`）をコピーします。
5.  `vault.html` 内のダウンロードボタンの `href` を、そのリンクに書き換えて再度プッシュしてください。

## ライセンス
Design: [HTML5 UP](https://html5up.net) (CCA 3.0)
