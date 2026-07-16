# 從硬終點到替代終點:CKD/心腎試驗 endpoint 典範轉移的來龍去脈

> 給內分泌科醫師的深度回顧 — 聚焦 endpoint 邏輯、監管路徑、方法學與趨勢,而非藥物療效本身

---

## 仲裁說明(本版相對原草稿之更動)

必修清單為 0 條;三方稽核提出 7 條「待議」,本版逐條處理如下(均經 PubMed 重新查證):

1. **INFINITY 標記降級**:本地檔 `find_ckd_nondiab_INFINITY_Neuen_2026.md` 明載 `status: abstract_only`(Lancet 付費牆),故第 1.2、7.2 節由 📄 改為 📌,並自證據分級第一層移至第二層。數字經與 abstract 逐字核對後保留。
2. **Neuen JAMA 標記降級**:本地檔 `find_ckd_nondiab_Neuen_2026.md` 亦為 `abstract_only`(JAMA 付費牆),第 7.2 節由 📄 改為 📌、移至第二層。
3. **FIND-CKD CV–腎複合終點改用本地全文**:此統計量在本地 NEJM 全文 `FIND-CKD_NEJMoa2604625.md` 內即可稽核,故第 4.2 節由外部 🌐 升級為 📄,並將原草稿 p=0.043 更正為與原文一致的 **P=0.04**(HR 0.77, 95% CI 0.60–0.99)。經 PubMed(NEJM 2026;394(10):—, DOI 10.1056/NEJMoa2604625, PMID 42246672)覆核無誤。
4. **Ref 27 為重複條目,已合併刪除**:PMID 42246672 經查即 FIND-CKD NEJM 全文本身(=Ref 19),並非獨立 congress abstract;內文原 [find_ckd_nondiab_Heerspink_2026]📌 一律改指 FIND-CKD 全文 📄。
5. **FINE-ONE 已有同儕審查全文,解除「未稽核」警語(部分)**:經 PubMed 確認 FINE-ONE 主結果已刊於 **N Engl J Med. 2026;394(10):947-957, DOI 10.1056/NEJMoa2512854, PMID 41780000(第一作者 Heerspink HJL)**;n=242、6 個月 UACR 相對變化為 primary、finerenone 較安慰劑 UACR 多降 25%(GMR 0.75, 95% CI 0.65–0.87, P<0.001)等數字已與 NEJM 刊出摘要逐項核對相符。惟本地資料夾仍**無** FINE-ONE 全文檔可 grep,故仍列外部層,但標記由「🌐 未稽核」升級為「🌐 已同儕審查、DOI 經 PubMed 核實」。新聞稿保留為 Priority Review 佐證。
6. **§2.3 終點階層表加註**:標明「依 Levey 2020 Table 8」,並補一句說明 30% GFR 下降在特定情境(高基線 GFR、強效應)亦可視為 valid surrogate(Levey 2020 原文),以消除與其行文的張力。
7. **§6.4 模糊 🌐 引用改寫**:原「CKJ / Frontiers in Endocrinology 2024–2025」在 References 無對應條目,已改寫為以既有本地可稽核來源(Collier 2023 效應修飾、Heerspink 2025 寬 BCI)支撐的一般性論述,移除無法回溯的 🌐。

---

## TL;DR(一段式直答)

**為什麼從硬終點轉向 surrogate?** 因為腎臟「真.硬終點」(ESKD、透析、腎因死亡)是罕見且晚期的事件,需要 10–20 年隨訪、上萬受試者才能累積足夠事件;而過去二十年累積了三條獨立證據線(觀察性世代、試驗層級 effect-on-effect、模擬設計),把 eGFR slope 與白蛋白尿變化「資格化(qualify)」為可預測硬終點的替代指標。其中 **3 年 total eGFR slope 的試驗層級 R²≈0.97**,是目前最強的腎臟替代終點 [egfr_slope_surrogate_Inker_2019]📄。

**FDA 為何接受以蛋白尿為 endpoint(FINE-ONE)?** 是的,核心動機正如您的假設 — 硬終點試驗要更多人、更久、更貴。監管框架把終點分成「validated / reasonably-likely-to-predict」兩級:validated surrogate 或 clinical outcome 走 traditional approval,而「reasonably likely」surrogate(如早期 UACR 下降)可走 accelerated approval,限嚴重疾病並通常要求上市後確認試驗 [egfr_slope_surrogate_Levey_2020]📄。early albuminuria 至今**尚未**被 FDA/EMA 核准為 valid surrogate [egfr_slope_surrogate_Taylor_2025]📄,故 FINE-ONE 以 UACR 為 primary 屬 surrogate 定位,不直接證明 kidney failure/CV/死亡獲益 🌐(FINE-ONE NEJM 全文,已同儕審查、DOI 經核)。

**趨勢是否「硬終點越來越少、surrogate 越來越多」?** 部分成立,但更準確的描述是**「雙軌並存、重心後移」**:過半 FDA/EMA 核准已以替代終點為基礎 [egfr_slope_surrogate_Taylor_2025]📄;但可負擔的大適應症(T2D-CKD、HFpEF)仍以硬終點打底(SGLT2i、GLP-1 FLOW、FINEARTS-HF),真正的轉向集中在早期 CKD、非糖尿病/罕見族群與 first-in-indication 情境(FIND-CKD 用 eGFR slope、FINE-ONE 用 UACR)。新藥呈現「大 outcome 試驗硬終點打底 + 擴適應症/早期試驗用 surrogate 加速」的混合設計。

---

## 1. 硬終點的困境:為什麼不夠用

### 1.1 罕見事件 × 晚期發生 = 統計功效的天敵

腎臟硬終點的根本問題是事件太少、太晚。以 FIDELITY 世代的觀察可見:

