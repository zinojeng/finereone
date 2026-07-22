---
tags: [素材摘要, 中介分析, 血鉀, 因果推論, 替代終點]
created: 2026-07-22
updated: 2026-07-22
sources: []
source_type: 筆記
source_path: raw/notes/05-potassium_mediation_of_cv_benefit.md
images: 0
image_paths: []
---

# 低血鉀減少 54% 是否「中介」了 finerenone 的心血管益處？

> 兩條平行下降的曲線（低血鉀 ↓54%、心律不整與 CV 事件 ↓13–14%）看似構成因果鏈，但正式 causal mediation 分析判決：血鉀**不中介** finerenone 的 CV 益處。

## 基本資訊
- **來源類型**：本地 Markdown 回顧稿
- **原文位置**：raw/notes/05-potassium_mediation_of_cv_benefit.md
- **消化日期**：2026-07-22

## 核心觀點

1. **誘人的平行關聯。** FIDELITY 中 finerenone 把嚴重低血鉀（K<3.5）從 placebo 的 10.2%（650/6403）壓到 4.8%（309/6420），**HR 0.46（95% CI 0.40–0.53）**＝相對下降約 **54%**；FINEARTS-HF 得到完全一致的 K<3.5 **HR 0.46（95% CI 0.38–0.56）**。同一族群 finerenone 把 CV 複合與心律不整複合分別降低 **14% 與 13%**，而 FIDELITY 心律不整複合終點的定義本身就包含 sudden cardiac death 📄 `label_guideline_safety_Pitt_2025`、`hf_renal_safety_Vardeny_2025`。

2. **「平行 ≠ 串聯」的方法學核心。** 兩種解釋畫出來的曲線一模一樣：(a) 中介路徑「finerenone → 矯正低血鉀 → 減少猝死」，血鉀是因果鏈中間那一環；(b) 共同上游「MR 阻斷」同時但各自獨立地生出兩個下游，兩下游之間沒有因果箭頭。要分辨只能做正式中介分析。

3. **兩個前提都成立，但都只是關聯。** 前提一（低血鉀確實被矯正）：K<4.0 從 48.3%（3094/6403）降到 33.9%（2174/6420），**HR 0.63（0.60–0.66）**；Jhund 2024 IPD meta（RALES/EMPHASIS/TOPCAT/FINEARTS，n=13,846）顯示 MRA 使低血鉀風險減半（**OR 0.51；95% CI 0.45–0.57；7% vs 14%**）📌 `hf_renal_safety_Jhund_2024`。前提二（低血鉀與壞結局相關）：K<3.5 對應 CV **HR 1.53**、心律不整 **HR 1.67**、全因死亡 **HR 1.56**；FINEARTS-HF time-updated 中 K<3.5 **HR 2.49（1.80–3.43）** > K>5.5 **HR 1.64（1.04–2.58）**。但前提二是**非隨機暴露**，低血鉀可能只是「病得更重」的 risk marker。

4. **Agarwal 2026 四中介分析是判決關鍵。** FIDELITY IPD（n=12,143），把第 4 個月四個 biomarker 變化同時當 mediator。四者都顯著改變：UACR ↓32.2%、SBP ↓3.6 mmHg、體重 ↓0.23 kg、**血鉀 ↑0.19 mEq/L（95% CI 0.17–0.20）**。中介比例：**UACR 39%（95% CI 7 to 71）✅**、**SBP 21%（95% CI 3 to 40）✅**、體重 4%（−1 to 9）❌、**血鉀 −1.5%（95% CI −38 to 7）❌ 不顯著且點估計為負** 📄 `albuminuria_mediation_Agarwal_2026`。

5. **作者的結論是直白的反證。** 「the protocol-permitted serum potassium increase **did not mediate** the cardiovascular benefit」、且「body weight and serum potassium are **not useful surrogates** for cardiovascular benefit」。UACR 與 SBP 合併中介 **50%（95% CI 21 to 100）**；剩下約一半歸因於 MR 阻斷對心肌、巨噬細胞、血管壁的直接抗纖維化與抗發炎效應 📄 `albuminuria_mediation_Agarwal_2026`。

6. **兩個補強細節。** (a) 穩健性：UACR 中介比例含交互 39%、不含交互 **36%（95% CI 7 to 64）**，兩模型一致，血鉀的不顯著非模型設定偶然。(b) 時間軸不支持血鉀路徑：CV 益處「emerges within months, before measurable kidney protection」（5 年 total effect relative mean survival **1.12；95% CI 1.04 to 1.21**），指向快速直接組織效應，而非需時間累積的電解質再置中。

