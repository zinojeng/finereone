# Claim Audit — background_guideline_placement_four_pillars.md

稽核方式：逐句抽取帶 [本地MD檔名] 標註之百分比/樣本數/HR/OR/RR/CI/引號字串，grep 回 `原始PDF/<檔名>.md` 逐字核對。

## 結論：全數 CONFIRMED，無 GREP_FAIL

檢核項目與結果：

1. **note_kdigo2024** — Rec 3.8.1 (2A)、PP 3.8.2、eGFR>25、albuminuria>30mg/g、Figure 18「first-line drug therapy for most patients」「targeted therapies」、Rec 3.7.1(1A, eGFR≥20)、Rec 3.6.1/3.6.3(1B)、三項證據缺口敘述 ✅ 全部逐字命中。

2. **guideline_position_de_2022** — layered therapy 定義、"Finerenone is currently the only ns-MRA with proven clinical kidney and cardiovascular benefits"（逐字引號命中 L83）、"additive, based on preclinical studies"／"further clinical research on these combinations is needed"（逐字命中 L264）、FIDELITY 18%/23%/20%/22%、13,191 total participants（逐字命中 L262）、SGLT2i 降低高血鉀風險 ✅ 全部命中。

3. **KDIGO_2026_Diabetes_CKD_draft** — Rec 4.4.1 全文逐字（含 1A）✅；"greater availability and familiarity"逐字命中✅；7 studies (41 reports)✅；統合表 9 個效應量（腎複合 HR 0.84[0.77–0.92]、kidney failure 0.84[0.71–0.99]、HF 0.78[0.66–0.92]、全死因 RR 0.90[0.81–1.00]、CV死亡 RR 0.88[0.76–1.02]、stroke RR 1.01[0.83–1.22]、MI RR 0.92[0.75–1.13]、hyperkalemia RR 2.09[1.82–2.39]、K≥5.5 RR 2.18[1.98–2.40]）逐字命中同一段（L3290-3294）✅；PP 4.4.2 全文逐字命中✅；CONFIDENCE 29%（LSM 0.71;0.61–0.82）／32%（0.68;0.59–0.79）逐字命中（L3306, L3348）✅；Rec 4.7.1(2C) T1D 全文逐字命中✅；Rec 4.5.1(1A) GLP-1 逐字命中✅；Figure 19「comprehensive strategy」逐字命中✅；foundational/additional risk-based pharmacotherapy 分類命中✅；"Direct head-to-head comparisons were not available..."逐字命中✅；"did not appear to mitigate the effect of hyperkalemia"逐字命中（L3348，非L3330之"issue"版本，文中用字正確對應到後者段落）✅。

4. **r2_Agarwal_2023** — HHF 25–35%✅、GLP-1RA 11 trials MI 11%✅、CREDENCE 30%／FIDELIO-DKD 18%✅、513,165 T2D adults✅、UACR 測試率 20/50/100% → 6/15/30%✅ 全部逐字命中。

5. **glp1_cardiorenal_Neuen_2024** — n=14,543（CANVAS+CREDENCE）✅、n=60,080（GLP-1RA 8 trials）✅、n=13,026（nsMRA 2 trials）✅、3,482 人✅、中位追蹤 2.5 年✅；單一支柱 HHF HR 表：SGLT2i 0.64(0.53–0.77)、nsMRA 0.78(0.66–0.92)、GLP-1RA 0.89(0.82–0.98) 全數命中✅；三藥合用 MACE 0.65(0.55–0.76)、HHF 0.45(0.34–0.58)、CKD 0.42(0.31–0.56)、CV death 0.64(0.51–0.80)✅；3年 ARR 4.4%(3.0–5.7)、NNT 23(18–33)✅；終生投射 MACE 3.2y(2.1–4.3)、HHF 3.2y(2.4–4.0)、CKD 5.5y(4.0–6.7)、CV death 2.2y(1.2–3.0)✅；50% additivity 敏感度分析 MACE 2.4y(1.1–3.5)、CKD 4.5y(2.8–5.9)、全死因 1.8y(0.7–2.8)✅ — 特別注意：全死因 1.8y 取自「50% additivity」段落（原文L142），非主模型之 2.4y(1.4–3.4)，文中未混淆兩者，正確。

6. **note_fidelity** — 13,026、UACR 30–5,000、eGFR≥25、mean eGFR 57.6、median UACR 515、追蹤 3.0年(IQR 2.3–3.8)、CV HR 0.86(0.78–0.95) P=0.0018 NNT46、腎 HR 0.77(0.67–0.88) P=0.0002 NNT60、HHF 0.78(0.66–0.92)、ESKD 0.80(0.64–0.99)、UACR 32%降幅 ratio 0.68(0.66–0.70)、高血鉀停藥 1.7% vs 0.6%、全死因P=0.051 ✅ 全部逐字命中；且原文明確標註「非正式 powered、exploratory p值、無multiplicity校正」，文中對應敘述誠實對應，未誤讀。