- FIDELIO-DKD 雖以腎臟複合硬終點為 primary 並達標(HR 0.82, 95%CI 0.73–0.93),但**拆解後單項的 kidney failure(HR 0.87, 0.72–1.05)、ESKD(HR 0.86, 0.67–1.10)、腎因死亡(2 vs 2 例)信賴區間全數跨 1**,真正驅動統計顯著的是較「軟」的 ≥40% eGFR 下降(HR 0.81, 0.72–0.92) [FIDELIO-DKD_NEJMoa2025845]📄。
- 為偵測 20% 風險下降、達 90% power,FIDELIO 需要 **5,734 名受試者、事件驅動 1,068 事件、中位隨訪 2.6 年** [FIDELIO-DKD_NEJMoa2025845]📄。

換言之,即便是一個「陽性」的硬終點試驗,其陽性也主要靠複合終點中較軟的成分撐起來 — 純硬終點事件本身功效不足。

### 1.2 用 pooling「借」事件:單一試驗撐不起硬終點

FIDELITY(FIDELIO + FIGARO 預先設定的 pooled analysis, **N=13,026**)正是為了讓稀少的硬腎終點達到顯著:pooled 後 kidney composite HR 0.77(0.67–0.88, P=0.0002)、ESKD HR 0.80(0.64–0.99, P=0.040)、≥57% eGFR 下降 HR 0.70(0.60–0.83, P<0.0001)才穩定顯著 [FIDELITY_Agarwal_2022]📄。更晚的 INFINITY(FIDELIO+FIGARO+FIND-CKD 個體資料匯集, **14,574 人**)才讓 kidney failure alone(HR 0.85, 0.74–0.99)、CV death(0.82, 0.67–0.999)、all-cause death(0.88, 0.79–0.99)這些最硬的單項達到顯著 [find_ckd_nondiab_INFINITY_Neuen_2026]📌(本地為 abstract-only,Lancet 全文付費牆;上列數字已與 abstract 逐字核對)。**要靠跨試驗匯集上萬人才能點亮硬終點**,恰恰說明單一試驗的硬終點功效困境。

### 1.3 成本、時程與早期 CKD 的可及性

從 1993 年起,血清肌酸酐加倍(≈eGFR 下降 57%)就被 FDA 接受為 CKD 進展替代終點,但它屬晚期事件,需長追蹤與大樣本 [r2_Coresh_2014]📄。改採較小的 eGFR 下降(30–40%)可縮短時程、降成本、提高效率 [r2_Coresh_2014]📄。CKD-PC 資料(高達 170 萬人、12,344 ESRD 事件)量化了差距:基線 eGFR<60 者,2 年 30% eGFR 下降的盛行率 6.9%,而 57% 下降僅 0.79%(相差約 10 倍)[r2_Coresh_2014]📄 — 較小閾值事件多約 10 倍,才適合較短的試驗。

Levey 2020 的模擬進一步量化:baseline GFR 高且無 acute effect 時,用 total slope 可把隨訪從 **4–6 年縮到 2 年**,效率提升 17%–64%、樣本節省 14%–39% [egfr_slope_surrogate_Levey_2020]📄。這就是硬終點「更大、更久、更貴」的直接數字證據,也是您問題 2 假設的實證來源。

---

## 2. Surrogate 如何被「資格化」:三條證據線與 R² 門檻

替代終點不是憑感覺替換,而是由 NKF 主辦、FDA/EMA 共同背書的一套 surrogacy 準則。

### 2.1 三準則 = 三條證據線

2018 NKF-FDA-EMA workshop(Levey 2020)確立 surrogacy 三準則,正好對應三條獨立證據線:(1) **生物合理性**;(2) **觀察性 cohort 的關聯強度與一致性**;(3) **臨床試驗中「治療對替代終點之效果可預測對硬終點之效果」(effect-on-effect / trial-level)** [egfr_slope_surrogate_Levey_2020]📄。Taylor 2025 以 Ciani framework 表述為 Level 3(生物合理性)、Level 2(個人層級觀察關聯)、Level 1(試驗層級治療效果關聯),並指出 **Level 1 在 HTA 決策中最關鍵** [egfr_slope_surrogate_Taylor_2025]📄。

### 2.2 三條線的「量級一致性」是 surrogate validation 的核心

Levey 2020 明示 cohort 與 trial 兩條線量級一致:**UACR 降 30% 或 eGFR slope 減 0.5–1.0 mL/min/1.73m²/年,在 cohort 與 trial 都對應約 HR 0.7** [egfr_slope_surrogate_Levey_2020]📄。這種「不同來源殊途同歸」正是您問題 1 所問的「intermediate effect 高機率一致於 hard endpoint」的直接佐證 — 支持,但下文會看到不確定性仍大。

### 2.3 R² 分級門檻與終點階層

Levey 2020 給出量化門檻:R² **<0.49 為 low、0.49–0.72 為 moderate、≥0.72 為 strong** [egfr_slope_surrogate_Levey_2020]📄。並訂出「硬到軟」的終點階層(**依 Levey 2020 Table 8**):

| 終點 | 證據等級 |
|---|---|
| Kidney failure(ESKD/透析) | Clinical outcome(硬終點) |
| 肌酸酐加倍(57% eGFR 下降)、GFR 下降 >40%、GFR slope 減 >0.5–1.0 | **Valid surrogate** |
| GFR 下降 >30%、UACR 下降 >30% | **Reasonably likely surrogate** |

出處 [egfr_slope_surrogate_Levey_2020]📄。

> **註(消除措辭張力)**:Levey 2020 內文另有「preventing a large GFR decline(30%–57%)is accepted as a valid surrogate... in some circumstances」一句。也就是說,**30% GFR 下降在特定情境(高基線 GFR、強而一致的治療效應)亦可被視為 valid surrogate**;上表把 30% 歸「reasonably likely」是就一般情境的保守分派,與「特定情境可入 valid」並不衝突。UACR 30% 下降則仍穩定歸於 reasonably likely。

這張階層表就是「哪種終點能用、走哪條監管路徑」的制度地圖。

---

## 3. 白蛋白尿 vs eGFR slope:效力差異取決於藥物機轉與族群

這是回答「intermediate effect 是否高機率一致於硬終點」最關鍵、也最需要誠實揭露不確定性的一節。**兩者不是等價的替代終點。**

### 3.1 eGFR total slope:目前最強的腎臟替代終點

