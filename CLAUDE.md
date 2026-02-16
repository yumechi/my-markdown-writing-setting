# My Markdown Writing Setting

このプロジェクトは、ブログ記事などのMarkdown記事の下書き用設定をまとめたリポジトリです。

## 構成

- `work/` ディレクトリ内に記事を執筆
- `mise` を使用した環境構成管理
- `textlint` による日本語記事の校正
- `prh` による表記ゆれチェック

## セットアップ

```bash
# mise による Node.js と pnpm のインストール
mise install

# 依存関係のインストール
pnpm install
```

## 使用方法

### 記事作成
`work/` ディレクトリ内に Markdown ファイルを作成して執筆します。

### 校正チェック
```bash
# 全ての記事をチェック
pnpm textlint work/

# 特定のファイルをチェック
pnpm textlint work/your-article.md
```

## 使用ツール

### 環境管理
- **mise**: Node.js と pnpm のバージョン管理

### 校正ツール
- **textlint**: 日本語記事の校正
  - `textlint-rule-preset-japanese`: 日本語の基本的な文章ルール（句読点、文体の統一など）
  - `textlint-rule-preset-ja-spacing`: 日本語の文字間隔をチェック
  - `textlint-rule-preset-ja-technical-writing`: 技術文書向けのルール
  - `textlint-rule-preset-ai-writing`: AI 生成文章の検出ルール
  - `textlint-rule-preset-jtf-style`: JTF（日本翻訳連盟）のスタイルガイド
  - `textlint-rule-prh`: 表記ゆれをチェック
  - `textlint-rule-spellcheck-tech-word`: 技術用語のスペルチェック

### 表記ゆれ設定
`prh.yml` で独自の表記ゆれルールを定義しています。