# label 與 guideline 的安全框架：KDIGO nsMRA 定位的等級演進（2020→2022→2024→2026）與 EMA/FDA label 規則

> 本文為主題五（高血鉀與 eGFR dip 的安全工程學）之延伸拆解，把主文 §2「label 與 guideline 的安全框架」獨立展開成專科化、可稽核的版本。聚焦三件事：(1) KDIGO 對 nsMRA/finerenone 定位的**等級演進**（2020→2022→2024→2026）；(2) EMA SmPC 與 FDA KERENDIA PI 的**起始／劑量／監測／停藥矩陣**，並對照 KDIGO 既有 RASi 監測邏輯；(3) **禁忌與交互作用**清單（CYP3A4 量化細節交叉指向 `cyp3a4_interaction_prescribing_rules.md`）。
>
> **引用標記慣例**：📄 = 本地全文可 grep 稽核；📌 = 僅取得 abstract（不對其未載內容作具體斷言）。每個數字句末以 `[本地MD檔名]` 標註來源供 grep 回溯。LLM 僅負責組織與改寫，所有條號／等級／數字均出自本地 MD 檔。
>
> **證據分層**：🟢 guideline routine（已進指引常規／label 明文）｜🟡 evidence expansion（post hoc／surrogate／模型）｜🔴 尚待驗證／尚未定稿（如 KDIGO 2026 公開審查草案）。

---

## 0. 一句話定位

nsMRA/finerenone 在 KDIGO 的角色，在四個版本間走過「**尚未存在 → 首度納入（2A, suggest）→ 沿用不變（2A）→ 升級為 1A（recommend）**」的軌跡；**適應人群與門檻（eGFR ≥25、血鉀正常、UACR ≥30 mg/g、最大耐受 RASi 上）四版一致，改變的只是「建議強度」與其背後的「可用性與熟悉度」判斷**。理解這條軸線，就能對聽眾清楚交代「為什麼 2026 草案敢從 suggest 升成 recommend，而監測節奏卻幾乎沒動」。

---

## 1. 重點一：KDIGO nsMRA/finerenone 定位的等級演進

### 1.1 演進總表（年份 × 條號 × 等級 × 監測邏輯）

| 年份／文件 | 條號 | 等級（wording） | 適應人群／門檻 | 監測邏輯 | 性質 |
|---|---|---|---|---|---|
| **KDIGO 2020**（Diabetes in CKD，首版） | — | nsMRA 未納入 | — | — | 歷史背景：finerenone 當時尚未取得藥證（見 §1.2） |
| **KDIGO 2022**（Diabetes in CKD 更新） | （對應後續 3.8.1） | **2A（suggest）** | T2D、eGFR >25、血鉀正常、UACR >30 mg/g、最大耐受 RASi | 沿用 FIDELIO/FIGARO 協定 | 首度納入；本地僅 PDF 未 parse，佐證見 §1.3 |
| **KDIGO 2024**（CKD 指引） | **Rec 3.8.1** | **2A（suggest）** | 同上（eGFR >25、正常 K⁺、>30 mg/g、最大耐受 RASi） | Figure 26：K⁺ ≤4.8 起始，1 個月後、其後每 4 個月；>5.5 暫停 | 定稿；nsMRA 建議完全 defer 給 2022 指引，無新 MRA 系統性回顧 |
| **KDIGO 2026**（Diabetes+CKD 更新・公開審查草案） | **Rec 4.4.1** | **1A（recommend）** | eGFR ≥25、正常 K⁺、UACR ≥30 mg/g、最大耐受 RASi（不變） | PP 4.4.3：措辭同 2024；併 CONFIDENCE 監測時點 | **尚未定稿**，內容可能因回饋而變（🔴 性質） |

（2024 欄 [📄 label_guideline_safety_Kidney_2024] [📄 label_guideline_safety_Levin_2024]；2026 欄 [📄 KDIGO_2026_Diabetes_CKD_draft]；2022 佐證 [📄 note_kdigo2024]）

