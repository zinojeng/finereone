---
tags: [實體, 統計指標]
created: 2026-07-22
updated: 2026-07-22
sources: [wiki/sources/2026-07-22-04-statistical_insights_myths.md]
entity_type: 統計指標
mentions: 1
---

# ITT 分析

> Intention-to-treat：依隨機分派而非實際用藥情形分析，是保住隨機化保護力的預設分析集。

## 定義與定位
ITT 分析解決的問題是選擇偏差：一旦分析只納入「有乖乖吃藥的人」，隨機化所建立的組間可比性就被打破。與之相對的 on-treatment（或 per-protocol）分析會排除停藥後的事件，看似排除了雜訊，實際上排除的往往是預後最差的一群人。誤用的典型情境是：作者強調 on-treatment 的顯著結果、把 ITT 的邊緣值當成「被稀釋的真相」——本知識庫的立場相反，on-treatment 比 ITT 漂亮時該警覺，而非慶祝。

## 不同素材中的觀點

### 來自 [[2026-07-22-04-statistical_insights_myths]]
以 Filippatos 2023 的死亡率分析為例：全因死亡 ITT HR 0.89（0.79–1.00，P=0.051），事件數 552 vs 614；on-treatment HR 0.82（0.70–0.96，P=0.014），事件數僅剩 280 vs 344。超過一半的死亡因發生在停藥 30 天後而被剔除，而停藥者（多因高血鉀、腎功能惡化而停）本身預後就較差，這正是 informative censoring 造成的選擇偏差。素材指出真正經得起考驗的是猝死終點，因為它在 ITT 分析中即已達顯著（HR 0.75，0.57–0.996，P=0.046）。

## 關鍵數字
- 全因死亡 ITT：HR 0.89（0.79–1.00），P=0.051；事件 552 vs 614
- 全因死亡 on-treatment：HR 0.82（0.70–0.96），P=0.014；事件 280 vs 344
- 猝死（ITT）：HR 0.75（0.57–0.996），P=0.046
- 停藥後 30 天為 on-treatment 的事件截尾窗

## 相關頁面
- [[NNT]]
- [[NNH]]
- [[FIDELITY]]
- [[比例風險假設]]
- [[競爭風險]]
