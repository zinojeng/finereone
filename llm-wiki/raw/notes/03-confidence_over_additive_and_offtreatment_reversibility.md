# CONFIDENCE 的 over-additive 與停藥後真相：UACR −52% 為何超加成、eGFR 為何疊加、停藥後 UACR 是「維持」還是「反彈」？

> 本檔為主題三（第四支柱還是提早聯用？）之延伸拆解，聚焦三個緊密相扣、且**極易被過度樂觀解讀**的問題：(1) combo 的 UACR −52% 為何稱「over-additive」而非只是相加？(2) 為什麼合併 finerenone + empagliflozin 時，eGFR 的急性 dip 會「疊加」？(3) **關鍵**——停藥後，UACR 是否「持續維持在顯著低於基線的極佳水平」（所謂殘餘蛋白尿防護）？本檔用 CONFIDENCE 的原始 30 天洗脫數據，**誠實檢驗**一個流行但方向錯誤的假說。試驗解剖與族群見 [`confidence_trial_deep_dive.md`](confidence_trial_deep_dive.md)；急性 dip 的跨 class 可逆性見 [`../05_hyperkalemia_egfr_dip_safety_engineering/egfr_dip_hemodynamic_reversible.md`](../05_hyperkalemia_egfr_dip_safety_engineering/egfr_dip_hemodynamic_reversible.md)。
>
> **引用標記慣例**：📄 = 本地全文可 grep 稽核；📌 = 僅取得 abstract。每個數字句末以 `[本地MD檔名]` 標註來源供 grep 回溯。LLM 僅負責組織、改寫與藥理詮釋；所有數字均出自本地全文 MD、可 grep 命中。
>
> **證據分層**：🟢 guideline routine｜🟡 evidence expansion（surrogate／prespecified／exploratory／模型）｜🔴 hypothesis（機轉合理、尚無隨機化硬終點驗證）。
>
> **一句話定位**：combo 的 −52% 是**乾淨的全加成**（🟡），eGFR dip 的疊加是**兩條互補血流動力學路徑相加**（🟡）；但使用者的「結構性殘餘防護、停藥後 UACR 維持極佳低水平」假說——就 CONFIDENCE 觀察到的 30 天洗脫窗而言——**不成立，數據甚至指向相反方向**（反彈為主導訊號，🟡）。

---


> 🔬 **機制深挖**：停藥後 UACR 為何反彈（腎絲球內壓「一個變因兩面」的可逆生理）見主題五 [`../05_hyperkalemia_egfr_dip_safety_engineering/uacr_rebound_reversibility_mechanism.md`](../05_hyperkalemia_egfr_dip_safety_engineering/uacr_rebound_reversibility_mechanism.md)。

## ❓ 三個問題，一句話先給答案

| 問題 | CONFIDENCE 的答案 | 等級 |
|---|---|---|
| Q1：−52% 為何叫 over-additive？ | 相對「只加一藥」的增益達 29%／32%，且 52% ≈ 32%+29% 的**全加成**，不見天花板 | 🟡 |
| Q2：eGFR dip 為何疊加？ | 兩藥各自下修球內壓，經**部分不同但同向**的血流動力學路徑相加，combo 急性降幅最大（26.6） | 🟡 |
| Q3：停藥後 UACR 維持極佳低水平？ | **否**。停藥 30 天 UACR 大幅反彈（LSMR 1.44–1.63），單藥組回到接近基線；combo 僅殘留約 −22%——是**可逆功能效應**，非「結構性殘餘防護」 | 🟡 |

---

## 📊 Q1｜為什麼 −52% 是「over-additive」而不是只是「additive」

### 1.1 三個數字的算術 🟡

Day 180 自基線的相對降幅：combination 約 **−52%**、finerenone 單藥約 **−32%**、empagliflozin 單藥約 **−29%**——作者明言 52% 與「finerenone 32% + empagliflozin 29% 的 full additive effect 預期」相符 [confidence_trial_Agarwal_2025] 📄。對應自基線的 least-squares mean ratio（baseline→Day 180）為 combination **0.48（95% CI 0.44–0.54）**、finerenone **0.68（0.61–0.76）**、empagliflozin **0.71（0.64–0.79）** [confidence_trial_Agarwal_2025] 📄。