> **一句話讀表**：橫看四版，**門檻欄幾乎完全不動**；縱看「等級」欄，只在 2024→2026 由 2A 跳到 1A。這正是回應「指引到底多相信 finerenone」時該放的單張投影片。

### 1.2 KDIGO 2020（歷史背景，不作條號斷言）🟢

KDIGO 首版 Diabetes in CKD 指引問世時，finerenone 尚未取得藥證，nsMRA 自然未被納入建議。本地**無 2020 版 parsed MD**，故此處僅作背景敘述、不對其做具體條號或等級斷言。可 grep 的時間錨點是 finerenone 的**歐盟藥證日**：CHMP 正面意見 2021 年 12 月 16 日、EU marketing authorisation 2022 年 2 月 16 日 [📄 label_guideline_safety_European_2022]——即 2020 版指引在藥證之前，nsMRA 未進指引屬時序必然，而非被否決。

### 1.3 KDIGO 2022（nsMRA 首度納入，2A）🟢

nsMRA/finerenone 於 2022 年 Diabetes in CKD 更新首度進入 KDIGO 建議，等級 **2A（suggest）**。本地 **KDIGO 2022 僅有 PDF、未 parse**，故不逐字引其原文；佐證來自 2024 版的自述——2024 CKD 指引「defers ns-MRA recommendations entirely to the 2022 Diabetes guideline」，且 2024 的 Rec 3.8.1 標為 **2A**、「cross-references KDIGO 2022 Diabetes in CKD guideline ... for the underlying FIDELIO-DKD and FIGARO-DKD trial data」[📄 note_kdigo2024]。2024 版對此段亦明言「there are no new systematic reviews of MRA trials in the 2024 CKD guideline itself for the MRA section」[📄 note_kdigo2024]——即 2A 的證據基礎自 2022 承襲、2024 未重做。

### 1.4 KDIGO 2024（Rec 3.8.1，維持 2A）🟢

2024 CKD 指引 **Recommendation 3.8.1（2A）**：「We suggest a nonsteroidal mineralocorticoid receptor antagonist with proven kidney or cardiovascular benefit for adults with T2D, an eGFR >25 ml/min per 1.73 m², normal serum potassium concentration, and albuminuria (>30 mg/g [>3 mg/mmol]) despite maximum tolerated dose of RAS inhibitor (RASi)」[📄 label_guideline_safety_Kidney_2024] [📄 label_guideline_safety_Levin_2024]。

- **療效依據（引自 2024 指引本文）**：FIDELITY pooled「reduced cardiovascular risk ... (HR: 0.86; 95% CI: 0.78–0.95)」，其中 HHF 貢獻主要「a 22% reduction in the risk of hospitalization for heart failure (HR: 0.78; 95% CI: 0.66–0.92)」[📄 label_guideline_safety_Kidney_2024]。
- **監測邏輯（Figure 26）**：K⁺ ≤4.8 → 起始（eGFR 25–59 用 10 mg、≥60 用 20 mg），起始後 1 個月、其後每 4 個月監測；K⁺ 4.9–5.5 → 續用；K⁺ >5.5 → 暫停 [📄 label_guideline_safety_Kidney_2024]。
- **工作小組自評「偏保守」**（逐字）：「The Work Group considers these potassium thresholds to be conservative, and it may be considered appropriate to continue MRAs in people with potassium of 5.5–6.0 mmol/l ... The US Food and Drug Administration (FDA) has approved initiation of K⁺ <5.0 mmol/l」[📄 label_guideline_safety_Kidney_2024]。

### 1.5 KDIGO 2026（Rec 4.4.1，2A→1A 升級）🔴（公開審查草案・尚未定稿）

2026 Diabetes+CKD 更新公開審查草案把建議改列為 **Recommendation 4.4.1**，並**由 2A 升級為 1A（recommend）**（逐字）：「We recommend adding a nonsteroidal mineralocorticoid receptor antagonist (nsMRA) with proven kidney or cardiovascular benefit for people with T2D, an eGFR ≥25 ml/min per 1.73 m², normal serum potassium concentration, and albuminuria (UACR ≥30 mg/g [≥3 mg/mmol]) while on maximum tolerated dose of RAS inhibitor (RASi) (1A)」[📄 KDIGO_2026_Diabetes_CKD_draft]。

