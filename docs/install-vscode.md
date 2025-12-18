# Visual Studio Codeのインストール方法

Visual Studio Codeは、Microsoft社が提供するコードエディタです。

## ダウンロード

公式サイトからインストーラーをダウンロードします。

<https://code.visualstudio.com/>

お使いのOS（Windows / macOS）に合わせたインストーラーを選択してください。

## インストール手順

### Windows

1. ダウンロードしたインストーラーを実行します
2. インストールウィザードの指示に従ってインストールを完了します

### macOS

1. ダウンロードしたファイルを開き、「Visual Studio Code.app」を「アプリケーション」フォルダに移動します
2. アプリケーションフォルダから「Visual Studio Code」を起動します

## コマンドラインから起動できるようにする（推奨）

ターミナルから`code`コマンドでVisual Studio Codeを起動できるようにします。ターミナルで以下のコマンドを実行し、バージョンが表示されればすでに使用可能です。

```bash
code --version
```

`code`コマンドが使えない場合は、以下を試してください。

- ターミナルを一度閉じて開き直す
- Visual Studio Codeのコマンドパレット（`Ctrl + Shift + P` / `Cmd + Shift + P`）から「Shell Command: Install 'code' command in PATH」を実行する

## 参考リンク

- [Visual Studio Code公式サイト](https://code.visualstudio.com/)
- [Visual Studio Code公式ドキュメント](https://code.visualstudio.com/docs)
