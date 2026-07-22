# 統計迷思與深度解讀 · 主題五（安全性統計的臨床轉換）

> 本檔為主題五「高血鉀與 eGFR dip 的安全工程學」之**統計深度解讀分冊**。同資料夾的臨床拆解檔已分別處理各安全議題的「怎麼做」；本檔提供的是**互補的統計素養層**——不重述臨床協定，而是回答「這些安全性統計該**怎麼正確地讀**」。核心手法：把主題四那條經典的「相對 vs 絕對」錨點**鏡像到傷害（harm）端**——同一組高血鉀數字，用相對尺度會製造恐懼、用絕對尺度會顯示可管理，NNH 是兩者之間的翻譯橋。每個迷思三段式：**❌ 常見誤解 → ✅ 統計正解（附本地數字）→ 💡 臨床亮點**。
>
> **與臨床拆解檔的分工（勿重複）**：benefit-risk 的 NNT/NNH 同尺權衡見 [`benefit_risk_discussion_nnt_nnh.md`](benefit_risk_discussion_nnt_nnh.md)；eGFR dip 血流動力學可逆見 [`egfr_dip_hemodynamic_reversible.md`](egfr_dip_hemodynamic_reversible.md)；雙向電解質見 [`hypokalemia_bidirectional_electrolyte.md`](hypokalemia_bidirectional_electrolyte.md)；binder 定位見 [`potassium_binder_role.md`](potassium_binder_role.md)；情境化高血鉀工程見 [`hyperkalemia_engineering_by_scenario.md`](hyperkalemia_engineering_by_scenario.md)；CYP3A4 處方規則見 [`cyp3a4_interaction_prescribing_rules.md`](cyp3a4_interaction_prescribing_rules.md)。本檔只借它們一句話當入口，然後轉向這些檔未展開的**統計判讀層**。
>
> **引用標記慣例**：📄 = 本地全文可 grep 稽核；📌 = 僅取得 abstract。每個具體數字句末以 `[本地MD檔名]` 標註來源供 grep 回溯。LLM 僅負責組織、改寫與**統計詮釋**；詮釋可延伸，數字一律出自本地全文。
>
> **證據分層**：🟢 已確立的統計方法學共識｜🟡 post hoc／次分析／模型／代理終點｜🔴 假說、僅摘要或未定稿。

---

## 迷思一：高血鉀「相對風險加倍」＝臨床災難——把 harm 端的相對／絕對分開讀

這是主題四錨點的鏡像版。主題四談的是「益處的相對恆定，會被基線風險放大成不同的絕對益處」；到了安全性，同一個統計把戲換了方向——**一個嚇人的相對風險，會被貼地的基線事件率壓成一個可管理的絕對風險**。

### ❌ 常見誤解
「finerenone 讓高血鉀多了一倍——14.0% vs 6.9%、風險 HR 2.13，這藥太危險。」把「相對加倍」直接讀成「病人危險加倍」。

### ✅ 統計正解
相對風險與絕對風險回答的是兩個不同問題，而恐懼幾乎全部來自相對尺度：

- **相對尺度（製造恐懼）**：FIDELITY pooled 任一高血鉀 **14.0% vs 6.9%**[label_guideline_safety_European_2022]；FIDELIO-DKD 校正多變量後 finerenone 的 ≥mild 高血鉀 **HR 2.13（95% CI 1.86–2.45）**、原文明言 "twofold higher risk of hyperkalemia"[pooled_safety_hyperkalemia_Agarwal_2022]。相對「加倍」是真的。
- **絕對尺度（顯示可管理）**：同一個 pooled 族群，真正有臨床意義的硬事件貼地——因高血鉀**住院 0.9% vs 0.2%**、因高血鉀**永久停藥 1.7% vs 0.6%**[label_guideline_safety_European_2022]。相對加倍發生在一個分母極低的基期上，換算成絕對，門診多面對的是「約多 1 個百分點的永久停藥」。
- **NNH 是兩把尺之間的橋**：把 RR 翻成床邊語言——FIDELIO-DKD 中約需處方 **71 名** finerenone 才有 1 名因高血鉀永久停藥；作對照，被放棄的雙重 RAS 阻斷策略 NNH 僅 **18（VA NEPHRON-D）／45（ALTITUDE）／26（ORIENT）**[pooled_safety_hyperkalemia_Agarwal_2022]。同樣「相對加倍」的兩類藥，NNH 差了約 4 倍——這正是相對尺度看不出、絕對尺度才看得到的東西。