**升級理由（Work Group 判斷，逐字要點）**：本建議「places a relatively lower value on the risk of hyperkalemia and monitoring of potassium during nsMRA treatment」，並判斷自前版以來「there is greater availability and familiarity with the use of nsMRAs and the majority of well-informed healthcare professionals and people with T2D and CKD ... would want to receive treatment with an nsMRA, while only a small proportion」不會 [📄 KDIGO_2026_Diabetes_CKD_draft]。草案另述：finerenone「regulatory approvals ... have been obtained in many parts of the world」、實務使用與安全資料已發表、實用指引已備，「increasing availability and familiarity with nsMRA may reduce the inertia」[📄 KDIGO_2026_Diabetes_CKD_draft]。

**監測邏輯不變**：對應 **Practice Point 4.4.3**（逐字）「To mitigate risk of hyperkalemia, select people with consistently normal serum potassium concentration and monitor serum potassium regularly after initiation of an nsMRA」——與 2024 版 Practice Point 3.8.3 措辭一致 [📄 KDIGO_2026_Diabetes_CKD_draft] [📄 label_guideline_safety_Kidney_2024]。草案重申試驗篩選採 K⁺ ≤4.8 mmol/L，惟依 FDA label「serum potassium should not be >5 mmol/l」，且「Most incidents of hyperkalemia can be managed with treatment pauses of 72 hours, as the drug has a short half-life」[📄 KDIGO_2026_Diabetes_CKD_draft]。「不同時使用類固醇型與 nsMRA」對應 **Practice Point 4.4.7**（逐字）「Do not use steroidal and nsMRA concurrently」[📄 KDIGO_2026_Diabetes_CKD_draft]。

- **監測時點的細化**：草案並列兩套協定——FIDELIO-DKD/FIGARO-DKD「serum potassium was checked 1 month after drug initiation, 4 months after drug initiation, and every 4 months thereafter」；CONFIDENCE「measured at baseline and after randomization on days 14, 30, 90, and 180」；三試驗皆「finerenone was continued with serum potassium ≤5.5 mmol/l」，>5.5 則暫停、72 小時內複測、回到 ≤5.0 再啟 [📄 KDIGO_2026_Diabetes_CKD_draft]。

> **誠實邊界（🔴）**：KDIGO 2026 為**公開審查草案（2026 年 3 月，Chapter 4）、尚未定稿**，等級與措辭可能因回饋而改變；文中所有「1A／4.4.x」引用均限定於草案狀態，不得當作已定稿指引引用 [📄 KDIGO_2026_Diabetes_CKD_draft]。

---

## 2. 重點二：EMA SmPC vs FDA KERENDIA PI 的起始／劑量／監測／停藥矩陣

### 2.1 CKD+T2D 的起始與續用矩陣

| 項目 | EMA SmPC | FDA (KERENDIA PI, rev. 8/2025) |
|---|---|---|
| K⁺ ≤4.8 | 可起始 | 起始不受此細分限制（見下界） |
| K⁺ >4.8 到 5.0 | 可考慮起始，**前 4 週更密切監測** | 未細分 |
| K⁺ >5.0 | **不建議起始** | **Do not initiate ... if serum potassium is > 5.0 mEq/L** |
| 起始劑量 | eGFR ≥60→20 mg；≥25 到 <60→10 mg；<25 不建議 | 同左（≥60→20 mg；≥25 到 <60→10 mg；<25 不建議） |
| 續用監測 | 起始／重啟／加量後 **4 週** 複測 K⁺ 與 eGFR，其後定期 | 治療期間定期測 K⁺ 與 eGFR |
| K⁺ >4.8 到 5.5 | 維持原劑量（10 或 20 mg） | 維持原劑量 |
| K⁺ >5.5 | 暫停；K⁺ ≤5.0 時以 10 mg 重啟 | 暫停；K⁺ ≤5.0 時以 10 mg 重啟 |

