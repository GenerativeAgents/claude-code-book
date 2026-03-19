# 実践Claude Code入門―現場で活用するためのAIコーディングの思考法

「実践Claude Code入門―現場で活用するためのAIコーディングの思考法」のGitHubリポジトリです。

<https://www.amazon.co.jp/dp/4297153548>

<img src="assets/cover.jpg" width="50%" />

## インストールガイド

ハンズオンを始める前に、以下のツールをインストールしてください。

- [Visual Studio Code](docs/install-vscode.md)
- [Docker](docs/install-docker.md)
- [Dev Containers拡張機能](docs/install-devcontainer.md)

## ハンズオンで使用するGitHubリポジトリ

本書のハンズオンで使用するGitHubリポジトリは、以下の2つです。

- 第1部2章のハンズオン：<https://github.com/GenerativeAgents/claude-code-book-template>
- 第1部4章のハンズオン：<https://github.com/GenerativeAgents/claude-code-book-chapter4>
- 第2部8章のハンズオン：<https://github.com/GenerativeAgents/claude-code-book-chapter8>

## 既知のエラー

### Claude Code Actionのリポジトリのアップデートに起因するエラー

書籍p128「Issueトリアージのカスタムスラッシュコマンドの作成」では、Claude Code Actionが公開している`label-issue.md`ファイルをコピーして使用します。

Claude Code Actionのリポジトリのアップデートにより、最新の`label-issue.md`ファイルを使用すると、追加の設定手順が必要となりました。

書籍の通りの手順で動かす場合は、以下の本書執筆時点の`label-issue.md`ファイルを使用してください。

<https://github.com/anthropics/claude-code-action/blob/69dec299f882fef0fff1652a1309b7e9771b9f98/.claude/commands/label-issue.md>

最新の[`label-issue.md`ファイル](https://github.com/anthropics/claude-code-action/blob/main/.claude/commands/label-issue.md)を使用する場合は、ファイルの内容を確認して必要なスクリプトを配置するなどの対応を実施してください。

## 書籍の誤り・エラーについて

書籍の誤り（誤字など）や、発生したエラーについては、GitHubのIssueからご連絡ください。

<https://github.com/GenerativeAgents/claude-code-book/issues>

## 正誤表

- [正誤表](./errata.md)

## リンク

- [技術評論社](https://gihyo.jp/book/2026/978-4-297-15354-0)
- [Amazon](https://www.amazon.co.jp/dp/4297153548)