### 1.2 「over-additive」的精確語意 🟡

CONFIDENCE 兩個主要比較的量化增益是：combo 較 **finerenone 單藥多降 29%**（LSMR 0.71；95% CI 0.61–0.82；P<0.001）、較 **empagliflozin 單藥多降 32%**（LSMR 0.68；95% CI 0.59–0.79；P<0.001）[confidence_trial_Agarwal_2025] 📄。

用白話比喻：把兩個各自能把蛋白尿壓下三成的藥合用，若它們搶同一條路（同一機轉），第二個藥會「撞天花板」、邊際效益遞減，合起來遠不到六成。CONFIDENCE 看到的卻是**兩份降幅幾乎完整相加、不見天花板**——這就是文獻與 editorial 沿用「over-additive」一詞的來由：相對於「只加一藥」的增益（over adding a single agent），而非統計上超越加成模型的協同（synergy）。Georgianos 的 editorial 把此定性得最清楚：兩藥「complementary modes of action」，combined use 產生「an **over-additive** cardiorenal protective effect relative to monotherapy」，臨床前資料中低劑量合用即引發「premature, sustained, and **over-additive** reduction in albuminuria」，並在心與腎均見更大的發炎／纖維化病灶回歸 [combination_editorial_Georgianos_2025] 📄。Cheng 的 narrative review 亦以 CONFIDENCE 證實兩藥「additive benefit」、可同步起始 [combination_editorial_Cheng_2025] 📄。

> **不要誤讀**：「over-additive」在 CONFIDENCE 是「≈ 全加成、無天花板」，不是「1+1>2 的統計協同」。此語意細節與 Goulooze 臨床前「over-additive proteinuria」的交叉連結見 [`../05_hyperkalemia_egfr_dip_safety_engineering/egfr_dip_hemodynamic_reversible.md`](../05_hyperkalemia_egfr_dip_safety_engineering/egfr_dip_hemodynamic_reversible.md) §1.1。

---

## 🔬 為什麼「不撞天花板」——互補機轉的量化（over-additive 的機制根據）

要能相加不撞天花板，兩藥必須**走部分不同的路**。CONFIDENCE 的 eGFR-mediation 分析（exploratory causal mediation）把這件事量化了 [confidence_egfr_mediation_Agarwal_2026] 📄：

- **把 empagliflozin 加到 finerenone 上**：多出的 UACR 益處，急性 eGFR 變化（baseline→Day 14）中介 **28%（P=0.07）**——相當部分走血流動力學（球內壓下修）[confidence_egfr_mediation_Agarwal_2026] 📄。
- **把 finerenone 加到 empagliflozin 上**：急性 eGFR 變化僅中介 **5.2%（P=0.23）**——幾乎全屬非血流動力學 [confidence_egfr_mediation_Agarwal_2026] 📄。

作者的原文結論句：finerenone 的加成效應「is **nonhemodynamic**」、empagliflozin 則「lowered urinary albumin-to-creatinine ratio in part driven by eGFR change」[confidence_egfr_mediation_Agarwal_2026] 📄；並推測 finerenone 的加成「possibly stems from other mechanisms, such as its direct **anti-inflammatory and antifibrotic** effects」，有臨床前資料（SGLT2 缺失可防高濾過卻不減腎纖維化／發炎標記）佐證 [confidence_egfr_mediation_Agarwal_2026] 📄。

> **這正是 over-additive 的機制解**：empagliflozin 主要在「血流動力學端」（球內壓、tubuloglomerular feedback）發力，finerenone 主要在「非血流動力學端」（抗發炎／抗纖維化）發力——兩把鑰匙開的是兩把不同的鎖，所以效應相加而不互相排擠。UACR 中介的機轉深挖與主題二 UACR 中介檔可交叉對讀。