（EMA 欄 [📄 label_guideline_safety_European_2022]；FDA 欄 [📄 label_guideline_safety_Bayer_2025]）

- EMA 另明訂：若 eGFR 較前次下降 **>30%**，10 mg 者維持 10 mg（不加量）[📄 label_guideline_safety_European_2022]。

### 2.2 心衰（LVEF ≥40%）的階梯——與 CKD 的關鍵差異在「>6.0 才暫停」

心衰 label 採更寬的鉀階梯（起始門檻 K⁺ ≤5.0；目標劑量最高 40 mg）：

| Current K⁺ | EMA（10/20/40 mg） | FDA（10/20/40 mg） |
|---|---|---|
| <5.0 | 依 eGFR 加量至 20／40 mg | 依 eGFR 加量 |
| 5.0 到 <5.5 | 維持 | 維持 |
| 5.5 到 <6.0 | 10 mg 者暫停；20/40 mg 者**減量** | 10 mg 者暫停（K⁺ <5.5 以 10 mg 重啟）；20→10 mg、40→20 mg |
| ≥6.0 | 暫停；K⁺ <5.5 重啟（反覆 ≥5.5 者待 <5.0 再啟） | 暫停；K⁺ <5.5 以 10 mg 重啟 |

（EMA [📄 label_guideline_safety_European_2022]；FDA [📄 label_guideline_safety_Bayer_2025]）

- **CKD 與 HF 的階梯差異**：CKD+T2D 以 **>5.5 暫停**；HF（LVEF ≥40%）以 **>6.0 暫停、5.5–<6.0 減量** [📄 label_guideline_safety_European_2022] [📄 label_guideline_safety_Bayer_2025]。
- **HF 的腎功能面向**：EMA 另設 worsening renal function 警示，eGFR 若較前次下降 **≥40%**，考慮減量或暫停，穩定後再加量／重啟 [📄 label_guideline_safety_European_2022]；FDA 亦要求心衰維持期定期測 eGFR、於顯著腎功能惡化時考慮延後加量或中斷治療 [📄 label_guideline_safety_Bayer_2025]。

### 2.3 監測節奏與既有 RASi 節奏一致（回應「多做很多抽血」的支點）🟢

finerenone 的監測頻率，本質上與 CKD 病人本來就該有的 RASi 監測節奏重疊：

- **KDIGO RASi 監測邏輯**：Practice Point 3.6.2「Changes in BP, serum creatinine, and serum potassium should be checked within 2–4 weeks of initiation or increase in the dose of a RASi」；PP 3.6.3「Hyperkalemia associated with use of RASi can often be managed by measures to reduce the serum potassium levels rather than decreasing the dose or stopping RASi」[📄 label_guideline_safety_Levin_2024]。
- **Wanner 明白對照**（逐字）：finerenone 的鉀監測「is actually similar to the recommended procedure for RASi oversight」，其引 KDIGO 糖尿病管理指引原文「Monitor serum creatinine and potassium」（起始或調整劑量後 2–4 週內）[📄 label_guideline_safety_Wanner_2022]。
- **頻率對齊**：兩試驗的鉀監測（Month 1、Month 4、其後每 4 個月）「was consistent with that recommended in the KDIGO guidelines for patients with CKD（UACR >300 mg/g 且 eGFR <60 者一年 3–4 次；UACR 30–300 mg/g 且 eGFR 15–59 者一年 2–3 次）」[📄 label_guideline_safety_Wanner_2022]。
- **「肌酸酐上升 <30% 續用」的對照邏輯**：SGLT2i 的可逆性 eGFR 下降「is generally not an indication to discontinue therapy」（PP 3.7.3），與 finerenone label 中 eGFR 下降 >30% 只調整劑量、下降 ≥40% 才考慮暫停的邏輯同源——都把「初期血流動力學性下降」與「真正的腎損傷」分開處理 [📄 label_guideline_safety_Levin_2024] [📄 label_guideline_safety_European_2022]。

> **框架**：這是回應「換來更多抽血」質疑的第一個支點——finerenone 的監測節奏並非額外負擔，而是**與 CKD 既有 RASi 監測節奏一致**；差別只是把「本就該做的抽血」明文協定化 [📄 label_guideline_safety_Wanner_2022]。

