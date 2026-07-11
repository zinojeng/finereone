# 初期 eGFR dip：血流動力學、可逆，且不該觸發停藥

> 本文為主題五（高血鉀與 eGFR dip 的安全工程學）之延伸拆解，把主文 §4「初期 eGFR dip」獨立擴充成專科化版本。核心命題：finerenone 起始後的初期 eGFR 下降是**血流動力學性、雙相型、可逆**的，且其與後續腎臟結局的關係在 finerenone 身上已「**脫鉤**」——因此不應把它當成停藥訊號。
>
> **引用標記慣例**：📄 = 本地全文可 grep 稽核；📌 = 僅取得 abstract（不對其未載內容作具體數字斷言）。每個數字句末以 `[本地MD檔名]` 標註來源供 grep 回溯。LLM 僅負責組織與改寫，所有作者／年份／數字均出自本地 MD 檔。
>
> **證據分層**：🟢 guideline routine（已進指引常規）｜🟡 evidence expansion（enabling／post hoc／surrogate／模型分析）｜🔴 尚待驗證（無直接 hard-outcome RCT 佐證，或屬未定稿草案）。

---

## 0. 一句話定位

初期 eGFR dip 不是腎損傷，而是**濾過壓下修的血流動力學指紋**——與 RAAS 阻斷、SGLT2i 同源的 class 現象。它可逆、雙相、幅度小；在 finerenone 身上，dip 甚至**不再預示更差的腎臟結局**。真正有代價的不是 dip，而是**因為看到 dip 而過早停藥**。

---

## 1. dip 的本質與量化

### 1.1 指引怎麼定義「該不該擔心」 🟢

KDIGO 2024 把 eGFR dip 寫入 **Practice Point 2.1.4**：對啟動血流動力學活性療法的 CKD 病人，**GFR 下降 >30%** 於後續檢測才「超出預期變異、需要評估」[label_guideline_safety_Kidney_2024]。指引明列 **10%–20% 的初期下降屬典型**（首 3 個月內），且為「hemodynamically mediated」，是血壓低於自我調節下閾的反應；多數為暫時、會隨 autoregulatory function 重設而穩定或回復；因此「acute rises in SCr (or declines in eGFR) of <20%–30% are expected and do not warrant changes in therapeutic agents」[label_guideline_safety_Kidney_2024]。這個現象「especially common when using ACEi/ARBs … and SGLT2i through similar hemodynamic mechanisms」——指引本身即把它定位為 class 現象 [label_guideline_safety_Kidney_2024]。與此並列的 **Practice Point 3.6.4**：除非 SCr 於起始後 4 週內上升 >30%，否則續用 ACEi/ARB [label_guideline_safety_Kidney_2024]。

### 1.2 finerenone 的 dip 幅度：小 🟡

EMA 產品文件記載 finerenone 初期 eGFR 下降**平均約 2 mL/min/1.73 m²**，隨時間衰減、於持續治療下 appeared reversible [label_guideline_safety_European_2022]。在 FINEARTS-HF，worsening renal function 事件為 **17.7% finerenone vs 10.9% placebo**（其中 renal impairment 6.6% vs 3.9%、GFR decreased 5.2% vs 3.6%、acute kidney injury 3.7% vs 2.1%、renal failure 2.6% vs 1.6%、blood creatinine increased 1.2% vs 0.8%）；與安慰劑相比的平均 GFR 差距約 **3–4 mL/min/1.73 m²（month 1–6）**，並於 month 6 後衰減至約 **2–3 mL/min/1.73 m²** [label_guideline_safety_European_2022]。這條「先擴大、後收斂」的曲線正是血流動力學 offset 的印記。

### 1.3 Goulooze 模型：最精緻的「雙相＋可逆」量化 🟡

FIDELIO 的 dose-exposure-response 群體模型（Goulooze）把 dip 的形狀拆解得最清楚 [egfr_dip_reversibility_Goulooze_2022]：