---

## 📉 Q2｜為什麼 eGFR 的急性 dip 會「疊加」

### 2.1 combo 的急性降幅最大 🟡

急性 eGFR 變化（baseline→Day 14）：combination **−26.6 mL/min/1.73 m²**、finerenone **−22.1**、empagliflozin **−24.8**（三組差異 P<0.001）[confidence_egfr_mediation_Agarwal_2026] 📄。combo 最大——這就是「疊加」的直接數據。以「>30% eGFR 下降於 Day 30」的門檻計，combo **17 人（6.3%）** vs finerenone **10 人（3.8%）** vs empagliflozin **3 人（1.1%）**，同樣是 combo 最高 [confidence_trial_Agarwal_2025] 📄。

### 2.2 為什麼會疊加——同向的血流動力學下修 🟡

eGFR 的急性 dip 是「濾過壓下修」的血流動力學指紋：empagliflozin 增加遠端鈉氯輸送、強化 tubuloglomerular feedback、收縮入球小動脈；finerenone 經 MR 阻斷降低容量／血壓與腎絲球內壓。**兩者都把球內壓往下壓、方向相同**，故合用時 dip 相加、combo 降幅最大。作者把它定位為腎絲球的「functional **unloading**」、similar to RAS inhibitors，並強調此 dip「**reversible** … subsequent return toward baseline」、「does not represent permanent nephron loss」[confidence_egfr_mediation_Agarwal_2026] 📄。

### 2.3 疊加但安全——dip 之後穩定、AKI 少、且集中在最禁得起的族群 🟡

疊加的 dip 並未轉成傷害：NEJM 主文載「the eGFR **stabilized** after the initial decline」、combo 的 AKI 僅 **1.9%** [confidence_trial_Agarwal_2025] 📄。決定「誰 dip 大」的是 baseline eGFR——baseline 越高、可壓縮的 hyperfiltration 空間越大，dip 越明顯（P<0.001）；baseline eGFR 30 者「未觀察到大而持續的下降」，提示晚期 CKD 血流動力學反應鈍化 [confidence_egfr_mediation_Agarwal_2026] 📄。與 KDIGO 分層一致：combo 的 >30% eGFR 下降（Day 30±4）**反而集中在 low/moderate（12.1%）與 high（8.2%），very high 最少（4.4%）** [confidence_trial_Vaduganathan_2025] 📄。

**臨床轉譯**：eGFR dip 會疊加，但它是「兩藥同向下修球內壓」的預期功能反應，不是損傷；dip 最大者恰是基線腎功能最好、最禁得起的人。跨 class 的可逆性與「不該因 dip 停藥」的完整論證見 [`../05_hyperkalemia_egfr_dip_safety_engineering/egfr_dip_hemodynamic_reversible.md`](../05_hyperkalemia_egfr_dip_safety_engineering/egfr_dip_hemodynamic_reversible.md)。

---

## 🧪 停藥洗脫的真實數據（Day 180 → Day 210，30 天）

這是檢驗 Q3 假說的關鍵切片。CONFIDENCE 於停藥後 30 天（Day 210）再測一次，用來評估可逆性。

**UACR 大幅反彈**——回升的 least-squares mean ratio（comparing Day 180 with Day 210）為 combination **1.63（95% CI 1.49–1.78）**、finerenone **1.45（1.32–1.59）**、empagliflozin **1.44（1.32–1.58）** [confidence_trial_Agarwal_2025] 📄。方向：全部往上（>1），combo 反彈幅度最大。

**把兩段 LSMR 乘起來估算「Day 210 相對基線」的殘餘降幅**（＝ baseline→Day180 的 LSMR × Day180→Day210 的 LSMR，二者皆 grep 可驗；下表為本檔推算，非原文直接數字）：