- Inker 2019(JASN, 47 RCT/12 介入/60,620 人):3 年 total slope median **R²=0.97(95% BCI 0.78–1.00)**、chronic slope R²=0.96;0.75 mL/min/1.73m²/年的 slope 獲益對應約 **27% 較低 hazard** [egfr_slope_surrogate_Inker_2019]📄。
- Inker 2023(Nat Med, 擴充至 66 比較/186,312 人):3 年 total slope **R²=0.97(0.82–1.00)**、但 chronic slope 僅 **R²=0.55(0.25–0.77)** [egfr_slope_surrogate_Inker_2023]📄。**total 與 chronic slope 的強弱差異是關鍵**:對大型試驗、0.75 的獲益,total slope 的 95% 預測區間排除 HR≥1(0.60–0.89),chronic slope 則否(0.51–1.18);達 97.5% 臨床獲益機率所需閾值 total 只要 0.44、chronic 需 1.26(近 3 倍)[note_inker_slope]📄。這就是 FDA/EMA 偏好 **total slope** 的理由。
- Collier 2023(CJASN):total slope 表現不受基線 GFR/UACR/進展速率影響(交互作用區間皆含 0,R²≈0.93–0.96),chronic slope 則有顯著效應修飾且 R² 僅 0.67–0.70 [egfr_slope_surrogate_Collier_2023]📄。

**Acute dip 如何處理?** Greene 2025(CJASN)把 acute 與 chronic slope 放進同一模型,證實最佳加權恰等於「3 年 total slope」(acute/chronic 權重比 0.078 ≈ 3/33) [egfr_slope_surrogate_Greene_2025]📄。臨床意義:對有負向 acute effect 的藥(SGLT2i、finerenone 的血流動力學效應),因 total slope 涵蓋 acute 段而**不會高估**療效;SGLT2i 雖有負向 acute dip,但被強勁的 chronic slope 獲益蓋過 [egfr_slope_surrogate_Greene_2025]📄。RENAAL post hoc(Holtkamp 2011)是生理學原型:losartan 初期急性 eGFR 下降較大(-2.3 vs 安慰劑 -1.6, P=0.031),但此急性下降越大者長期衰退反而越慢 [r2_Holtkamp_2011]📄 — 解讀 slope 型終點必須把可逆的血流動力學初期變化與結構性長期效應分開。

### 3.2 白蛋白尿:較弱、且高度情境依賴

- **試驗層級 R² 較低且不確定性大**:Heerspink 2019(41 比較/29,979 人)early UACR 變化 median R²=0.47(0.02–0.96),限縮於 ACR>30 mg/g 才升至 0.72;每降 30% albuminuria → 27% 較低 hazard [editorial_endpoints_Heerspink_2019]📄。最新最大的 Heerspink 2025(Nat Med, 48 RCT/85,681 人)median **R²=0.66,但 95% BCI 極寬 0.06–0.98**;每降 30% UACR → 19% 較低 hazard(95% BCI 5–30%)[r2_Heerspink_2025]📌。**寬到 0.06 的下界代表 UACR 對硬終點的替代效力點估計中等、但情境不確定性極高** — 這是對「高機率一致」最誠實的限縮。
- **觀察性基礎穩固,但非一對一**:Coresh 2019(28 世代/693,816 人/7,461 ESKD)2 年 ACR 降 30% → ESKD HR 0.83(校正後 0.78),且**基線 ACR 越高、效力越強(p-interaction<0.001)** [egfr_slope_surrogate_Coresh_2019]📄。但作者坦承 **1/3 至 1/2 的 ESKD 病例在基線期白蛋白尿完全沒上升就發生** [egfr_slope_surrogate_Coresh_2019]📄 — surrogacy 的本質限制。

### 3.3 mediation 分析:白蛋白尿解釋多少療效,依藥物與族群而異

這批 finerenone 特有的中介分析最能回答「一致性到什麼程度」:

- **Agarwal 2023(FIDELITY, N=12,512)**:早期 UACR 下降(連續)中介 **84% 的腎臟終點效果、但僅 37% 的 CV 效果**;二分閾值 ≥30% 則為 64% / 26% [albuminuria_mediation_Agarwal_2023]📌。作者明確自我限制:**"not readily extendable to other drugs"** — 中介比例是 finerenone 特有,不能外推 [albuminuria_mediation_Agarwal_2023]📌。
- **Agarwal 2026(NDT, causal mediation)**:CV 效益中 UACR 中介 39%(7–71)、SBP 21%(3–40),合計 50%(21–100)[albuminuria_mediation_Agarwal_2026]📌。
- **Mc Causland 2025(FINEARTS-HF, 心衰族群, 低基線 UACR 中位 17 mg/g)**:即使起點很低,早期 UACR 下降僅中介 CV 複合終點 34%(連續)或 15%(≥30%)[albuminuria_mediation_Mc_2025]📌。

跨藥物類別的差異同樣鮮明:Matyjek 2026 引用 CKD Trials Consortium 資料,UACR 能解釋的療效比例 **RAASi/ERA 82%、SGLT2i 45%、免疫抑制劑 41%** [editorial_endpoints_Matyjek_2026]📄。

> **小結(問題 1 直答)**:eGFR total slope 是驗證強(R²≈0.97)、跨族群普適的替代終點;白蛋白尿較弱、R² 不確定性大,且主要適用於「白蛋白尿型 CKD + 透過白蛋白尿路徑作用的藥物(RAASi、ns-MRA、ERA)」。「intermediate effect 高機率一致於 hard endpoint」有實證支持,但**並非鐵證,依終點類型(腎 vs CV)、藥物機轉、基線白蛋白尿高低而變動**。

---

## 4. 監管里程碑:workshop → eGFR slope 被接受 → FIND-CKD/FINE-ONE

以下為監管史敘述,外部來源集中於此章並標 🌐,與前述本地可稽核數字分流。

### 4.1 監管時間線

