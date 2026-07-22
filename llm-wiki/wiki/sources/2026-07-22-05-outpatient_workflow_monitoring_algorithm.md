---
tags: [素材摘要, 門診流程, 血鉀監測, 劑量調整, 暫停重啟]
created: 2026-07-22
updated: 2026-07-22
sources: []
source_type: 筆記
source_path: raw/notes/05-outpatient_workflow_monitoring_algorithm.md
images: 0
image_paths: []
---

# 門診可執行 workflow：K⁺ 監測與暫停-重啟 algorithm

> finerenone 的安全性不是靠「小心」，而是靠一套有明確進入條件、監測節奏、退出與重啟規則的 protocol——把「看到一個 K⁺ 數字」變成「照流程走下一步」。

## 基本資訊
- **來源類型**：本地 Markdown 回顧稿
- **原文位置**：raw/notes/05-outpatient_workflow_monitoring_algorithm.md
- **消化日期**：2026-07-22

## 核心觀點

1. **三個問句就是整套流程**：能不能起始？（K⁺ 與 eGFR 閾值）→ 起始後何時複測？（**第 1 月、第 4 月、其後每 4 月**）→ 追蹤數字往哪走？（加量／維持／暫停-重啟）。三個問句都有 label 與 KDIGO 明文答案，門診只要對號入座 📄（已核准）。

2. **起始前四項並行檢核**：(a) 量 K⁺——FDA 明訂 **K⁺ >5.0 mEq/L 不得起始**；(b) 量 eGFR——決定起始劑量並作為日後 dip 監測基線；(c) 審視 CYP3A4 併用藥——強效抑制劑（itraconazole、clarithromycin、ketoconazole、ritonavir）**禁忌**、葡萄柚汁避免；(d) 盤點其他升鉀／損害排鉀藥——不得與保鉀利尿劑（amiloride、triamterene）及其他 MRA（spironolactone、eplerenone、esaxerenone）併用，與 K⁺ 補充劑、含鉀鹽替代品、trimethoprim／複方磺胺併用需加強監測 📄。原文的操作邏輯是：**起始前把可逆的升鉀因素先清掉，之後 K⁺ 一上升才知道是藥物還是背景干擾**。

3. **K⁺ 閘門（EMA 三分法）**：≤4.8 可起始；**>4.8 至 5.0 可考慮起始但前 4 週加強監測**；>5.0 不起始、先矯正可逆因素。trial 的實際入選門檻更嚴——FIDELIO-DKD／FIGARO-DKD／CONFIDENCE 皆要求篩選期 K⁺ 一致 **≤4.8 mmol/L** 📄（此點出自 KDIGO 2026 草案，**尚待驗證：未定稿**）。

4. **eGFR → 起始劑量（CKD+T2D）**：≥60 → **20 mg qd**；≥25 至 <60 → **10 mg qd**；<25 不建議起始。CKD+T2D 目標劑量為 **20 mg qd**；HF（LVEF≥40%）起始劑量相同但目標劑量依起始 eGFR 為 **40 mg 或 20 mg** 📄。

5. **監測節奏**：trial 用的節奏就是門診該抄的——**第 1 月、第 4 月、其後每 4 月**複測 K⁺＋eGFR，與 KDIGO 對 CKD 病人的常規生化監測一致（UACR>300 且 eGFR<60 者一年 3–4 次）。額外複測時機：EMA 要求**起始／重啟／增量後 4 週**再測；KDIGO 對 RASi 則為「起始或調量後 2–4 週」。**creatinine／eGFR 必須與 K⁺ 同時監測** 📄。

6. **追蹤 K⁺ 三段式分岔（CKD+T2D）**：≤4.8 → 在 10 mg 者增量至 20 mg（**但若 eGFR 較前值下降 >30% 則維持 10 mg**，為 EMA Table 2 註腳明文）；>4.8 至 5.5 → 維持原劑量；>5.5 → 暫停，K⁺ ≤5.0 時以 10 mg 重啟 📄。

7. **K⁺ >5.5 的降鉀階梯**：**第一線（先找可逆因素）**——檢視並停用／調整 NSAID、trimethoprim、含鉀鹽替代品與其他升鉀藥，moderate dietary potassium intake，盤點共病用藥；**第二線（藥理降鉀）**——加用 potassium-wasting diuretics、以 sodium bicarbonate 矯正代謝性酸中毒、必要時加 potassium binder。binder 在 trial 中屬 investigator discretion、使用率不高（**FIDELIO-DKD 10.8% vs 6.5%、FIGARO-DKD 4.5% vs 2.8%**）📄。

8. **暫停有效的藥理根據**：finerenone **半衰期短、僅 2–3 小時且無活性代謝物**，停藥即可讓 K⁺ 快速回收；KDIGO 2026 草案據此指出**多數高血鉀事件可用 72 小時的暫停處理**（暫停後 72 小時內複測 K⁺）📄（**尚待驗證：草案未定稿**）。永久停藥是最後手段——trial 資料佐證代價值得承受：因高血鉀永久停藥僅 **1.7% vs 0.6%**，13,000 餘人、追蹤中位 3 年**無任何高血鉀相關死亡** 📄。