- **幅度**：finerenone 組於 month 4 出現 **median 3.3 mL/min/1.73 m² decline**，安慰劑僅 **0.8 mL/min/1.73 m² decline**；到 year 2 安慰劑中位 eGFR 反而略低於 finerenone，「the curves cross again within 2 years」[egfr_dip_reversibility_Goulooze_2022]。
- **雙相型態（biphasic pattern）**：模型辨識出兩個 finerenone 效應——**(i) acute eGFR-decreasing effect**（一次性 offset，於前幾週內發生）＋ **(ii) superimposed flattening of the chronic slope**（慢性斜率趨緩，益處隨時間累積並最終壓過急性效應）[egfr_dip_reversibility_Goulooze_2022]。
- **完全可逆的假設能擬合資料**：一個「assuming full reversibility of the acute eGFR decline」的模型良好描述資料，**包括停藥後的資料**（與先前 ARTS-DN phase IIb 分析一致）[egfr_dip_reversibility_Goulooze_2022]。
- **量化 rebound**：校正 standard-of-care eGFR 下降後，停藥者 eGFR **回升 6.9%（95% CI +3.9% 至 +10.0%）**，與模型模擬之 finerenone 20 mg OD 急性下降 **5.4%** 相稱；停藥者自起始至停藥的中位時間為 **1.8 years（5th–95th percentiles: 0.4 to 3.6 years）**，並於停藥後 90 天內取得 eGFR 追蹤 [egfr_dip_reversibility_Goulooze_2022]。
- 作者定性：acute decline「is generally considered to represent **hemodynamic effects**, where even an eGFR decline is considered beneficial for the kidney rather than representing disease progression」[egfr_dip_reversibility_Goulooze_2022]。
- **誰的慢性斜率獲益最大**：模擬 finerenone 20 mg OD 對 chronic eGFR slope 的效應，從 **−22.1%（high baseline UACR 3366 mg/g）到 −41.3%（low baseline eGFR 26.7 mL/min/1.73 m²）**——低 eGFR 者比例上獲益最大 [egfr_dip_reversibility_Goulooze_2022]。
- **與 SGLT2i 獨立可加**（詳見下方 §1.1）：concomitant SGLT2i 對 finerenone 的 acute eGFR-decreasing effect **無顯著影響（95% CI 73.2–120%）**，支持兩者機轉獨立、效應可加 [egfr_dip_reversibility_Goulooze_2022]。

> **性質誠實**：Goulooze 為群體藥動／藥效**模型分析**、以 eGFR/UACR 為代理，屬 evidence expansion；「完全可逆」是能良好擬合資料的模型假設，而非直接臨床終點證明。

### 1.1 與 SGLT2i 的 dip「獨立且可加」：把交互作用量化到信賴區間 🟡

這是把「finerenone 加在 SGLT2i 上、會不會讓 eGFR dip 疊加成問題」講清楚的關鍵分析。Goulooze 的 FIDELIO-DKD 群體 PK/PD 模型（分析集 **5674 名**病人、**37,296 筆 UACR** 與 **78,132 筆 eGFR** 觀測；治療期任一時點曾用 SGLT2i 者 **528 名**）把病人分成四組同時建模——安慰劑無 SGLT2i（N=2553）、安慰劑用 SGLT2i（N=288）、finerenone 無 SGLT2i（N=2593）、finerenone 用 SGLT2i（N=240）[egfr_dip_reversibility_Goulooze_2022]。

**核心發現：SGLT2i 不修飾 finerenone 的效應**——三個交互作用的 95% 信賴區間都跨越／涵蓋「無交互作用（100%）」，方向一致地指向獨立性：

| finerenone 效應 | SGLT2i × finerenone 交互作用（95% CI） | 解讀 |
|---|---|---|
| UACR 降幅 | **94.1–122%** | 以 97.5% 信心，SGLT2i 使用者中 finerenone 至少保有 **94.1%** 的 UACR 療效 |
| **急性 eGFR 下降效應** | **73.2–120%** | 對 finerenone 的急性 dip **無顯著影響**——加 SGLT2i 不會顯著放大或抵消初期 dip |
| UACR 中介之慢性 eGFR slope 效應 | **9.5–144%** | 亦無顯著修飾（區間寬，因慢性效應樣本資訊較少）|

（三組區間均取自 [egfr_dip_reversibility_Goulooze_2022]；作者結論句為「suggesting independence」。）

**機轉為何「獨立」**：模型顯示 finerenone 的慢性 eGFR 益處**完全經由其 UACR 效應中介**（加入非 UACR 中介的 finerenone 效應無法改善擬合）；而 SGLT2i 除了 UACR 途徑，還被辨識出一個**UACR-獨立**的慢性 eGFR slope 效應（finerenone 沒有這條）[egfr_dip_reversibility_Goulooze_2022]。兩藥各走部分不同的路徑，是「獨立」在藥效模型上的具體意義。

