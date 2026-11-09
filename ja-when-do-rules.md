---
title: "オートバトラーの行動設計：WHEN→DOルールとプリセットの使い分け（Boss Lab）"
layout: default
---

# オートバトラーの行動設計：WHEN→DOルールとプリセットの使い分け（Boss Lab）

Boss Lab: Robot Battle Builder では、戦闘そのものは自動ですが、マシンの「優先順位」はプレイヤーが決めます。本稿は、Hunter / Counterstrike / Berserker のプリセットと、その下に重ねる最大3本の WHEN→DO ルールを、開発・理論構築の両面から整理します。

*開示：筆者は Boss Lab Studio の開発メンバーです。アートとオーディオはAI支援、デザイン・コード・バランスはチーム制作です。*

## プリセットは「足場」、ルールは「例外処理」

| レイヤ | 役割 | 失敗しやすい使い方 |
|---|---|---|
| パーツ構成 | 射程・耐久・熱・重量 | 役割が矛盾する混装 |
| ブレインプリセット | デフォルトの距離感・攻撃性 | 射程と性格が噛み合わない |
| WHEN→DO（最大3） | 特定状況の上書き | 広い条件を先に置いて狭い条件を殺す |

ルールは移動・武器・ユーティリティ・防御それぞれで「最初に条件を満たしたもの」が勝ちます。だから **具体→広い** の順が基本です。

## 実験プロトコル（安く学ぶ）

1. パーツを固定したまま、ブレインだけ変えて同じ相手と戦う  
2. 勝敗画面だけでなく、射程内にいた時間・旋回・支援の発動を見る  
3. それでも直らないときだけルールを1本足す  
4. Scrap でレベルを上げるのは最後  

レベルは有効なアタッチメントの耐久・ダメージを上げますが、移動優先度は書き換えません。「怒って突っ込んで負ける」Berserker は、火力不足ではなく距離設計の問題であることが多いです。

## プロダクト前提（再掲）

- Android のみ・接続必須・無料＋IAP  
- 60+パーツ、20地区・100ボス、非同期Arena  
- レベルエディタ／UGCなし、Phaser製、2026年公開  

## FAQ

**Q. 生成AIで行動を学習しますか？** A. しません。プリセットとルールです。  
**Q. Gladiabotsと同じ？** A. 粒度が違います。Boss Labは少数ルール＋プリセットに閉じた設計です。  
**Q. オフラインは？** A. 不可。

詳細: [brain-presets](https://www.bosslab.xyz/blog/brain-presets?utm_source=github_pages_asia&utm_campaign=sprint_when-do-brain-rules-ja)  
サイト: [bosslab.xyz](https://www.bosslab.xyz/?utm_source=github_pages_asia&utm_campaign=sprint_when-do-brain-rules-ja)  
Play: [Boss Lab](https://play.google.com/store/apps/details?id=com.bosslab.game&utm_source=github_pages_asia&utm_campaign=sprint_when-do-brain-rules-ja)