9. **CKD vs HF 是兩套矩陣（門診最容易踩雷處）**：CKD+T2D——K⁺ ≤5.5 續用、**>5.5 暫停**、≤5.0 以 10 mg 重啟；HF（LVEF≥40%）——K⁺ <5.5 續用、**5.5 至 <6.0 減量一階**、**≥6.0 暫停**、K⁺ <5.5 以 10 mg 重啟。即 HF 把 5.5–6.0 設為**減量帶**而非暫停帶。這與 KDIGO 2024 Figure 26 註腳呼應：工作組認為 5.5 閾值「偏保守」，**K⁺ 5.5–6.0 者續用 MRA 亦屬合理** 📄。誠實邊界：兩套閾值來自 label 對兩適應症之分別核准，**非同一 RCT 頭對頭比較**。

10. **eGFR dip 用另一把尺平行判讀**：初期平均下降約 **2 mL/min/1.73 m²** 屬預期；**>30% 才啟動評估**（查 AKI、容積缺失、腎動脈狹窄、利尿劑／NSAID）；EMA 另設 **≥40% 考慮減量／暫停**，穩定後再上調；即使 K⁺ 允許增量，**eGFR 較前值下降 >30% 仍維持 10 mg 不加量**。RASi 歷史更寬——Ku 的 17 試驗、n=11,800 顯示 3 個月 ≤13%（95% CI 8–17%）或 1 個月 ≤21%（95% CI 15–27%）仍優於「無下降」（13% 閾值處 adjusted HR 1.02, 0.86–1.22）📄（可外推：跨 class 外推）。

11. **觸發加密監測的六類情境（Wanner 實務清單）**：低 eGFR（EMA：**eGFR <60 及高齡者**應更頻繁監測）、高 baseline K⁺ 或既往高血鉀 episode、併用升鉀或損害排鉀之藥（含 K⁺ 補充劑、鹽替代品）、急性病（AKI、容積缺失、腹瀉等腸胃問題、感染）、新增 NSAID 或手術、**中度肝功能不全（Child-Pugh B）**應考慮額外 K⁺ 監測（重度肝損害則不應使用）📄。

12. **指引升級方向（誠實揭露草案狀態）**：KDIGO 2026 草案 **Recommendation 4.4.1 為 1A**（T2D、eGFR ≥25、血鉀正常、UACR ≥30 mg/g、已用最大耐受 RASi），並以 **Practice Point 4.4.2** 支持**同步起始 SGLT2i 與 nsMRA**（CONFIDENCE 佐證）。因屬公開審查草案，臨床採用仍應以正式定稿與在地核准為準 📄（**尚待驗證**）。

## 關鍵概念

- [[血鉀監測]]
- [[Finerenone]]
- [[高血鉀]]
- [[eGFR dip]]
- [[鉀離子結合劑]]
- [[CYP3A4]]
- [[KDIGO 2026 糖尿病與 CKD 指引草案]]
- [[FIDELIO-DKD]]
- [[CONFIDENCE]]

## 與其他素材的關聯

本檔是主題五主文 §9 的可執行版，把散落在 label 與 KDIGO 的閾值收攏成單一決策流。原文明列交叉連結，構成主題五的內部引用網：

- 起始前 CYP3A4 併用藥審查 → [[2026-07-22-05-cyp3a4_interaction_prescribing_rules]]
- 場景化高血鉀工程 → [[2026-07-22-05-hyperkalemia_engineering_by_scenario]]
- eGFR dip 血流動力學可逆性 → [[2026-07-22-05-egfr_dip_hemodynamic_reversible]]
- potassium binder 角色 → [[2026-07-22-05-potassium_binder_role]]

本檔亦指向兩份不在本組範圍的姊妹檔：`label_guideline_safety_framework.md`（HF 三劑量 10/20/40 mg 完整暫停矩陣）與 `hypokalemia_bidirectional_electrolyte.md`（雙向電解質）。
<!-- confidence: AMBIGUOUS --> 主文 §9 流程圖標「初期 dip ≤某閾值屬預期」未給數字，本延伸檔則明確化為「約 2 mL/min 屬預期、>30% 才評估、≥40% 考慮減量」；兩者不衝突，但主文的模糊表述宜以本檔為準。

## 原文精彩摘錄

> 「起始前的目標是把**可逆的升鉀因素先清掉**，再讓 finerenone 進場——這樣後續一旦 K⁺ 上升，才知道是藥物本身還是背景干擾。」

> 「門診最容易踩雷之處：**暫停/減量閾值依適應症不同**……HF 適應症把『5.5–6.0』設為**減量帶**而非暫停帶、暫停門檻抬高到 ≥6.0，重啟門檻放寬到 <5.5。」

> 「永久停藥是最後手段，KDIGO 的核心倫理是暫停後務必在事件解除、條件允許時擇日重啟，別讓高風險病人被剝奪所需藥物。」

## 相關頁面

- [[2026-07-22-05-05_hyperkalemia_egfr_dip_safety_engineering]]
- [[2026-07-22-05-cyp3a4_interaction_prescribing_rules]]
- [[2026-07-22-05-hyperkalemia_engineering_by_scenario]]
- [[2026-07-22-05-egfr_dip_hemodynamic_reversible]]
- [[2026-07-22-05-potassium_binder_role]]
