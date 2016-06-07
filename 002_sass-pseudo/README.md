# ブートキャンプ \#2

## テーマ

- 擬似要素について。

## 環境まわり

#### 前提

- node, npmはインストール済み。
  - versionはstable推奨。

#### パッケージインストール

- node-sassが必要。
- package.jsonがあるので、npm i でOK


# シラバス

- 今回のブートキャンプのテーマの発端となったスライド。
  - [プログラム組んだら負け！実はHTML/CSSだけでできること2015夏](http://www.slideshare.net/yusukehirao/htmlcss2015)

## ハンズオン

1. $ npm install
2. $ npm run watch:css
3. ./index.htmlをブラウザで開く。
4. ./src/stylesheets/main.scssに追記していく。

### \#1. 単純な擬似要素

- 消化済タスクにafter要素を使って、×マークを付与。
- 参考：[css脱初心者？ :before :after擬似要素の使い方とか基本的なこと](http://qiita.com/aquamikan/items/cfa53c3b5d6ae1502180)
  - ※インライン要素への擬似要素はインライン属性となり、ブロックレベル要素への擬似要素はブロックレベル属性となる。

### \#2. Newラベル

- 擬似要素自体に、複雑なスタイルを充ててみる。

### \#3. hoverライク

- hoverした時(マウスカーソルがあたった時)に、擬似要素を出現させる。

### \#4. hoverスライドアップ

- 擬似要素だけで、スライドアップを実現する。

## まとめ

- 適材適所で擬似要素を使うことで無駄なスクリプトが減らせるかもしれない。
- 構造とスタイルを分離できるかもしれない。


### 参考文献

- カンタンなSass環境の構築についてはこちら。
  - [npmでミニマムに始めるSass](http://qiita.com/micchyboy/items/0074f002d8f1663577a2)
  - 上記の記事では、sassのwatchコンパイルにnodemonパッケージが必要とあるが、実は不要。以下参照。
    - [Sass(sccs) のコンパイルは node-sass がRuby不要でシンプルかつ高速！](http://celtislab.net/archives/20160302/node-sass-cl/)
- content内で複雑なことをしたい場合には。
  - [【CSS】beforeのcontentで改行する](http://mementoo.info/archives/665)
