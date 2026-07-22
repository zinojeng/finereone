---
tags: [素材摘要, 統計迷思, NNT, 競爭風險, fragility index]
created: 2026-07-22
updated: 2026-07-22
sources: []
source_type: 筆記
source_path: raw/notes/04-statistical_insights_myths.md
images: 0
image_paths: []
---

# 統計迷思與深度解讀 · 主題四（臨床流行病學的統計陷阱）

> 五個「數字都對、結論卻錯」的陷阱：NNT 的三大內在缺陷、ITT vs on-treatment 的選擇偏差、競爭風險、比例風險假設失效、fragility index。

## 基本資訊
- **來源類型**：本地 Markdown 回顧稿
- **原文位置**：raw/notes/04-statistical_insights_myths.md
- **消化日期**：2026-07-22

## 核心觀點

1. **本檔的分工定位**。相對 vs 絕對、「各亞群一致 ≠ 人人同樣受益」、subgroup multiplicity、ICEMAN、risk-based HTE 已由姊妹檔 `methodology_subgroup_relative_vs_absolute.md` 完整處理，本檔**不重述**，只借經典錨點（statin 相對降 29.2% 一致，10 年風險 5% 者 ARR 1.5%、50% 者 14.6%📄）作入口，轉向下一層問題：把絕對受益濃縮成一個 NNT、或用單一 HR 概括整段追蹤時會踩到哪些坑。

2. **迷思一：NNT 不是可搬運的常數**。NNT = 1/ARR，而 ARR 隨三件事變動。**(a) 時間依賴**：FIDELITY stage 4 CKD 亞群（890 人，占 7%）的 Aalen–Johansen 累積發生率顯示，腎臟複合終點的 NNT 第 1 年 **41**、第 2 年 **19**、第 3 年 **−40**、第 4 年 **−20**（負值即 NNH，方向翻轉）；同一分析裡心血管複合終點的 NNT 卻穩定為 1/2/3/4 年 **29/29/31/24**📄🟡。一個「NNT ≈ 20」的斷言，不講時點等於沒講。

3. **(b) 信賴區間常被省略且可能極寬**。華人 FIDELIO ≥40% 腎臟終點 NNT **8，95% CI 4–84**（30 個月，ARR 12.2%，HR 0.59）📄；華人 FIGARO ≥40% 終點月 36 NNT **7，95% CI 4–22**📄。CI 上界 22、甚至 84，意思是真值可能要治療 84 人才防一件事。**(c) 不可跨基線風險移植**：FIDELITY 整體心血管 NNT **46（29–109）**、整體腎臟 NNT **60（38–142）**📄，不能套到高風險華人（腎臟 NNT 7–12）也不能套到低風險早期病人身上。

4. **迷思一的臨床亮點**。床邊正確說法是「在像您這樣的高風險（高 UACR、低 eGFR）病人、以 3 年為期，大約每 7 到 12 人可避免一次腎臟惡化事件」——時間窗、族群、不確定性一起交代。看到 stage 4 腎臟 NNT 第 3 年翻成 NNH，正確反應不是「後來有害」，而是「這是 PH 失效＋競爭風險的產物」，單一 NNT 在這裡本就不該被計算。

5. **迷思二：on-treatment 顯著、ITT 不顯著，不能挑顯著的用**。全因死亡 ITT **HR 0.89（0.79–1.00，P=0.051）**，事件數 finerenone 552 vs placebo 614；on-treatment **HR 0.82（0.70–0.96，P=0.014）**，事件數只剩 280 vs 344；CV 死亡 ITT 0.88（0.76–1.02，P=0.092）→ on-treatment 0.82（0.67–0.99，P=0.040）📄。**超過一半的死亡因為發生在停藥超過 30 天之後而被剔除**，而會停藥的人往往不是隨機的（因高血鉀、腎功能惡化、身體變差而停藥者本來預後就差），等於系統性替治療組「洗掉」高風險個案——informative censoring 造成的選擇偏差。

6. **迷思二的臨床亮點**。誠實講法是「finerenone 顯示降低死亡的趨勢，但 ITT 未達統計顯著（HR 0.89，P=0.051）」，不能講成「證實降低死亡率」。真正經得起考驗的硬訊號是**猝死**——在 **ITT** 族群就達顯著（**HR 0.75，95% CI 0.57–0.996，P=0.046**）📄。準則：**當 on-treatment 比 ITT 漂亮時，要警覺不是要慶祝。**

7. **迷思三：競爭風險**。在 CKD+T2D 尤其 stage 4，死亡與腎衰竭互相競爭：先死的人永遠不可能再進展到透析。把死亡當獨立設限會**高估**腎衰竭累積發生率（KM 隱含假設被 censor 者日後有相同事件率，而死人的事件率是零）。這正是 FIDELITY 腎臟分析採 **Aalen–Johansen 估計並明確把全因死亡當競爭風險**的原因📄。兩種 HR 要分清：**cause-specific hazard**（Cox 算出的 HR，如腎臟複合 0.77（0.67–0.88））適合談機轉／生物學效果；**subdistribution hazard（Fine–Gray）**適合談絕對負擔／衛生政策。晚期病人死亡率高，Aalen–Johansen 下競爭死亡吃掉後段腎臟事件空間，是 stage 4 腎臟 NNT 第 3、4 年翻負的部分成因。