### 2.4 label 側的高血鉀量化（供對照主文表 5）🟢

- **EMA 摘述**：最常見不良反應為 hyperkalaemia (**12.6%**)；起始首月平均 K⁺ 較安慰劑上升 up to **0.2 mmol/L**，其後穩定 [📄 label_guideline_safety_European_2022]。
- **Pooled FIDELIO+FIGARO（EMA）**：hyperkalaemia **14.0% vs 6.9%**；serious **1.1% vs 0.2%**；K⁺ >5.5 **16.8% vs 7.4%**；>6.0 **3.3% vs 1.3%**；因高血鉀永久停藥 **1.7% vs 0.6%**；因高血鉀住院 **0.9% vs 0.2%** [📄 label_guideline_safety_European_2022]。
- **FINEARTS-HF（EMA）**：hyperkalaemia **9.7% vs 4.2%**；永久停藥 **0.4% vs 0.2%**；住院 **0.5% vs 0.2%** [📄 label_guideline_safety_European_2022]。
- **FDA pooled 不良反應表（n=6510 vs n=6489）**：Hyperkalemia **912 (14.0%) vs 448 (6.9%)**；Hypotension **302 (4.6%) vs 194 (3.0%)**；Hyponatremia **82 (1.3%) vs 47 (0.7%)** [📄 label_guideline_safety_Bayer_2025]。
- **安全的「可管理性」證據**：Wanner 指出在 >13,000 名病人、中位追蹤約 3 年間「there were no hyperkalemia-related deaths」；且高血鉀端隨 eGFR 而異——FIGARO（平均 eGFR 68）10.8% vs FIDELIO（平均 eGFR 44）18.3% [📄 label_guideline_safety_Wanner_2022]。篩選期即有 **640/7114 (9.0%)** 因 K⁺ >4.8 落選，凸顯「選對起點」的重要 [📄 label_guideline_safety_Wanner_2022]。

---

## 3. 重點三：禁忌與交互作用清單

### 3.1 禁忌（Contraindications）🟢

| | EMA SmPC | FDA KERENDIA PI |
|---|---|---|
| 過敏 | 對成分過敏 | 對任一成分過敏 |
| CYP3A4 | **併用強效 CYP3A4 抑制劑**（itraconazole、ketoconazole、ritonavir、nelfinavir、cobicistat、clarithromycin、telithromycin、nefazodone） | **併用強效 CYP3A4 抑制劑** |
| 腎上腺 | **Addison 氏病** | **腎上腺功能不全（adrenal insufficiency）** |

（EMA [📄 label_guideline_safety_European_2022]；FDA [📄 label_guideline_safety_Bayer_2025]）

### 3.2 保鉀／MRA 併用禁令與加成升鉀藥 🟢

- EMA 明文**禁止**與保鉀利尿劑（amiloride、triamterene）或其他 MRA（eplerenone、esaxerenone、spironolactone、canrenone）併用 [📄 label_guideline_safety_European_2022]。
- 與鉀補充劑／含鉀代鹽、trimethoprim 或 trimethoprim/sulfamethoxazole 併用時須小心並監測 K⁺（必要時暫停 finerenone）[📄 label_guideline_safety_European_2022]。
- 此與 KDIGO 2026 草案 Practice Point 4.4.7「Do not use steroidal and nsMRA concurrently」方向一致——因無同時使用類固醇型與 nsMRA 的研究，且預期高血鉀風險顯著增加，故應避免 [📄 KDIGO_2026_Diabetes_CKD_draft]。

### 3.3 CYP3A4 交互作用（量化細節交叉指向 `cyp3a4_interaction_prescribing_rules.md`）🟢🟡

finerenone 為 CYP3A4 受質，交互作用是禁忌與監測的藥動學根基（完整量化與處方規則見同資料夾 `cyp3a4_interaction_prescribing_rules.md`）：