**「可加」的量化（Table 4 模擬，vs 未用 SGLT2i 之標準治療）**——把兩藥效應疊起來，UACR 與慢性 slope 的改善確實加成，且急性 dip 隨之更明顯但仍在可逆範圍 [egfr_dip_reversibility_Goulooze_2022]：

| 效應 | Finerenone 20 mg | SGLT2i | Finerenone 20 mg + SGLT2i |
|---|---|---|---|
| 最大 UACR 降幅（%） | −53.6 | −19.1 | **−62.4** |
| 慢性 eGFR slope vs placebo（%） | −36.9 | −56.1 | **−71.5** |

**臨床轉譯**：對「已用 SGLT2i、要不要加 finerenone」的病人，此分析支持——(1) 初期 dip **不會因為併用 SGLT2i 而顯著加重**（急性交互作用 73.2–120%）；(2) 兩藥的 UACR／慢性腎保護**可加**（combo UACR −62.4%、slope −71.5%）；(3) 併用 SGLT2i 另有降高血鉀的方向性益處（見 [`hyperkalemia_engineering_by_scenario.md`](hyperkalemia_engineering_by_scenario.md) 與 [`benefit_risk_discussion_nnt_nnh.md`](benefit_risk_discussion_nnt_nnh.md)）。同步起始之臨床證據見主題三與 CONFIDENCE（[`hyperkalemia_engineering_by_scenario.md`](hyperkalemia_engineering_by_scenario.md) §3.4 對讀）。

> **性質誠實（重要保留）**：此為**模型分析**、以 eGFR/UACR 為代理終點（evidence expansion）。更關鍵的是——**FIDELIO-DKD 並未針對 SGLT2i 使用隨機化**，SGLT2i 使用者為觀察性次組（N=240 finerenone 組），故作者明示「SGLT2i 的量化效應大小須謹慎解讀（potential selection bias）」；「獨立且可加」的方向由統計無顯著交互作用支持，並有臨床前資料（finerenone + empagliflozin 呈現 early、sustained、**over-additive** proteinuria reduction）佐證，但非隨機化證明 [egfr_dip_reversibility_Goulooze_2022]。

---

## 2. 可逆性的機轉根據：這是一個 class 現象

把 finerenone 的 dip 放進 RAAS 阻斷／SGLT2i 的可逆 dip 文獻中對讀，可看出它並非 nsMRA 獨有，而是「濾過壓下修」的共同表現。

### 2.1 SGLT2i（CREDENCE / Oshima）🟡

CREDENCE 的 post hoc（Oshima）：canagliflozin「induces a **reversible acute drop** in eGFR, believed to be a **hemodynamic effect**」，機轉為增加遠端鈉氯輸送、augment tubuloglomerular feedback、逆轉入球小動脈血管擴張、降低腎小球內壓 [egfr_dip_reversibility_Oshima_2021]。量化：4289 名於 baseline 與 week 3 皆有 eGFR 者，week 3 平均急性變化 **−7.0%（SE 0.4%）canagliflozin vs 0.3%（SE 0.4%）placebo（mean difference −7.3%；95% CI −8.5% 至 −6.1%）**；**>10% drop 45%（956）vs 21%（450）**，**>30% drop 4.2%（89）vs 1.8%（39）**，>10% drop 的 **OR 3.03（95% CI 2.65–3.47）**；關鍵是初期 dip 後「long-term eGFR trajectories … and kidney safety profiles … were similar across eGFR decline categories」——臨床益處不因 dip 大小而異 [egfr_dip_reversibility_Oshima_2021]。

### 2.2 RAAS 阻斷之真實世界因果（Oh 2026）🟡

