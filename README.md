# 学生LT 公式サイト

学生LTの[公式サイト](https://student-lt.tech/)のリポジトリ。  
静的サイトジェネレータの Hugo を利用して開発している。

![がぞう](https://i.gyazo.com/9908c8b06e251b275d1011704981988f.jpg)

Hugo の触り方は下記リンク参照。

http://qiita.com/yakimeron/items/42d537374abde5517267

ホスティングは下記ブランチで行っている。

https://github.com/student-lt/student-lt/tree/gh-pages

キャッシュ及びHTTPS化は [CloudFlare](https://www.cloudflare.com/) で行っている。

# ローカルプレビュー方法

```
hugo server --theme=minimal --buildDrafts --watch
```

# 編集方法

ヘッダーは `themes/minimal/layouts/partials/_index_header.html` を修正。  
(同じ階層に `header.html` というのがあるが、これはトップページ以外で使われる。)  
本文は `content/_index.md` を修正。  
その他CSSやJS等は `themes/minimal` 以下にある。


# 開発に参加する

公式サイトに要望がある場合はIssueに記述して頂き、何か改善して頂いた場合はプルリクお願いします！  
プルリクが溜まっている場合はローカルで動作確認後に良さそうだったらLGTMを出してOKです！  
プルリクを出した人はLGTMを貰ったらmasterにマージして構いません。  
Issueとプルリクが紐付いている場合はIssueのcloseもお願いします。  
マージ後はpullした後に `./build.sh` を実行して頂けるとデプロイされます。  
(この手順はCircleCI等で自動化予定)

何か問題が発生した場合は、学生LTの [Discord](https://discord.gg/F4u9yKN) の「公式サイト開発部」チャンネルまでお願いします！

## 注意点

- LGTMはプルリクを出した人以外の人が出す
- マージする場合は必ず `./build.sh` の実行まで行う


© 2017-2019 学生LT. All rights reserved.