- **強效 CYP3A4 抑制劑**：itraconazole 使 finerenone 的 AUC 增加 **more than 400%**——故強效抑制劑列為禁忌 [📄 label_guideline_safety_Ashjian_2023]。
- **中效 CYP3A4 抑制劑**（如 erythromycin、verapamil、diltiazem）：起始或調整時**監測 K⁺**、考慮 finerenone 或該藥的劑量調整 [📄 label_guideline_safety_Ashjian_2023] [📄 label_guideline_safety_Wanner_2022]。
- **CYP3A4 誘導劑**（rifampicin、carbamazepine、phenytoin、phenobarbital、St John's wort；中效如 efavirenz）：降低 finerenone 血中濃度、減弱療效，應避免 [📄 label_guideline_safety_Ashjian_2023] [📄 label_guideline_safety_Wanner_2022]。
- **葡萄柚**：應避免葡萄柚或葡萄柚汁 [📄 label_guideline_safety_Wanner_2022]。
- **藥動學背景**：finerenone 由 CYP3A4（~90%）與 CYP2C8 代謝、口服生體可用率約 **44%**、終末半衰期 **2 至 3 小時**、無活性代謝物——短半衰期正是「暫停 72 小時可處理多數高血鉀」的藥動學依據 [📄 label_guideline_safety_Ashjian_2023] [📄 KDIGO_2026_Diabetes_CKD_draft]。
- **選擇性佐證**：finerenone 對 MR 有 **500-fold** 選擇性，spironolactone、eplerenone 分別為 **3-fold、22-fold**——說明 nsMRA 較低性荷爾蒙副作用之機轉基礎 [📄 label_guideline_safety_Ashjian_2023]。
- **肝功能**：中度肝損（Child-Pugh B）使 finerenone AUC 增加 **38%**、未結合型 AUC 增加 **55%**（Cmax 不變），故 Child-Pugh B 應額外監測 K⁺、Child-Pugh C 應避免 [📄 label_guideline_safety_Ashjian_2023]。

---

## 4. 誠實邊界（Evidence limits）

- **KDIGO 2026 為尚未定稿草案** 🔴：所有 1A／4.4.x／Practice Point 引用限定於「2026 年 3 月 Chapter 4 公開審查草案」狀態，等級與措辭可能因回饋改變 [📄 KDIGO_2026_Diabetes_CKD_draft]。
- **KDIGO 2022 未 parse**：2022 版「2A、nsMRA 首度納入」係經 2024 版自述（defer + cross-reference）間接佐證，非直接引 2022 原文 [📄 note_kdigo2024]。
- **KDIGO 2020 無本地 parsed MD**：僅作背景時序敘述，不對其做條號／等級斷言；時間錨點為 finerenone EU 藥證 2022-02-16 [📄 label_guideline_safety_European_2022]。
- **2A→1A 升級的性質**：草案自述升級主要基於「可用性與熟悉度提高」及 Work Group 對「多數病人會選擇使用」的價值判斷，並非新增 hard-outcome RCT——升級屬 GRADE 判斷面（value/feasibility）之變動，而非新療效證據 [📄 KDIGO_2026_Diabetes_CKD_draft]。
- **EMA/FDA 起始門檻的措辭差**：EMA 對 K⁺ >4.8–5.0 保留「可考慮起始但加強監測」的灰帶，FDA 則以 >5.0 為硬性不起始線——臨床上兩者非矛盾，而是同一保守精神的不同顆粒度 [📄 label_guideline_safety_European_2022] [📄 label_guideline_safety_Bayer_2025]。

---

## 證據分層小結

