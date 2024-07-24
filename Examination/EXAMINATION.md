# KDW が採用する Git Flow に関するテスト

`production`、`develop`、`next-dev`等の文言を使用し、回答ください。

1. リリースしている製品で緊急度の高いバグが発生した場合はどのように対処しますか？
productionからhotfixのブランチをきって修正を加え、修正後developにマージ、productionへプルリクを作成する
可能であればdevelopでの動作確認をするがproductionへのマージとデプロイを急ぐ

1. リリースしている製品で緊急度の低いバグが発生した場合はどのように対処しますか？
developから修正ブランチをきってdevelopへマージする
定期的なリリース起点でdevelopからproductionへマージされデプロイされる

1. Version Up などで予定されている機能を開発する場合はどのように対処しますか？
next-devから機能追加ブランチを作成して機異能追加後next-devへマージをする
リリース時にnext-devからdevelop、developからproductionへマージしてデプロイする

1. `develop`と`next-dev`で Conflict を極力減らすために何が必要ですか？
定期的にdevelopからnext-devへのマージを行いファイル構成等の乖離が出すぎないように管理する


## 提出方法

`main`ブランチから、作業ブランチを切って、`main`に PR を提出してください。

ブランチ名は`社員コード_exam`としてください。

また、提出データ確認を簡単にするために、PR 作成時のタイトルに`社員コード`を入れてください。

[サンプル](https://github.com/KDW-DevDiv/git-starter-practice/pull/43)

## チェック担当者

Filter を設定してあります。

[こちら](https://github.com/KDW-DevDiv/git-starter-practice/pulls?q=is%3Apr+is%3Aopen+base%3Amain)からご確認ください。
