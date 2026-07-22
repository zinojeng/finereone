# 方法學對讀 · 相對 vs 絕對、multiplicity、可信度評估與風險基礎 HTE

> 本檔為主題四（誰得到最大效益）之延伸拆解＋簡報數據集，把主文 §6「方法學對讀」獨立擴充成專科化、且**用更淺白語言**說明「怎麼正確讀次族群」的骨架。
>
> **引用標記慣例**：📄 = 本地全文可 grep 稽核；📌 = 僅取得 abstract。每個數字句末以 `[本地MD檔名]` 標註來源供 grep 回溯。
>
> **證據分層**：🟢 已確立方法學共識｜🟡 post hoc／觀察性｜🔴 假說。
>
> **一句話定位**：多數 subgroup 資料的用途是「**校準臨床判讀**」，不是「重寫 eligibility」；而「consistent across subgroups（各亞群一致）」必須被正確翻譯成「**絕對受益隨基線風險放大**」，不能被誤講成「人人同樣受益」。

---

## 1. 相對 vs 絕對：為什麼「各組一樣」反而保證「絕對受益不一樣」🟢

**先用白話講**：藥物的效果有兩種講法——「打幾折（相對效果／HR）」和「省多少錢（絕對效果／ARR）」。臨床試驗裡，「打幾折」在不同風險的病人身上通常**很穩定**；但同樣打七折，本來風險高的人省下的**絕對數字**就大得多。所以「各亞群 HR 一樣」不是「人人受益一樣」，恰恰相反——它**保證**了高風險族群的絕對受益更大。

Sun 2010 把這件事講成一條定理：相對效果在多數情況下跨基線風險恆定，而絕對風險下降必隨基線風險變動；**若已知的預後因子能定義不同風險組、而相對效果無異質性，則絕對效果的 subgroup effect 就「必然存在」**[subgroup_methodology_Sun_2010] 📄。其 statin 範例最直觀：相對降 **29.2%** 一致，但 10 年基線風險 5% 的人 ARR 僅 **1.5%**、50% 的人 ARR 高達 **14.6%**——同一個 RRR，ARR 差了近 10 倍 [subgroup_methodology_Sun_2010] 📄。

**套回 finerenone**：主文各叢集的「不顯著交互」——Agarwal 2023 的 eGFR×UACR 交互 P=0.66、Bakris 2023 的 P-interaction 0.62/0.67、Neves 2026 的各 P-interaction 0.61–0.75——**正是「絕對受益梯度」的保證書**，而不是「人人一樣」的證據 [stage4_ckd_Agarwal_2023] 📄 [stage4_ckd_Bakris_2023] 📄 [baseline_goals_absolute_Neves_2026] 📄。這是全主題的方法學樞紐。

---

## 2. Multiplicity、power 與「方向相反」交互的稀有性 🟢

**先用白話講**：一個試驗切出十幾個亞群、每個都做檢定，總會有幾個「看起來有差」純粹是運氣。真正該擔心的不是「程度差一點」，而是「方向相反」（某亞群反而有害）——而後者其實**非常罕見**。所以看到某個小亞群「無效」甚至「有害」的極端數字，第一直覺應該是「樣本太小的雜訊」，而不是「這群人真的不一樣」。