Oh 以 staggered difference-in-differences ＋ PS matching 之準實驗設計，重現了 RCT 的型態：1,204 名成人（375 treated、829 not-yet-treated controls）追蹤 3 年，**overall ATE −1.47 mL/min/1.73 m²（p = 0.33，不顯著）**，但 event time 0/1/3 出現顯著急性下降 **−3.87、−2.34、−2.54 mL/min/1.73 m²（p < 0.05）**，3 個月後衰減不再顯著；治療組中 **73 人（19.5%）於前 3 個月出現 ≥30% eGFR 下降**，但平均下降僅約 **6.5%**，well within safe thresholds [egfr_dip_reversibility_Oh_2026]。作者結論：初期下降「are early, transient, and primarily **hemodynamic** in nature rather than reflective of structural kidney injury」，且準實驗真實世界資料「reproduced the findings of randomized trials」[egfr_dip_reversibility_Oh_2026]。

### 2.3 ARB 的「dip 越大、長期越好」悖論（RENAAL / Holtkamp）🟡

RENAAL 的 post hoc（Holtkamp）在 losartan 上示範了「acute dip 是好事」的反直覺關係：3 個月時 losartan 的急性下降大於安慰劑（**−2.3；95% CI −2.7 至 −1.8 vs −1.6；−2.0 至 −1.1 mL/min/1.73 m²；P = 0.031**），但其後的長期斜率反而較平緩（**losartan −4.2；95% CI −3.9 至 −4.6 vs placebo −5.0；−4.7 至 −5.4 mL/min/1.73 m² per year；P < 0.001**）[r2_Holtkamp_2011]。個體差異極大（losartan 組初期變化 mean **−2.3；min −18.3；max +14.7**）[r2_Holtkamp_2011]。核心訊息：「the greater the acute fall in eGFR, during losartan treatment, the slower the rate of long-term eGFR decline」——初期 dip 與長期斜率**呈負相關**，不是傷害訊號 [r2_Holtkamp_2011]。

### 2.4 高濾過的病理生理背景（Tonneijck 2017）🟡

Tonneijck 的糖尿病高濾過綜述提供機轉背景：糖尿病早期的 single-nephron 高濾過屬適應不良，RAS 阻斷等介入可 mitigate 此初期反應、attenuate renal hemodynamic 異常——即「dip」實為把病理性高濾過拉回的血流動力學修正 [egfr_dip_reversibility_Tonneijck_2017]。

### 2.5 class 的一致定性（Haidar 2026，SGLT2i）🟡

Haidar 對 SGLT2i eGFR dip 的定性總結可直接套用到 class：dip「typically ranges from **3–6 mL/min/1.73 m²** in the general population and is usually **reversible**」、「primarily reflects **hemodynamic** changes rather than structural kidney injury」、「discontinuation is generally unnecessary unless an unexplained eGFR decline exceeds 30%」[egfr_dip_reversibility_Haidar_2026]。即使在高風險的 HIV 族群（295 對配對）：6 個月 ≥10% 下降 **58.2% vs 37.4%（aHR 1.79；95% CI 1.40–2.28）**、≥30% **17.3% vs 9.8%（aHR 1.69；95% CI 1.05–2.73）**、平均 eGFR 變化 **−2.62 vs 0.05 mL/min/1.73 m²**，但長期曲線仍呈「initial decline followed by stabilization and a slower subsequent decline」[egfr_dip_reversibility_Haidar_2026]。

---

## 3. 預後脫鉤（本節最重要）

### 3.1 RASi 的歷史：dip 有可容忍的寬閾值（Ku 2024）🟡

傳統教條「肌酸酐上升 30% 就停藥」其實過嚴。Ku 整合 **17 個 RASi 試驗、n = 11,800**（mean eGFR 43，SD 11；median UACR 362 mg/g，IQR 50–1367；其中 **1162（10%）發生 kidney failure**）發現：相較於「comparator 組 0% 下降」，RASi 使用下 **3 個月內 ≤13%（95% CI 8% 至 17%）** 或 **1 個月內 ≤21%（95% CI 15% 至 27%）**（1 個月子集 N = 3651）的 eGFR 下降，其 kidney failure 風險仍**優於「無下降」**[r2_Ku_2024]。在 13% 閾值處，3 個月風險的 **adjusted HR 為 1.02（95% CI 0.86 至 1.22）**；kidney failure 或死亡的複合終點閾值同為 **13%（95% CI 7.5% 至 16%）**[r2_Ku_2024]。作者指出現行「creatinine >30%」教條約等於 **27% 的 eGFR 下降**，而其保守分析顯示益處可延伸到此程度 [r2_Ku_2024]。換言之：dip 的可容忍範圍遠寬於床邊直覺。

