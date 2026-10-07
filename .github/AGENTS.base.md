# 組織共通ルール（AGENTS.base.md）

このファイルは `github-settings-as-code` から Terraform で全リポジトリに配布している。
直接編集しないこと。変更は `github-settings-as-code` への PR で行う。
リポジトリ固有の指示は、このファイルではなく各リポジトリの `AGENTS.md` に書く。

## リポジトリ設定

- ブランチ保護、マージ方式、ラベル、Dependabot は Terraform で管理している。GitHub の UI で変更しない。
- マージは squash のみ。マージ後のブランチは自動削除される。

## コミットと PR

- コミットメッセージは Conventional Commits（`feat:` `fix:` `chore:` など）に従う。
- `Co-Authored-By:` 行や生成ツールの署名は付けない。
- PR 本文に社外ツールの issue 番号や URL を書かない。

## 秘密情報

- トークン、鍵、`.tfstate`、`.tfvars` をコミットしない。
- コミットの author には GitHub の noreply アドレスを使う。