- **Yusuf 1991**：量化交互（程度差異）常見且多為真；**質化交互（方向相反）罕見且多為假**。因此「整體結果」通常比「某亞群內的表面效果」更能指引該亞群的真實方向；GISSI 鏈激酶「只在前壁 MI、<65 歲、<6 小時有效」後來被證明是 power 不足造成的假象 [r2_Yusuf_1991] 📄。
- **對 finerenone 的直接啟示**：華人／亞洲心血管終點「不顯著」、華人 FIGARO 非致死 MI「HR 4.75（CI 0.55–40.75）」這類極端點估計，幾乎確定是**小樣本雜訊**，不該被解讀為「finerenone 對華人心臟無效或有害」；整體 CV HR 0.86 才是這些亞群更可靠的方向指引 [asian_subgroup_Li_2025] 📄。
- **Assmann 2000**：多數試驗呈現 subgroup 卻**缺乏適當的交互檢定**、且過度強調 subgroup；應事前擬定 baseline 資料分析計畫 [r2_Assmann_2000] 📄。
- **Wallach 2017**：64 個 RCT 摘要中 **117 項** subgroup 宣稱，僅 **39.3%** 有顯著交互支持；其中僅 34.8% 有分層隨機、28.3% 事前設定、**僅 2.2% 校正多重比較**；曾被嘗試重現的 5 項**全部無法重現、效果量向虛無收斂** [subgroup_methodology_Wallach_2017] 📄。這是「publication layering（層層堆疊的次分析論文）」最有力的警示——其顯著訊號的先驗可信度本就偏低。

---

## 3. 可信度評估工具：ICEMAN 與 credibility criteria 🟢

**先用白話講**：不是每個「亞群有差」都同等可信。有一套結構化的問句可以幫你打分數：這個亞群是不是事前設定的？有沒有生物學理由？是不是只有這一個亞群跳出來？有沒有校正多重比較？分數低的，就當「假設」看，別拿去改處方。

**Schandelmaier 2020 的 ICEMAN 工具**（RCT 5 題、統合分析 8 題核心問項＋視覺類比信度評分）提供結構化評估；其開發指出約 **14–26%** 的 RCT／統合分析會在摘要或討論強調至少一項效果修飾，而「錯誤宣稱的根本原因是機率（chance）」——即使真實效果對所有病人相同，檢驗夠多候選變項必然出現表面上的效果修飾 [subgroup_methodology_Schandelmaier_2020] 📄。

**用 ICEMAN／Sun 的精神快速稽核 finerenone 的訊號**：

| 訊號 | 方向合理？ | 事前？多重校正？ | 可信度判定 |
|---|---|---|---|
| LVH × HHF（P=0.0024） | 合理（MR 活化與 LVH 相關） | 事後、ECG 無中央裁決、未校正 | **中低** → hypothesis-generating [hf_kidney_spectrum_Filippatos_2024] 📄 |
| 亞洲 × 腎臟（P=0.0009–0.0493） | 合理（鈉敏感／高鹽機轉） | 跨多獨立分析方向一致，但華人單獨 P-interaction 不顯著 | **較高，但仍屬「校準」非「重寫適應症」** [stage4_ckd_Wada_2025] 📄 [asian_subgroup_Raza_2025] 📄 [asian_subgroup_Li_2026] 📄 |

---

## 4. 風險基礎的 HTE：比單變量 subgroup 更貼近門診 🟢

**先用白話講**：與其一個一個問「亞洲人？stage 4？有心衰？」，不如把病人的風險因子**加起來**算一個「整體基線風險」，再看效益。因為同一個試驗裡，病人之間的風險差距其實非常大，多數人的風險還低於「試驗平均值」——用平均值講效益，會誤導。

**Kent 2016**（32 個大型試驗、39 分析）證實：試驗族群內結果風險常有巨大異質性（極端四分位風險比 EQRR 中位 **4.3**、最高達 **50.7**），**多數病人的風險低於試驗平均值**；在 18 個整體顯著的比較中，只有 1 個在比例尺度上有顯著的「治療×基線風險」交互，但**極端風險四分位間的絕對風險下降差異中位 5.1%、四分之一試驗超過 10%** [subgroup_methodology_Kent_2016] 📄。**Kent 2018** 進一步主張以「reference class forecasting／多變量風險模型」取代單一變量 subgroup，才能給個別病人更貼身的效益預測 [subgroup_methodology_Kent_2018] 📄。

