# Dev Containers拡張機能のインストール方法

Dev Containersは、Visual Studio Codeの拡張機能で、Dockerコンテナ内で開発環境を構築・実行できます。本書のハンズオンでは、この拡張機能を使用して開発環境を構築します。

## 前提条件

Dev Containersを使用するには、以下がインストールされている必要があります。

- [Visual Studio Code](install-vscode.md)
- [Docker](install-docker.md)

## インストール手順

1. Visual Studio Codeを起動します
2. 左側のサイドバーで拡張機能アイコン（四角が4つ並んだアイコン）をクリックします
   - または、`Ctrl + Shift + X`（macOSは`Cmd + Shift + X`）を押します
3. 検索ボックスに「Dev Containers」と入力します
4. 「Dev Containers」（Microsoft製）を選択します
5. 「インストール」ボタンをクリックします

## Dev Containerで開発環境を開く

本書のハンズオン用リポジトリをDev Containerで開くには、以下の手順に従います。

1. リポジトリをクローンします

```bash
git clone https://github.com/GenerativeAgents/claude-code-book-template.git
```

2. Visual Studio Codeでリポジトリを開きます

```bash
cd claude-code-book-template
code .
```

3. Visual Studio Codeがリポジトリ内の`.devcontainer/devcontainer.json`を検出し、「Reopen in Container」（コンテナで再度開く）という通知が表示されます
4. 通知をクリックするか、コマンドパレットから「Dev Containers: Reopen in Container」を実行します
5. 初回起動時はコンテナのビルドに数分かかります。完了すると、コンテナ内の開発環境でVisual Studio Codeが開きます

## トラブルシューティング

### Dockerが起動していない場合

「Cannot connect to the Docker daemon」というエラーが表示される場合は、Docker Desktopが起動しているか確認してください。

### コンテナのビルドに失敗する場合

1. Docker Desktopに十分なリソース（メモリ、CPU）が割り当てられているか確認してください
2. コマンドパレットから「Dev Containers: Rebuild Container」を実行して、再ビルドを試みてください

## 参考リンク

- [Dev Containers拡張機能（Visual Studio Marketplace）](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)
- [Dev Containers公式ドキュメント](https://code.visualstudio.com/docs/devcontainers/containers)
