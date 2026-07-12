# 為什麼停藥後 UACR 會反彈、eGFR dip 會回復？——腎絲球內壓的「一個變因兩面」與可逆功能效應

> 本檔為主題五（高血鉀與 eGFR dip 的安全工程學）之**機制層深挖**。它不重複「dip 的預後與該不該停藥」（見 [`egfr_dip_hemodynamic_reversible.md`](egfr_dip_hemodynamic_reversible.md)），也不重複「反彈的事實與 over-additive 判決」（見 [`../03_fourth_pillar_or_early_combination/confidence_over_additive_and_offtreatment_reversibility.md`](../03_fourth_pillar_or_early_combination/confidence_over_additive_and_offtreatment_reversibility.md)）；本檔只回答一個生理問題：**停藥 30 天內，UACR 為什麼會「反彈」、eGFR 的急性 dip 為什麼會「回復」——為什麼這兩件看似相反的事，其實是同一個血流動力學變因（腎絲球內壓 P_glomerular）的兩面，而且是「可逆的功能效應」而非「結構性損傷或結構性殘餘保護」。**
>
> **引用標記慣例**：📄 = 本地全文可 grep 稽核；📌 = 僅取得 abstract（不對其未載內容作具體數字斷言）。每個數字句末以 `[本地MD檔名]` 標註來源供 grep 回溯。LLM 僅負責組織、改寫與生理詮釋；所有作者／年份／數字均出自本地全文 MD、可 grep 命中。詮釋可有深度，數字不可杜撰。
>
> **證據分層**：🟢 guideline routine｜🟡 evidence expansion（surrogate／post hoc／模型／代理終點）｜🔴 hypothesis（機轉合理、尚無隨機化硬終點驗證）。
>
> **一句話定位**：把腎絲球想成一座「加壓的水壩」。藥物是壓在壩體上的一隻手，把壩內水壓（P_glomerular）往下按——**濾過流量（eGFR）因此下降＝dip，同時滲漏（filtered albumin→UACR）也因此減少**。手一放（停藥），壓力回彈，兩者同步彈回。反彈的存在本身，就是「主導效應是可逆功能性壓力調節、不是結構改變」最直接的證據。

---

## ❓ 1. 反彈的事實：一整組指標在停藥 30 天內「一起回原形」

CONFIDENCE 在治療 180 天後停藥，再於第 210 天（停藥 30 天）測一次。這一個切片同時捕捉到 **UACR 反彈**與**多個功能訊號同步回復**——這是本檔全部推論的實證起點。

| 訊號 | 治療期（建立） | 停藥 30 天（回復） | 來源 |
|---|---|---|---|
| **UACR**（baseline→Day180 LSMR） | combo **0.48（0.44–0.54）**／fine **0.68（0.61–0.76）**／empa **0.71（0.64–0.79）** | 反彈 LSMR（Day180→Day210）combo **1.63（1.49–1.78）**／fine **1.45（1.32–1.59）**／empa **1.44（1.32–1.58）** | `confidence_trial_Agarwal_2025` 📄 |
| **UACR 時程** | 「most of the reduction occurred **within 4 weeks** after the initiation」——快建立 | 對稱地快消退 | `confidence_trial_Agarwal_2025` 📄 |
| **血鉀** | Day14 combo 升 **0.27 mmol/L（0.22–0.32）** | 「declined to **near baseline** levels 30 days after」 | `confidence_trial_Agarwal_2025` 📄 |
| **血壓** | combo 降幅最大 | 「generally **reversible** with drug discontinuation in all treatment groups」 | `confidence_trial_Agarwal_2025` 📄 |
| **eGFR（急性 dip）** | 急性變化 combo **−26.6**／fine **−22.1**／empa **−24.8 mL/min/1.73 m²**（P<0.001） | 「The mean reduction in eGFR was **reversible and returned toward baseline** after drug withdrawal」 | `confidence_egfr_mediation_Agarwal_2026` 📄 |

作者對 eGFR 的定性最關鍵：這個可逆的下降「**do not represent permanent nephron loss**」，急性 dip 是「driven by **tubuloglomerular** feedback adaptation」、且 finerenone「is **not associated with AKI**」；因此把它定位為腎絲球的「functional '**unloading**' of the glomerulus, similar to the effects observed with renin–angiotensin system inhibitors」[confidence_egfr_mediation_Agarwal_2026] 📄。

