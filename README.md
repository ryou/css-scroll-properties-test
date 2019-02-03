# 最近のスクロール関係のCSSプロパティのテスト

[Demo(Firebase)](https://vue-test-bfb52.firebaseapp.com/)

PWA対応しているので、ホーム画面に登録でPWA時の動作を確認可能（iOSは試していないのでわからない）

## scroll-snap

CSSだけでスライダーが作れるやつ。

何が良いかというと、ピンチイン/ピンチアウトが可能。JSでこれをやろうとするとめちゃくちゃ面倒。

## overscroll-behavior

[「端っこ」におけるスクロールの挙動を制御する overscroll-behavior プロパティ | ダーシマ・ヱンヂニヤリング](https://necomesi.jp/blog/tsmd/posts/180)

上記記事の通り、Androidの`pull to refresh`の抑制や、前面に出てくる要素がスクロール仕切った後更に背面の要素がスクロールしてしまう挙動を抑制出来る。
