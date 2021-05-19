# es6-study-4-14-35
JavaScript 学習コース IV > クラスの継承 > オーバーライド（2）

### コンストラクタのオーバーライド
メソッドと同じように、コンストラクタもオーバーライドすることができる。
例えば、子クラスにプロパティを追加したい場合などに用いられる。
ただし、コンストラクタをオーバーライドする際は1行目に「super()」と記述する必要がある。
```
class 親クラス {
  constructor() {
  *******
  }
}
↓ オーバーライド ↓
class 子クラス extends 親クラス {
  constructor() {
  super()　/** 1行目にsuper()が必要
  子クラスのコンストラクタの処理
  }
}
```











## コーディングトレーニング
「ハウスM21」のレイアウト構造をレスポンシブで写経する。

#### サイト構造
- header > logo - nav/toggle
- main > section（p-index__mainVisual） - section（p-index__event） - section（p-index__news） - section（p-index__brand） - section（p-index__voice） - section（footer__own__wrap） - section（p-index__exhibition） - section（p-index__works）
- footer
- aside(※smartphoneのみ)

#### ブレイクポイント
- desktop（1200px ↑）
- tablet（1199px ↓）
- smartDevice（1023px ↓）

## チャレンジ
- ハンバーガーメニューに画像やSVGを使わずcssで描画する
- ヘッダーを上部固定にする
- スマホビューの時だけasideを表示し、ページ下部に固定する
