---
tags: [實體, 統計指標]
created: 2026-07-22
updated: 2026-07-22
sources: [wiki/sources/2026-07-22-04-statistical_insights_myths.md, wiki/sources/2026-07-22-05-benefit_risk_discussion_nnt_nnh.md]
entity_type: 統計指標
mentions: 2
---

# NNT

> Number Needed to Treat，需治療人數：NNT = 1/ARR，一個看起來像物理常數、其實綁死了時間與族群的估計值。

## 定義與定位
NNT 解決的問題是把相對風險降幅翻譯成「我這間診間要治療幾個人才救到一個事件」。它會被誤用的情境有三：把某試驗的 NNT 搬到基線風險不同的病人身上、忽略它是某個追蹤時長下的快照、以及只報點估計而不報信賴區間。當比例風險假設不成立時，單一 NNT 甚至不該被計算——此時逐年 NNT 可能翻成負值（即 [[NNH]]）。

## 不同素材中的觀點

### 來自 [[2026-07-22-04-statistical_insights_myths]]
原稿的定性是「NNT 看起來像一個物理常數，其實是一個綁定了時間、綁定了族群、還常常藏起信賴區間的估計值」，並列出三個內建陷阱。其一是時間依賴：FIDELITY stage 4 腎臟 NNT 第 1–4 年為 41／19／−40／−20，而心血管 NNT 相對穩定，為 29／29／31／24。其二是信賴區間常被省略且可能極寬，例如華人亞群的 8（4–84）與 7（4–22）。其三是不可跨基線風險移植：整體 CV 為 46（29–109）、腎臟為 60（38–142），對比華人腎臟的 7–12。

### 來自 [[2026-07-22-05-benefit_risk_discussion_nnt_nnh]]
Stage 4 CKD 心血管複合 NNT 為 1 年 29、2 年 29、3 年 31、4 年 24，來自 Sarafidis 2023 的 FIDELITY Stage 4 亞群（eGFR <30；890/13,023 ＝ 7%），CV 複合 HR 0.78（95% CI 0.57 to 1.07），以 Aalen–Johansen 法換算。素材明列誠實邊界：該分析為 exploratory，且腎複合的 proportional hazards 假設不成立——腎複合 NNT 第 3 年變 −40、第 4 年 −20（負值即 NNH），因此只能宣稱前 2 年的 HR 0.63（0.42–0.95）。屬 🟡🔴。

## 關鍵數字
- 定義：NNT = 1/ARR
- FIDELITY stage 4 腎臟 NNT（第 1–4 年）：41／19／−40／−20
- FIDELITY stage 4 心血管 NNT（第 1–4 年）：29／29／31／24
- Stage 4 CKD CV 複合 HR：0.78（95% CI 0.57 to 1.07）
- Stage 4 前 2 年腎複合 HR：0.63（0.42–0.95）
- 華人亞群 NNT：8（4–84）、7（4–22）；華人腎臟 7–12
- 整體 CV NNT：46（29–109）；整體腎臟 NNT：60（38–142）
- 亞群規模：890/13,023 ＝ 7%（eGFR <30）

## 相關頁面
- [[NNH]]
- [[ITT 分析]]
- [[FIDELITY]]
- [[比例風險假設]]
- [[相對風險與絕對風險]]
