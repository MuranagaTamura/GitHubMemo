# はじめに

田村村長のGitHubの環境は[GitHub Desktop](https://desktop.github.com/)ですので、あらかじめご了承ください

基本的な流れは、

**リポジトリをクローン→ブランチを切る→コミットする→プッシュする→プルリクする→マージする**

です



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



# クローン

1. Codeタブの緑色の「Code」ボタンをクリックする
2. Cloneダイアログの「Open with GitHub  Desktop」をクリックする
3. 許可を求めるアラートが表示されるので、許可にチェックしてプログラムを選択ボタンをクリックする
4. プログラムを選択して、リンクを開くボタンをクリックする
5. リポジトリをクローンする先をChoose...から選択する
6. これでローカル環境にクローンできました



# ブランチ

1. Current branchをクリックする
2. Filter欄に新しいブランチ名を入力する
3. New branch ボタンをクリックする
4. Create branch ボタンをクリックする



# コミット

1. コミットする前にコミット対象を選択します
   * 左サイドバーにあるChangesタブからチェックするとコミット対象になります
   * 正確には「ステージング」という行為も同時に行っています
2. コミットタイトルとその詳細を入力する
   * コミットタイトルは左サイドバーのSummary(required)
   * 詳細は左サイドバーのDescription
3. Commit to ブランチ名 をクリックする



# プッシュ

1. コミットする（コミットを参照）
2. 上部にあるPush origin ボタンをクリックする



# プルリクエスト（プルリク）

1. リボンにあるBranch > Create pull request でプルリクを作成する
   * Ctrl + R でも可能
2. ブラウザが起動される
3. プルリクのタイトルのその詳細を入力
4. Create pull request ボタンをクリック



# Issueを発行

1. リボンにあるRepository> Create issue on GitHub でプルリクを作成する
   * Ctrl + I でも可能
2. ブラウザが起動される
3. プルリクのタイトルのその詳細を入力
4. Submit new issue ボタンをクリック



# プルリクをIssueにリンク

1. リボンにあるRepository> View on GitHub でプルリクを作成する
   * Ctrl + Shift + Gでも可能
2. Pull requests タブをクリックする
3. リンクしたいプルリクを選択する
4. 右サイドバーのLinked issues をクリックする
5. リンク対象のissueを選択する
   * 最大10個までリンクできる



# 更新履歴

## 2021年11月22日

* はじめに、SSH接続、クローン、ブランチ、コミット、プッシュ、プルリクエスト（プルリク）、プルリクをIssuesにリンクを追加した