- **1993**:FDA 接受血清肌酸酐加倍為 CKD 進展替代終點 [r2_Coresh_2014]📄。
- **2012 workshop 後**:FDA 接受 confirmed **40%(常見 CKD)/ 30%(罕見 CKD)eGFR 下降**作為完全批准依據;對顯著蛋白尿的原發性腎絲球疾病,接受蛋白尿「完全緩解/近正常化」為完全批准 surrogate、其他「substantial」蛋白尿改善為 accelerated approval 的 reasonably-likely surrogate 🌐(Thompson A et al. FDA Viewpoint, 2019, AJKD; PMID 31672253)。
- **2018 NKF-FDA-EMA workshop(Levey 2020)**:平行完成 cohort meta、trial meta、模擬三路分析,確立 surrogacy 三準則,並訂 FDA/EMA 路徑對應:validated/clinical outcome → traditional approval / full MA;reasonably likely → accelerated approval(限嚴重疾病,通常需上市後確認試驗) [egfr_slope_surrogate_Levey_2020]📄。
- **2023 年 9 月**:EMA 發布 qualification opinion,將 **GFR slope 認定為「validated surrogate endpoint for CKD progression」**;但 **early change in albuminuria 至今未被 FDA 或 EMA 核准為 valid surrogate** [egfr_slope_surrogate_Taylor_2025]📄。Taylor 2025 稱 GFR slope 為 **"first in class" surrogate**,其 R²trial 高達 97%,強於腫瘤(PFS→OS)與心血管(SBP→stroke)常用替代終點 [egfr_slope_surrogate_Taylor_2025]📄。

### 4.2 FIND-CKD:eGFR slope 的旗艦落地(問題 2/4)

FIND-CKD(finerenone 首個非糖尿病 CKD phase 3)primary 明確採 **total eGFR slope**(baseline→month 32 年化下降率,雙斜率線性樣條混合模型),硬複合終點僅列 key secondary [find_ckd_nondiab_Heerspink_2024]📄。樣本大幅縮小到 **1,584 人**,僅需偵測 0.7 mL/min/年的斜率差即 >90% power [FIND-CKD_NEJMoa2604625]📄。結果 primary 達標:finerenone 年 eGFR 下降 -3.3 vs 安慰劑 -4.0(**差 0.7, 95%CI 0.3–1.1, P<0.001**);但硬性 CV 複合事件極少(10 vs 16),HR 0.60 未達顯著 [FIND-CKD_NEJMoa2604625]📄。這正說明:**在小樣本、非糖尿病族群,硬終點無法作 primary,只能靠 surrogate。** 而 key secondary 的 **CV–腎複合終點降 23%(HR 0.77, 95% CI 0.60–0.99, P=0.04)**,同樣可在本地 NEJM 全文直接稽核 [FIND-CKD_NEJMoa2604625]📄(此數字經 PubMed 覆核與刊出摘要一致;原草稿誤記 p=0.043,已更正為 P=0.04)。

### 4.3 FINE-ONE:以 UACR 為 primary 的代表案例(問題 2)

FINE-ONE(第 1 型糖尿病相關 CKD)以 **6 個月 UACR 相對變化為 primary endpoint**。**主結果已刊於同儕審查全文**(N Engl J Med. 2026;394(10):947-957, DOI 10.1056/NEJMoa2512854;NCT05901831):共 **242 人**隨機分派,finerenone 使 UACR 較基線降 34%(GMR 0.66, 95% CI 0.60–0.73)、安慰劑降 12%(GMR 0.88, 0.79–0.98),**相對安慰劑多降 25%(GMR 0.75, 95% CI 0.65–0.87, P<0.001)**;最常見不良事件為高血鉀(10.1% vs 3.3%);6 個月 eGFR 變化 -5.6 vs -2.7(差 -2.9, 95% CI -5.1 至 -0.7),洗滌期後回升接近基線 🌐(FINE-ONE NEJM 全文,已同儕審查;上列數字經 PubMed 與刊出摘要逐項核實)。FDA 對 sNDA 給予 **Priority Review** 🌐(Bayer 新聞稿佐證)。評論明確指出 albuminuria 下降本身**不直接證明** kidney failure/CV/死亡獲益,屬 surrogate 定位。

> **稽核狀態更新**:本地資料夾有 FIND-CKD 全文檔,但**仍無 FINE-ONE 原始檔可 grep**;不過 FINE-ONE 主結果現已有 NEJM 同儕審查全文,n=242、~25% UACR 相對下降等數字已與 PubMed 刊出摘要交叉核實。故本節警語由原草稿的「🌐 全部未稽核」升級為「🌐 已同儕審查、DOI 經 PubMed 核實」。仍建議引用前回溯 NEJM 全文表格。

---

## 5. finerenone 試驗世代的 endpoint 軌跡(對照表)

finerenone 本身就是「endpoint 典範轉移」的縮影:primary 從硬腎終點 → CV 硬終點 → eGFR slope surrogate → UACR surrogate,伴隨樣本與追蹤縮短。

| 試驗 (世代/年份) | Primary endpoint | 終點類型 | N | 追蹤 | Primary 結果 | 來源 |
|---|---|---|---|---|---|---|
| ARTS-DN (phase 2, 2015) | UACR day 90 / baseline 比值 | Surrogate | 823 | 90 天 | 劑量依賴 ↓;15mg 0.67(0.58–0.77) | [arts_dn_dosefinding_Bakris_2015]📄 |
| FIDELIO-DKD (1代, 2020) | 腎臟複合(kidney failure/≥40% eGFR/腎因死亡) | **硬終點** | 5,734 | 2.6 年 | HR 0.82(0.73–0.93) | [FIDELIO-DKD_NEJMoa2025845]📄 |
| FIGARO-DKD (2代, 2021) | CV 複合(CV死亡/MI/stroke/HHF) | **硬終點** | 7,437 | 3.4 年 | HR 0.87(0.76–0.98) | [FIGARO-DKD_NEJMoa2110956]📄 |
| FIDELITY (pooled, 2022) | (預設 pooled 分析) | 硬終點 | 13,026 | 3.0 年 | kidney HR 0.77;CV HR 0.86 | [FIDELITY_Agarwal_2022]📄 |
| FINEARTS-HF (2024) | CV death + total HF events | 硬/半硬 | mediation n=5,086 | — | RR 0.84(0.74–0.95) | [albuminuria_mediation_Mc_2025]📌 / 🌐(Solomon 2024, 10.1056/NEJMoa2407107) |
| FIND-CKD (3代, 2026, 非糖尿病) | **Total eGFR slope**(→month 32) | **Surrogate** | 1,584 | ~32–36.6 月 | 差 0.7 mL/min/年(0.3–1.1), P<0.001 | [FIND-CKD_NEJMoa2604625]📄 |
| FINE-ONE (2026, T1D-CKD) | **6 個月 UACR 相對變化** | **Surrogate** | 242 | 6 月 | UACR 較安慰劑多降 25%(GMR 0.75, 0.65–0.87, P<0.001) | 🌐(FINE-ONE NEJM 全文, 10.1056/NEJMoa2512854;已同儕審查、DOI 經核) |