| 組別 | baseline→Day180 LSMR | Day180→Day210 LSMR | 推算 Day210 相對基線 | 殘餘降幅（推算） |
|---|---|---|---|---|
| Combination | 0.48 | 1.63 | ≈ 0.78 | 約 **−22%** |
| Finerenone | 0.68 | 1.45 | ≈ 0.99 | 約 **−1%（≈ 回到基線）** |
| Empagliflozin | 0.71 | 1.44 | ≈ 1.02 | 約 **+2%（≈ 回到基線）** |

（LSMR 數字均取自 [confidence_trial_Agarwal_2025] 📄；乘積為本檔算術推算，四捨五入，僅供量級判讀，非原文報告之點估計。）

**同時，其他可逆訊號一起回復**——三者共同構成「功能性、可逆」的圖像：
- **UACR 本就快起快落**：作者記載「most of the reduction occurred **within 4 weeks** after the initiation」[confidence_trial_Agarwal_2025] 📄——快速建立的效應，撤藥後也快速消退。
- **血壓**：combo 降幅最大，但「generally **reversible** with drug discontinuation in all treatment groups」[confidence_trial_Agarwal_2025] 📄。
- **血鉀**：Day 14 combo 升 0.27 mmol/L，「declined to **near baseline** levels 30 days after the trial treatment was stopped」[confidence_trial_Agarwal_2025] 📄。
- **eGFR dip**：撤藥後「return toward baseline」、「does not represent permanent nephron loss」[confidence_egfr_mediation_Agarwal_2026] 📄。

---

## ⚖️ Q3｜假說檢驗判決：「結構性殘餘防護、UACR 維持極佳低水平」——不成立

**使用者的假說**：血流動力學壓力調控在停藥 30 天內打回原形（eGFR 回升），但被修復的腎臟物理結構與被壓制的纖維化需要更久才退化，所以停藥洗脫期仍享有結構性改善帶來的殘餘 UACR 防護，UACR 持續維持在遠低於基線。

**CONFIDENCE 的判決：不支持，甚至指向相反方向。** 🟡

1. **反彈是主導訊號，不是維持**。停藥 30 天 UACR 大幅回升（LSMR 1.44–1.63），單藥組推算回到接近基線（−1%／+2%），combo 也回升到只剩約 −22%——這是**藥理性、功能性、可逆**效應的典型特徵，不是「UACR 維持在極佳低水平」的圖像 [confidence_trial_Agarwal_2025] 📄。
2. **多個功能訊號同步回復**。BP「reversible」、血鉀「near baseline」、eGFR dip「return toward baseline」、UACR「most reduction within 4 weeks」——一整組指標一起打回原形，正是「拔掉藥、壓力就鬆開」的可逆藥效學，而非「結構已改變、效益黏著」[confidence_trial_Agarwal_2025][confidence_egfr_mediation_Agarwal_2026] 📄。
3. **「non-hemodynamic」被誤讀成「結構性／不可逆」**。假說的核心誤解，是把「finerenone 的加成為 non-hemodynamic（非經急性 eGFR 中介，5.2%）」等同於「不可逆的結構重塑」。但 **non-hemodynamic ≠ permanent**——finerenone 的抗發炎／抗纖維化是**持續受體佔據下的藥理壓制**，藥一停、MR 重新被醛固酮活化，效應同樣會鬆開。UACR 的快速反彈本身，就是這條非血流動力學效應**仍然可逆**的直接證據 [confidence_egfr_mediation_Agarwal_2026][confidence_trial_Agarwal_2025] 📄。

### 但要公允補上兩點（避免矯枉過正）

- **(a) combo 起點更低，回落後仍略低於基線**。Day 210 推算 combo 約 −22% vs 單藥組約 0%——combo 確實殘留**略多**降幅，因為它起點更低（0.48 vs 0.68／0.71）、同樣反彈後絕對位置仍較低。但這是**程度差異、時間差**，不是「維持極佳水平」；把 −22%（且仍在上升軌跡上）說成「持續維持顯著低於基線的極佳防護」是過度解讀 [confidence_trial_Agarwal_2025] 📄。
- **(b) CONFIDENCE 無力回答「長期結構性殘餘保護」**。本試驗療程僅約 6 個月 + 30 天洗脫，**觀察窗太短**，既無法證實、也非設計來評估長期結構重塑。因此正確的說法不是「假說被否證為永遠不可能」，而是「**就此 30 天洗脫窗，反彈為主導訊號**；長期結構性殘餘保護在本試驗中未被觀察到，屬本試驗答不了的問題」🔴。