補一個常被忽略的機制學統計細節：finerenone 造成的血鉀上升幅度小且平台化，組間平均差最大僅 **0.23 mmol/L（月 4）**[pooled_safety_hyperkalemia_Agarwal_2022]。RR 2 倍不等於「鉀濃度飆高 2 倍」，只是「跨過某門檻的人數比例多一倍」。

### 💡 臨床亮點
床邊正確的一句話：「這個藥讓抽血跨過 5.5 的人數大約多一倍，但真正因此住院或必須永久停藥的絕對機會只多約 1 個百分點，而且是可逆的（停藥即解）。」報高血鉀風險時，**永遠把相對倍率與絕對事件率、NNH 三者一起講**——單獨丟出「風險加倍」是統計上誠實、臨床上誤導。

---

## 迷思二：「13,000 人零高血鉀死亡」＝零風險——零事件不等於零風險

### ❌ 常見誤解
「跨試驗這麼多人、追蹤 3 年，沒有一例高血鉀死亡——所以高血鉀致死風險是零，不用擔心。」把「觀察到 0 次」直接讀成「真值為 0」。

### ✅ 統計正解
「零事件」是三個大型資料集一致的觀察，但統計上它是一個**有上界的區間**，不是一個點：

- Wanner 實務綜述："**there were no hyperkalemia-related deaths in more than 13,000 patients over a median follow-up of 3 years**"[label_guideline_safety_Wanner_2022]。
- INFINITY（FIDELIO＋FIGARO＋FIND-CKD IPD 合併）："**no deaths attributable to hyperkalaemia**"，且因高血鉀永久停藥 **122（1.7%）vs 39（0.5%）**[pooled_safety_hyperkalemia_Neuen_2026]。
- FINE-HEART（n=14,180）："**There were no deaths related to hyperkalemia in either treatment arm**"[hf_renal_safety_Ostrominski_2026]。

關鍵統計工具是 **rule of three（三的法則）**：若在 n 人中觀察到 0 次事件，其發生率的 95% 信賴上界約為 **3/n**。以 n≈13,000 代入，上界約 3/13,000 ≈ 0.023%，即「真實的高血鉀致死率**可能**高達每約 4,300 人 1 例」。所以「零」的正確解讀有兩層：(a) **不是證明風險為零**——樣本再大，尾端罕見事件仍有殘餘不確定性；(b) 但這個上界本身**極低**，足以支撐「絕對危害微乎其微」的臨床結論。零事件的力量來自 n 很大，而不是來自「零」這個字。

### 💡 臨床亮點
對病人可以說「在超過一萬三千人、平均三年的試驗裡，沒有人因高血鉀而死亡」——這是誠實的。但別把它升級成「不可能發生」。正確的統計姿態是：**罕見致命事件的『零』要配 rule of three 的上界一起讀**；上界夠低，才是「可以放心、但仍要監測」的依據。這也正是為什麼監測節奏不能因「零死亡」而取消——監測就是把這條上界持續壓低的機制。

---

## 迷思三：eGFR dip 的預後脫鉤＝「finerenone 讓 dip 變無害」——條件式、非隨機暴露的因果陷阱

### ❌ 常見誤解
「Matsumoto 證明在 finerenone 組初期 eGFR 下降不再預示壞結局（P-interaction 0.04），所以 finerenone 把 dip 這件壞事變成無害了。」把一個**穩健的觀察關聯**讀成**因果證明**。

### ✅ 統計正解
先看數字本身，它確實漂亮且值得引用。FINEARTS-HF 中 ≥15% 初期 eGFR 下降在 finerenone 更常見（**23.0% vs 13.4%，OR 1.95**）[hf_renal_safety_Matsumoto_2025]；而預後上——**安慰劑組的 dip 預示更差結局（adjusted RR 1.50, 95% CI 1.20–1.89），finerenone 組卻不然（adjusted RR 1.07, 95% CI 0.84–1.35；P-interaction 0.04）**，且 finerenone 的療效橫跨整個 eGFR 變化範圍一致（**P-interaction 0.50**）[hf_renal_safety_Matsumoto_2025]。

但要提醒三件統計事：

