# TortoiseGit版

* インストール時のChoose SSH Client で、「OpenSSH, Git default SSH Client」を選択すると幸せになるかもです
* 基本的にGUIというより、エクスプローラーの左クリックメニューから選択して、操作する



## クローン

1. クローンしたいリポジトリをブラウザで開く
2. Codeタブの緑色の「Code」ボタンをクリックする
3. CloneダイアログのタブにあるHTTPSをクリックする
4. HTTPSタブのすぐしたにある「https://github.com/〇〇/〇〇.git」となっている箇所をコピーする
5. エクスプローラーを開く
6. 何もない（ディレクトリやファイルではない）ところで左クリックする
7. Git Clone ... をクリックする
8. Clone Existing Repository 内のURL: に先ほどコピーした文字列をペーストする



## ブランチ

（エクスプローラーでの操作です）

1. 何もない（ディレクトリやファイルではない）ところで左クリックする
2. TortoiseGit > Create Branch ... をクリックする
3. （ダイアログが表示されます）
4. Name内のBranch欄につけたいブランチ名を入力する
5. Options内のSwitch to new branch にチェックマークを付ける
6. 下部にあるOKボタンをクリックする



## コミット

（エクスプローラーでの操作です）

1. 何もない（ディレクトリやファイルではない）ところで左クリックする
2. Git Commit -> "ブランチ名"...をクリックする
3. （ダイアログが表示されます）
4. Message: 内の文字列を入力できる欄にコミット内容を入力する
5. Changes made (double-click on file for diff)内のPathやExtension、Statusが書いてあるところにコミット対象を選択する
6. 下部にあるCommitボタンをクリックする



## プッシュ

（エクスプローラーでの操作です）

1. 何もない（ディレクトリやファイルではない）ところで左クリックする
2. TortoiseGit > Push ... をクリックする
3. （ダイアログが表示されます）
4. 下部にあるOKボタンをクリックする



## プルリクエスト（プルリク）

（ブラウザでの操作です）

1. Pull requests タブをクリックする
2. New pull request ボタン（緑ボタン）をクリックする
3. Comparing changes 少し下のbase: をマージ先のブランチに設定する
4. Comparing changes 少し下のcompare: をマージ元のブランチに設定する
5. Comparing changes 少し下のcompare: より右の文字列で Able to merge. と表示されていることを確認する
   * そもそもマージすることが不可能な場合があるので、ここで確認することができます
6. Create pull request ボタン（緑ボタン）をクリックする
7. プルリクのタイトルのその詳細を入力
8. Create pull request ボタン（緑ボタン）をクリック



## Issueを発行

（ブラウザでの操作です）

1. Issuesタブをクリックする
2. New issue ボタン（緑ボタン）をクリックする
3. Issueのタイトルのその詳細を入力
4. Submit new issue ボタン（緑ボタン）をクリック



## プルリクをIssueにリンク

（ブラウザでの操作です）

1. Pull requests タブをクリックする
2. リンクしたいプルリクを選択する
3. 右サイドバーのLinked issues をクリックする
4. リンク対象のissueを選択する
   * 最大10個までリンクできる