> **正確的框架（可貼門診牆）**：CONFIDENCE 的益處是**持續用藥才維持**的可逆功能效應——像「持續按住彈簧」，手一放（停藥），UACR、BP、血鉀、eGFR 一起彈回。combo 只是把彈簧一開始按得更低。這正是「disease-modifying 療法**不宜輕易停**」的臨床理由（停藥流失益處的長期硬終點對讀見 [`../05_hyperkalemia_egfr_dip_safety_engineering/egfr_dip_hemodynamic_reversible.md`](../05_hyperkalemia_egfr_dip_safety_engineering/egfr_dip_hemodynamic_reversible.md) §4 Singh/FIDELITY）。

---

## 💡 臨床意涵

1. **over-additive 是真的，值得同步起始**：兩藥走互補路徑、效應近全加成（−52%），且益處跨 KDIGO 風險層一致 [confidence_trial_Agarwal_2025][confidence_trial_Vaduganathan_2025] 📄——支持「不必等到極高風險才聯用」。
2. **eGFR dip 會疊加但屬功能性、可逆**：combo 急性降幅最大（26.6），但隨後穩定、AKI 少（1.9%）、最大 dip 集中在基線腎功能最好者——**不應把 dip 當停藥訊號** [confidence_trial_Agarwal_2025][confidence_egfr_mediation_Agarwal_2026] 📄。
3. **益處靠「持續用藥」維持，不是靠「結構已改變、可以停」**：停藥 30 天 UACR 反彈至接近基線（單藥）／僅剩約 −22%（combo）——這是**堅持治療、避免無故停藥**的直接論據，而非「療程後可安全撤藥仍享殘餘防護」的證據 [confidence_trial_Agarwal_2025] 📄。

---

## 🔴 誠實邊界（Evidence limits）

- **surrogate + 短窗**：主終點為 UACR、療程約 180 天 + 30 天洗脫，無 hard renal/CV outcome；「30 天反彈為主導」是可逆性訊號，**不能**外推成「長期無任何結構性殘餘益處」——後者本試驗無力評估 🔴 [confidence_trial_Agarwal_2025]。
- **Day 210 殘餘降幅為推算**：本檔的「≈ −22%／−1%／+2%」由兩段 grep 可驗 LSMR 相乘得出，屬量級判讀，非原文報告之點估計；原文直接報告的是兩段 LSMR 本身 🟡 [confidence_trial_Agarwal_2025]。
- **mediation 為 exploratory**：28% 與 5.2% 的中介百分比 CI 寬、P>0.05（0.07／0.23），屬機轉方向推論而非統計證明；「non-hemodynamic」是機轉定性，不等於「不可逆」 🟡 [confidence_egfr_mediation_Agarwal_2026]。
- **數字專屬 CONFIDENCE 世代**：eGFR 30–90、UACR 100–5000、T2D、已服 RASi、血鉀 ≤4.8；外推須保留 🔴。

---

## 證據分層小結

