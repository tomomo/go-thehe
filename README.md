# GO-THERE

Go言語の実験環境

## 構築
### ツール
- [Docker Desktop](https://www.docker.com/products/docker-desktop/)
- [Visual Studio Code](https://azure.microsoft.com/ja-jp/products/visual-studio-code/)
  - [リモート系extention](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack)
### 使い方
- `Reopen in Container`をクリック。
- Webサーバーを起動。
  ```bash
  air -c .air.toml
  ```
- http://localhost へアクセス。