> **讀法**：反彈不是「藥失效」的壞消息，而是「可逆功能效應」的指紋。一整組指標（UACR、K、BP、eGFR）在同一個 30 天窗口一起回原形——這種「拔掉藥、整組鬆開」的行為，正是藥理性壓力調節的定義，而非結構改變（結構改變不會 30 天內同步復原）。

---

## 🩺 2. 核心洞見：「一個變因、兩個面向」——UACR 下降與 eGFR dip 是 P_glomerular 的一體兩面

這是全檔的樞紐。UACR「下降」與 eGFR「dip」看似方向相反（一個變好、一個變差），但它們**同受一個變因驅動：腎絲球微血管內的濾過壓（intraglomerular pressure，P_glomerular）**。

用水壩比喻把物理講清楚：

- **eGFR ∝ 濾過的驅動壓**。壩內水壓（P_glomerular）越高，越過濾網（腎絲球濾過膜）的水流（GFR）越大。把水壓往下按 → 流量下降 → 這就是 **eGFR dip**。
- **UACR ∝ 濾過膜承受的壓力**。白蛋白本不該漏；當壩內高壓把濾過膜「撐開／衝擊」時，白蛋白被壓力擠過膜（pressure-driven filtration of albumin）→ 尿中白蛋白上升。把水壓往下按 → 膜承受的壓力下降 → 白蛋白滲漏減少 → **UACR 下降**。

兩者是**同一次「按壓 P_glomerular」的兩個可測讀數**：壓力↓ 同時造成「濾過流量↓（eGFR dip）」與「白蛋白漏出↓（UACR↓）」。所以在起始時，我們看到 eGFR 掉、UACR 也掉——**方向相反的兩個數字，其實同源**。

而停藥時，藥物清除 → 按壓的手鬆開 → P_glomerular 回彈 → **同一個變因的兩面同步逆轉**：濾過流量回升（eGFR dip 回復）、白蛋白漏出恢復（UACR 反彈）。CONFIDENCE 的數據正是這個對稱：eGFR「returned toward baseline」與 UACR「反彈 LSMR 1.44–1.63」發生在**同一個 30 天窗口**[confidence_egfr_mediation_Agarwal_2026][confidence_trial_Agarwal_2025] 📄。

> **一句話**：eGFR dip 與 UACR 下降不是兩件事，是**一件事（P_glomerular 下修）的兩個投影**。所以它們一起來、也一起走——這就是「一個變因兩面」。

---

## 🔬 3. afferent／efferent／TGF：兩條路各自下修 P_glomerular（也解釋 over-additive）

P_glomerular 由入球小動脈（afferent）與出球小動脈（efferent）的張力**共同**決定，並受 tubuloglomerular feedback（TGF）調控 filtration fraction。要下修壩內壓力，物理上只有兩條路：**把上游進水口關小（收縮 afferent）**，或**把下游出水口開大（放鬆 efferent）**。CONFIDENCE 的兩隻手各走一條：

### 3.1 SGLT2i（empagliflozin）：收縮 afferent、經 TGF 🟡
Tonneijck 綜述：SGLT2 抑制在近端小管阻斷 Na/glucose 再吸收，使到達 macula densa 的 **sodium-chloride** 濃度恢復，經 **TGF-mediated afferent arteriolar vasoconstriction** 收縮入球小動脈；並以增加 Bowman's space 內 hydraulic pressure 而 constrains filtration pressure——兩機轉都下修 hyperfiltration [egfr_dip_reversibility_Tonneijck_2017] 📄。Oshima 在 CREDENCE 把它講成一句話：SGLT2i 增加遠端 Na/Cl 輸送、augments **tubuloglomerular feedback**、causing **reversal of afferent arteriolar vasodilatation**，故 cause an acute reduction in **intraglomerular pressure** and GFR——並且是 **reversible acute drop**、hemodynamic [egfr_dip_reversibility_Oshima_2021] 📄。

