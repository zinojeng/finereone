---
tags: [實體, 生物分子]
created: 2026-07-22
updated: 2026-07-22
sources: [wiki/sources/2026-07-22-01-pk_pd_hysteresis_offrate_hold_restart.md, wiki/sources/2026-07-22-07-07_aldosterone_synthase_inhibitor_vs_finerenone.md]
entity_type: 生物分子
mentions: 2
---

# ENaC

> 上皮鈉通道；MR 排鉀效應的終端執行者，也是 finerenone 停藥後「藥沒了、藥效還在」那段 PD lag 的物理原因。

## 定義與定位

ENaC（上皮鈉通道）的 α 次單元由 [[SCNN1A]] 編碼。MR 的排鉀效應是**基因體效應**：MR 活化 → 招募 SRC-1 與 RNA polymerase II 到 SCNN1A 調控序列 → 轉錄 → 轉譯 ENaC → 定位到頂膜 → 遠端腎小管排鉀。ENaC 是這條鏈的最後一環，也是唯一需要「重建工時」的一環。

用藥期間，MR 被拮抗 → SRC-1／RNA Pol II 無法在 SCNN1A 上組裝 → ENaC 等排鉀蛋白新合成被關掉，既有蛋白隨自然週轉逐漸下架 → 排鉀能力下降 → 血鉀傾向上升。停藥後，血中藥物清除（PK）與受體解離（off-rate）都很快，但 ENaC 必須從轉錄重新造起——這段是**內源性、與藥物濃度無關**的時間，構成 PD lag。

## 不同素材中的觀點

### 來自 [[2026-07-22-01-pk_pd_hysteresis_offrate_hold_restart]]

Amazit 2015 以 ChIP 拆出分子節點：aldosterone 誘導 MR、SRC-1、RNA polymerase II 招募至 SCNN1A（編碼 ENaC α 次單元）調控序列；finerenone 不僅抑制這三者在 aldosterone 存在下的招募，連基礎狀態的 MR 與 SRC-1 結合都顯著壓低（[[inverse agonist]] 行為）📄。素材以工廠比喻收尾：「拮抗 MR 像是停掉工廠的生產線；停藥像是解除停工令。解除停工令（受體解封）可以一瞬間，但生產線重新開機、把庫存零件（ENaC）重新造出來、裝回機台（頂膜）需要時間。你撤走的是命令，不是重建的工時。」

**明示缺口（🔴 尚待驗證）**：ENaC 從轉錄到膜定位的重建半衰期、cofactor 重新配置到 SCNN1A 的時間常數，本地與已檢索學術來源（含 Consensus／PubMed）**全部未提供**。因此對 PD lag 只作方向性推論，不賦予具體小時數。

### 來自 [[2026-07-22-07-07_aldosterone_synthase_inhibitor_vs_finerenone]]

在 PA 的脈絡中提出「血鉀上升較少」的雙重解讀（🔴）：finerenone 血鉀升幅小，對 CKD／糖尿病／高血鉀高風險者是優勢；但在嚴重低血鉀 PA 中，也可能代表**遠端腎小管 MR/ENaC 阻斷不夠強**。原文明言這只是假說，需 urine Na/K、TTKG、容量標記與劑量反應研究才能區分「安全性較佳」與「阻斷不足」。<!-- confidence: INFERRED -->

## 關鍵數字

（本知識庫目前未記錄具體數值——ENaC 重建的時間常數與半衰期為明示缺口；可對照的相鄰數字是受體解離半衰期約 50 分鐘、finerenone 血漿清除 10–15 小時）

## 相關頁面
- [[SCNN1A]]
- [[inverse agonist]]
- [[停藥可逆性]]
- [[血鉀]]
- [[受體滯留時間]]