軌跡總結(可由 FIDELITY 對照佐證):FIDELIO(N5734, kidney composite, 2.6y)→ FIGARO(N7437, CV composite, 3.4y)→ FIND-CKD(N1584, eGFR slope, ~32月)— **樣本與追蹤隨終點軟化而下降** [FIDELITY_Agarwal_2022]📄 [FIND-CKD_NEJMoa2604625]📄。

> FINEARTS-HF 全試驗 N 不在本地檔;表中 n=5,086 為 Mc Causland 2025 mediation 子集(📌 abstract-only),RR 0.84 主結果引自外部 NEJM(🌐)。FINE-ONE 數字引自其 NEJM 同儕審查全文(🌐,無本地檔,但 DOI/數字已經 PubMed 核實)。

---

## 6. 整體趨勢:cardiorenal 新藥是否都走 surrogate?(問題 3/4)

### 6.1 硬終點仍是大適應症的骨幹

在能負擔大樣本、長追蹤的適應症,業界仍以事件驅動硬終點為金標準,且多為陽性(以下皆外部,🌐):

- **SGLT2i**:CREDENCE(canagliflozin, ESKD/肌酸酐加倍/腎或CV死亡, HR 0.70)🌐(Perkovic 2019, 10.1056/NEJMoa1811744);DAPA-CKD(≥50% eGFR/ESKD/腎或CV死亡)🌐(Heerspink 2020, 10.1056/NEJMoa2024816);EMPA-KIDNEY(腎病進展或 CV death)🌐(EMPA-KIDNEY Collaborative Group 2023)。
- **GLP-1**:FLOW(semaglutide, T2D-CKD, n=3,533)primary 為 major kidney outcomes 硬複合,因療效提前中止,主要腎臟事件降 24%(HR 0.76, 0.66–0.88)🌐(Perkovic V et al. 2024, 10.1056/NEJMoa2403347)。
- **心衰**:FINEARTS-HF primary 為 CV death + total worsening HF events 的硬/半硬複合(RR 0.84)🌐(Solomon/McMurray 2024, 10.1056/NEJMoa2407107)。

### 6.2 轉向集中在早期/罕見/first-in-indication + 早期相/組合療法

- **FIND-CKD**(非糖尿病 CKD, eGFR slope primary)、**FINE-ONE**(T1D-CKD, UACR primary):見第 4–5 節。
- **CONFIDENCE**(phase 2, finerenone+empagliflozin, T2D-CKD):以 Day 180 UACR 相對變化為 primary,雙藥組各 KDIGO 風險層 UACR 降 -52% 至 -62% 🌐(Green/Agarwal 2025, NDT, academic.oup.com/ndt/article/40/8/1559)。
- **醛固酮合成酶抑制劑(ASI)**:EASi-KIDNEY 的 phase 2(vicadrostat/BI 690517, 586 人)以 14 週 UACR 變化為主要評估,10mg 使 UACR 較安慰劑降約 40%,以此支持進入大型 cardiorenal outcome trial 🌐(Herrington/Haynes 2025, NDT, academic.oup.com/ndt/article/40/6/1175)。**注意 ASI 的打法仍是「早期用 UACR 加速 → 大型 outcome trial 打硬終點」的雙軌**。
- **IgAN 的 nefecon**:以 2 年 eGFR slope 建模外推長期硬終點(預測硬終點風險降 62%)🌐(Barratt J, CKJ, 2024 online/2025 issue, 10.1093/ckj/sfae404)。

### 6.3 監管與 HTA 的成長,但 payer 較保守

- 過半 FDA/EMA 藥物/生物製劑核准已以替代終點為基礎;FDA 2018 Adult Surrogate Endpoint Table 收錄 >100 項「reasonably likely to predict clinical benefit」終點 [egfr_slope_surrogate_Taylor_2025]📄。
- 但 HTA/payer 較保守:291 份 HTA 報告中 61 份依賴 surrogate,IQWiG/EuNetHTA 要求 correlation ≥0.85(R²trial ≥0.72)才算「high」關聯 [egfr_slope_surrogate_Taylor_2025]📄。**這解釋了為何 FIND-CKD 這類試驗仍保留硬終點複合作 key secondary — 為報銷鋪路。**

### 6.4 反面觀點與批評(誠實揭露)

surrogate 的正向改變不必然轉化為硬終點益處,甚至可能掩蓋危害(外部案例標 🌐):

