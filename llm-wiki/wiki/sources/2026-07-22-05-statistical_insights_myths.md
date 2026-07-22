---
tags: [素材摘要, 統計迷思, 安全性統計, NNH, 替代終點]
created: 2026-07-22
updated: 2026-07-22
sources: []
source_type: 筆記
source_path: raw/notes/05-statistical_insights_myths.md
images: 0
image_paths: []
---

# 統計迷思與深度解讀 · 主題五（安全性統計的臨床轉換）

> 把主題四「相對 vs 絕對」的錨點鏡像到**傷害端**：同一組高血鉀數字，用相對尺度製造恐懼、用絕對尺度顯示可管理，NNH 是兩者之間的翻譯橋。

## 基本資訊
- **來源類型**：本地 Markdown 回顧稿
- **原文位置**：raw/notes/05-statistical_insights_myths.md
- **消化日期**：2026-07-22

## 核心觀點

1. **迷思一：高血鉀「相對加倍」＝臨床災難。** 相對尺度（製造恐懼）：FIDELITY pooled 任一高血鉀 **14.0% vs 6.9%**；FIDELIO-DKD 校正多變量後 ≥mild 高血鉀 **HR 2.13（95% CI 1.86–2.45）**，原文明言 "twofold higher risk of hyperkalemia"。絕對尺度（顯示可管理）：因高血鉀**住院 0.9% vs 0.2%**、**永久停藥 1.7% vs 0.6%**。NNH 是橋：FIDELIO-DKD 約需處方 **71 名**才有 1 名因高血鉀永久停藥，對照被放棄的雙重 RAS 阻斷 NNH 僅 **18（VA NEPHRON-D）／45（ALTITUDE）／26（ORIENT）** 📄 `label_guideline_safety_European_2022`、`pooled_safety_hyperkalemia_Agarwal_2022`。常被忽略的細節：組間血鉀平均差最大僅 **0.23 mmol/L（月 4）**——RR 2 倍不等於鉀濃度飆高 2 倍，只是跨過門檻的人數比例多一倍。

2. **迷思二：「13,000 人零高血鉀死亡」＝零風險。** 零事件是三個大型資料集的一致觀察——Wanner「there were no hyperkalemia-related deaths in more than 13,000 patients over a median follow-up of 3 years」📄 `label_guideline_safety_Wanner_2022`；INFINITY（FIDELIO＋FIGARO＋FIND-CKD IPD）「no deaths attributable to hyperkalaemia」，因高血鉀永久停藥 **122（1.7%）vs 39（0.5%）** 📄 `pooled_safety_hyperkalemia_Neuen_2026`；FINE-HEART（n=14,180）「There were no deaths related to hyperkalemia in either treatment arm」📄 `hf_renal_safety_Ostrominski_2026`。

3. **rule of three（三的法則）是正確讀法。** 若 n 人中觀察到 0 次事件，發生率 95% 信賴上界約為 **3/n**；以 n≈13,000 代入約 **3/13,000 ≈ 0.023%**，即真實高血鉀致死率可能高達每約 **4,300 人 1 例**。兩層解讀：(a) 不是證明風險為零；(b) 但上界本身極低，足以支撐「絕對危害微乎其微」。**零事件的力量來自 n 很大，而不是來自「零」這個字**——這也是監測節奏不能因「零死亡」而取消的理由。

4. **迷思三：eGFR dip 的預後脫鉤＝「finerenone 讓 dip 變無害」。** 數字本身漂亮：FINEARTS-HF 中 ≥15% 初期 eGFR 下降在 finerenone 更常見（**23.0% vs 13.4%，OR 1.95**）；預後上安慰劑組的 dip 預示更差結局（**adjusted RR 1.50, 95% CI 1.20–1.89**），finerenone 組卻不然（**adjusted RR 1.07, 95% CI 0.84–1.35；P-interaction 0.04**），且療效橫跨整個 eGFR 變化範圍一致（**P-interaction 0.50**）📄 `hf_renal_safety_Matsumoto_2025`。

