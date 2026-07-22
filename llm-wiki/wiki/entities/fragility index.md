---
tags: [實體, 統計指標]
created: 2026-07-22
updated: 2026-07-22
sources: [wiki/sources/2026-07-22-04-statistical_insights_myths.md]
entity_type: 統計指標
mentions: 1
---

# fragility index

> 脆弱指數：問「要把多少個未發生事件的病人改成發生事件，顯著結果才會翻回不顯著」。

## 定義與定位

Fragility index（FI）衡量一個顯著結果對少數事件重新分類的抵抗力：**需要把多少名未發生事件的病人改判為發生事件，P 值才會跨回不顯著**。FI 越小，結果越脆弱。

Zuin 2026（本地僅有摘要 📌）將此指標套用到 finerenone 試驗：[[FIDELIO-DKD]] 的主要心血管複合終點雖然顯著（HR 0.86、NNT 56），但 **FI 僅為 4**；而合併後的 [[FIDELITY]]（HR 0.86、NNT 59）**FI 達 38**、FIDELITY 的心衰竭住院終點（HR 0.78、NNT 91）**FI 23**，屬穩固。相對地，CV 死亡／MI／中風等單項終點屬脆弱。

該分析僅納入 FIDELIO-DKD、[[FIGARO-DKD]] 與 pooled FIDELITY，**未納入 [[FINEARTS-HF]]**。這是「要引用合併分析而非單一試驗」的量化理由。

## 不同素材中的觀點

### 來自 [[2026-07-22-04-statistical_insights_myths]]
記錄 FIDELIO-DKD 主要心血管複合雖然顯著（HR 0.86、NNT 56），但 FI 僅為 4。Zuin 2026（僅摘要 📌）：合併後的 FIDELITY（HR 0.86、NNT 59）FI 達 38、FIDELITY 的 HF 住院終點（HR 0.78、NNT 91）FI 23，屬穩固；CV 死亡／MI／中風單項終點屬脆弱。該分析僅納入 FIDELIO-DKD、FIGARO-DKD 與 pooled FIDELITY，未納入 FINEARTS-HF。這是「要引用合併分析而非單一試驗」的量化理由。

## 關鍵數字

| 終點 | HR | NNT | FI |
|---|---|---|---|
| FIDELIO-DKD 主要心血管複合 | 0.86 | 56 | 4 |
| FIDELITY 心血管複合 | 0.86 | 59 | 38 |
| FIDELITY 心衰竭住院 | 0.78 | 91 | 23 |

判為脆弱的單項終點：CV 死亡、MI、中風。

## 相關頁面

- [[FIDELIO-DKD]]
- [[FIGARO-DKD]]
- [[FIDELITY]]
- [[FINEARTS-HF]]
- [[NNT]]
- [[trial sequential analysis]]
- [[E-value]]
- [[多重比較校正]]
- [[ICEMAN]]
- [[心衰竭住院]]
