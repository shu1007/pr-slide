---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://source.unsplash.com/collection/94734566/1920x1080
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# some information about the slides, markdown enabled
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
---

# 自己紹介

## 成ヶ澤 秀

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 p-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Press Space for next page <carbon:arrow-right class="inline"/>
  </span>
</div>

<a href="https://sli.dev/" target="_blank" alt="slidev"
  class="abs-br m-6 text-xl icon-btn opacity-50 !border-none !hover:text-white">
created by Slidev
</a>

---

# 略歴

- 1991 年 10 月 7 日、北海道生まれ
- 2014 年3月北見工業大学情報システム工学科卒
- 2017 年3月北海道大学理学院数学専攻修士課程を修了
- 同年インタープリズム株式会社入社
- 現在に至る


<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---

# スキル

## プログラミング言語

Java, C#, PHP, JavaScript, TypeScript, Powershell, Bash

## DB

SQL Server, MySQL

## FW

.NET, ASP.NET, Laravel, D3.js, Vue.js React, Next.js... etc


***直近はNext.jsでPHP製のWebサービスの共通化、リプレースを担当***

---

# どんなコードを書くのか?

業務以外にブラウザの拡張機能や Slack, discord の bot など同僚や同じ仕事をしている人に少し楽になるようなものを目指していくつかコードを書いてきました。いくつかを紹介します。

- レビュー依頼用 Slack アプリ
- 社内チャットでシンタックスハイライト表示ができるようになる chrome 拡張
- discord の voice channel で話した人を text channel に記録する bot

---

# レビュー依頼用 Slack アプリ

使っていたプロジェクト管理アプリケーションで複数プロジェクトをまたいで管理することがあまり向いておらず、レビュー依頼を Slack に集約。リンクを書いてお願いする運用。
しかし依頼が貯まると依頼されたものがわからなくなった。

<div grid="~ cols-2 gap-4">
<img src="/public/slack_bot2.png" width='350'/>
<div>
        任意のチャンネルでslash commandで左のイメージのようにモーダルが出現。

        タイトル、内容、通知したい相手を選んで送る。

        するとチャンネルに入力した内容でメッセージが送信され、メンションされるのでレビュアーはレビューされたことが認識出来ます。
</div>
</div>

---

# レビュー依頼用 Slack アプリ

<div grid="~ cols-2 gap-4">
<div>
appの画面からレビュー依頼したもの、されたものが表示され、されたものはOK、NGを出せる。

依頼したレビューに OK か NG かまだ見ていないという状態も同画面で確認でき、OK や NG が出されたときには同時に通知の DM がアプリからくる。

</div>
<video controls autoplay='true' muted='true' loop='true' width='600'>
    <source src="/public/slack_bot.mp4" type="video/mp4">
</video>
</div>
<a href="https://github.com/shu1007/request-review-slack-bot" target="_blank" alt="GitHub"
  class="abs-br m-6 text-xl icon-btn opacity-50 !border-none !hover:text-white">
<carbon-logo-github />
</a>

---

# 社内チャット用 Chrome 拡張

関連会社製のチャットツールが社内で使用されており業務のメッセージのやり取りにも使われている。<br/>
Slack 等になれていると少し辛いが、チームで使用している人もいるのでちょっとでも便利に使えるようにシンタックスハイライトができる chrome 拡張を作りました。

<div grid="~ cols-2 gap-2" m="-t-2">

<div>Before</div>
<div>After</div>

<img border="rounded" src="/public/sg_before.png">

<img border="rounded" src="/public/sg_after.png">
</div>
<a href="https://github.com/shu1007/sg-code-highlighter" target="_blank" alt="GitHub"
  class="abs-br m-6 text-xl icon-btn opacity-50 !border-none !hover:text-white">
<carbon-logo-github />
</a>

---


# discord bot

discord を普段の連絡で使用しており、voice channel にちょっとした離席時に誰かが話しかけてきた場合、それに気づくことができません。そこで以下のようなbotを作りました。

- text channel に voice channel を登録
- その voice channel で誰かが mic の mute を ON にした場合に text channel に通知を送る


<style>
video {
margin: 0 auto;
}
</style>

<video controls autoplay='true' muted='true' loop='true' width='500'>
    <source src="/public/discord-bot.mp4" type="video/mp4">
</video>

<a href="https://github.com/shu1007/discord-speaker-log" target="_blank" alt="GitHub"
  class="abs-br m-6 text-xl icon-btn opacity-50 !border-none !hover:text-white">
<carbon-logo-github />
</a>
---

# その他

- 社内の技術ブログに寄稿
    - http://interprism.hatenablog.com/entry/2021/05/14/094339
- ハッカソンに参加
    - 2019年10月5日にサポーターズCoLabさん主催のビアッカソンというハッカソンイベントに参加
    - 良いメンバーと出会えて優勝出来た
    - https://note.com/spzcolab/n/n1ef7ae944fe0
- OSS活動
    - PHP製のSQLパーサーがコメントありのパースしたものからSQLが生成出来ないため、コメントを除くオプションを追加
    - 放置されている。。。
    - https://github.com/greenlion/PHP-SQL-Parser/pull/330

---

-