> **對 finerenone 的整合結論**：與其逐一問單變量亞群，不如以 **eGFR × UACR（±HF 病史、±LVH）構成的多維風險**估計個別病人的**基線絕對事件率**，再乘上穩定的相對效果（CV ~14%、腎臟 ~23%），得到個人化的 ARR/NNT。這就是從 average treatment effect 走向 precision-layered 判讀的操作定義。

---

## 5. 穩健性補充（fragility）🟡

Zuin 2026 對 finerenone 心血管結果做 fragility 分析（納入 FIDELIO、FIGARO、FIDELITY）；**僅取得摘要（📌）**，已知 FIDELIO 主要複合 CV NNT **56** [baseline_goals_absolute_Zuin_2026] 📌。fragility index 的細節未能取得，故不對其穩健性作具體斷言。

---

## 📊 簡報數據參考（從原文圖／表擷取）

> 供做投影片時直接引用；每列附來源檔，做簡報前可回原文二次核對。

### 表 M-1 — 「相對一致 → 絕對放大」的教學數字
| 概念 | 數字 | 來源檔 |
|---|---|---|
| statin RRR（一致） | 29.2% | `subgroup_methodology_Sun_2010` |
| 10 年風險 5% → ARR | 1.5% | `subgroup_methodology_Sun_2010` |
| 10 年風險 50% → ARR | 14.6% | `subgroup_methodology_Sun_2010` |
| finerenone eGFR×UACR 交互 P | 0.66 | `stage4_ckd_Agarwal_2023` |
| finerenone Bakris P-interaction | 0.62 / 0.67 | `stage4_ckd_Bakris_2023` |

### 表 M-2 — 為何「subgroup 訊號」先驗可信度低（Wallach 2017）
| 指標 | 數字 |
|---|---|
| subgroup 宣稱總數（64 RCT 摘要） | 117 |
| 有顯著交互支持 | 39.3% |
| 有分層隨機 | 34.8% |
| 事前設定 | 28.3% |
| 校正多重比較 | **2.2%** |
| 嘗試重現者（5 項） | 全部無法重現、向虛無收斂 |

（全列 `subgroup_methodology_Wallach_2017`。）

### 表 M-3 — 風險基礎異質性（Kent 2016）
| 指標 | 數字 | 來源檔 |
|---|---|---|
| 試驗數 / 分析數 | 32 / 39 | `subgroup_methodology_Kent_2016` |
| 極端四分位風險比 EQRR（中位 / 最高） | 4.3 / 50.7 | `subgroup_methodology_Kent_2016` |
| 極端風險四分位間 ARD 差（中位） | 5.1% | `subgroup_methodology_Kent_2016` |
| ICEMAN：RCT/統合強調≥1 效果修飾 | 14–26% | `subgroup_methodology_Schandelmaier_2020` |

### 表 M-4 — 次族群判讀檢查清單（簡報用一頁）
| 問題 | 通過 = 較可信 |
|---|---|
| 事前設定（prespecified）？ | 是 |
| 有分層隨機？ | 是 |
| 校正多重比較？ | 是 |
| 交互檢定顯著（非僅組內 P）？ | 是 |
| 方向為量化（非方向相反）？ | 是 |
| 有生物學／機轉理由？ | 是 |
| 跨多個獨立資料一致？ | 是 |
| 整體結果本身穩健？ | 是 |

（清單綜合 Sun 2010 / Yusuf 1991 / Assmann 2000 / Wallach 2017 / ICEMAN / Kent 之判準；用途為「校準」而非「重寫適應症」。）

---

## 證據分層小結

