---
tags: [主題, PK-PD, 停藥可逆性, hold-restart]
created: 2026-07-22
updated: 2026-07-22
sources: [wiki/sources/2026-07-22-01-pk_pd_hysteresis_offrate_hold_restart.md, wiki/sources/2026-07-22-01-mr_receptor_dissociation_residence_time.md, wiki/sources/2026-07-22-05-uacr_rebound_reversibility_mechanism.md, wiki/sources/2026-07-22-03-confidence_over_additive_and_offtreatment_reversibility.md, wiki/sources/2026-07-22-01-01_finerenone_not_just_safer_spironolactone.md, wiki/sources/2026-07-22-00-KDIGO_2026_Diabetes_CKD_draft.md]
---

# PK-PD 解耦與停藥可逆性

> 回答 purpose.md 關鍵問題二的最後一段（停藥後 UACR 反彈說明了什麼）與問題五的機制底層（為什麼「暫停即解毒」在 finerenone 成立、在 spironolactone 不成立）。

## 為什麼重要

「停藥後多久解毒」在臨床被當成一個數字問，但它其實是三個速率完全不同的過程疊在一起：血中藥物清除、藥物從受體解離、下游排鉀機器重建。finerenone 之所以能把「暫停用藥」變成門診可執行的第一線解毒動作，不是因為它加速了任何生理過程，而是因為它同時抹掉了兩個拖慢回復的變因。同一組 PK-PD 邏輯往反方向讀，就解釋了 CONFIDENCE 停藥 30 天後 UACR、血壓、血鉀、eGFR 為何一起彈回——效益要靠持續給藥維持。這一頁把「安全上的好消息」與「療效上的壞消息」放在同一個機制框架下。

## 素材匯總

| 素材 | 對本主題的貢獻 | 證據層級 |
|------|----------------|----------|
| [[2026-07-22-01-pk_pd_hysteresis_offrate_hold_restart]] | 三個時鐘的完整拆解與 hold-restart 的藥理根據 | 已核准（PK 與指引閾值）／尚待驗證（PD 重建無定量） |
| [[2026-07-22-01-mr_receptor_dissociation_residence_time]] | 提供 off-rate 的實測錨點與 spironolactone 代謝物接力的對照 | 尚待驗證（in-vitro） |
| [[2026-07-22-05-uacr_rebound_reversibility_mechanism]] | 用腎絲球內壓「一個變因兩面」統一 UACR 反彈與 eGFR dip 回復 | 可外推（機制整合） |
| [[2026-07-22-03-confidence_over_additive_and_offtreatment_reversibility]] | 提供停藥 30 天的實測反彈 LSMR，判決「結構性殘餘防護」假說不成立 | 尚待驗證（surrogate、30 天窗） |
| [[2026-07-22-01-01_finerenone_not_just_safer_spironolactone]] | 對照組：spironolactone 停藥後 3 週仍可測得尿中代謝物 | 可外推 |
| [[2026-07-22-00-KDIGO_2026_Diabetes_CKD_draft]] | 指引級 hold-restart 協定與 72 小時複驗規則 | 已核准（指引） |

## 核心觀點

1. **三個必須分開計時的時鐘**：①PK 清除（血中藥物濃度）、②受體 off-rate（藥物從 MR 解離）、③PD 回復（下游排鉀機器重建）。把「停藥後多久解毒」講成一個數字，就是混淆了這三個速率不同的過程（來源：[[2026-07-22-01-pk_pd_hysteresis_offrate_hold_restart]]）。

2. **PK 清除是最硬的一格**：finerenone 終末半衰期 2–3 小時、代謝為 inactive metabolites（[[CYP3A4]] ~90%）、系統清除率 25 L/h；5 個半衰期 ≈ 10–15 小時近乎清除。指引直接把這點寫進解毒邏輯——短半衰期且無活性代謝物，因此高血鉀可藉停藥處理 📄（來源：[[2026-07-22-01-pk_pd_hysteresis_offrate_hold_restart]]）。