### 3.2 finerenone／RAAS-axis：放鬆 efferent 🟡
Tonneijck：angiotensin II 造成 net increase in **postglomerular（efferent）resistance**，故 ACEi/ARB 阻斷之後 lowers **FF and PGLO**（filtration fraction 與腎絲球壓）[egfr_dip_reversibility_Tonneijck_2017] 📄。Holtkamp 把生理鏈條寫得最完整：RAAS blockade causes **efferent vasodilation → reduced intraglomerular pressure, reduced filtration fraction, and an acute fall in GFR**[r2_Holtkamp_2011] 📄。MR 阻斷同軸下修容量／血壓與腎絲球內壓——CONFIDENCE 作者即把 finerenone 的 dip 類比為 RAS inhibitor 的 glomerular 「unloading」[confidence_egfr_mediation_Agarwal_2026] 📄。

### 3.3 兩把鑰匙、兩把鎖——為什麼「互補」而非「撞天花板」
一收上游、一放下游，都指向同一結果（P_glomerular↓），但**走部分不同的路徑**。CONFIDENCE 的 mediation 分析量化了這個「部分不同」：把 empagliflozin 加到 finerenone 上，多出的 UACR 益處有 **28%（P=0.07）**經急性 eGFR 變化（＝血流動力學）中介；反過來把 finerenone 加到 empagliflozin 上，急性 eGFR 只中介 **5.2%（P=0.23）**——finerenone 的加成 is **nonhemodynamic**[confidence_egfr_mediation_Agarwal_2026] 📄。這正是「兩把不同的鎖」在數字上的樣子，也是 combo UACR 近全加成、combo 急性 dip 最大（−26.6）的機制根據（over-additive 的完整拆解見主題三檔）。

> **關鍵限定**：這兩條路都是**功能性壓力調節**——調的是小動脈張力（可秒級／分鐘級改變的血管平滑肌收縮狀態），不是把腎元「拆掉」或「重砌」。功能性的東西，藥在就在、藥走就走。這是「為什麼可逆」的血管生理根本。

---

## ⏱️ 4. PK→PD 耦合：藥物清除如何讓 P_glomerular 復原、UACR 恢復漏出

把「可逆」從空間（血管張力）延伸到時間軸。afferent／efferent 的張力調節**需要藥物持續佔據其標的**（SGLT2 轉運體、MR）才能維持。一旦停藥：

1. **藥物清除**（finerenone 為短半衰期、每日給藥維持受體佔據；PK 細節交叉連結 pk_pd 檔）→ 標的重新被內源性配體活化（MR 重新被醛固酮活化、SGLT2 恢復再吸收）。
2. **張力調節撤除** → afferent 重新舒張／efferent 重新收縮 → **P_glomerular 回升**。
3. **P_glomerular 回升的兩面同步顯現** → 濾過流量回升（eGFR dip 回復、「returned toward baseline」）＋ 濾過膜壓力回升 → 白蛋白重新被壓過膜（**UACR 反彈**）[confidence_egfr_mediation_Agarwal_2026][confidence_trial_Agarwal_2025] 📄。

時間尺度也吻合：UACR 本就「most of the reduction **within 4 weeks**」——建立與消退都是**週級**，與「停藥 30 天大幅反彈」完全對稱 [confidence_trial_Agarwal_2025] 📄。這種「快起快落」正是短時間常數的功能效應（藥效隨血中濃度走），而非長時間常數的結構重塑。

> **水壩比喻收束**：這隻按住壩體的手，要靠「每天補充握力」（每日給藥）才能維持。斷藥＝鬆手，時間常數是「藥清掉的速度」，不是「壩體被重建的速度」——所以以週計就回彈。

---

## 📉 5. 兩段斜率模型：急性成分「完全可逆」，慢性斜率才是結構層次

把 GFR 隨時間的走勢拆成兩段，可以把「可逆的是哪一段」講到量化層次。

**Holtkamp（RENAAL／losartan）two-slope model** 🟡：RAAS 阻斷之 GFR 走勢 = 「an acute fall in GFR up to 3 months」＋「an attenuation of the long-term GFR slope」。關鍵的可逆性論證：作者指出 the acute fall could be structural or hemodynamic，而「after **withdrawal** of antihypertensive therapy, GFR **increases** in the majority of patients and correlates with the initial GFR fall, supporting a **hemodynamic (not structural) origin**」[r2_Holtkamp_2011] 📄。換言之——**停藥後 GFR 回升這件事本身，就是判定「急性成分是功能性、非結構性」的判準**。這正是 CONFIDENCE 反彈所復刻的邏輯。

