## markdown から pdf を生成する
個々人で使っているエディタは異なると思いますが、ここでは VS Code を用いて markdown から pdf (jpeg, html, ...) を生成する方法を備忘録として残しておきます。

#### 実行環境
- Windows
- Visual Studio Code

#### 生成手順
1. プラグイン "Markdown Preview Enhanced" をインストール
2. .md ファイルを開いた状態で Ctrl+K → V でプレビューを表示
3. プレビュー上で右クリック → Chrome(Puppeteer) → PDF により生成

※PDF(prince) という如何にもなコマンドがあるのですが、princexml をダウンロードしてきて Path を通してもうまくいかないみたいなので非推奨

#### 関連リンク
- pdf に改ページを作成
https://qiita.com/0xmks/items/4fec4116bb42120f5180

- VS Code で markdown 環境を整える
https://qiita.com/kumapo0313/items/a59df3d74a7eaaaf3137