3. **最反直覺的一點：受體解離比血中清除還快**。off-rate 對應的解離半衰期約 50 分鐘，短於 2–3 小時的血漿半衰期。只要血中還有藥，受體會不斷「解離→再被重新結合」；真正決定受體何時長時間空出來的不是 off-rate，而是血中藥物先清乾淨。①+②合起來在 10–15 小時內大致收尾 📄（來源：[[2026-07-22-01-pk_pd_hysteresis_offrate_hold_restart]]、[[2026-07-22-01-mr_receptor_dissociation_residence_time]]）。

4. **PD 回復是唯一剩下的滯後，且無定量數據**：MR 的排鉀效應是基因體效應——停藥後需重新轉錄 [[SCNN1A]] → 轉譯 ENaC → 定位到頂膜才恢復排鉀，這段是內源性、與藥物濃度無關的時間 📄（來源：[[2026-07-22-01-pk_pd_hysteresis_offrate_hold_restart]]）。

5. **與 spironolactone 的對比在 PK 而非受體端**：以 canrenone 16.5 h 外推，5 個半衰期 ≈ 82.5 小時（約 3–4 天）才近乎清除，遠慢於 finerenone 的 10–15 小時；在 eGFR 25–45 的患者中，停藥後長達 3 週仍有 38% 患者可測得尿中代謝物，且停藥 2 週後仍保留過半的收縮壓降幅 📄（來源：[[2026-07-22-01-pk_pd_hysteresis_offrate_hold_restart]]、[[2026-07-22-01-01_finerenone_not_just_safer_spironolactone]]）。

6. **工程學總結**：finerenone 把「解毒延遲」的方程式從「PK 滯後 + PD 滯後」簡化成「≈ 只剩 PD 滯後」。它無法縮短身體重建排鉀機器的內源工時，但取消了會疊加在前面的長效藥物殘留變因（來源：[[2026-07-22-01-pk_pd_hysteresis_offrate_hold_restart]]）。

7. **落地成 hold-restart 規則**：血鉀 > 5.5 mmol/L 即暫停，待血鉀 ≤ 5.0 mmol/L 再以 10 mg 重啟；KDIGO 2026 草案補上「>5.5 暫停並於 72 小時內複驗」與監測時程（FIDELIO/FIGARO 於起始後 1 個月、4 個月、其後每 4 個月；CONFIDENCE 於 day 14、30、90、180）📄（來源：[[2026-07-22-01-pk_pd_hysteresis_offrate_hold_restart]]、[[2026-07-22-00-KDIGO_2026_Diabetes_CKD_draft]]）。

8. **同一套 PK-PD 耦合往反方向讀就是療效反彈**：停藥後藥物清除 → MR 重新被醛固酮活化 → 張力調節撤除 → 腎絲球內壓回升。UACR 本就「most of the reduction occurred within 4 weeks after the initiation」，建立與消退都是週級，與停藥 30 天大幅反彈完全對稱 📄（來源：[[2026-07-22-05-uacr_rebound_reversibility_mechanism]]）。

9. **CONFIDENCE 的停藥 30 天實測**：UACR 回升 LSMR combination 1.63（1.49–1.78）／finerenone 1.45（1.32–1.59）／empagliflozin 1.44（1.32–1.58），全部 >1；血鉀 Day 14 combo 升 0.27 mmol/L，停藥 30 天後降至接近基線；血壓在所有治療組皆可逆；eGFR dip 回復至接近基線 📄（來源：[[2026-07-22-03-confidence_over_additive_and_offtreatment_reversibility]]、[[2026-07-22-05-uacr_rebound_reversibility_mechanism]]）。

10. **反彈同時排除兩種「結構」誤讀**：一個效應停藥即回彈，就同時排除了「結構性損傷」（損傷不會回彈）與「結構性殘餘保護」（保護若靠結構，停藥不會塌）。核心誤解是把「non-hemodynamic（中介僅 5.2%）」等同於「不可逆的結構重塑」——non-hemodynamic ≠ permanent（來源：[[2026-07-22-05-uacr_rebound_reversibility_mechanism]]、[[2026-07-22-03-confidence_over_additive_and_offtreatment_reversibility]]）。

11. **[[eGFR dip]] 的可逆性有獨立模型佐證**：Holtkamp 的 two-slope 模型判準是停用降壓治療後多數病人 GFR 回升、且與初始 GFR 下降相關，支持血流動力學（非結構性）來源；Goulooze 的 FIDELIO 群體模型在假設急性下降完全可逆下良好描述資料，並量化停藥者 eGFR 回升 6.9%（95% CI +3.9% 至 +10.0%），與模擬 20 mg 急性下降 5.4% 相稱 📄（來源：[[2026-07-22-05-uacr_rebound_reversibility_mechanism]]）。