### 3.2 finerenone：dip 與腎結局「脫鉤」（Matsumoto 2025，FINEARTS-HF）🟡

FINEARTS-HF 的前瞻分析（Matsumoto）把「脫鉤」講得最直接。以 randomization 到 1 個月的 ≥15% 下降為界：**≥15% 下降在 finerenone 23.0%（n 644 of 2,798）vs placebo 13.4%（374），OR 1.95（95% CI 1.69–2.24；P < 0.001）**；**≥30% 下降在 finerenone 4.9%（136）vs placebo 2.0%，OR 2.51（95% CI 1.83–3.44；P < 0.001）**[hf_renal_safety_Matsumoto_2025]。

關鍵在於**預後**：調整後，初期 eGFR 下降在**安慰劑組**預示更差主要結局（**adjusted rate ratio 1.50；95% CI 1.20–1.89**），但在 **finerenone 組不然（adjusted rate ratio 1.07；95% CI 0.84–1.35；P-interaction 0.04）**；且 finerenone 的療效**橫跨整個 1 個月 eGFR 變化範圍皆一致（P-interaction 0.50）**[hf_renal_safety_Matsumoto_2025]。作者結論可直接貼在門診牆上：初期 eGFR 下降「can be anticipated with finerenone and **should not automatically lead to the discontinuation of this disease-modifying therapy**」[hf_renal_safety_Matsumoto_2025]。

**「一致性」到底一致在哪？** Matsumoto 分析的 primary outcome 是「total HF events 與 cardiovascular death 的複合」[hf_renal_safety_Matsumoto_2025]。所謂 finerenone 療效「橫跨整個 1 個月 eGFR 變化範圍皆一致（P-interaction 0.50）」，意思是：**不論病人 dip 深或淺，finerenone vs placebo 的臨床益處方向與幅度都維持**；而且這種「dip 不預示更差結局」的中性關係，不只見於主要複合終點，也延伸到分項的 the other outcomes examined（total HF events、cardiovascular death、first HF event or CV death）[hf_renal_safety_Matsumoto_2025]。作者把初期下降定位為「reﬂecting changes in glomerular hemodynamics」——即濾過端血流動力學的調整，而非結構性腎損傷 [hf_renal_safety_Matsumoto_2025]。

> **意義**：在安慰劑組，dip 是「疾病在惡化」的被動訊號；在 finerenone 組，dip 是「藥物正在下修濾過壓」的主動印記——同一個數字，因為背後機轉不同，預後意義相反。這就是「脫鉤」。

#### 3.2.1 把「脫鉤」再拆一層：dip 深的病人，我們到底看到什麼、還沒看到什麼

用機轉語言說：finerenone 下修 MR 驅動的容量／血壓與腎絲球內壓，**dip 較深往往對應濾過壓（含糖尿病常見的 glomerular hyperfiltration）被拉得更低**——而 hyperfiltration 正是 CKD 進展的血流動力學驅動之一（intraglomerular 高壓、tubuloglomerular feedback 失調）[egfr_dip_reversibility_Tonneijck_2017]。因此「dip 深」在 finerenone 身上更像是「濾過壓被有效下修」的**過程指標**，其後轉換成的，是慢性 eGFR slope 的趨緩與穩定（見 §1 Goulooze 的雙相模型）。

但這裡要非常誠實地畫出證據邊界——**我們目前看到的「一致性」，是在 biomarker／臨床複合終點層級（eGFR 變化 × finerenone 療效無交互作用）**，而**不是**「dip 的深度本身**因果地**帶來額外益處」的證明：

1. **這是條件式、非隨機化的關聯**。Matsumoto 自陳：初期 eGFR 下降是「a nonrandomized exposure」，故 eGFR 下降與後續結局之關聯「may be confounded by variables beyond those we adjusted for」，並提醒此分析具「conditional nature」[hf_renal_safety_Matsumoto_2025]。換言之，「dip 中性／脫鉤」是**穩健的觀察關聯**，但不等於「越深越好」的因果宣稱。
2. **「一致」不代表「更好」**。資料支持的是：dip 深或淺，finerenone 的療效**都在**（P-interaction 0.50）；資料**沒有**證明「dip 更深的病人反而獲得更大益處」。目前只能說 dip 的深度**不折損**療效，不能說它**放大**療效。
3. **超出 eGFR／既測結局的其他面向仍屬未知** 🔴。是否有其他 biomarker 或長期硬結局會因為「dip 更深（hyperfiltration 下修更多）」而不受影響、甚至受益，**目前臨床證據並無定論**；這是一個**機轉上合理、但尚未被隨機化終點驗證的假說**，不應在門診被講成已確立的因果。