| 論點 | 等級 | 主要本地全文來源 |
|------|------|------------------|
| combo −52% ≈ full additive（多降 29%／32%，P<0.001） | 🟡 surrogate RCT | `confidence_trial_Agarwal_2025` 📄 |
| over-additive 之互補機轉（加 fine 中介 5.2%、加 empa 28%） | 🟡 exploratory | `confidence_egfr_mediation_Agarwal_2026` 📄 |
| eGFR 急性 dip 疊加（combo 26.6 最大；>30% Day30 6.3%） | 🟡 | `confidence_egfr_mediation_Agarwal_2026`／`confidence_trial_Agarwal_2025` 📄 |
| dip 疊加但穩定、可逆、AKI 少（1.9%） | 🟡 | `confidence_trial_Agarwal_2025` 📄 |
| 停藥 30 天 UACR 反彈（LSMR 1.44–1.63） | 🟡 secondary | `confidence_trial_Agarwal_2025` 📄 |
| BP／血鉀／eGFR 同步回復（reversible／near baseline） | 🟡 | `confidence_trial_Agarwal_2025`／`confidence_egfr_mediation_Agarwal_2026` 📄 |
| 「結構性殘餘防護、UACR 維持極佳低水平」假說 | 🟡 **不成立（30 天洗脫窗）** | `confidence_trial_Agarwal_2025` 📄 |
| 長期結構性殘餘保護（>30 天）之評估 | 🔴 本試驗無力回答（誠實揭露） | —（療程僅 ~6 月 + 30 天洗脫） |

## 本地全文語料（可 grep 稽核）

📄 全文：`confidence_trial_Agarwal_2025`（NEJM 主文：−52%／29%／32%、LSMR 0.48/0.68/0.71、反彈 1.63/1.45/1.44、>30% eGFR Day30、reversible/near baseline/within 4 weeks）、`confidence_egfr_mediation_Agarwal_2026`（JASN：急性 eGFR 26.6/22.1/24.8、中介 28%/5.2%、nonhemodynamic、return toward baseline）、`confidence_trial_Vaduganathan_2025`（KDIGO 分層：Day30 eGFR 12.1%/8.2%/4.4%）、`combination_editorial_Georgianos_2025`（over-additive／complementary 定性）、`combination_editorial_Cheng_2025`（additive benefit／同步起始）。

---

## References（Vancouver + 本地檔名）

1. Agarwal R, Green JB, Heerspink HJL, et al. Finerenone with empagliflozin in chronic kidney disease and type 2 diabetes (CONFIDENCE). N Engl J Med. 2025;393(6):533–543. doi:10.1056/NEJMoa2410659. 📄 [confidence_trial_Agarwal_2025]
2. Agarwal R, Correa-Rotter R, Navaneethan SD, et al. Acute eGFR changes and their mediation of albuminuria reduction with empagliflozin and finerenone (CONFIDENCE). J Am Soc Nephrol. 2026. doi:10.1681/ASN.0000001071. 📄 [confidence_egfr_mediation_Agarwal_2026]
3. Vaduganathan M, Green JB, Heerspink HJL, et al. Simultaneous initiation of finerenone and empagliflozin across the spectrum of kidney risk in the CONFIDENCE trial. Nephrol Dial Transplant. 2026;41(1):161–170. doi:10.1093/ndt/gfaf160. 📄 [confidence_trial_Vaduganathan_2025]
4. Georgianos PI, Koufakis T, Arampatzis S, Liakopoulos V. CONFIDENCE in the safety and efficacy of dual therapy with an SGLT-2 inhibitor and finerenone in patients with chronic kidney disease and type 2 diabetes. Diabetes Obes Metab. 2025;27(11):6097–6100. doi:10.1111/dom.70026. 📄 [combination_editorial_Georgianos_2025]
5. Cheng AYY, Mottl A, Magwire M. Pillar risk-based treatment for chronic kidney disease in people with type 2 diabetes: a narrative review. Diabetes Ther. 2025;16(11):2083–2099. doi:10.1007/s13300-025-01796-7. 📄 [combination_editorial_Cheng_2025]

---

*此檔為主題三之延伸拆解，撰寫日期基準 2026-07-12。所有具體數字均可 grep 回上列本地全文 MD；Day 210 相對基線之殘餘降幅為兩段 LSMR 相乘之推算並已明示。核心判決：使用者「結構性殘餘防護使 UACR 持續維持顯著低於基線」之假說，就 CONFIDENCE 觀察到的 30 天洗脫窗而言不成立（反彈為主導訊號）；長期結構性殘餘保護則非本 Phase 2 試驗所能回答，屬明示之研究缺口。*
