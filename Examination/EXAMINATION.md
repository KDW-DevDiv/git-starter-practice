# KDW が採用する Git Flow に関するテスト

`production`、`develop`、`next-dev`等の文言を使用し、回答ください。

1. リリースしている製品で緊急度の高いバグが発生した場合はどのように対処しますか？

A.
①prductionから緊急修正用のブランチ(A)を切って修正し、productionにマージする。
②(A)のブランチをdevelopにマージする。

2. リリースしている製品で緊急度の低いバグが発生した場合はどのように対処しますか？

A.
①developからブランチを切って修正し、developにマージ。
②修正が反映されたdevelopをproductionにマージ。

3. Version Up などで予定されている機能を開発する場合はどのように対処しますか？

A.
①バージョンアップ直後のdevelopからnext-devブランチを切る。
②next-devで次のバージョンアップ用の修正を入れていく。
③バージョンアップのタイミングで、next-dev→develop、develop→productionへとマージしてリリースする。

4. `develop`と`next-dev`で Conflict を極力減らすために何が必要ですか？

A.
developでの修正を、管理者が定期的にnext-devへ反映させていく。
そうすることで、バージョンアップ時にnext-dev→developへマージする際の競合が起きにくくなる。

## 提出方法

`main`ブランチから、作業ブランチを切って、`main`に PR を提出してください。

ブランチ名は`社員コード_exam`としてください。

また、提出データ確認を簡単にするために、PR 作成時のタイトルに`社員コード`を入れてください。

[サンプル](https://github.com/KDW-DevDiv/git-starter-practice/pull/43)

## チェック担当者

Filter を設定してあります。

[こちら](https://github.com/KDW-DevDiv/git-starter-practice/pulls?q=is%3Apr+is%3Aopen+base%3Amain)からご確認ください。