> **一句話總結（誠實版）**：finerenone 的初期 dip 可以**放心不停藥**（脫鉤＋可逆，證據穩健）；但「dip 越深越好」目前**只是機轉假說**——我們看到的是「深淺不影響療效」的一致性，而非「深 dip 額外獲益」的證明。兩者不要混為一談。

### 3.3 誰會 dip：baseline eGFR 越高、越容易出現看似驚人的 dip（Vaduganathan 2025）🟡

CONFIDENCE 的 KDIGO 風險分層分析補上「地形圖」：合併治療下 **>30% eGFR 下降（day 30 ± 4）在 low/moderate risk（12.1%）與 high risk（8.2%）反而比 very-high risk（4.4%）更常見**[hf_renal_safety_Vaduganathan_2025]。原因是 baseline eGFR 與風險層負相關（low/moderate **73.1 ± 10.9**、high **69.5 ± 13.0**、very-high **43.0 ± 8.6 mL/min/1.73 m²**）——baseline 越高、可掉的空間越大 [hf_renal_safety_Vaduganathan_2025]。同時 investigator-reported AKI 在各層皆 infrequent（**≤3%**）[hf_renal_safety_Vaduganathan_2025]。

> **anticipatory guidance**：eGFR 較好的病人反而更可能出現數字上驚人的初期 dip。門診應**事先**向這類病人與團隊預告，避免把「基線好、掉得多但仍安全」誤讀為惡化而過早停藥。

---

## 4. 停藥的代價：益處會隨之流失（Singh 2026，FIDELITY）

若因 dip 或高血鉀而過早永久停藥，代價是實在的。FIDELITY 停藥分析（Singh，post hoc）納入 **12,990 名**，其中 **2,889（22.2%）**因死亡以外原因提前停藥（**finerenone 22.8% vs placebo 21.6%**）[egfr_dip_reversibility_Singh_2026]。停藥主因為 AE（9.0% vs 8.7%），治療相關 AE 導致停藥 6.4% vs 5.4%，其中**因高血鉀停藥僅 1.7% vs 0.6%**[egfr_dip_reversibility_Singh_2026]。

療效隨停藥衰減：以 time-varying covariate 之分層 Cox 分析，finerenone 對複合**腎**終點的效益在**治療中 HR 0.65（95% CI 0.54–0.78）**、**停藥後 HR 0.82（95% CI 0.66–1.02；p_interaction 0.0959）**；複合 **CV** 終點在**治療中 HR 0.79（95% CI 0.70–0.88）**、**停藥後 HR 0.93（95% CI 0.79–1.09；p_interaction 0.0960）**[egfr_dip_reversibility_Singh_2026]。對應的每 100 病人年粗事件率：腎（治療中 1.09 vs 1.71；停藥後 11.95 vs 13.67）、CV（治療中 2.98 vs 3.78；停藥後 14.07 vs 14.73）[egfr_dip_reversibility_Singh_2026]。

**誰最容易停藥？** random survival forest 排序出最重要的四個 baseline 變數為 **eGFR、UACR、age、serum potassium**；風險隨 eGFR 升高而降（vs eGFR <45：**45–≤60 HR 0.71，95% CI 0.62–0.81**；**≥60 HR 0.62，95% CI 0.53–0.72**）[egfr_dip_reversibility_Singh_2026]。也就是說，**low eGFR、high UACR、high baseline K⁺、高齡**——正是最該被保住治療的高風險族群——最容易停藥。在同一 FIDELITY，finerenone 降低複合腎、CV 終點各 **23%** 與 **14%**，這些正是停藥會流失的益處 [egfr_dip_reversibility_Singh_2026]。

這與 KDIGO 的核心倫理一致：暫停 RASi 可以，但務必在不良事件解除後重新啟動，別讓病人被剝奪所需藥物（Practice Point 3.6.4 對應之續用原則）[label_guideline_safety_Kidney_2024]。