- **dip 是 nonrandomized exposure。** 病人被隨機分到 finerenone/placebo，但**沒有人被隨機分到「會不會 dip」**。「有 dip vs 無 dip」是治療後才浮現的分層，兩群人在體質、容積狀態、baseline eGFR 上本就不同——關聯 **may be confounded**，即使已 adjusted。
- **這是 conditional analysis。** 「在有 dip 的人裡比較 finerenone vs placebo」是一個**條件於治療後變數**的分析，本質上會削弱隨機化所保護的可比性。
- **「一致（P-interaction 0.50）≠ 更好」。** 效果橫跨 eGFR 變化一致，只說明「療效不因 dip 大小而異」，不等於「dip 對這個病人是好事」。correlation ≠ causation：資料**相容於**「finerenone 的 dip 是良性血流動力學」的假說，但沒有**證明**它。

### 💡 臨床亮點
Matsumoto 的結論——「finerenone 的初期 eGFR 下降是可預期的，不應自動導致停用這個 disease-modifying 藥物」[hf_renal_safety_Matsumoto_2025]——**臨床上正確且可據以行動**，因為它與 RASi 的歷史證據（可容忍的 dip 閾值遠寬於 30% 教條）方向一致、機轉合理。但論述時要把它定位成「**穩健的觀察關聯＋合理機轉**」，而非「隨機化證明的因果」。實務轉換不變：看到初期 dip 先查因（>30% 才評估 AKI/狹窄/容積），別把一個非隨機的分層結果當成停藥或不停藥的鐵證。

---

## 迷思四：只監測高血鉀那一端就安全——U 形風險與「只看一端」的框架偏差

### ❌ 常見誤解
「nsMRA 的血鉀風險就是高血鉀，門診盯著 K>5.5 就好。」把血鉀當成單向、單門檻的二元變數。

### ✅ 統計正解
血鉀與結局是 **U 形**：兩端都危險，而低血鉀端其實更常見、也更容易被忽略。

- **低血鉀端更常見。** FIDELITY 中治療浮現的低血鉀 **K<4.0 達 41.1%、K<3.5 達 7.5%**[label_guideline_safety_Pitt_2025]；安慰劑組 4 年累積發生率，低血鉀甚至**高於**高血鉀——K<4.0 **57.2%（95% CI 55.6–58.8）** vs K>5.5 僅 **10%（9.1–11.0）**[label_guideline_safety_Pitt_2025]。只盯高血鉀＝選擇性忽略了發生率高數倍的那一端。
- **低血鉀端可能更致命。** FINEARTS-HF 的 **time-updated Cox** 顯示：以最近一次血鉀為準，K<3.5 對應的主要結局風險 **HR 2.49（95% CI 1.80–3.43）**，竟**高於** K>5.5 的 **HR 1.64（95% CI 1.04–2.58）**[hf_renal_safety_Vardeny_2025]。FIDELITY 平行結果：最低 K<3.5 者 CV 複合 **HR 1.53**、心律不整 **HR 1.67**、全因死亡 **HR 1.56**[label_guideline_safety_Pitt_2025]。
- **nsMRA 其實把血鉀往中央收斂。** finerenone 顯著**減少**低血鉀：K<4.0 **HR 0.63（0.60–0.66）**、K<3.5 **HR 0.46（0.40–0.53）**[label_guideline_safety_Pitt_2025]；FINEARTS-HF 一致（K<3.5 HR 0.46）[hf_renal_safety_Vardeny_2025]。

**統計亮點**：把血鉀當**連續變項＋時間更新（time-updated）**，比「二元門檻（>5.5 vs 否）」更貼近真相。time-updated 用的是事件前最近一次的血鉀，捕捉了「當下暴露」而非「基線一次量」，這才是 U 形兩端風險能同時浮現的原因。

### 💡 臨床亮點
門診敘事不該只算高血鉀那一邊的帳。一個只被提醒「小心升鉀」的處方者，會系統性低估更常見的低血鉀端——而 nsMRA 恰好在**兩端都有利**（降低血鉀、把整體分布往最低風險帶 4.0–5.0 收斂）。這也校準了 benefit-risk：把 finerenone 貼上「升鉀藥」標籤，是只讀了 U 形的一半。

---

## 迷思五：PBPK 的 fm、AUCR、「完全可逆」都是實測鐵證——模型基礎推論的邊界

### ❌ 常見誤解
把三類**模型輸出**當成直接實測事實：「itraconazole 讓 AUC 升 6.31 倍」「急性 dip 完全可逆是被證明的」「合併 SGLT2i 對急性 dip 無交互，證明兩者完全獨立」。