- **BEACON**(bardoxolone, stage 4 CKD):約 3/4 病患 eGFR 提升,卻因心衰事件增加提前終止並有死亡風險訊號 🌐(de Zeeuw 2013, NEJM/後續分析)。
- **ROADMAP**(olmesartan):顯著延遲微量白蛋白尿發生,卻在 CV death 出現不利訊號 🌐(Haller 2011, NEJM)。
- **移植領域**:校正蛋白尿、mTOR 抑制劑造成的蛋白尿變化,未如預期轉化為移植物存活改變 🌐(Transplant International 2022, 10.3389/ti.2022.10136)。
- **情境依賴性(以本文既有可稽核來源支撐)**:eGFR slope 作 primary 的替代效力隨 CKD 分期與 slope 評估期間而異 — Collier 2023 已示 **chronic slope 有顯著效應修飾(R² 僅 0.67–0.70)、total slope 才穩健(R²≈0.93–0.96)** [egfr_slope_surrogate_Collier_2023]📄;albuminuria surrogacy 則隨基線 UACR/族群大幅擺盪,Heerspink 2025 的 R² 95% BCI 寬達 0.06–0.98 即為明證 [r2_Heerspink_2025]📌。本地端亦呼應:Coresh 2014 指「強而一致的風險關聯是必要但非充分條件」,還需 trial-level 驗證與模擬,並警告較小 eGFR 下降的 HR 可能被急性效應衰減 [r2_Coresh_2014]📄。(原草稿此處引「CKJ / Frontiers in Endocrinology 2024–2025」但 References 無對應條目,已改以上述可稽核來源取代,移除無法回溯的 🌐 標記。)

> **趨勢直答(問題 3/4)**:確有「surrogate 越來越多」的趨勢,但**非全面取代硬終點**。準確描述是「**大型 outcome 試驗用硬終點打底,擴適應症/早期相/組合療法用 surrogate 加速**」的雙軌收斂。SGLT2i、GLP-1(FLOW)仍走硬終點;ns-MRA(FIND-CKD/FINE-ONE)、ASI(vicadrostat 早期相)、IgAN 藥物則明顯採 eGFR slope/UACR primary。

---

## 7. Take-home + 證據分級

### 7.1 給內分泌科醫師的四點結論

1. **硬 → 軟不是妥協,是資格化**:eGFR total slope 因 R²≈0.97 已被 EMA 認定為 validated surrogate;白蛋白尿較弱(R²≈0.47–0.66,不確定性大),尚未被核准為 valid surrogate。
2. **UACR primary(FINE-ONE)確因樣本/時程/成本 + reasonably-likely surrogate 框架**:走 accelerated approval / priority review 精神,但明確屬 surrogate 定位,不直接證明硬終點獲益。
3. **一致性依藥物機轉與族群而異**:UACR 對 finerenone 的腎臟終點中介 84%、CV 僅 37%;RAASi/ns-MRA 這類「靠降白蛋白尿作用」的藥,UACR 才是好的 surrogate。
4. **趨勢是雙軌並存**:解讀新藥試驗時,務必分辨 primary 是硬終點還是 surrogate,並檢視 acute dip 校正(是否用 total slope)、基線 UACR 與 CKD 分期 — 這些決定 surrogate 能否外推到您關心的硬結局。

### 7.2 證據分級(三層 + 限制揭露)

**第一層:本地全文可稽核 📄(信心最高)**
- eGFR total slope R²≈0.97 之 trial-level validation:Inker 2019 [egfr_slope_surrogate_Inker_2019]、Inker 2023 [egfr_slope_surrogate_Inker_2023]、Collier 2023 [egfr_slope_surrogate_Collier_2023]、Greene 2025 [egfr_slope_surrogate_Greene_2025]。
- surrogacy 三準則、終點階層、監管路徑:Levey 2020 [egfr_slope_surrogate_Levey_2020]。
- finerenone 硬終點結果(本地全文):FIDELIO [FIDELIO-DKD_NEJMoa2025845]、FIGARO [FIGARO-DKD_NEJMoa2110956]、FIDELITY [FIDELITY_Agarwal_2022]、**FIND-CKD 全文含 CV–腎複合 HR 0.77 [FIND-CKD_NEJMoa2604625]**。
- 觀察性基礎:Coresh 2019 [egfr_slope_surrogate_Coresh_2019]、Coresh 2014 [r2_Coresh_2014]、Holtkamp 2011 [r2_Holtkamp_2011]。

**第二層:本地 abstract-only 📌(信心中等,數字已與 abstract 逐字核對,但未經全文表格交叉驗證)**
- **INFINITY 個體資料匯集 [find_ckd_nondiab_INFINITY_Neuen_2026]📌**(Lancet 全文付費牆;14,574 人、kidney failure alone HR 0.85 等數字均對 abstract 核實無誤)。
- **Neuen JAMA 腎絲球疾病次群 [find_ckd_nondiab_Neuen_2026]📌**(JAMA 全文付費牆,本文未從此檔抽取具體數字)。
- 白蛋白尿 surrogate 最新驗證:Heerspink 2025 Nat Med [r2_Heerspink_2025]📌(R² 95% BCI 極寬 0.06–0.98,務必附此不確定性)。
- finerenone mediation:Agarwal 2023 [albuminuria_mediation_Agarwal_2023]📌、Agarwal 2026 [albuminuria_mediation_Agarwal_2026]📌、Mc Causland 2025 [albuminuria_mediation_Mc_2025]📌、Levey 2014 abstract [egfr_slope_surrogate_Levey_2014]📌。
- **限制**:上述中介比例(84%/37% 等)有寬信賴區間、且作者聲明不可外推至其他藥物;abstract-only 檔未經全文表格核對,子群 R²/方法細節不可引申。

**第三層:外部來源 🌐(無本地 grep 可稽核檔)**
- **已同儕審查、DOI 經 PubMed 核實**(信心較高,但無本地全文檔):**FINE-ONE NEJM 全文**(Heerspink 2026, 10.1056/NEJMoa2512854;n=242、UACR 較安慰劑多降 25%[GMR 0.75, 0.65–0.87, P<0.001]已核)。
- **監管立場**:Thompson 2019 FDA Viewpoint(PMID 31672253)。
- **對照試驗**:FLOW(10.1056/NEJMoa2403347)、CREDENCE(10.1056/NEJMoa1811744)、DAPA-CKD(10.1056/NEJMoa2024816)、EMPA-KIDNEY、FINEARTS-HF(10.1056/NEJMoa2407107)、CONFIDENCE、EASi-KIDNEY/vicadrostat、nefecon(10.1093/ckj/sfae404)。
- **新聞稿層級(信心最低)**:FIND-CKD / FINE-ONE 之 Bayer press release,僅作 topline 與 Priority Review 佐證。
- 反面案例(BEACON/ROADMAP/移植)為外部轉述,未逐字核對。