## 尚有爭議或未解之處

1. **PD 回復完全沒有定量半衰期**：finerenone 停藥後下游基因表達恢復速度、cofactor 重新配置到 SCNN1A 的時間常數、ENaC 從轉錄到膜定位的重建半衰期，本地與已檢索學術來源全部未提供。任何「停藥後 X 小時血鉀回正」的觀察是 PK+off-rate+PD+腎功能+併用藥的綜合結果，不可回推成單一 PD 回復半衰期（來源：[[2026-07-22-01-pk_pd_hysteresis_offrate_hold_restart]]）。**尚待驗證**

2. **spironolactone/eplerenone 的 off-rate 無定量值**：兩者的「持久」只能以代謝物 PK 解釋，不能反推成受體端 koff 較小（來源：[[2026-07-22-01-mr_receptor_dissociation_residence_time]]）。**尚待驗證**

3. **「急性成分完全可逆」在 Goulooze 是模型假設**：它是能良好擬合資料（含停藥後資料）的假設，而非直接的臨床終點證明；rebound 6.9% 才是最接近實測的相容證據（來源：[[2026-07-22-05-uacr_rebound_reversibility_mechanism]]）。**尚待驗證**

4. **觀察窗太短，長期結構性殘餘保護答不了**：CONFIDENCE 療程僅約 6 個月加 30 天洗脫；combination 起點更低（LSMR 0.48 vs 0.68／0.71），回落後仍殘留約 −22%（本推算為素材檔的兩段 LSMR 相乘推估、非原文點估計），但這是程度差異與時間差，不是「維持極佳水平」（來源：[[2026-07-22-03-confidence_over_additive_and_offtreatment_reversibility]]）。**尚待驗證**

5. **[[eGFR dip]] 在晚期 CKD 可能鈍化**：CONFIDENCE 顯示基線 eGFR 30 者未觀察到大而持續的下降，提示晚期 CKD 的血流動力學反應不同——這使「dip 是療效訊號」的解讀不能無條件跨 eGFR 層外推（來源：[[2026-07-22-05-uacr_rebound_reversibility_mechanism]]）。<!-- confidence: INFERRED -->

6. **「短半衰期在其他情境是缺點、在怕高血鉀時是安全特徵」的反轉尚未被療效端檢驗**：同一個 PK 特性是否讓漏服的療效代價更大，本地素材未提供資料（來源：[[2026-07-22-01-pk_pd_hysteresis_offrate_hold_restart]]）。<!-- confidence: INFERRED -->

## 關鍵實體

- [[受體滯留時間]] — 三個時鐘中的第二個；本主題最反直覺的結論就出自它比 PK 清除更快
- [[CYP3A4]] — 承擔約 90% 代謝，是 PK 清除這一格的速率決定者，也是交互作用的入口
- [[SCNN1A]] — PD 重建鏈的起點，也是這條鏈唯一沒有定量數據的一段
- [[血鉀]] — hold-restart 規則所依據的可測量，也是三個時鐘的臨床出口
- [[停藥可逆性]] — 本主題的核心命題，正反兩面（解毒快 / 效益也退得快）共用同一機制
- [[UACR 反彈]] — 停藥 30 天的主導訊號，是可逆功能效應的直接指紋
- [[eGFR dip]] — 與 UACR 下降同源於腎絲球內壓下修，停藥後同步逆轉
- [[腎絲球內壓]] — 統一 UACR 與 eGFR 兩個方向相反數字的單一變因
- [[管球回饋]] — empagliflozin 端下修腎絲球內壓的路徑，與 finerenone 端互補
- [[Spironolactone]] — PK 對照組；代謝物接力使其解毒方程式多一項滯後
- [[CONFIDENCE]] — 唯一提供停藥 30 天前瞻性再測資料的試驗

## 相關頁面

- [[受體藥理與 nsMRA 分野]]
- [[CONFIDENCE 與 over-additive 效應]]
- [[BP-independent 心腎保護]]