7. **第二條獨立證據線：益處在高血鉀端仍維持。** FINEARTS-HF time-updated Cox 比較「發生 K>5.5 之前 vs 之後」的 finerenone 相對益處：**HR 0.84（0.55–1.30）vs 0.83（0.74–0.92），interaction P = 0.72**；FIDELITY 平行印證 CV 益處 **HR 0.86（0.78–0.95），P-interaction 0.95** 跨基線血鉀次組一致。若血鉀值真的決定臨床結局，益處早該在高血鉀端被抵消——但沒有。

8. **必須誠實的細緻區分：被反證的 ≠ 被檢定的全部。** 「血鉀**淨變化**（+0.19 mEq/L）中介 **CV 複合**」🟡 未支持中介（−1.5%，CI −38 to 7；「未達顯著」≠「證明零效應」）；「益處被高/低血鉀次組修飾」🟡 已被反證（P-int 0.95／0.72）；但「**嚴重低血鉀的矯正**是否中介**猝死**」🔴 **從未被任何正式 mediation 分析檢定**。落差有二：Agarwal 的 mediator 是全族群血鉀淨變化（一個小幅**上升**），概念上不同於「在原本會低血鉀的少數人身上把 K 拉回正常」；且因變數是 CV 複合而非猝死。Vardeny 自己也只寫「may relate to」的假說措辭。

9. **臨床意涵：別把血鉀正常化當療效替代指標。** Finerenone 的藥效端點是血鉀**小幅上升**（+0.19 mEq/L）而非下降，把「血鉀漂亮」讀成「藥在起作用」會方向性誤導；真正該追蹤的並行療效訊號是**月 4 的 UACR 與 SBP 反應**。反過來這讓 benefit-risk 更清爽：正因血鉀不中介益處，K>5.5（finerenone **HR 2.16**）是可用劑量調整/監測獨立管理的安全性議題，管理它**不會犧牲療效**。

10. **中介比例的精確度有限。** UACR 39%（7–71）、SBP 21%（3–40）、聯合 50%（21–100）——上界觸及 100% 表示「一半」是點估計而非窄區間；因果中介另依賴「mediator-outcome 無未測混淆」這一不可檢驗假設 🟡。

## 關鍵概念

- [[中介分析]]
- [[血鉀]]
- [[Finerenone]]
- [[UACR]]
- [[收縮壓]]
- [[FIDELITY]]
- [[FINEARTS-HF]]
- [[心律不整複合終點]]
- [[替代終點]]
- [[中介分析]]

## 與其他素材的關聯

- 本檔是 `05-hypokalemia_bidirectional_electrolyte.md` 的因果推論續篇：該檔建立「finerenone 減少低血鉀」的臨床事實，本檔判決該事實**不承載** CV 益處的傳遞。兩檔刻意互補不重複。<!-- confidence: EXTRACTED -->
- 原文明示與主題二 `uacr_sbp_mediation_of_cv_benefit.md` 正向互補：血鉀不中介，那什麼中介？UACR 39% + SBP 21% ≈ 一半。<!-- confidence: EXTRACTED -->
- 與 `05-statistical_insights_myths.md` 迷思三、四共用「關聯≠因果」「time-updated 非隨機暴露」的統計素養；本檔把該素養用在血鉀中介這一個具體命題上。<!-- confidence: EXTRACTED -->
- 與 `05-benefit_risk_discussion_nnt_nnh.md` 相接：「血鉀不中介益處」是「管理高血鉀不犧牲療效」這個處方安心感的機制根據。<!-- confidence: INFERRED -->
- Agarwal 2026 的「約一半 CV 益處來自未被捕捉的抗纖維化/抗發炎路徑」指向主題一的機轉層，但本檔未展開。<!-- confidence: AMBIGUOUS -->

## 原文精彩摘錄

> **淺白比喻**：兩條曲線平行下降，有兩種完全不同的解釋。(a)**中介路徑**——「finerenone → 矯正低血鉀 → 減少猝死」，血鉀是**串在因果鏈中間的那一環**；(b)**共同上游**——「finerenone → MR 阻斷」這個上游**同時、但各自獨立地**生出兩個下游……**平行 ≠ 串聯。要分辨，只能做正式的中介分析。**

> UACR 這一環被切斷，益處掉了 39%——所以它**是**中介；血鉀這一環被切斷，益處**紋風不動**（點估計甚至 −1.5%）——所以血鉀**不是**傳遞益處的路徑……這是本命題最強的一塊反證：不是「沒去驗」，而是**驗了、且驗出血鉀不中介**。

> 正確說法是：**「血鉀淨變化不中介 CV 複合」已被反證；「嚴重低血鉀矯正是否中介猝死」則尚未被檢定**，是一個開放的空缺，不能拿前者去宣稱後者、也不能拿「電生理合理」去填補它。

## 相關頁面

- [[中介分析]]
- [[Finerenone]]
- [[UACR]]
- [[血鉀]]
- [[FIDELITY]]