| 論點 | 等級 | 主要本地全文來源 |
|------|------|------------------|
| KDIGO 2024 Rec 3.8.1 = 2A（suggest），Figure 26 監測 | 🟢 guideline | `label_guideline_safety_Kidney_2024` 📄／`label_guideline_safety_Levin_2024` 📄 |
| 2024 nsMRA 建議完全 defer 給 2022 指引、標 2A | 🟢 | `note_kdigo2024` 📄 |
| KDIGO 2026 草案 Rec 4.4.1 升為 1A（recommend） | 🔴 尚未定稿 | `KDIGO_2026_Diabetes_CKD_draft` 📄 |
| 2A→1A 理由＝可用性與熟悉度提高（非新 RCT） | 🔴 判斷面變動 | `KDIGO_2026_Diabetes_CKD_draft` 📄 |
| EMA/FDA 起始（>5.0 不起始）／CKD >5.5 vs HF >6.0 階梯 | 🟢 label | `label_guideline_safety_European_2022` 📄／`label_guideline_safety_Bayer_2025` 📄 |
| 監測節奏與 KDIGO RASi（2–4 週、<30% 續用）一致 | 🟢 | `label_guideline_safety_Wanner_2022` 📄／`label_guideline_safety_Levin_2024` 📄 |
| CYP3A4 禁忌／itraconazole AUC >400%／半衰期 2–3 h | 🟢🟡 | `label_guideline_safety_Ashjian_2023` 📄 |

## 本地全文語料（可 grep 稽核）

📄 全文：`label_guideline_safety_Kidney_2024`（KDIGO 2024 Rec 3.8.1、Figure 26）、`label_guideline_safety_Levin_2024`（KDIGO 2024 practice points 摘錄）、`note_kdigo2024`（2024 defer 2022、2A）、`KDIGO_2026_Diabetes_CKD_draft`（2026 草案 Rec 4.4.1／1A、PP 4.4.3／4.4.7）、`label_guideline_safety_European_2022`（EMA SmPC）、`label_guideline_safety_Bayer_2025`（FDA KERENDIA PI rev. 8/2025）、`label_guideline_safety_Wanner_2022`（鉀管理與 RASi 節奏對照）、`label_guideline_safety_Ashjian_2023`（藥動學／CYP3A4）。
（KDIGO 2020、KDIGO 2022 本地僅有 PDF／或缺，未 parse，故不逐字引用。）

---

## References（本地可稽核，Vancouver 風格）

1. Kidney Disease: Improving Global Outcomes (KDIGO) CKD Work Group. KDIGO 2024 Clinical Practice Guideline for the Evaluation and Management of Chronic Kidney Disease (Rec 3.8.1; Figure 26). Kidney Int. 2024;105(4S):S117–S314. 📄 [label_guideline_safety_Kidney_2024] [note_kdigo2024]
2. Levin A, Stevens PE, et al. KDIGO 2024 CKD Guideline — practice points on RASi/SGLT2i/nsMRA monitoring (PP 3.6.2, 3.6.3, 3.7.3, 3.8.1, 3.8.3). 📄 [label_guideline_safety_Levin_2024]
3. KDIGO Diabetes & CKD Work Group. KDIGO 2026 Clinical Practice Guideline for Diabetes Management in CKD — Public Review Draft, Chapter 4 (Rec 4.4.1 [1A]; PP 4.4.3, 4.4.7). March 2026. **尚未定稿**. 📄 [KDIGO_2026_Diabetes_CKD_draft]
4. European Medicines Agency; Bayer AG. Kerendia (finerenone) EPAR — Product Information / SmPC (Annex I). EMEA/H/C/005200; MA 2022-02-16. 📄 [label_guideline_safety_European_2022]
5. Bayer HealthCare Pharmaceuticals Inc. KERENDIA (finerenone) US Prescribing Information. NDA 215341; rev. 8/2025 (DailyMed). 📄 [label_guideline_safety_Bayer_2025]
6. Wanner C, et al. Potassium management with finerenone: practical recommendations from the FIDELIO-DKD/FIGARO-DKD program. 2022. 📄 [label_guideline_safety_Wanner_2022]
7. Ashjian E, et al. Finerenone: pharmacology, CYP3A4 interactions, and clinical use in CKD/T2D. 2023. 📄 [label_guideline_safety_Ashjian_2023]

---
*此檔為主題五之延伸拆解，撰寫日期基準 2026-07-11。所有具體條號／等級／數字均可 grep 回上列本地全文 MD；KDIGO 2026（1A）為公開審查草案・尚未定稿，KDIGO 2020／2022 本地未 parse，均已於文中明示邊界。*
