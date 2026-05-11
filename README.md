# うちごはん

> **サボるほど、食卓が笑う。**
> 思考はAIに、味付けは愛で。

[![Hackathon](https://img.shields.io/badge/AWS%20Summit%20Japan-2026-orange)](https://aws.amazon.com/jp/summits/japan/)
[![Methodology](https://img.shields.io/badge/AI--DLC-Inception-blue)](https://zenn.dev/aws_japan/articles/aidlc-workflows)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Inception-lightgrey)]()

AWS Summit Japan 2026 AI-DLC ハッカソン提出物。  
共働き家庭の「今日何作ろう」を考えなくする献立AI。家族の冷蔵庫・仕事疲労・体調をリアルタイム統合し、親等モデルで親世帯・兄弟まで自然に拡張します。

---

## Why うちごはん

みなさん、子供との時間、もっと欲しくないですか？
家族との時間、両親との時間、作れていますか？
部下や先輩との時間、ちゃんと取れていますか？

家族との団欒は、プライスレス。
離れた両親を思いやれることは、親孝行。

これが、自動で集約できる「怠惰」なら ── 最高ですよね？

**うちごはん。サボるほど、食卓が笑う。**

---

## テーマ再解釈

本ハッカソンのテーマ「**人をダメにする**」を、私たちは「**サボらせる**」として再解釈しました。  
ダメにしていい部分（思考・選択・調整）と、ダメにしてはいけない部分（料理・食卓・愛情）を意図的に分けて設計します。

---

## なぜ「うちごはん」なのか ── 3つの価値の同時提供

身内が作る料理と、赤の他人が作る料理には、栄養価では測れない差があります。
"今日のあなた" を想って作られているか、否か。

しかし従来の家庭料理にも限界がありました：

- 作り手の "気分" や "得意料理" にメニューが固定化される
- 「今日の体調」までは考慮しきれない
- 新しいチャレンジには時間と気力が必要

ナッシュ等の冷凍宅配は、栄養を「過去の平均基準」で最適化します。
ただし「あなたの今日」には合っていません。そして何より、
"誰かのために作られた料理" ではありません。

うちごはんは、3つの価値を同時に提供します：

| 軸 | 内容 |
|---|---|
| **現在性** | 今日の体調・疲労・在庫をリアルタイム統合 |
| **愛情** | 作るのはあいかわらず家族。AIが引き受けるのは思考だけ |
| **チャレンジ** | 家庭の "いつもの味" に、新しいレシピの幅を持ち込む |

「考える疲れ」をAIに渡すと、作り手は新しい料理に挑戦する余裕が生まれる。
ナッシュが諦めたものを、うちごはんは諦めません。

---

## 設計思想：良い怠惰／悪い怠惰

```
┌─────────────────────────────────────────────────┐
│  AIに渡す（=良い怠惰）                            │
│  ・献立を考える、選ぶ、調整する                    │
│  ・在庫管理、栄養計算、買い物リスト生成            │
├─────────────────────────────────────────────────┤
│  人間に残す（=人をダメにしない）                   │
│  ・実際に作る、味見する、盛り付ける                │
│  ・食卓を囲む、話す、分かち合う                    │
└─────────────────────────────────────────────────┘
```

ナッシュ等の冷凍宅配は「料理」を代行します。
うちごはんは「考える疲れ」だけを代行します。
作る人が、家族のままでいられるように。

---

## ドキュメント

提出物の本体は [aidlc-docs/](aidlc-docs/) 配下にあります。

| ファイル | 内容 |
|---|---|
| [aidlc-docs/README.md](aidlc-docs/README.md) | サービス概要・設計思想・ファイル索引 |
| [aidlc-docs/01-requirements-analysis.md](aidlc-docs/01-requirements-analysis.md) | 要件分析（背景・課題・価値提案・成功指標） |
| [aidlc-docs/02-user-stories.md](aidlc-docs/02-user-stories.md) | ペルソナ3名 × ユーザーストーリー（ビフォー/アフター物語付き） |
| [aidlc-docs/03-application-design.md](aidlc-docs/03-application-design.md) | アプリケーション設計（LINE Bot軸・Tier構造・AI×Human境界） |
| [aidlc-docs/04-unit-decomposition.md](aidlc-docs/04-unit-decomposition.md) | Unit分解（10 Units、U10は意図的にAI比率0%） |
| [aidlc-docs/business-context.md](aidlc-docs/business-context.md) | ビジネス文脈（競合・収益モデル・API規約・リスク） |
| [PROJECT_BRIEF.md](PROJECT_BRIEF.md) | プロジェクト全体サマリ |
| [DECISIONS_AND_OPEN_QUESTIONS.md](DECISIONS_AND_OPEN_QUESTIONS.md) | 決定事項と未決事項のロックドキュメント |

---

## キャッチコピー体系

```
【メインキャッチ】 サボるほど、食卓が笑う。
【サブコピー】    思考はAIに、味付けは愛で。
【設計思想】      愛情を守る、良い怠惰。
```

---

## ハッカソン情報

- **イベント**：AWS Summit Japan 2026 AI-DLC ハッカソン
- **テーマ**：「人をダメにするサービスを考えよう」
- **メソドロジー**：AI-DLC（AI-Driven Development Life Cycle）
- **書類審査締切**：2026-05-10
- **予選**：2026-05-30（MVPデモ）
- **決勝**：2026-06-26（幕張メッセ）

---

## チーム

2名構成（IT企画 + エンジニア）

---

## ライセンス

[MIT License](LICENSE)