**Goulooze（FIDELIO 群體模型）** 🟡：模型辨識出 finerenone 的兩個效應——(i) an **acute eGFR-decreasing effect**＋(ii) a superimposed flattening of the chronic slope；而一個「assuming **full reversibility of the acute eGFR decline**」的模型良好描述資料，**包括停藥後的資料**[egfr_dip_reversibility_Goulooze_2022] 📄。量化 rebound：校正 standard-of-care 下降後，停藥者 eGFR **回升 6.9%（95% CI +3.9% 至 +10.0%）**，與模擬之 finerenone 20 mg 急性下降 **5.4%** 相稱——回升幅度≈當初下降幅度，即「完全可逆」在數字上的樣子 [egfr_dip_reversibility_Goulooze_2022] 📄。

| 模型元素 | 急性成分 | 慢性成分 |
|---|---|---|
| 生理本質 | afferent/efferent 張力調節、P_glomerular 一次性 offset | eGFR slope 的長期趨緩（延緩結構性腎元流失）|
| 可逆性 | **完全可逆**（停藥即回彈，數字對稱：−5.4% ↔ +6.9%）| 需持續用藥累積；停藥則不再累積 |
| 對應 CONFIDENCE 觀察 | UACR/eGFR/BP/K 的 30 天回復 | 6 個月試驗＋30 天洗脫**看不到** |

> **重點**：CONFIDENCE 的 30 天洗脫窗，捕捉的正是**急性、完全可逆的功能成分**。它看得到反彈，是因為反彈的就是這一段；它看不到慢性結構斜率的去留，是因為窗太短（見 §7）。

---

## ⚖️ 6. 為什麼是「可逆功能效應」而不是「結構」——兩個方向都要講清楚

「結構」在這裡有兩種被誤用的方向，都要拆掉：

**(A) dip 不是「結構性損傷」**。跨 class 一致：Oshima 稱 SGLT2i 的 drop 為 hemodynamic、reversible[egfr_dip_reversibility_Oshima_2021]；Oh（RAAS 真實世界準實驗）結論初期下降「are early, transient, and primarily **hemodynamic** in nature rather than reflective of **structural** kidney injury」、「This functional decrease is generally **reversible**」，且平均降幅僅約 **6.5%**、well within safe thresholds[egfr_dip_reversibility_Oh_2026] 📄；CONFIDENCE 直言「do not represent permanent nephron loss」、not associated with AKI[confidence_egfr_mediation_Agarwal_2026] 📄。**反彈的存在，是「非結構損傷」的正面證據**——真的死掉的腎元不會 30 天長回來。

**(B) UACR 的維持也不是「結構性殘餘保護」**。這是反方向的誘惑：既然 finerenone 的加成是 non-hemodynamic（抗發炎／抗纖維化），會不會停藥後仍留下「結構性」低 UACR？CONFIDENCE 的答案是**否**——停藥 30 天 UACR 大幅反彈（LSMR 1.44–1.63），單藥組回到接近基線 [confidence_trial_Agarwal_2025] 📄。關鍵在於：**non-hemodynamic ≠ permanent**。finerenone 的抗發炎／抗纖維化是「**持續受體佔據下的藥理壓制**」，藥一停、MR 重新被醛固酮活化，這條非血流動力學效應同樣鬆開。**UACR 的快速反彈本身，就是「非血流動力學效應仍然可逆」的直接證據**（此判決的完整算術見主題三檔 §Q3）。

> **兩面合起來的判準**：一個效應「停藥即回彈」，就同時排除了「結構性損傷」（損傷不會回彈）與「結構性殘餘保護」（保護若靠結構，停藥不會塌）。**反彈是可逆功能效應的雙向指紋。**

---

## 💡 7. 臨床意涵：dip 不是損傷、反彈不是失效、益處要靠持續給藥維持

