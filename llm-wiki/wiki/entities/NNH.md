---
tags: [實體, 統計指標]
created: 2026-07-22
updated: 2026-07-22
sources: [wiki/sources/2026-07-22-04-statistical_insights_myths.md, wiki/sources/2026-07-22-05-benefit_risk_discussion_nnt_nnh.md]
entity_type: 統計指標
mentions: 2
---

# NNH

> Number Needed to Harm，需傷害人數：要處方多少人才會多出一件不良事件，是把相對風險翻譯成診間語言的另一半。

## 定義與定位
NNH 解決的問題是「相對風險上升聽起來很嚇人，但實際上多少人會被傷到」。它與 [[NNT]] 共用同一個換算邏輯（1/絕對風險差），因此也共享同樣的陷阱：綁定時間、綁定基線風險、常常省略信賴區間。誤用的兩個典型情境是——把不同試驗的 NNH 直接並列當成療效比較，以及在比例風險假設失效時仍照算不誤（此時 [[NNT]] 可能翻成負值，形式上等於 NNH，但意義並非「藥物開始有害」）。

## 不同素材中的觀點

### 來自 [[2026-07-22-04-statistical_insights_myths]]
在 FIDELITY stage 4 CKD 亞群（890 人，占 7%）的腎臟複合終點上，NNT 於第 3 年變成 −40、第 4 年 −20，負值即 NNH，代表方向翻轉。原稿明言正確的反應不是宣稱「finerenone 後來有害」，而是認識到這是比例風險假設失效加上競爭死亡共同造成的產物——在這種情況下，單一 NNT 本來就不該被計算。

### 來自 [[2026-07-22-05-benefit_risk_discussion_nnt_nnh]]
NNH 被定位為相對尺度與絕對尺度之間的翻譯橋。FIDELIO-DKD 的數字是：約需處方 71 名 finerenone 才有 1 名因高血鉀永久停藥。這個 71 用來對照已被放棄的雙重 RAS 阻斷策略——VA NEPHRON-D 18、ALTITUDE 45、ORIENT 26，傷害門檻寬約 4 倍。素材同時聲明跨試驗換算各屬其原始族群、設計與終點定義不同，並列僅作量級對照，屬 🟡 可外推。

## 關鍵數字
- FIDELIO-DKD 高血鉀永久停藥 NNH：約 71
- 對照：VA NEPHRON-D 18、ALTITUDE 45、ORIENT 26（傷害門檻寬約 4 倍）
- FIDELITY stage 4 CKD 亞群：890 人，占 7%
- 該亞群腎臟複合 NNT：第 3 年 −40、第 4 年 −20（負值即 NNH）

## 相關頁面
- [[NNT]]
- [[ITT 分析]]
- [[高血鉀]]
- [[FIDELITY]]
- [[比例風險假設]]
