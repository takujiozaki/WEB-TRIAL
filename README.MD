# WEB体験授業
## まず始めに
WEBに触れてみることを主眼においた体験レッスンです。  
PCはもちろん、iPadでも試していただけます。 

アプリケーションのインストールは不要です。
インターネットにつながっていれば利用いただけます。

## 環境
JSFIDDLEというWEBサービスを利用します。  
WEBブラウザを使ってWEBページやWEBアプリケーションを開発することが出来ます。

[JSFIDDLE](https://jsfiddle.net/)

![QRCode](jsfiddle.png)

## JSFIDDLEの基本的な使い方
左上がHTML、右上がCSS、左下がJavaScript記述するエリアになっています。
右下が結果を表示するプレビュー画面です。

変更をしたらRUN、保存をするにはSAVEをクリック(タップ)します。

## 基本のWEBページ
スタートのページを開いてみましょう。  
基本的な構成のWebページを作成しています。

[最初のページ](https://jsfiddle.net/ozhy9e7p/)

![QRCode](QR001.png)

## 画像を加えてみる
WEBページに画像を加えてみましょう。
創造社デザイン専門学校のロゴを加えてみる
```
<img src="https://www.sozosha.ac.jp/asset/images/common/logo.svg" alt="創造社デザイン専門学校">
```

Web専攻のイメージ画像を加えてみる
```
<div class="keyvisual">
  <img src="https://takujiozaki.com/opencanpus/webdesign.jpg" alt="">
</div>
```

## CSSを書いてみる
センターレイアウトにしてみる
HTML  
全体をDIVタグで覆う、覆うのでwrap(ラップ)という名前をよく使います。
```
<div class="wrapper">
  <!-- センターレイアウトにしたい項目を配置 -->
</div>
```
CSS  
marginとは外側の余白
```
.wrapper{
  width:80%;
  margin:0 auto;
}
```
見出しをセンター合わせに、TEXT-ALIGNはワープロの文字寄せと同じです。
```
h2{
  text-align:center;
}
```
見出しに装飾を加えてみる
```
h3{
  border-left:solid 3px blue;
  border-bottom:solid 1px blue;
  padding-left:2px;
}
```
箇条書きを横並びにする
```
ul>li{
  display:inline-block;
  margin-right:2em;
}
```
文字高さを設定して読みやすく
```
p{
  line-height:2em;
}
```
画像を画面内に収めてみよう
```
div.keyvisual img{
  max-width:100%;
}
```

## 完成ページ
[ここまでの完成ページ](https://jsfiddle.net/v5pwLtqz/3/)