5. **但 dip 是 nonrandomized exposure。** 病人被隨機分到 finerenone/placebo，但沒有人被隨機分到「會不會 dip」；這是**條件於治療後變數**的分析，會削弱隨機化保護的可比性；「一致（P-int 0.50）≠ 更好」。Matsumoto 的臨床結論——初期 eGFR 下降是可預期的、不應自動導致停用 disease-modifying 藥物——**正確且可據以行動**，但應定位成「穩健的觀察關聯＋合理機轉」，而非隨機化證明的因果。

6. **迷思四：只監測高血鉀那一端就安全。** 血鉀與結局是 **U 形**。低血鉀端更常見：FIDELITY 治療浮現的 **K<4.0 達 41.1%、K<3.5 達 7.5%**；安慰劑組 4 年累積 K<4.0 **57.2%（95% CI 55.6–58.8）** vs K>5.5 僅 **10%（9.1–11.0）**。低血鉀端可能更致命：FINEARTS-HF time-updated Cox 中 K<3.5 **HR 2.49（95% CI 1.80–3.43）** 高於 K>5.5 的 **HR 1.64（95% CI 1.04–2.58）**；FIDELITY 平行結果最低 K<3.5 者 CV **HR 1.53**、心律不整 **HR 1.67**、全因死亡 **HR 1.56**。nsMRA 反而把血鉀往中央收斂（K<4.0 **HR 0.63**、K<3.5 **HR 0.46**）📄 `label_guideline_safety_Pitt_2025`、`hf_renal_safety_Vardeny_2025`。統計亮點：把血鉀當**連續變項＋time-updated**（用事件前最近一次血鉀，捕捉當下暴露）才能讓 U 形兩端風險同時浮現。

7. **迷思五：PBPK 的 fm、AUCR、「完全可逆」都是實測鐵證。** 三者都是模型陳述。(a) finerenone PBPK 估總 **fm_CYP3A4 ≈ 0.93（腸壁 0.42 ＋ 肝 0.51）**，與 Heinig 靜態估計（0.88、0.89）一致，傳播 90% CI 後範圍 **0.83–0.94**；**itraconazole AUCR 6.31、clarithromycin 5.28 是 predicted**，而 erythromycin 3.48、verapamil 2.70 才是實測 📄 `label_guideline_safety_Wendl_2022`。(b) Goulooze 的雙相模型「assuming **full reversibility of the acute eGFR decline** described the data well」——完全可逆是**能良好擬合資料的假設**；最接近實測的支持是停藥後 model-free eGFR **回升 6.9%（95% CI +3.9% 至 +10.0%）**，與模型預測 20 mg 急性下降 **5.4%** 相稱。(c) SGLT2i×finerenone 對急性 eGFR dip 的交互 **95% CI 73.2–120%** 跨越 100%（＝無交互）才判定無顯著修飾——這是「證據不足以否定獨立」，不是「證明完全獨立」；UACR 交互 CI 94.1–122%、慢性斜率交互 CI 9.5–144%（極寬、資訊量低）📄 `egfr_dip_reversibility_Goulooze_2022`。

8. **迷思六：binder 試驗「有效」＝改善硬結局。** 兩個關鍵試驗主要終點都是 surrogate。**AMBER**（patiromer + spironolactone；resistant HTN + CKD）：week 12 仍在使用 spironolactone 的比例由 **66.2%（98/148）提升至 85.7%（126/147），組間差 19.5%（95% CI 10.0–29.0），P<0.0001** 📄 `potassium_binders_monitoring_Agarwal_2019`。**DIAMOND**（patiromer + RAASi；HFrEF）：主要終點為血鉀調整後平均變化之組間差，並降低 **K⁺ >5.5 事件 HR 0.63（95% CI 0.45–0.87，P=0.006）** 📄 `potassium_binders_monitoring_Butler_2022`。代理終點鏈：binder → 血鉀受控 → 續用有效治療 →（外推）更好結局；前兩環有 RCT 支撐，最後一環**無專屬硬結局 RCT** 🟡。