**總體限制聲明**:本回顧的 R²、HR、樣本數皆逐字轉錄自素材,未虛構任何作者/年份/DOI/數字;凡 📌 為 abstract-only、凡 🌐 為外部來源(其中 FINE-ONE NEJM 全文已同儕審查且 DOI 經 PubMed 核實,但無本地全文檔),讀者採用前應回溯原文。硬終點趨勢「越來越少」缺乏直接逐年統計,本文僅以「>50% 核准基於 surrogate、surrogate table >100 項」等間接證據推論 [egfr_slope_surrogate_Taylor_2025]📄。

---

## References(Vancouver + DOI)

### 本地全文可稽核(📄)

1. Levey AS, et al. Change in Albuminuria and GFR as End Points for Clinical Trials in Early Stages of CKD (NKF-FDA-EMA Workshop). Am J Kidney Dis. 2020. doi:10.1053/j.ajkd.2019.06.009. PMID 31473020. [egfr_slope_surrogate_Levey_2020]
2. Heerspink HJL, et al. Change in albuminuria as a surrogate endpoint for progression of kidney disease: meta-analysis of treatment effects in RCTs. Lancet Diabetes Endocrinol. 2019. doi:10.1016/S2213-8587(18)30314-0. PMID 30635226. [editorial_endpoints_Heerspink_2019]
3. Coresh J, et al. Change in albuminuria and subsequent risk of ESKD: IPD consortium meta-analysis of observational studies. Lancet Diabetes Endocrinol. 2019. doi:10.1016/S2213-8587(18)30313-9. PMID 30635225. [egfr_slope_surrogate_Coresh_2019]
4. Coresh J, et al. Decline in estimated GFR and subsequent risk of ESRD and mortality. JAMA. 2014. doi:10.1001/jama.2014.6634. PMID 24892770. [r2_Coresh_2014]
5. Inker LA, et al. GFR slope as a surrogate end point for kidney disease progression in clinical trials. J Am Soc Nephrol. 2019. doi:10.1681/ASN.2019010007. PMID 31292197. [egfr_slope_surrogate_Inker_2019 / note_inker_slope]
6. Inker LA, et al. A meta-analysis of GFR slope as a surrogate endpoint for kidney failure. Nat Med. 2023. doi:10.1038/s41591-023-02418-0. PMID 37330614. [egfr_slope_surrogate_Inker_2023]
7. Collier W, et al. Effect modification of GFR slope surrogacy by disease severity. Clin J Am Soc Nephrol. 2023. doi:10.2215/CJN.0000000000000050. PMID 36754007. [egfr_slope_surrogate_Collier_2023]
8. Greene T, et al. Joint model of acute and chronic GFR slope for kidney failure surrogacy. Clin J Am Soc Nephrol. 2025. doi:10.2215/CJN.0000000662. PMID 40237639. [egfr_slope_surrogate_Greene_2025]
9. Collier W, et al. Bayesian hierarchical meta-regression methods for surrogate evaluation. BMC Med Res Methodol. 2024. doi:10.1186/s12874-024-02170-0. [egfr_slope_surrogate_Collier_2024]
10. Holtkamp FA, et al. An acute fall in eGFR during treatment with losartan predicts a slower decrease in long-term renal function (RENAAL post hoc). Kidney Int. 2011. doi:10.1038/ki.2011.79. PMID 21451458. [r2_Holtkamp_2011]
11. Matyjek A, et al. Albuminuria as a surrogate endpoint in CKD (In Context). Clin Kidney J. 2026. doi:10.1093/ckj/sfag054. PMID 42100716. [editorial_endpoints_Matyjek_2026]
12. Taylor RS, et al. Use of surrogate endpoints in HTA and reimbursement of CKD treatments. eClinicalMedicine. 2025. doi:10.1016/j.eclinm.2025.103465. PMID 40932851. [egfr_slope_surrogate_Taylor_2025]
13. Rossing P, et al. Finerenone in CKD and T2D by SGLT2i use (FIDELITY). Diabetes Care. 2022. doi:10.2337/dc22-0294. PMID 35972218. [biomarker_Rossing_2022]
14. Agarwal R, et al. Cardiovascular and kidney outcomes with finerenone: FIDELITY pooled analysis. Eur Heart J. 2022. doi:10.1093/eurheartj/ehab777. PMID 35023547. [FIDELITY_Agarwal_2022]
15. Bakris GL, et al. Effect of finerenone on albuminuria in patients with diabetic nephropathy (ARTS-DN). JAMA. 2015. doi:10.1001/jama.2015.10081. [arts_dn_dosefinding_Bakris_2015]
16. Bakris GL, et al. Effect of Finerenone on CKD Outcomes in T2D (FIDELIO-DKD). N Engl J Med. 2020. doi:10.1056/NEJMoa2025845. [FIDELIO-DKD_NEJMoa2025845]
17. Pitt B, et al. Cardiovascular Events with Finerenone in Kidney Disease and T2D (FIGARO-DKD). N Engl J Med. 2021. doi:10.1056/NEJMoa2110956. [FIGARO-DKD_NEJMoa2110956]
18. Heerspink HJL, Neuen BL, Agarwal R, et al. Finerenone in Persons with Chronic Kidney Disease without Diabetes (FIND-CKD). N Engl J Med. 2026. doi:10.1056/NEJMoa2604625. PMID 42246672. NCT05047263. [FIND-CKD_NEJMoa2604625]（註:原草稿 Ref 27「find_ckd_nondiab_Heerspink_2026」PMID 42246672 經查即本篇全文,非獨立摘要,已合併於此;內文該 citation key 一律指本篇 📄）
19. Heerspink HJL, et al. Design and baseline characteristics of FIND-CKD. Nephrol Dial Transplant. 2024. doi:10.1093/ndt/gfae132. NCT05047263. [find_ckd_nondiab_Heerspink_2024]

### 本地 abstract-only(📌 — 數字逐字轉錄自 abstract、未全文交叉驗證)