7. **hyperkalemia_combo_Rossing_2022** — 877/13,026(6.7%)✅、CV HR 無SGLT2i 0.87(0.79–0.96) vs 有 0.67(0.42–1.07) P-interaction=0.46✅、腎 HR 無 0.80(0.69–0.92) vs 有 0.42(0.16–1.08) P-interaction=0.29✅、高血鉀 有SGLT2i finerenone10.3% vs placebo2.7%、無SGLT2i 14.3% vs 7.2%✅ 全部逐字命中；設計標示「prespecified pooled analysis」與原文一致（非 post hoc）。

8. **hyperkalemia_combo_Wen_2026** — PROSPERO CRD420251023918✅、搜尋至2025-06-06（原文"6 June 2025"）✅、8 studies（5 RCT + 3 retrospective cohort，原文"Five RCTs and three retrospective cohort studies"）✅、71,567✅；vs finerenone單藥：全死因OR 0.58(0.36–0.93)、MACE 0.70(0.51–0.97)、MAKE 0.63(0.44–0.89)、高血鉀1.09(0.52–2.28)無顯著✅；vs SGLT2i單藥：全死因0.73(0.47–1.13)、MACE0.77(0.55–1.08)、MAKE0.87(0.58–1.31)均未達顯著、高血鉀3.00(2.50–3.61)顯著↑✅；TSA「未越過monitoring boundary」逐字對應✅；GRADE：全死因/UACR moderate、MACE/MAKE low、hyperkalemia very low✅；UACR分析為組內pre-post變化（非組間直接比較）✅ 全部逐字命中，且文中正確標示 Wen 混合 RCT 與觀察性研究、SGLT2i使用為回溯辨識（information bias）之誠實邊界。

9. **combination_editorial_Cheng_2025** — 513,165（實際出自r2_Agarwal_2023,交叉引用一致）、STRONG-HF N=1078、"risk ratio 0.66; 95% CI 0.50–0.86"逐字命中✅。

## 特別檢查結果

- **研究設計標示**：FIDELITY／Rossing 2022 正確標為「prespecified pooled/subgroup」（非post hoc）；Neuen 2024 正確標為「跨試驗間接比較＋actuarial 投射」（非head-to-head RCT）；Wen 2026 正確標示「5 RCT + 3 retrospective cohort」混合設計；KDIGO 2026 正確標示「公開審查草案，尚未定稿」🟡，未被誤植為定稿指引常規。無 RCT/cohort 誤植。
- **數字位數**：抽查之樣本數（13,026、13,191、14,543、60,080、877、71,567、513,165、3,482、1078）與原文位數完全一致，無 confabulated digit（如 n=133 vs n=1330 類錯誤）未發現。
- **引號逐字比對**：所有帶引號之英文原文句子（"We recommend adding a nonsteroidal..."、"greater availability and familiarity..."、"Finerenone is currently the only ns-MRA..."、"Direct head-to-head comparisons were not available..."、"did not appear to mitigate the effect of hyperkalemia"）均逐字命中原文，無 quote fabrication。
- **P值/顯著性判讀**：文中對「未達顯著」（如全死因RR 0.90[0.81–1.00]、CV死亡RR 0.88[0.76–1.02]等）之描述均正確使用「未達顯著」而非誤稱「證明無差異」；全死因死亡P=0.051（FIDELITY）亦正確標為「未達顯著」而非「無差異」。
- **abstract_only 誤用檢查**：本檔引用之 9 個來源檔（note_kdigo2024、guideline_position_de_2022、KDIGO_2026_Diabetes_CKD_draft、r2_Agarwal_2023、glp1_cardiorenal_Neuen_2024、note_fidelity、hyperkalemia_combo_Rossing_2022、hyperkalemia_combo_Wen_2026、combination_editorial_Cheng_2025）經檢查均為全文（📄），檔案存在且非空（1.6KB–540KB不等），文中未見引用僅有 abstract 之檔案（如 confidence_trial_Mottl_2025、confidence_trial_McGill_2026 等 abstract_only 檔）之具體數字斷言。

## 總結

background_guideline_placement_four_pillars.md 中所有帶來源標註的數字、效應量、引號字串、研究設計描述，逐一 grep 回本地全文 MD 均逐字命中，無 ❌GREP_FAIL 項目。全文通過稽核。