| 論點 | 等級 | 主要本地全文來源 |
|---|---|---|
| 相對一致 → 絕對受益必放大（statin 29.2% → ARR 1.5% vs 14.6%） | 🟢 | `subgroup_methodology_Sun_2010` 📄 |
| 質化交互罕見、多為假（整體 > 亞群） | 🟢 | `r2_Yusuf_1991` 📄 |
| subgroup 宣稱僅 2.2% 校正多重、多不可重現 | 🟢 | `subgroup_methodology_Wallach_2017` 📄 |
| 效果修飾多源於 chance（14–26% 過度強調） | 🟢 | `subgroup_methodology_Schandelmaier_2020` 📄 |
| 風險基礎 HTE（EQRR 4.3、ARD 差 5.1%）> 單變量 subgroup | 🟢 | `subgroup_methodology_Kent_2016`／`Kent_2018` 📄 |
| finerenone fragility（NNT 56） | 🟡（abstract） | `baseline_goals_absolute_Zuin_2026` 📌 |

## 本地全文語料（可 grep 稽核）

📄 全文：`subgroup_methodology_Sun_2010`（BMJ，相對 vs 絕對準則）、`r2_Yusuf_1991`（質化 vs 量化交互）、`r2_Assmann_2000`（subgroup 分析陷阱）、`subgroup_methodology_Wallach_2017`（subgroup 宣稱可重現性）、`subgroup_methodology_Schandelmaier_2020`（ICEMAN）、`subgroup_methodology_Kent_2016`（風險基礎 HTE）、`subgroup_methodology_Kent_2018`（PATH / reference class）。
📌 abstract：`baseline_goals_absolute_Zuin_2026`（fragility）。
（finerenone 側佐證：`stage4_ckd_Agarwal_2023`、`stage4_ckd_Bakris_2023`、`stage4_ckd_Wada_2025`、`asian_subgroup_Li_2025/2026`、`asian_subgroup_Raza_2025`、`hf_kidney_spectrum_Filippatos_2024`、`baseline_goals_absolute_Neves_2026`——詳見叢集一～三檔。）

---

## References（Vancouver 風格，含本地檔）

1. Sun X, Briel M, Walter SD, Guyatt GH. Is a subgroup effect believable? Updating criteria to evaluate the credibility of subgroup analyses. BMJ. 2010;340:c117. 📄 [subgroup_methodology_Sun_2010]
2. Yusuf S, Wittes J, Probstfield J, Tyroler HA. Analysis and interpretation of treatment effects in subgroups of patients in randomized clinical trials. JAMA. 1991;266(1):93-98. 📄 [r2_Yusuf_1991]
3. Assmann SF, Pocock SJ, Enos LE, Kasten LE. Subgroup analysis and other (mis)uses of baseline data in clinical trials. Lancet. 2000;355(9209):1064-1069. 📄 [r2_Assmann_2000]
4. Wallach JD, Sullivan PG, Trepanowski JF, et al. Evaluation of evidence of statistical support and corroboration of subgroup claims in randomized clinical trials. JAMA Intern Med. 2017;177(4):554-560. 📄 [subgroup_methodology_Wallach_2017]
5. Schandelmaier S, Briel M, Varadhan R, et al. Development of the Instrument to assess the Credibility of Effect Modification Analyses (ICEMAN). CMAJ. 2020;192(32):E901-E906. 📄 [subgroup_methodology_Schandelmaier_2020]
6. Kent DM, Nelson J, Dahabreh IJ, et al. Risk and treatment effect heterogeneity: re-analysis of individual participant data from 32 large clinical trials. Int J Epidemiol. 2016;45(6):2075-2088. 📄 [subgroup_methodology_Kent_2016]
7. Kent DM, Steyerberg E, van Klaveren D. Personalized evidence based medicine: predictive approaches to heterogeneous treatment effects (PATH statement). BMJ. 2018;363:k4245. 📄 [subgroup_methodology_Kent_2018]
8. Zuin M, et al. Fragility analysis of cardiovascular outcomes with finerenone. 2026 (abstract). 📌 [baseline_goals_absolute_Zuin_2026]

---
*此檔為主題四之延伸補充，撰寫日期基準 2026-07-11。所有具體數字均可 grep 回上列本地全文 MD；Zuin 2026 僅取得摘要，其穩健性細節不作具體斷言。*