> **性質誠實**：Singh 為 post hoc，p_interaction 均不顯著（0.0959／0.0960），故「停藥使療效衰減」為 numerically／方向性觀察，非統計上證實之交互作用；但方向明確、與生理一致。

---

## 5. 門診決策：把「看到 dip」變成「按流程走」

1. **起始前預告（anticipatory guidance）**：告知病人初期 eGFR 可能小幅下降，尤其 baseline eGFR 較高者（Vaduganathan：12.1% vs 4.4%）[hf_renal_safety_Vaduganathan_2025]。
2. **用對閾值**：<20%–30% 的初期下降屬預期、不改藥（KDIGO PP 2.1.4）[label_guideline_safety_Kidney_2024]；RASi 歷史顯示 3 個月 ≤13%／1 個月 ≤21% 仍優於無下降（Ku）[r2_Ku_2024]。
3. **>30% 才評估**：查 AKI、容量、共病用藥（利尿劑、NSAID）、腎動脈狹窄；EMA 另設 ≥40% 考慮減量／暫停、穩定後再上調 [label_guideline_safety_European_2022] [label_guideline_safety_Kidney_2024]。
4. **別把 dip 當停藥理由**：finerenone 的 dip 與腎結局脫鉤（Matsumoto RR 1.07）[hf_renal_safety_Matsumoto_2025]；停藥會流失益處（Singh）[egfr_dip_reversibility_Singh_2026]。
5. **暫停要重啟**：不良事件解除後重新啟動，別讓高風險族群被永久剝奪 disease-modifying 療法 [label_guideline_safety_Kidney_2024] [egfr_dip_reversibility_Singh_2026]。

---

## 6. 誠實邊界（Evidence limits）🟡🔴

- Goulooze（模型）、Matsumoto／Vaduganathan（前瞻／post hoc 次分析）、Singh（post hoc）、Oshima／Holtkamp／Oh／Haidar（跨 class 的 post hoc／觀察／準實驗）——**多為代理終點（eGFR/UACR）或探索性分析**，屬 evidence expansion；「dip 可逆且與結局脫鉤」方向明確且跨 class 一致，但非以「dip → hard outcome」為主終點的隨機化證明 🟡。
- Singh 的 p_interaction 不顯著（0.0959／0.0960），「停藥使療效衰減」為方向性、非統計證實 🟡。
- Goulooze「完全可逆」為模型假設；Oh 為真實世界準實驗，殘餘干擾（confounding by indication）無法完全排除 🔴。
- 具體數字專屬其原始族群（FIDELITY／FINEARTS-HF／CONFIDENCE／CREDENCE／RENAAL／韓國 EMR／HIV 世代），外推至其他情境須保留 🔴。

---

## 證據分層小結

| 論點 | 等級 | 主要本地全文來源 |
|------|------|------------------|
| >30% 才需評估、10%–20% 屬典型（KDIGO PP 2.1.4） | 🟢 guideline | `label_guideline_safety_Kidney_2024` 📄 |
| finerenone dip 小（EMA ~2 mL/min，reversible） | 🟡 | `label_guideline_safety_European_2022` 📄 |
| 雙相＋完全可逆＋停藥 rebound 6.9%（Goulooze 模型） | 🟡 model | `egfr_dip_reversibility_Goulooze_2022` 📄 |
| SGLT2i 可逆 dip 為 class 現象（CREDENCE −7.3%、OR 3.03） | 🟡 | `egfr_dip_reversibility_Oshima_2021` 📄 |
| RAAS dip 真實世界可逆（Oh −3.87、3 月後衰減） | 🟡 | `egfr_dip_reversibility_Oh_2026` 📄 |
| dip 越大長期越好之悖論（RENAAL losartan） | 🟡 | `r2_Holtkamp_2011` 📄 |
| RASi dip 可容忍寬閾（Ku：3 月 ≤13%、1 月 ≤21%） | 🟡 | `r2_Ku_2024` 📄 |
| finerenone dip 與腎結局脫鉤（Matsumoto RR 1.50→1.07，P-int 0.04） | 🟡 | `hf_renal_safety_Matsumoto_2025` 📄 |
| baseline eGFR 高者更易 dip（CONFIDENCE 12.1% vs 4.4%） | 🟡 | `hf_renal_safety_Vaduganathan_2025` 📄 |
| 停藥使益處流失（Singh 治療中 0.65 vs 停藥 0.82） | 🟡 post hoc | `egfr_dip_reversibility_Singh_2026` 📄 |
| 「dip → hard outcome」為主終點之 RCT | 🔴 尚無 | —（誠實揭露） |

