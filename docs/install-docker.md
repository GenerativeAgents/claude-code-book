# Dockerのインストール方法

Dockerは、コンテナ技術を利用してアプリケーションの開発・実行環境を構築するためのツールです。本書ではDev Containerを利用するためにDockerが必要です。

## Docker Desktop

Windows、macOSでは「Docker Desktop」をインストールします。Docker Desktopには、Docker Engine、Docker CLI、Docker Composeなどが含まれています。

<https://www.docker.com/products/docker-desktop/>

※ Docker Desktopは個人利用・教育目的・小規模事業者は無償ですが、大企業等での商用利用は有償プランが必要な場合があります。詳細は[Docker公式のライセンス情報](https://www.docker.com/pricing/)を確認してください。

## インストール手順

### Windows

#### システム要件

詳細は公式ドキュメントを参照してください。

<https://docs.docker.com/desktop/setup/install/windows-install/>

#### WSL 2の有効化

Docker Desktopは通常WSL 2バックエンド（推奨）を使用します。WSL 2が未設定の場合は、以下の手順で有効化してください。

1. PowerShellを管理者として実行します
2. 以下のコマンドを実行します：

```powershell
wsl --install
```

3. PCを再起動します

#### Docker Desktopのインストール

1. [公式サイト](https://www.docker.com/products/docker-desktop/)からインストーラーをダウンロードします
2. ダウンロードしたインストーラーを実行します
3. インストールウィザードの指示に従います
4. 「Use WSL 2 instead of Hyper-V」オプションが選択されていることを確認します
5. インストールが完了したら、PCを再起動します
6. Docker Desktopを起動し、サービス規約に同意します

### macOS

#### システム要件

詳細は公式ドキュメントを参照してください。

<https://docs.docker.com/desktop/setup/install/mac-install/>

#### インストール手順

1. [公式サイト](https://www.docker.com/products/docker-desktop/)からインストーラーをダウンロードします
2. ダウンロードしたファイルを開きます
3. DockerアイコンをApplicationsフォルダにドラッグ＆ドロップします
4. アプリケーションフォルダから「Docker」を起動します
5. 初回起動時にシステムパスワードの入力を求められる場合があります
6. サービス規約に同意します
7. メニューバーにDockerアイコン（クジラのマーク）が表示されれば起動完了です

## インストールの確認

ターミナル（コマンドプロンプト）で以下のコマンドを実行し、バージョンが表示されればインストール成功です。

```bash
docker --version
```

さらに、以下のコマンドでDockerが正しく動作することを確認できます。

```bash
docker run hello-world
```

「Hello from Docker!」というメッセージが表示されれば、Dockerが正常に動作しています。

## 参考リンク

- [Docker公式サイト](https://www.docker.com/)
- [Docker Desktop公式ドキュメント](https://docs.docker.com/desktop/)
