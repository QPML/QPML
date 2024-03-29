# QPML: Quick Prototyping Markup Language

QPMLはより手軽に、より高速にプロトタイプの作成をサポートするフレームワーク/ライブラリです。

## 基本機能(草案)

- [Twitter Boostrap](http://twitter.github.com/bootstrap/)にあるUI群をモジュールとして実装
- [Stylus](http://learnboost.github.com/stylus/)を利用
- [Components](http://tjholowaychuk.com/post/27984551477/components)ライクな構造とモジュール群の管理、拡張
- [StyleDocco](http://jacobrask.github.com/styledocco/)を利用してスタイルガイドを作成、プロトタイプライブラリページとする

## ディレクトリ/ファイル構成

画像、スタイル、スクリプトなど:

```text
assets/
	fonts/ @font-face
		icons/ @font-faceアイコン
	images/ 画像
		sprites/ スプライト用画像
		datauris/ DataURI変換前画像
		textures/ テクスチャ画像
	scripts/ JavaScript
	styles/ スタイルシート(stylus)
		base/ デフォルト用スタイル
		layout/ レイアウト用スタイル
		modules/ モジュール用スタイル
		presentation/ 表層用スタイル
		master.styl マスタースタイル @import用
```

Jade:

```text
includes/ インクルード用
	layouts/ レイアウト用
	modules/ モジュール用(ボタン、ナビなど)
	systems/ システム用(ヘッダ、</body>前)
index.jade マスターファイル
```

その他:

```text
docs/ スタイルガイド用(StyleDocco)
package.json Grunt.jsなどnode.jsパッケージ用メタファイル
Gruntfile.js Grunt.js用ファイル(0.4.x系)
config.json Jadeが読み込む設定ファイル
.gitignore git用
readme.md 本ファイル
```

## マイルストーン

- 0.0.x: 仕様概要策定
- 0.1.x: 公開ブランチのディレクトリ/ファイル構成策定
- 0.5.x: プロジェクトホームページのプロトタイプを本ツールで作成
- 0.8.x: クローズドベータ公開
- 0.9.x: リファクタリング
- 1.0.0rc: パブリックベータ公開