8. **迷思四：比例風險假設失效**。FIDELITY stage 4 CKD 腎臟複合終點以 treatment×log(time) 交互檢定，**PH 假設不成立（P<0.01）**，作者因此**拒絕報告整段的 HR**，改報「**前 2 年 HR 0.63（0.42–0.95）**」，並明講保護只出現在頭 2 年📄。對應累積風險差：1 年 −2%（−5 至 0）、2 年 −5%（−10 至 −1）、3 年 +3%（−4 至 9）、4 年 +5%（−4 至 14）——先降後升，任何單一 HR 都無法誠實概括；整份 stage 4 分析因此被標為 **exploratory**。臨床含意反而積極：早期保護真實存在，支持在病人還沒走到最晚期時就介入。

9. **迷思五：fragility index**📌🔴。FI 問的是「要把多少個未發生事件的病人改成發生事件，顯著結果才會翻回不顯著」。Zuin 2026（**僅摘要**，不擴張細節）：FIDELIO-DKD 主要心血管複合雖顯著（HR 0.86、**NNT 56**），但 **FI 僅為 4**；合併後的 FIDELITY（HR 0.86、NNT 59）**FI 達 38**、FIDELITY 的 HF 住院終點（HR 0.78、NNT 91）**FI 23**，屬穩固訊號📌。（註：該分析僅納入 FIDELIO-DKD、FIGARO-DKD 與 pooled FIDELITY，**未**納入 FINEARTS-HF。）摘要並指出 CV 死亡／MI／中風等單項終點「favourable 但不顯著、reverse FI 低」，屬脆弱。臨床亮點：這正是為什麼**要引用合併分析（FIDELITY，FI 38）而非單一試驗**來支撐心血管論述。

10. **統計素養檢查表（查房／簡報用一頁）**：讀到一個 NNT → 問哪個時點、CI 多寬、哪個族群的基線風險；on-treatment 比 ITT 漂亮 → 問被 censor 的事件是否非隨機地偏向高風險者，主結論該用 ITT；腎臟／硬終點累積發生率 → 問有沒有把死亡當競爭風險；一個概括整段追蹤的 HR → 問 PH 假設成立嗎；「P<0.05 顯著」→ 問 FI 多少、是單一試驗還是合併分析；任何次分析結論 → 問這是拿來「校準判讀」還是被誤用來「改寫適應症」。

## 關鍵概念

[[NNT]]、[[NNH]]、[[競爭風險]]、[[競爭風險]]、[[比例風險假設]]、[[fragility index]]、[[ITT 分析]]、[[競爭風險]]、[[競爭風險]]、[[絕對風險差]]

## 與其他素材的關聯

- 本檔明示與 [[2026-07-22-04-methodology_subgroup_relative_vs_absolute]] 刻意互補不重複，兩者合為主題四的方法學雙軸。
- 迷思一的 NNT 案例（華人 8〔4–84〕、7〔4–22〕）來自 [[2026-07-22-04-cluster2_asian_chinese_japanese_subgroup]]；整體 NNT 46/60 來自 [[2026-07-22-04-cluster1_advanced_ckd_absolute_event_gradient]]。
- 迷思二的 ITT vs on-treatment 數字與 [[2026-07-22-04-cluster1_advanced_ckd_absolute_event_gradient]] 第 4 節同源（Filippatos 2023）。
- 迷思三、四的主要來源 `pooled_safety_hyperkalemia_Sarafidis_2023` 位於**主題五資料夾**，屬跨主題引用的本地全文。<!-- confidence: EXTRACTED -->
- 迷思四的 PH 失效解釋了 [[2026-07-22-04-cluster1_advanced_ckd_absolute_event_gradient]] 中 Bakris Figure 3「eGFR <30 之 HR 未計算」的原因。<!-- confidence: INFERRED -->
- 迷思五的 fragility 結論（引用合併分析而非單一試驗）與方法學檔「整體效果比單一亞群更可靠」的精神一致。

## 原文精彩摘錄

> NNT 看起來像一個物理常數，其實是一個**綁定了時間、綁定了族群、還常常藏起信賴區間**的估計值。

> 死亡不是「還沒發生的腎臟事件」，而是「讓腎臟事件不可能發生」的排他終點……這不是藥失效，而是族群的殘酷算術，反而支持「趁 eGFR 還沒掉到 stage 4 就早用」。

> 準則：**當 on-treatment 比 ITT 漂亮時，要警覺不是要慶祝。**

## 相關頁面
