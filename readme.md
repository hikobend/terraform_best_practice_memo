# 概要
このリポジトリはTerraformのペストプラクティスを自分なりにまとめたものです。

## ベストプラクティスをまとめようと思ったきっかけ
terraformは自由度が非常に高いです。ディレクトリ構成やリソースの書き方が開発者によってまちまちになることが考えられます。
そこで、ベストプラクティスに沿って書くことで可読性を得る狙いがあって今回まとめてみました。

## IaCのベストプラクティス
- 手動での変更をせず、バージョン管理を使用する
CI/CDワークフローを実装して、インフラの構成を実行する

## Terraformリポジトリを構築する
main.tf
variables.tf : 使用する変数を宣言する
readme.md : ディレクトリに対して、コードの説明を説明する
outputs.tf : プロジェクトの出力値を定義する
providers.tf : 構成するために使用したパージョンを管理する
terraform.tfvars : variable.tfで定義した変数を割り当てる

### module


## 参考文献
[standard module structure](https://developer.hashicorp.com/terraform/language/modules/develop/structure)
[20 Terraform Best Practices to Improve your TF workflow](https://spacelift.io/blog/terraform-best-practices)