# search_app
YouTube検索補助アプリ

### 概要

「バレエ動画視聴が止まらなくなるアプリ」

### 背景

バレエ好きの方はよくYouTubeで検索して動画を観ます。

ただ主に海外のものなので、日本語より外国語で検索したほうがよりヒットします。
その事実を知らない人がほとんど＆バレエ用語は癖が強いのでスペルを覚えづらい！

### 課題

- 日本語より外国語のほうがヒットするが、都度用語を調べて検索するのが面倒。
- ロシア語、フランス語などで検索したいケースもある。

### 機能

- 日本人に親しみのある日本語のUIから、直接外国語でYouTube検索ができる。

### 

### モック

![https://i.gyazo.com/1865d3091b06511271b7499a49450124.gif](https://i.gyazo.com/1865d3091b06511271b7499a49450124.gif)

### イメージ

- とりあえずログイン機能なし
- `{ 日本語: 検索ワード }`の組み合わせデータをあらかじめ入れておく？
    - e.g`{ りんご: apple, バレエ: ballet, 眠りの森の美女: sleeping beauty }`
- ビューに表示されているのは日本語のリンクで、クリックするとその日本語に対応する検索ワードで検索された状態のYoutube検索結果画面に遷移する
- ビューでは絞り込み機能でデータを出し分ける（タブ、プルダウン）
    - 作品名、ダンサー名など
- カスタム検索機能（単語を自由に組み合わせて検索）

### 〜〜〜バックエンドがシンプル過ぎるという懸念〜〜〜
[追加要素]
- YouTubeのAPIを利用する
    - 自分のアプリ内に検索結果ごと表示させる（YouTubeアプリに飛ばさない）
    - 独自のレコメンド機能の追加（バレエ関連の動画しか出てこないようにする）

### 聞きたいこと

- スマホファーストについて
- YouTube APIを利用して、バレエ視聴に特化したミニYouTube的なものをアプリ内に作ってしまう選択肢
- 永続的なデータを持たないとは？ [https://developers.google.com/youtube/v3/getting-started?hl=ja#resources](https://developers.google.com/youtube/v3/getting-started?hl=ja#resources)
- SPA、PWA、Firebase（しょうちゃんさんのPF解説で紹介されていた）
- Vue.js、Reactが気になる（使ってみたい）
