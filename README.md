# Try_Review
Reviewを触って動かしてみてみるまでやる

# 参考ページ

* インストールに関して
    * https://review-knowledge-ja.readthedocs.io/ja/latest/faq/faq-usage.html
* クイックスタートガイド
    * https://github.com/kmuto/review/blob/master/doc/quickstart.ja.md
* フォーマットガイド
    * https://github.com/kmuto/review/blob/master/doc/format.ja.md

# ステップ

* gem 版でやってみる
* Docker 版でやってみる
* それを運用フローと合わせて告知
* Docker版をCIで回せるようにする

## gem 版でやってみる

クイックスタートガイドを参照

1. Gemをinstallする
    1. `gem install review`
    1. もちろん bundle 使ってやっても良い
1. ReView用のテンプレートフォルダを作る
    1. `review-init <project_name>`
    1. bundle で入れている場合は `bundle exec review-init <project_name>`
1. `cd <project_name>` でプロジェクトの中へ
1. `<project_name>.re` ファイルを編集する
1. `rake` でコンパイルする
    1. `rake epub` で epub 形式のものができる
    1. `rake pdf` で pdf 形式のものができるらしいが、TeX環境が必要らしい
        1. 今TeX環境構築してないので、暇な時に試す
    1. うまくいけば `book.epub` ができる
    1. 失敗したときはエラー吐かれたので、それを頑張って読む
1. `open book.epub` とかで見てみる

## Docker版

TBW
