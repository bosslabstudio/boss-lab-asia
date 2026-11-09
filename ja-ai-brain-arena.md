---
title: "ロボットの「性格」を選ぶゲーム、知ってる？Boss LabのAIブレインとアリーナ雑記"
layout: default
---

# ロボットの「性格」を選ぶゲーム、知ってる？Boss LabのAIブレインとアリーナ雑記

最近ハマってる（というか作ってる）Androidゲームの話をゆるく書きます。タイトルは **Boss Lab: Robot Battle Builder**。ロボットのボスを60以上のパーツで組み立てて、AIの「脳みそ」を選んで、あとは自動で戦わせるタイプです。反射神経ゲーじゃないので、通勤のスキマとか夜のソファでも頭だけ使えます。

*開示：わたしは開発チーム Boss Lab Studio の一員です。絵と音はAIの力を借りていて、ゲームデザイン・コード・バランスは人間チームがやってます。*

## ブレイン3兄弟のイメージ

公式のブレイン解説を噛み砕くと、だいたいこんな感じ。

| 名前 | ひとことで | 合いやすい組み立て |
|---|---|---|
| Hunter | 追いかけて距離を詰める | 近接寄り |
| Counterstrike | 反応して間合いを取る | 遠距離寄り |
| Berserker | ダメージを食うほど怒る | 耐久と火力の両立 |

ポイントは、ブレインを変えても **武器の届く距離そのものは変わらない** こと。ノコギリ二刀流なのに Counterstrike で後退ばかり、みたいな噛み合わせミスは普通に起きるので、「パーツの仕事」と「性格」をセットで見るのがコツです。

上級者向けには WHEN→DO のルールを最大3本まで足せますが、最初はプリセットのままで十分です。強化にScrapを使う前に、ブレインだけ差し替えて同じ相手ともう一回見る——これが一番安い実験です。

## アリーナは「非同期」がうれしい

Boss Lab のアリーナはリアルタイムで相手を待つ必要がありません。自分のボスを公開しておけば、オフライン中でも他プレイヤーのボスが攻めてきます。こちらからも、公開されている相手に自分のタイミングで挑戦できます。

キャンペーンで育てた強化がそのまま有利、というわけではなく、アリーナではアタッチメントレベルが正規化されます。だから「コレクションの仕組み」と「相性」が相対的に効く。防衛ログを見て、痛い相手の射程やモジュール構成を読むのが楽しいポイントです。

## さくっとスペック

- 2026年・Android専用（iPhoneなし）・接続必須  
- 無料＋アプリ内課金  
- キャンペーン：20地区・100ボス  
- レベルエディタやユーザー投稿ステージはない（作るのはボス本体）  
- エンジンは Phaser  

似た系統で物理マシンが好きな人は CATS、行動を細かくプログラムしたい人は Gladiabots もチェックしてみてください（体験はそれぞれ違います）。

## FAQ

**ブレインって生成AI？** → ちがいます。行動プリセットです。  
**オフラインできる？** → できません。接続が必要です。  
**操作はするの？** → 戦闘は基本自動。組み立てとブレインがメイン。

もっとちゃんとした解説は公式へ：  
[Brain presets](https://www.bosslab.xyz/blog/brain-presets?utm_source=github_pages_asia&utm_campaign=sprint_brain-presets-arena-ja)  
[Arena guide](https://www.bosslab.xyz/blog/arena-guide?utm_source=github_pages_asia&utm_campaign=sprint_brain-presets-arena-ja)  
[公式サイト](https://www.bosslab.xyz/?utm_source=github_pages_asia&utm_campaign=sprint_brain-presets-arena-ja)  
[Google Play](https://play.google.com/store/apps/details?id=com.bosslab.game&utm_source=github_pages_asia&utm_campaign=sprint_brain-presets-arena-ja)
