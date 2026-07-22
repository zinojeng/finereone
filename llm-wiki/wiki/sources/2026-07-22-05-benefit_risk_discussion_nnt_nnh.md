---
tags: [素材摘要, 效益風險, NNT, NNH, 高血鉀]
created: 2026-07-22
updated: 2026-07-22
sources: []
source_type: 筆記
source_path: raw/notes/05-benefit_risk_discussion_nnt_nnh.md
images: 0
image_paths: []
---

# 爭議與對讀：把「多一種藥＝多抽血＋更多高血鉀」翻譯成 benefit-risk

> 反對 finerenone 的最強說法不是「它沒效」，而是「它讓門診多一種要盯血鉀的藥」；正確回應不是否認風險，而是把「相對加倍」翻譯成「絕對可管理」，並把 NNH 與 NNT 放上同一把尺。

## 基本資訊
- **來源類型**：本地 Markdown 回顧稿
- **原文位置**：raw/notes/05-benefit_risk_discussion_nnt_nnh.md
- **消化日期**：2026-07-22

## 核心觀點

1. **先承認：高血鉀確實加倍（跨試驗一致）🟡。** FIDELIO-DKD post hoc：treatment-emergent ≥mild 高血鉀（K⁺ >5.5）**597/2785（21.4%）finerenone vs 256/2775（9.2%）placebo**；≥moderate（K⁺ >6.0）**126/2802（4.5%）vs 38/2796（1.4%）**；作者明言高血鉀「was about twofold higher with finerenone than placebo and was the only AE/serious AE to demonstrate excess cases with finerenone」📄 `pooled_safety_hyperkalemia_Agarwal_2022`。Wanner 對讀：**14.0% vs 6.9%，"more than doubled"**，且此差距是在「其他升鉀藥被禁用、baseline K⁺ >4.8 已被排除」條件下仍出現 📄 `label_guideline_safety_Wanner_2022`。

2. **支點 (a)：絕對硬結局極低 🟡。** Pooled FIDELITY（>13,000 人）：**serious hyperkalaemia 1.1% vs 0.2%**、**住院 0.9% vs 0.2%**、**永久停藥 1.7% vs 0.6%** 📄 `label_guideline_safety_European_2022`；最硬的終點——「there were no hyperkalemia-related deaths in more than 13,000 patients over a median follow-up of 3 years」📄 `label_guideline_safety_Wanner_2022`。差異隨 eGFR 走：FIDELIO 住院 1.4% vs 0.3%、永久停藥 2.3% vs 0.9%；FIGARO 住院 0.6% vs 0.1%、永久停藥 1.2% vs 0.4%。

3. **支點 (b)：監測節奏本來就與 CKD 例行監測重疊 🟢。** 樞紐試驗血鉀量測節奏為 **Month 1、Month 4、其後每 4 個月**，Wanner 指出這「is actually similar with the usual biological monitoring recommended in CKD patients by the KDIGO 2012 guidelines」——UACR >300 mg/g 且 eGFR <60 者本就建議每年 3–4 次、UACR 30–300 者每年 2–3 次。**新增的抽血次數趨近於零。**

4. **支點 (c)：NNH 對照歷史，遠優於雙重 RASi 阻斷 🟡。** FIDELIO-DKD：**約需處方 71 名 finerenone 才有 1 名因高血鉀永久停藥**；對照已被放棄的雙重 RAS 阻斷——**VA NEPHRON-D NNH 18、ALTITUDE 45、ORIENT 26** 📄 `pooled_safety_hyperkalemia_Agarwal_2022`。同一份 VA NEPHRON-D 的 severe hyperkalemia（K⁺ >6.0 或需急診／住院／透析）為 **losartan 4.4% vs losartan+lisinopril 9.9%**。finerenone 的傷害門檻比那些組合寬約 4 倍。

5. **同尺對讀 NNT vs NNH。** 傷害端：高血鉀永久停藥 **NNH ≈ 71**。益處端：在最脆弱的 **Stage 4 CKD（eGFR <30；890/13,023 ＝ 7%）** 亞群，CV 複合終點 **HR 0.78（95% CI 0.57 to 1.07）**，Aalen–Johansen 對應 NNT 為 **1 年 29、2 年 29、3 年 31、4 年 24** 📄 `pooled_safety_hyperkalemia_Sarafidis_2023`；全體 FIDELITY 益處幅度 **腎複合 ↓23%（HR 0.77；95% CI 0.67–0.88）**、**心血管複合 ↓14%（HR 0.86；95% CI 0.78–0.95）**。天平明顯偏向益處，且傷害端可逆（停藥即解）、益處端是硬結局。

6. **Counter-advocate：五個成立的反問與邊界。** (i) Stage 4 NNT 為 **exploratory**，且腎複合 PH 假設 **not met**——「a protective effect only shown up to 2 years, after which the direction of association was inconsistent」，腎複合 NNT **3 年變 −40、4 年變 −20（負值即 NNH）**；只能說「前 2 年 HR 0.63（95% CI 0.42–0.95）」。(ii) CONFIDENCE 主要終點是 **180 天 UACR 變化**，屬代理終點，「合併治療降低硬結局」無專屬 RCT。(iii) FINEARTS-HF worsening renal function **17.7% vs 10.9%**，CKD+T2D 的 benefit-risk 不能無縫外推到 HFmrEF/HFpEF。(iv) 真實世界監測依從性——本地語料**無**資料可 grep，「可管理」嚴格說是「在被監測的前提下可管理」。(v) binder 續用證據以 surrogate 為終點。

