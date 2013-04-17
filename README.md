基礎演習手順書
==============

統合開発環境と Git による Web ページ開発
----------------------------------------

HTML の書き方
現在 HTML 5 という規格が策定されている最中で,
主要な Web ブラウザはそれに対応しているものが殆どであるため HTML 5 を前提に演習を行う.

### HTML5
先ず、HTML 5 のテンプレートについて触れる.


> ### 演習 1. HTML5 のテンプレートから HTML ファイルを作成表示の確認を行う.
> [HTML5 テンプレート](template/html5.html "test")

HTML 5 では、ファイルの先頭の記述が
``
<!DOCTYPE html>
``
に変わっている事に注意する事.
また、使用する文字のエンコーディングの指定は
``
<meta charset="utf-8" />
``
に変更されている事にも注意する.


> ### 演習 2. CSS の初期化を行う
> 演習 1 で作成したファイルに CSS 読み込みの記述を行う事.
> 尚, 以降の演習での編集ファイルは全て同じものを指す.
>
> [CSS 初期化ファイル](template/initialize.css)

``<link>`` タグでは外部ファイルから CSS を読み込む事が出来る.
CSS は, ブラウザ毎に仕様と設定が異なる為, 予期しない動作を引き起こす事
がある. その為, あらかじめ設定を初期化して置く事で予期しないレイアウト
になる事を防ぐ事が出来る.


> ### 演習 3. Twitter Bootstrap の読み込みを行う.
> Bootstrap のダウンロードを行なう.
> ファイルは zip 形式で圧縮されている為, 伸長を行い, 適切な場所にファイルを配置する.
> ファイルを配出来たなら, ``css/bootstrap.min.css``, ``bootstrap.min.js``
> の両ファイルを読み込む事.
> 下記リンクは Twitter Bootstrap の Official Page である.
>
> [Twitter Bootstrap](http://twitter.github.io/bootstrap/index.html)

Twitter Bootstrap を読み込む為のテンプレートは Official Page の HTML
template という項目にサンプルが存在する為, 読み込み方がわからない場合
は参照する事.


> 演習 4. メニューバーの作成
> Bootstrap を使用し, メニューバーを作成する.
> ``css/bootstrap.min.css`` の他に ``css/bootstrap-responsive.css`` を
> 読み込む. ただし, 読み込む順番は ``bootstrap-responsive.css`` を後に
> する.
>
> 読み込みの記述後 [ナビゲーションバー作成サンプル](template/navbar.html) を参考にナビゲーションバーを作成する.

ナビゲーションバーとは, ユーザーがサイトを巡回する際に,
コンテンツ毎のアクセスをナビゲートする機能である.
複数ページから出来ているサイトの場合はリンクを記述する事が多い.

演習 4 にて初めて body 部分の記述を行ったが, 今回の記述で Twitter
Bootstrap によるレイアウトを行う為には class を使用する事が分かる. 
その他のページを構成する書式は HTML のままで良い.
また, 複数の class を組み合わせる事で実装出来るレイアウトもある.

class に Twitter Bootstrap によって決められた属性を割りあてる
事で任意のレイアウトを実装出来るので実際にナビゲーションバーの class
属性を削除, 変更して変化を見て置くと理解し易い為推奨する.