20. Levey AS, et al. GFR decline as an end point for clinical trials in CKD. Am J Kidney Dis. 2014. doi:10.1053/j.ajkd.2014.07.030. PMID 25441437. [egfr_slope_surrogate_Levey_2014]
21. Neuen BL, et al. Finerenone in Patients With CKD Due to Glomerular Diseases: A Randomized Clinical Trial. JAMA. 2026. doi:10.1001/jama.2026.9923. PMID 42246414. [find_ckd_nondiab_Neuen_2026]（本地全文付費牆,僅 publisher abstract;原草稿誤置於全文可稽核層,已改標 📌）
22. Neuen BL, et al. Efficacy and safety of finerenone in patients with CKD: an individual participant data pooled analysis (INFINITY). Lancet. 2026;407(10546):2375-2386. doi:10.1016/S0140-6736(26)01009-3. PMID 42248158. [find_ckd_nondiab_INFINITY_Neuen_2026]（本地全文付費牆,僅 abstract;原草稿誤置於全文可稽核層,已改標 📌）
23. Heerspink HJL, et al. A meta-analysis of albuminuria as a surrogate endpoint for kidney failure. Nat Med. 2025. doi:10.1038/s41591-025-04057-z. PMID 41198855. [r2_Heerspink_2025]
24. Agarwal R, et al. UACR reduction as mediator of finerenone effects (FIDELITY mediation). Ann Intern Med. 2023. doi:10.7326/M23-1023. PMID 38048573. [albuminuria_mediation_Agarwal_2023]
25. Agarwal R, et al. Causal mediation of finerenone CV benefit by UACR and SBP (FIDELITY). Nephrol Dial Transplant. 2026. doi:10.1093/ndt/gfag150. PMID 42360710. [albuminuria_mediation_Agarwal_2026]
26. Mc Causland FR, et al. Albuminuria change as mediator in FINEARTS-HF. Nephrol Dial Transplant. 2025. doi:10.1093/ndt/gfaf116.0475. [albuminuria_mediation_Mc_2025]

### 外部(🌐 — 無本地 grep 可稽核檔;27 已同儕審查且 DOI 經 PubMed 核實)

27. **Heerspink HJL, Birkenfeld AL, Cherney DZI, et al. Finerenone in Type 1 Diabetes and Chronic Kidney Disease (FINE-ONE). N Engl J Med. 2026;394(10):947-957. doi:10.1056/NEJMoa2512854. PMID 41780000. NCT05901831.**（同儕審查全文,DOI/PMID 經 PubMed 核實;n=242、UACR 較安慰劑多降 25%[GMR 0.75, 95% CI 0.65–0.87, P<0.001]）
28. Thompson A, et al. (US FDA). Change in eGFR and Albuminuria as End Points in Clinical Trials: A Viewpoint From the FDA. Am J Kidney Dis. 2019. PMID 31672253. https://pubmed.ncbi.nlm.nih.gov/31672253/
29. Greene T, et al. Performance of GFR Slope as a Surrogate End Point: A Statistical Simulation. J Am Soc Nephrol. 2019. doi:10.1681/ASN.2019010009
30. Perkovic V, et al. Effects of Semaglutide on CKD in T2D (FLOW). N Engl J Med. 2024. doi:10.1056/NEJMoa2403347
31. Perkovic V, et al. Canagliflozin and Renal Outcomes (CREDENCE). N Engl J Med. 2019. doi:10.1056/NEJMoa1811744
32. Heerspink HJL, et al. Dapagliflozin in Patients with CKD (DAPA-CKD). N Engl J Med. 2020. doi:10.1056/NEJMoa2024816
33. EMPA-KIDNEY Collaborative Group. Empagliflozin in Patients with CKD. N Engl J Med. 2023.
34. Solomon SD, McMurray JJV, et al. Finerenone in HFmrEF/HFpEF (FINEARTS-HF). N Engl J Med. 2024. doi:10.1056/NEJMoa2407107
35. Green JB, Agarwal R, et al. CONFIDENCE trial (finerenone + empagliflozin), baseline characteristics. Nephrol Dial Transplant. 2025. https://academic.oup.com/ndt/article/40/8/1559/7997692
36. Herrington WG, Haynes R, et al. Vicadrostat (BI 690517) and the EASi-KIDNEY trial rationale. Nephrol Dial Transplant. 2025. https://academic.oup.com/ndt/article/40/6/1175/7896419
37. Barratt J, et al. eGFR slope modelling predicts long-term benefit with nefecon in IgAN. Clin Kidney J. 2024 (online) / 2025 (issue). doi:10.1093/ckj/sfae404
38. de Zeeuw D, et al. Bardoxolone Methyl in T2D and Stage 4 CKD (BEACON). N Engl J Med. 2013.
39. Haller H, et al. Olmesartan for the Delay or Prevention of Microalbuminuria (ROADMAP). N Engl J Med. 2011.
40. Surrogate Endpoints for Late Kidney Transplantation Failure. Transpl Int. 2022. doi:10.3389/ti.2022.10136
41. Bayer / FIND-CKD investigators. Phase III FIND-CKD topline (press release). 2026. https://www.bayer.com/en/us/news-stories/kerendia-for-non-diabetic-chronic-kidney-disease
42. Bayer / FINE-ONE investigators. KERENDIA meets UACR primary endpoint in FINE-ONE; FDA Priority Review for T1D-CKD (press release). 2025–2026. https://www.bayer.com/en/us/news-stories/kerendia-for-type-1-diabetes-and-chronic-kidney-disease

---

*本文由 LLM 依 Phase A 蒐集素材組織改寫,僅做結構化與轉譯,未新增任何未提供之數字或引用;仲裁階段對 FINE-ONE、FIND-CKD、INFINITY、Neuen JAMA 之標記與 DOI 另經 PubMed 覆核。📄=本地全文可稽核;📌=本地僅 abstract(數字逐字轉錄、未全文核對);🌐=外部來源(Ref 27 FINE-ONE 為已同儕審查全文、DOI 經 PubMed 核實,惟無本地全文檔,故仍列外部層)。*