## 本地全文語料（可 grep 稽核）

📄 全文：`egfr_dip_reversibility_Goulooze_2022`（FIDELIO 群體模型）、`egfr_dip_reversibility_Oshima_2021`（CREDENCE post hoc）、`egfr_dip_reversibility_Oh_2026`（RAAS 準實驗）、`egfr_dip_reversibility_Tonneijck_2017`（高濾過綜述）、`egfr_dip_reversibility_Haidar_2026`（SGLT2i／HIV 世代）、`egfr_dip_reversibility_Singh_2026`（FIDELITY 停藥分析）、`r2_Holtkamp_2011`（RENAAL losartan）、`r2_Ku_2024`（17 RASi 試驗整合）、`hf_renal_safety_Matsumoto_2025`（FINEARTS-HF dip 前瞻分析）、`hf_renal_safety_Vaduganathan_2025`（CONFIDENCE KDIGO 分層）、`label_guideline_safety_Kidney_2024`（KDIGO 2024 PP 2.1.4／3.6.4）、`label_guideline_safety_European_2022`（EMA 產品文件）。

---

## References（本地可稽核）

1. Kidney Disease: Improving Global Outcomes (KDIGO) CKD Work Group. KDIGO 2024 Clinical Practice Guideline for the Evaluation and Management of CKD (Practice Points 2.1.4, 3.6.4). 📄 [label_guideline_safety_Kidney_2024]
2. European Medicines Agency. Kerendia (finerenone) product information / assessment. 2022. 📄 [label_guideline_safety_European_2022]
3. Goulooze SC, et al. Dose–exposure–response modelling of finerenone effects on UACR and eGFR in FIDELIO-DKD. 2022. 📄 [egfr_dip_reversibility_Goulooze_2022]
4. Oshima M, et al. Insights from CREDENCE: an acute drop in eGFR during canagliflozin treatment and its clinical implications. *Kidney Int.* 2021. 📄 [egfr_dip_reversibility_Oshima_2021]
5. Oh S, et al. Transient, hemodynamic eGFR decline after RAAS inhibitor initiation: a quasi-experimental staggered DID cohort. 2026. 📄 [egfr_dip_reversibility_Oh_2026]
6. Holtkamp FA, et al. An acute fall in eGFR during losartan treatment predicts a slower long-term decline in renal function (RENAAL post hoc). 2011. 📄 [r2_Holtkamp_2011]
7. Ku E, et al. Subacute declines in eGFR after RAS inhibitor initiation and risk of kidney failure: pooled analysis of 17 trials (n=11,800). 2024. 📄 [r2_Ku_2024]
8. Matsumoto S, et al. Initial decline in eGFR with finerenone and clinical outcomes in HFmrEF/HFpEF: FINEARTS-HF. 2025. 📄 [hf_renal_safety_Matsumoto_2025]
9. Vaduganathan M, et al. Combination finerenone + empagliflozin across KDIGO risk categories (CONFIDENCE). 2025. 📄 [hf_renal_safety_Vaduganathan_2025]
10. Singh V, et al. Predictors and consequences of finerenone discontinuation in FIDELITY. *Am J Nephrol.* 2026. 📄 [egfr_dip_reversibility_Singh_2026]
11. Tonneijck L, et al. Glomerular hyperfiltration in diabetes: mechanisms, clinical significance, and treatment. 2017. 📄 [egfr_dip_reversibility_Tonneijck_2017]
12. Haidar M, et al. Acute eGFR dip after SGLT2i initiation among people with HIV: a matched cohort. 2026. 📄 [egfr_dip_reversibility_Haidar_2026]

---
*此檔為主題五之延伸拆解，撰寫日期基準 2026-07-11。所有具體數字均可 grep 回上列本地全文 MD。「dip 可逆且與結局脫鉤」跨 class 一致但多屬 post hoc／模型／代理終點；以「dip → hard outcome」為主終點之前瞻 RCT 目前不存在，屬明示之研究缺口。*
