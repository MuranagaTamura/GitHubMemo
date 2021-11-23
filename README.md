# はじめに

~~田村村長のGitHubの環境は[GitHub Desktop](https://desktop.github.com/)ですので、あらかじめご了承ください~~

基本的に[GitHub Desktop](https://desktop.github.com/)だけですが、[TortoiseGit](https://tortoisegit.org/)も使えるように導入しました

基本的な流れは、

**リポジトリをクローン→ブランチを切る→コミットする→プッシュする→プルリクする→マージする**

です



# 各種ソフトウェアの使い方リンク

* [GitHub Desktop](GitHubDesktop.md)
* [TortoiseGit](TortoiseGit.md)



# SSH接続

1. コマンドプロンプトで「ssh-keygen -t rsa」と入力する
2. 3回エンターキーを押す
3. カギの中身をコピーする
   1. clip < ~.ssh/id_rsa.pub
4. GitHubからSettings > SSH and GPG keysを選択
5. New SSH Keyをクリックする
6. Titleと先ほどコピーしたカギ文字列をKeyに貼り付ける
7. Add SSH Keyをクリックする
8. （以下は一応SSH接続ができるのかを確認するためなので、無視してもいいがやって損はない）
9. コマンドプロンプトで「ssh -T git@github.com」と入力する
10. 「Hi (アカウント名)! You've successfully authenticated, but GitHub does not provide shell access.」で接続成功です



# エラー対処

## error: failed to push some refs to 'https://gothub.com/USERNAME/REPOSITORY'

原因としてGitの参照するURLがHTTPSとなっていることだと考えられます。現在のGitHubはパスワードによる接続を許可しておらず、SSH接続のみ有効となっています。そのため、Gitの参照するURLをHTTPSからSSHに変更すれば問題ありません。変更方法はリポジトリ下で以下のコマンドを実行すると変更できます。

```
git remote set-url origin git@github.com:USERNAME/REPOSITORY.git
```



# 更新履歴

## 2021年11月23日

* ブランチの一部修正した
* エラー対処を追加した
* GitHub Desktop だけでなく、TortoiseGitでの操作方法も各所追記した
* ファイル構成を変更しました



## 2021年11月22日

* はじめに、SSH接続、クローン、ブランチ、コミット、プッシュ、プルリクエスト（プルリク）、プルリクをIssuesにリンクを追加した