9. **一頁式安全性統計素養檢查表。** 讀到「高血鉀風險加倍／HR 2.13」先問絕對事件率與 NNH；讀到「零高血鉀死亡」先問是零風險還是 n 大所以上界低；讀到「dip 在 finerenone 不預示壞結局」先問 dip 是否隨機分派、是否條件式分析；讀到「血鉀風險＝高血鉀」先問低血鉀那一端；讀到「AUCR 6.31／完全可逆／無交互」先問是 predicted、model-assumed 還是區間含無交互點；讀到「binder 試驗有效」先問主要終點是硬結局還是續用率／血鉀。

10. **明示的誠實邊界。** 迷思三之 dip 脫鉤為非隨機、條件式觀察關聯（非因果）；迷思五之 fm/AUCR/完全可逆/無交互為模型基礎推論；迷思六之 binder 主終點為 surrogate、無專屬硬結局 RCT。作者自己也提醒 Goulooze 分析中 SGLT2i 非隨機、量化效果須謹慎。**能行動 ≠ 已證明。**

## 關鍵概念

- [[NNH]]
- [[相對風險與絕對風險]]
- [[三的法則（rule of three）]]
- [[time-updated 分析]]
- [[替代終點]]
- [[高血鉀]]
- [[低血鉀]]
- [[eGFR dip]]
- [[PBPK 模型]]
- [[鉀離子結合劑]]

## 與其他素材的關聯

- 原文明示分工：benefit-risk 的 NNT/NNH 同尺權衡見 `05-benefit_risk_discussion_nnt_nnh.md`、雙向電解質見 `05-hypokalemia_bidirectional_electrolyte.md`、eGFR dip 血流動力學可逆見 `egfr_dip_hemodynamic_reversible.md`、binder 定位見 `potassium_binder_role.md`、CYP3A4 處方規則見 `cyp3a4_interaction_prescribing_rules.md`。本檔只借它們一句話當入口，轉向統計判讀層。<!-- confidence: EXTRACTED -->
- 迷思四與 `05-hypokalemia_bidirectional_electrolyte.md` 共用完整同一組低血鉀數字，是同一內容的統計視角版。<!-- confidence: EXTRACTED -->
- 迷思三的「非隨機暴露／條件式分析」正是 `05-potassium_mediation_of_cv_benefit.md` 判決血鉀不中介時所援引的統計素養基礎（該檔明示引用本檔迷思三、四）。<!-- confidence: EXTRACTED -->
- 迷思五的 Goulooze「完全可逆為模型假設」直接限定了 `05-uacr_rebound_reversibility_mechanism.md` 中「急性成分完全可逆」的證據強度。<!-- confidence: EXTRACTED -->
- 迷思一的 NNH 71 vs 18/45/26 與 `05-benefit_risk_discussion_nnt_nnh.md` 的傷害端完全重疊，兩檔互為論述與判讀。<!-- confidence: EXTRACTED -->

## 原文精彩摘錄

> 報高血鉀風險時，**永遠把相對倍率與絕對事件率、NNH 三者一起講**——單獨丟出「風險加倍」是統計上誠實、臨床上誤導。

> 零事件的力量來自 n 很大，而不是來自「零」這個字。……**罕見致命事件的『零』要配 rule of three 的上界一起讀**；上界夠低，才是「可以放心、但仍要監測」的依據。

> 模型輸出可以放心拿來做**方向性決策**……但講述時要標明「predicted／model-assumed／區間含無交互」。特別是「無顯著交互」——它常被過度讀成「證明兩藥互不影響」，正解是「在現有樣本下，看不出交互，但區間寬到不能排除」。這是把統計謙遜寫進處方語言：**能行動 ≠ 已證明**。

## 相關頁面

- [[NNH]]
- [[高血鉀]]
- [[低血鉀]]
- [[eGFR dip]]
- [[替代終點]]
