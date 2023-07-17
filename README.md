# README

## 環境構築
```
$ bundle install --without=production
$ bin/rails db:setup
$ yarn install
$ bin/webpack
$ bin/rails s
```

## 事業をエンジニアリングしよう提案編の回答は以下に記述してください
```
選択した事業側の課題
サービス登録者数の内、男性60%に対して、女性は40%。一方で、サービス内のもくもく会に参加した人の比率は、男性90%：女性10%と大きな差が出ています。もっと女性が使いやすいようなサービス設計にする必要があるのではないか？

提案内容
もくもく会に性別のタグ(女子会)を設定 & 絞り込みができるようにする
→ 女性の参加率の低さから、『参加前に同性の女性が少なく、もくもく会に参加しても居場所がないかもしれない』と思うのではないかと考えられる。女性が参加しやすいように女性専用のもくもく会を開催できるような仕組みを作る。

実装方針
もくもく会の作成時にタグ(女子会)を指定できるようにする。プルダブで選択できるようにする。
ヘッダーにある検索フォームにタグの条件を追加する。その際セレクトボックスにする。
もくもく会一覧画面において、各イベントに付与されているタグ(女子会)をタップするとそのタグで絞り込みが行われるようにする。
タグ(女子会)が付与されているもくもく会については、バリデーションで女性のユーザーしか参加できないようにする。
```