### ✅ 統計正解
這三者都是「能良好擬合資料的模型陳述」，強度介於實測與假說之間，讀法各有邊界：

- **fm 與 AUCR 是 predicted，不是全部實測。** finerenone 的 PBPK 模型估總 **fm_CYP3A4 ≈ 0.93（腸壁 0.42 ＋ 肝 0.51）**，與 Heinig 靜態估計（點估計 0.88、0.89）一致，**傳播 90% CI 後範圍 0.83–0.94**[label_guideline_safety_Wendl_2022]。強效抑制劑的倍率如 **itraconazole AUCR 6.31、clarithromycin 5.28** 是 PBPK 的**模型預測**（predicted）[label_guideline_safety_Wendl_2022]；部分中效抑制劑（erythromycin 3.48、verapamil 2.70）才是實測。把 predicted 與 observed 混為一談，會高估「已知」的確定性——但 fm≈0.9 這個高值本身，已足以支撐「強效抑制劑列禁忌」的穩健決策。
- **「急性 dip 完全可逆」是模型假設，不是直接臨床證明。** Goulooze 的雙相模型「**assuming full reversibility of the acute eGFR decline described the data well**」——即「完全可逆」是一個**能良好擬合資料（含停藥後資料）的假設**，非直接量到每個病人回到 baseline[egfr_dip_reversibility_Goulooze_2022]。支持它的最接近實測的證據是停藥後 model-free 的 eGFR **回升 6.9%（95% CI +3.9% 至 +10.0%）**，與模型預測的 20 mg 急性下降 5.4% 相稱[egfr_dip_reversibility_Goulooze_2022]。方向與量級對得上，是**相容證據**，不是逐一驗證的因果。
- **「無顯著交互」是『區間含無交互點』，不是『證明完全獨立』。** SGLT2i×finerenone 對**急性 eGFR dip** 的交互 **95% CI 73.2–120%**——因為這個區間**跨越 100%（＝無交互）**，才判定「無顯著修飾」[egfr_dip_reversibility_Goulooze_2022]。這是「證據不足以否定獨立」，不是「證明完全獨立」。同理 UACR 交互 CI 94.1–122%、慢性斜率交互 CI 9.5–144%（後者極寬，資訊量低）[egfr_dip_reversibility_Goulooze_2022]。作者自己也提醒 SGLT2i 非隨機、量化效果須謹慎[egfr_dip_reversibility_Goulooze_2022]。

### 💡 臨床亮點
模型輸出可以放心拿來做**方向性決策**（強效抑制劑禁忌、預期 dip 可逆、合併 SGLT2i 不放大 dip），但講述時要標明「predicted／model-assumed／區間含無交互」。特別是「無顯著交互」——它常被過度讀成「證明兩藥互不影響」，正解是「在現有樣本下，看不出交互，但區間寬到不能排除」。這是把統計謙遜寫進處方語言：**能行動 ≠ 已證明**。

---

## 迷思六：binder 試驗「有效」＝改善硬結局——替代終點的外推邊界

### ❌ 常見誤解
「AMBER、DIAMOND 證明 binder 有效，所以加 binder 能改善病人的死亡與腎衰結局。」把**續用率／血鉀**這類代理終點的成功，直接讀成硬結局獲益。

### ✅ 統計正解
兩個關鍵 binder 試驗的**主要終點都是 surrogate**，不是心腎硬結局：

- **AMBER**（patiromer + spironolactone；resistant HTN + CKD）：主要終點是「week 12 仍在使用 spironolactone 的比例之組間差」——續用率由 **66.2%（98/148）提升至 85.7%（126/147），組間差 19.5%（95% CI 10.0–29.0），P<0.0001**[potassium_binders_monitoring_Agarwal_2019]。終點是「留在藥上」，不是「活更久／腎更好」。
- **DIAMOND**（patiromer + RAASi；HFrEF）：主要終點是「血鉀調整後平均變化之組間差」，並降低 **K⁺ >5.5 事件 HR 0.63（95% CI 0.45–0.87，P=0.006）**[potassium_binders_monitoring_Butler_2022]。同樣是電解質與續用的代理終點。

代理終點鏈是：**binder → 血鉀受控 → 續用有效治療 → （外推）更好結局**。前兩環有 RCT 支撐，最後一環（續用是否真的轉成硬結局改善）是**機轉合理的外推**，目前**無專屬硬結局 RCT**。這不否定 binder 的價值，但界定了它的證據等級。

