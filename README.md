# my-markdown-writing-setting
## 概要

markdown の Linter 系の設定を自分用にまとめたもの。

## 参考

* [textlint と VS Code で始める文章校正 - Qiita](https://qiita.com/takasp/items/22f7f72b691fda30aea2)
* [textlint-ja/textlint-rule-preset-ja-technical-writing： 技術文書向けのtextlintルールプリセット](https://github.com/textlint-ja/textlint-rule-preset-ja-technical-writing)

## Dependabot Configuration

このリポジトリでは Dependabot を使用して依存関係を管理しています。Dependabot は毎週金曜日の21:00 JSTに更新をチェックするように設定されています。

### パッケージエコシステム

- **npm**
- **pnpm**

### ディレクトリ

Dependabot はリポジトリのルートディレクトリをチェックするように設定されています。

## GitHub Actions

このリポジトリでは、Dependabot からのプルリクエストを自動的にマージするための GitHub Actions ワークフローを使用しています。新しいワークフローは `auto-merge-dependabot.yml` というファイルに記述されています。
