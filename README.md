# Kitとは
gitは素晴らしいツールですが、素晴らしすぎて少し使いづらいです。
元々はLinuxを開発するために使われたツールらしいのですが、誰もがLinux並みの巨大プロジェクト
をやっているわけではない。だからシンプルにしてみたんです。
kitは小さなプロジェクトを個人で開発しているユーザに特化したgitラッパーです。

# 使い方
```
# インストール
curl https://raw.githubusercontent.com/endows/kit/master/install.sh | sudo bash
cd myProject
# 変更を保存
kit commit
# 直前のcommitに戻る
kit rollback
```

# 機能
## kit commit
現在のディレクトリの状態を保存します。
```
git add .
git commit -m "<timestamp>"
```
## kit rollback
直前のcommitに戻ります。ディレクトリの状態も変更されます。
つまりcommitされていない変更はすべてなかったことになります。
```
git add .
git commit -m "end"
git reset --hard HEAD~1
```

# 開発中の機能
## kit todo
ToDo形式でプロジェクトを開発することができる。
## kit create
リモートサーバ(kit.endows.tk)にレポジトリを作成

# 問い合わせ
[@kyouzyuuuuuuuu1](https://twitter.com/kyouzyuuuuuuuu1)