### 💡 臨床亮點
binder 的正確定位是「把被迫停藥轉為持續治療」的**工程手段**，其證據是「能維持有效治療」，而非「本身改善死亡／腎衰」。溝通時說「binder 幫病人留在該用的藥上」是誠實的；說「binder 降低死亡率」則越過了代理終點的邊界。這與主題四「別把次分析／surrogate 誤用成硬結論」精神一致。

---

## 安全性統計素養檢查表（查房／簡報用一頁）

| 讀到這個時 | 先問這一句 | 對應迷思 |
|---|---|---|
| 「高血鉀風險加倍／HR 2.13」 | 絕對事件率多少？NNH 多少？（相對嚇人、絕對可管理） | 一 |
| 「零高血鉀死亡」 | 這是零風險，還是 n 很大所以上界很低（rule of three）？ | 二 |
| 「dip 在 finerenone 不預示壞結局」 | dip 是隨機分派的嗎？這是條件式分析嗎？關聯≠因果 | 三 |
| 「血鉀風險＝高血鉀」 | 低血鉀那一端呢？連續變項＋time-updated 才看得到 U 形 | 四 |
| 「AUCR 6.31／完全可逆／無交互」 | 是 predicted、model-assumed、還是區間含無交互點？ | 五 |
| 「binder 試驗有效」 | 主要終點是硬結局還是續用率／血鉀（surrogate）？ | 六 |

---

## 證據分層小結

| 論點 | 等級 | 主要本地全文來源 |
|---|---|---|
| 相對加倍（14.0% vs 6.9%；HR 2.13）vs 絕對低（住院 0.9/0.2、停藥 1.7/0.6）；NNH 71 vs 18/45/26 | 🟡 post hoc／pooled | `label_guideline_safety_European_2022`、`pooled_safety_hyperkalemia_Agarwal_2022` 📄 |
| 零高血鉀死亡（>13,000／INFINITY／FINE-HEART）＋ rule of three 上界 | 🟡 pooled；🟢 方法學 | `label_guideline_safety_Wanner_2022`、`pooled_safety_hyperkalemia_Neuen_2026`、`hf_renal_safety_Ostrominski_2026` 📄 |
| dip 預後脫鉤（P-interaction 0.04／0.50；OR 1.95）為非隨機、條件式關聯 | 🟡 前瞻次分析 | `hf_renal_safety_Matsumoto_2025` 📄 |
| U 形雙向 K⁺（低血鉀 41.1%/7.5%；time-updated HR 2.49 > 1.64；保護 HR 0.63/0.46） | 🟡 post hoc | `label_guideline_safety_Pitt_2025`、`hf_renal_safety_Vardeny_2025` 📄 |
| 模型邊界：fm≈0.93（CI 0.83–0.94）、AUCR 6.31 為 predicted、完全可逆為模型假設、交互 CI 73.2–120% 含 100% | 🟡 模型／🟢 方法學 | `label_guideline_safety_Wendl_2022`、`egfr_dip_reversibility_Goulooze_2022` 📄 |
| binder 主終點為 surrogate（AMBER 續用 66.2→85.7%；DIAMOND K>5.5 HR 0.63） | 🟡 surrogate | `potassium_binders_monitoring_Agarwal_2019`、`potassium_binders_monitoring_Butler_2022` 📄 |

---

## 本地全文語料（可 grep 稽核）

📄 全文：`label_guideline_safety_European_2022`（pooled 硬結局 14.0/6.9、住院 0.9/0.2、停藥 1.7/0.6）、`pooled_safety_hyperkalemia_Agarwal_2022`（HR 2.13、NNH 71、0.23 mmol/L）、`label_guideline_safety_Wanner_2022`（13,000 零死亡）、`pooled_safety_hyperkalemia_Neuen_2026`（INFINITY 零死亡、停藥 1.7/0.5）、`hf_renal_safety_Ostrominski_2026`（FINE-HEART n=14,180、NNT 131、零死亡）、`hf_renal_safety_Matsumoto_2025`（dip P-interaction 0.04/0.50、OR 1.95）、`label_guideline_safety_Pitt_2025`（低血鉀 41.1/7.5%、累積 57.2 vs 10%、保護 HR 0.63/0.46、min-K HR 1.53/1.67/1.56）、`hf_renal_safety_Vardeny_2025`（time-updated HR 2.49 vs 1.64、K<3.5 HR 0.46）、`label_guideline_safety_Wendl_2022`（fm 0.93、CI 0.83–0.94、AUCR 6.31/5.28）、`egfr_dip_reversibility_Goulooze_2022`（完全可逆假設、rebound 6.9%、交互 CI 73.2–120%）、`potassium_binders_monitoring_Agarwal_2019`（AMBER 66.2→85.7%、19.5%）、`potassium_binders_monitoring_Butler_2022`（DIAMOND K>5.5 HR 0.63）。