7. **三層證據疊成一張投影片。** KDIGO 2024：nsMRA 為 **Rec 3.8.1，等級 2A**（normal serum potassium、eGFR >25、albuminuria、on max RASi）；KDIGO 2026 公開審查草案升為 **Rec 4.4.1，等級 1A**，並新增 **Practice Point 4.4.2**「SGLT2i 與 nsMRA 可同步起始」——**尚未定稿** 🔴。EMA/FDA label：K⁺ **≤4.8 可起始**、**>4.8 到 5.0** 可考慮但首 4 週加強監測、**>5.0 不起始**；起始/重啟/增量後 **4 週**複測；K⁺ **>5.5 暫停**，降至 **≤5.0 以 10 mg 重啟** 📄 `label_guideline_safety_European_2022`。

8. **合併 SGLT2i 未放大高血鉀。** CONFIDENCE：「combination therapy resulted in numerically lower rates of hyperkalemia compared with the finerenone arm alone in all KDIGO risk categories」——**數字上還略低** 📄 `hf_renal_safety_Vaduganathan_2025`；機轉相符：Agarwal post hoc 中 **SGLT-2i use OR 0.45（95% CI 0.27–0.75）** 降低高血鉀風險，KDIGO 2026 統合估計 **SGLT2i 降 hyperkalemia RR 0.79（95% CI 0.68–0.93）**。AKI 亦不放大（investigator-reported AKI「infrequent（≤3%）with combination therapy」）。

9. **Binder／飲食的定位校準：別把第二線工具當常規。** 樞紐試驗新起用 binder 者 FIDELIO **finerenone 10.9% vs placebo 6.5%**（Wanner 記 10.8% vs 6.5%）、FIGARO **4.5% vs 2.8%**。KDIGO 高血鉀處置階梯（Figure 32，K⁺ >5.5）：第一線＝檢視非 RASi 藥物（NSAID、trimethoprim）＋評估飲食鉀；第二線＝利尿劑、優化 bicarbonate、licensed potassium exchange agents；**最後手段**＝減量或停 RASi/MRA。KDIGO 逐字：「In early stages of CKD, high intake of foods naturally rich in potassium appears to be protective against disease progression, and dietary restriction…may be harmful to cardiac health; therefore, such restriction is not endorsed」📄 `label_guideline_safety_Kidney_2024`。

10. **四項明示的誠實邊界。** Stage 4 NNT 為 exploratory 且腎益處 2 年後翻轉 🟡🔴；combination 未放大高血鉀屬 UACR surrogate 🟡；NNH 71/18/45/26 為跨試驗換算、僅作量級對照 🟡；KDIGO 2026 為未定稿草案 🔴；「可管理」以 structured monitoring 為前提 🔴。**「風險 → hard-outcome 淨損益」之專屬前瞻 RCT 目前不存在。**

## 關鍵概念

- [[NNT]]
- [[NNH]]
- [[高血鉀]]
- [[Finerenone]]
- [[FIDELIO-DKD]]
- [[FIGARO-DKD]]
- [[FIDELITY]]
- [[KDIGO]]
- [[鉀離子結合劑]]
- [[相對風險與絕對風險]]

## 與其他素材的關聯

- 原文明示交叉連結：label 起始／暫停-重啟矩陣見 `05-label_guideline_safety_framework.md`；高血鉀情境工程見 `hyperkalemia_engineering_by_scenario.md`；eGFR dip 可逆見 `egfr_dip_hemodynamic_reversible.md`；hypokalemia 雙向見 `05-hypokalemia_bidirectional_electrolyte.md`；binder 續用見 `potassium_binder_role.md`。<!-- confidence: EXTRACTED -->
- 與 `05-statistical_insights_myths.md` 迷思一、二、六共用同一組數字（14.0% vs 6.9%、住院 0.9/0.2、停藥 1.7/0.6、NNH 71 vs 18/45/26、零高血鉀死亡、binder surrogate），但分工不同：本檔做 benefit-risk 論述，該檔做統計判讀層。<!-- confidence: EXTRACTED -->
- 本檔只算高血鉀端的傷害帳；`05-hypokalemia_bidirectional_electrolyte.md` 補上低血鉀端的保護，兩檔合起來才是完整的電解質淨損益。<!-- confidence: INFERRED -->
- 「管理高血鉀不犧牲療效」的機制根據見 `05-potassium_mediation_of_cv_benefit.md`（血鉀不中介 CV 益處）。<!-- confidence: INFERRED -->

## 原文精彩摘錄

> 反方主張成立的部分只有一句：finerenone 讓**高血鉀相對風險約 2 倍**，且需要例行血鉀監測。但「相對加倍」與「絕對可管理」是兩件事——當基期事件率極低、監測節奏本來就存在、退出與重啟規則明確時，2 倍的相對風險可以被工程化成一個「值得付的代價」。

> **同尺結論**：即使在最容易高血鉀的 Stage 4 族群，「約 24–31 人得 1 個心血管獲益」的 NNT，與「約 71 人得 1 個高血鉀永久停藥」的 NNH 相比，天平明顯偏向益處——而且傷害那一端是可逆的（停藥即解），益處那一端是硬結局。

> **校準後的敘事**：finerenone 的高血鉀多數用「監測＋暫停-重啟」即可管理；binder 與限鉀是保留給反覆 >5.5、Stage 4 或多重升鉀藥者的第二／末段工具，不是每個處方的附帶條件。

## 相關頁面

- [[NNT]]
- [[NNH]]
- [[高血鉀]]
- [[Finerenone]]
- [[KDIGO]]