1. **eGFR dip 不是損傷，是「壓力被下修」的預期功能訊號**。應事先向病人預告（尤其 baseline eGFR 高、可壓縮 hyperfiltration 空間大者；CONFIDENCE 顯示 baseline eGFR 30 者急性 dip 反而 absent，提示晚期 CKD 血流動力學反應鈍化）[confidence_egfr_mediation_Agarwal_2026] 📄。**不該因 dip 停藥**（完整預後脫鉤論證見 [`egfr_dip_hemodynamic_reversible.md`](egfr_dip_hemodynamic_reversible.md)）。
2. **UACR 反彈不是「藥失效」，而是「壓力保護需要持續給藥」**。像持續按住彈簧——手一放就彈回。這是 disease-modifying 療法**不宜輕易停**的生理理由，而非「療程後可安全撤藥仍享殘餘防護」的證據。
3. **combo 只是把彈簧一開始按得更低**（起點 LSMR 0.48）；停藥後同樣反彈，只是絕對位置仍略低。程度差、時間差，不是「維持極佳低水平」。
4. **臨床操作**：見到 dip，先排除 NSAID、容量不足、過度利尿等外在因素，再談是否調整 disease-modifying 療法——與「unloading the pressure in the kidney」的框架一致 [confidence_egfr_mediation_Agarwal_2026] 📄。

---

## 🔴 8. 誠實邊界（Evidence limits）

- **代理終點＋短窗**：CONFIDENCE 主終點為 UACR、療程約 180 天＋30 天洗脫，無 hard renal/CV outcome；「30 天反彈為可逆功能效應」證據方向明確，但「急性成分完全可逆」在 Goulooze 是**能良好擬合資料的模型假設**，非直接臨床終點證明 🟡 [egfr_dip_reversibility_Goulooze_2022]。
- **本檔看得到什麼、看不到什麼**：30 天洗脫窗捕捉的是**急性可逆功能成分**；**慢性結構性斜率（§5 表右欄）的長期去留，本試驗窗太短、無力評估**——「長期結構性殘餘保護」既未被證實、也非本 Phase 2 設計能回答，屬明示之研究缺口 🔴。
- **mediation 為 exploratory**：28%／5.2% 之 CI 寬、P>0.05（0.07／0.23），「non-hemodynamic」是機轉定性、不等於「不可逆」也不等於「結構」🟡 [confidence_egfr_mediation_Agarwal_2026]。
- **跨 class 佐證多為 post hoc／模型／準實驗**（Holtkamp/Goulooze/Oshima/Oh），方向跨 class 一致但非以「dip→hard outcome」為主終點之 RCT 🟡🔴。
- **PDF 轉檔限制**：Tonneijck 等檔英文長引句多處字元黏連，本檔對其生理內容採概念改寫並保留可 grep 之關鍵詞（afferent／efferent／tubuloglomerular feedback／hyperfiltration／FF／PGLO），未硬填無法 grep 之 verbatim 引號。
- **數字專屬其原始族群**（CONFIDENCE／FIDELIO／RENAAL／CREDENCE／韓國 EMR），外推須保留 🔴。

---

## 證據分層小結

| 論點 | 等級 | 主要本地全文來源 |
|------|------|------------------|
| 停藥 30 天 UACR 反彈（LSMR 1.63/1.45/1.44）+ K/BP/eGFR 同步回復 | 🟡 secondary | `confidence_trial_Agarwal_2025`／`confidence_egfr_mediation_Agarwal_2026` 📄 |
| eGFR「reversible／returned toward baseline／不代表 permanent nephron loss」、TGF adaptation、非 AKI | 🟡 | `confidence_egfr_mediation_Agarwal_2026` 📄 |
| SGLT2i 經 TGF 收縮 afferent → 下修 intraglomerular pressure（可逆） | 🟡 | `egfr_dip_reversibility_Oshima_2021`／`egfr_dip_reversibility_Tonneijck_2017` 📄 |
| RAAS/MR 阻斷放鬆 efferent → 降 FF/PGLO → 急性 GFR 下降 | 🟡 | `r2_Holtkamp_2011`／`egfr_dip_reversibility_Tonneijck_2017` 📄 |
| 兩段斜率：急性成分完全可逆（停藥回升；−5.4%↔+6.9%） | 🟡 model | `r2_Holtkamp_2011`／`egfr_dip_reversibility_Goulooze_2022` 📄 |
| dip 是 hemodynamic 非 structural、functional、可逆（跨 class） | 🟡 | `egfr_dip_reversibility_Oh_2026`／`egfr_dip_reversibility_Oshima_2021` 📄 |
| 長期結構性殘餘保護（>30 天）之去留 | 🔴 本試驗無力回答（誠實揭露） | —（療程 ~6 月＋30 天洗脫）|