---

## References（Vancouver 風格，含本地檔）

1. European Medicines Agency / Bayer AG. Kerendia (finerenone) EPAR — Product Information (SmPC; pooled FIDELITY safety). EMEA/H/C/005200; 2022. 📄 [label_guideline_safety_European_2022]
2. Agarwal R, Joseph A, Anker SD, et al. Hyperkalemia Risk with Finerenone: Results from the FIDELIO-DKD Trial. J Am Soc Nephrol. 2022;33(1):225–237. 📄 [pooled_safety_hyperkalemia_Agarwal_2022]
3. Wanner C, Fioretto P, Kovesdy CP, et al. Potassium management with finerenone: practical aspects. 2022. 📄 [label_guideline_safety_Wanner_2022]
4. Neuen BL, Heerspink HJL, Perkovic V, et al. Efficacy and safety of finerenone in patients with CKD: an individual participant data pooled analysis (INFINITY). Lancet. 2026. 📄 [pooled_safety_hyperkalemia_Neuen_2026]
5. Ostrominski JW, Filippatos G, Claggett BL, et al. Effect of Finerenone on Morbidity and Mortality in CKD (FINE-HEART pooled analysis). 2026. 📄 [hf_renal_safety_Ostrominski_2026]
6. Matsumoto S, Jhund PS, Henderson AD, et al. Initial Decline in GFR With Finerenone in HFmrEF/HFpEF: A Prespecified Analysis of FINEARTS-HF. J Am Coll Cardiol. 2025;85(2):173–185. 📄 [hf_renal_safety_Matsumoto_2025]
7. Pitt B, Agarwal R, Anker SD, et al. Hypokalaemia in patients with T2D and CKD: the effect of finerenone — a FIDELITY analysis. Eur Heart J Cardiovasc Pharmacother. 2025;11(1):11–19. 📄 [label_guideline_safety_Pitt_2025]
8. Vardeny O, Vaduganathan M, Claggett BL, et al. Finerenone, Serum Potassium, and Clinical Outcomes in HFmrEF/HFpEF. JAMA Cardiol. 2025;10(1). 📄 [hf_renal_safety_Vardeny_2025]
9. Wendl T, Frechen S, Gerisch M, Heinig R, Eissing T. PBPK modeling to predict CYP3A4-mediated DDIs of finerenone. CPT Pharmacometrics Syst Pharmacol. 2022;11(2):199–211. 📄 [label_guideline_safety_Wendl_2022]
10. Goulooze SC, Heerspink HJL, van Noort M, et al. Dose–Exposure–Response Analysis of Finerenone on UACR and eGFR: FIDELIO-DKD. Clin Pharmacokinet. 2022;61(7):1013–1025. 📄 [egfr_dip_reversibility_Goulooze_2022]
11. Agarwal R, Rossignol P, Romero A, et al. Patiromer versus placebo to enable spironolactone use in resistant hypertension and CKD (AMBER). Lancet. 2019;394(10208):1540–1550. 📄 [potassium_binders_monitoring_Agarwal_2019]
12. Butler J, Anker SD, Lund LH, et al. Patiromer for the management of hyperkalemia in HFrEF (DIAMOND). Eur Heart J. 2022;43(41):4362–4373. 📄 [potassium_binders_monitoring_Butler_2022]

---
*此檔為主題五之統計深度解讀分冊，撰寫日期基準 2026-07-11。所有具體數字均可 grep 回上列本地全文 MD。誠實邊界：迷思三之 dip 脫鉤為非隨機、條件式觀察關聯（非因果）；迷思五之 fm/AUCR/完全可逆/無交互為模型基礎推論（predicted／model-assumed／區間含無交互點）；迷思六之 binder 主終點為 surrogate（續用率／血鉀），無專屬硬結局 RCT。臨床協定內容見同資料夾各拆解檔，本檔刻意互補不重複。*