## 本地全文語料（可 grep 稽核）

📄 全文：`confidence_trial_Agarwal_2025`（NEJM 主文：反彈 1.63/1.45/1.44、LSMR 0.48/0.68/0.71、within 4 weeks、K 0.27／near baseline、BP reversible）、`confidence_egfr_mediation_Agarwal_2026`（JASN：急性 eGFR 26.6/22.1/24.8、reversible／returned toward baseline／permanent nephron loss／tubuloglomerular feedback／unloading、中介 28%/5.2%、nonhemodynamic）、`egfr_dip_reversibility_Tonneijck_2017`（高濾過生理：afferent/efferent/TGF/FF/PGLO）、`r2_Holtkamp_2011`（RENAAL two-slope、efferent vasodilation、withdrawal GFR increases）、`egfr_dip_reversibility_Goulooze_2022`（FIDELIO 模型：full reversibility、rebound 6.9%／5.4%）、`egfr_dip_reversibility_Oshima_2021`（CREDENCE：reversible acute drop、TGF、afferent、intraglomerular pressure）、`egfr_dip_reversibility_Oh_2026`（RAAS 準實驗：transient、hemodynamic、reversible、非 structural、~6.5%）。

---

## References（Vancouver + 本地檔名）

1. Agarwal R, Green JB, Heerspink HJL, et al. Finerenone with empagliflozin in chronic kidney disease and type 2 diabetes (CONFIDENCE). N Engl J Med. 2025;393(6):533–543. doi:10.1056/NEJMoa2410659. 📄 [confidence_trial_Agarwal_2025]
2. Agarwal R, Correa-Rotter R, Navaneethan SD, et al. Acute eGFR changes and their mediation of albuminuria reduction with empagliflozin and finerenone (CONFIDENCE). J Am Soc Nephrol. 2026. doi:10.1681/ASN.0000001071. 📄 [confidence_egfr_mediation_Agarwal_2026]
3. Tonneijck L, Muskiet MHA, Smits MM, et al. Glomerular hyperfiltration in diabetes: mechanisms, clinical significance, and treatment. J Am Soc Nephrol. 2017;28(4):1023–1039. 📄 [egfr_dip_reversibility_Tonneijck_2017]
4. Holtkamp FA, de Zeeuw D, Thomas MC, et al. An acute fall in estimated glomerular filtration rate during treatment with losartan predicts a slower decrease in long-term renal function (RENAAL post hoc). Kidney Int. 2011;80(3):282–287. 📄 [r2_Holtkamp_2011]
5. Goulooze SC, et al. Dose–exposure–response modelling of finerenone effects on UACR and eGFR in FIDELIO-DKD. 2022. PMID 35508594. 📄 [egfr_dip_reversibility_Goulooze_2022]
6. Oshima M, Jardine MJ, Agarwal R, et al. Insights from CREDENCE: an acute drop in eGFR during canagliflozin treatment and its clinical implications. Kidney Int. 2021. 📄 [egfr_dip_reversibility_Oshima_2021]
7. Oh S, et al. Transient, hemodynamic eGFR decline after RAAS inhibitor initiation: a quasi-experimental staggered DID cohort. 2026. 📄 [egfr_dip_reversibility_Oh_2026]

---
*此檔為主題五之機制層深挖，撰寫日期基準 2026-07-12。所有具體數字均可 grep 回上列本地全文 MD。核心論證：UACR 反彈與 eGFR dip 回復是同一個腎絲球內壓（P_glomerular）下修撤除後的兩個投影，屬急性、完全可逆的功能性壓力調節；「反彈存在」同時排除「結構性損傷」與「結構性殘餘保護」。長期結構性斜率之去留非本 30 天洗脫窗所能評估，屬明示之研究缺口。*
