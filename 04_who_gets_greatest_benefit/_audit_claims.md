# Claim Audit — KDIGO 2026 事實稽核(主題04)

稽核範圍:`04_who_gets_greatest_benefit.md` 第 251 行(第8節末段)與第 290 行(參考文獻34)所有新加入的 KDIGO 2026 事實。
來源檔:`原始PDF/KDIGO_2026_Diabetes_CKD_draft.md`(6389 行,PUBLIC REVIEW DRAFT, MARCH 2026)。

---

## ✅ 通過(Grep 命中且標示草案狀態正確)

| 論斷 | 命中位置(來源檔行號) | 備註 |
|---|---|---|
| Recommendation 4.4.1 全文(eGFR≥25、血鉀正常、UACR≥30 mg/g、最大耐受劑量RASi、nsMRA、**1A**) | L598, L3188 | 逐字命中,"(1A)" 確認 |
| Practice Point 4.4.2「SGLT2i 與 nsMRA 可同步起始」(依CONFIDENCE) | L602, L3346 | 逐字命中;CONFIDENCE 29%/32% 數字亦於 L3306/L3348 命中 |
| Practice Point 4.4.3(血鉀監測) | L606, L3350 | 命中(文中提及但非本文明確斷言主體,列供交叉核對) |
| Practice Point 4.4.7「Do not use steroidal and nsMRA concurrently」 | L614, L3376 | 命中 |
| Recommendation 4.7.1 全文(T1D、eGFR≥25、UACR≥200 mg/g、**2C**) | L771, L781, L4485, L4510 | 逐字命中,"(2C)" 確認 |
| Work Group「因 nsMRA 可用性與熟悉度提高、多數知情病人與醫師會選擇使用」 | L3192 | 語意對應:"greater availability and familiarity...majority of well-informed healthcare professionals and people with T2D and CKD...would want to receive treatment with an nsMRA, while only a small proportion would not" |
| 文件狀態標示「公開審查草案 / Public Review Draft, March 2026 / 尚未定稿」 | L5–10("PUBLIC REVIEW DRAFT" "MARCH 2026" "content of this draft will change...") | 主文與參考文獻34均已標註「公開審查草案,尚未定稿」,狀態標示到位 |
| 亞洲風險描述背景句(4.7.1 之上下文:T1D 治療缺口、FINE-ONE 242人、UACR 200–<5000、eGFR 25–<90) | L4510–4517 | 命中,支持 4.7.1 制定脈絡 |

---

## ❌ GREP_FAIL — 必修

### 1. 【必修】KDIGO 前版建議號「3.8.1」與前版等級「2A」— 全文找不到任何依據,且指引名稱本身有誤

**文中原句(L251)**:
> 「…自 KDIGO 2024(ADA-KDIGO 2022)Recommendation 3.8.1 的 **2A(suggest)升級為 1A(recommend)**——Work Group 明言…」

**未命中字串**:
- `3.8.1` — 全文 grep 僅命中一處無關內容(L3508 表格中的數字 "3.8",非建議編號),**無任何 "Recommendation 3.8.1" 字樣**。
- 前版「2A」等級 — 全文找不到任何處將 nsMRA/finerenone 建議標示為 "2A" 或描述其從 2A 升級為 1A 的具體措辭。原文僅泛稱「Since the previous iteration of the guideline」(L3192),**未給出前版的建議編號或證據等級**。
- 指引名稱錯置:本草案(2026)明確指出其更新對象是 **「KDIGO 2022 Clinical Practice Guideline for Diabetes Management in Chronic Kidney Disease」**(L293、L4582、L4908、L5116、L6018,ref. 362),而文中所稱「**KDIGO 2024**」在本檔案中實際指向**另一份不同的指引**——「KDIGO 2024 Clinical Practice Guideline for the **Evaluation and Management of Chronic Kidney Disease**」(通用CKD指引,非糖尿病專版;L404, L523, L1154, L1732, L4656, L4821, L5222, ref. 1)。文中所寫的「KDIGO 2024(ADA-KDIGO 2022)」把兩份不同指引(通用CKD 2024版 vs. 糖尿病CKD 2022版)混為一談,且「ADA-KDIGO 2022」此命名法在原始草案中未出現。

**結論**:此為典型的 confabulated detail——具體到「3.8.1」建議編號與「2A」等級的精確斷言,在來源檔案中完全找不到對應文字,且指引名稱本身有明顯錯置/混淆之虞。**必修**:應刪除或大幅弱化此「從 2A 升級為 1A」的具體編號/等級比較,只保留可驗證的部分(即「Since the previous iteration...greater availability and familiarity...」的定性描述,已於上方列入✅通過)。若作者手上另有 KDIGO 2022 糖尿病版原文可佐證 3.8.1/2A,應改標其真實來源檔,而非掛在 `KDIGO_2026_Diabetes_CKD_draft` 這個 grep 標籤下。

---

## ⚠️ 待議

### 2. 【待議】「首度納入 T1D 的 nsMRA 建議」— 屬合理推論,但非逐字命中

**文中原句(L251)**:
> 「…同一草案並新增 Practice Point 4.4.2…及**首度納入 T1D 的 nsMRA 建議**(Recommendation 4.7.1,2C,UACR ≥200 mg/g)…」

Recommendation 4.7.1 本身確實逐字命中(見✅通過),且上下文(L4510–4517)描述 T1D 族群過去在 nsMRA/SGLT2i/GLP-1 相關 RCT 中「被排除或僅少量納入」("people with T1D were excluded or represented only in small numbers")、"important uncertainties remain...in comparison to those with T2D",並描述 FINE-ONE(T1D 專屬試驗)為此建議的實證基礎。這些脈絡**支持**「首度」的推論,但草案原文**並未使用「first」「for the first time」或等義字眼明確自稱這是 KDIGO 糖尿病-CKD 指引史上首次針對 T1D 提出的 nsMRA 建議**——grep 找不到逐字佐證此「首度」的斷言本身。

**建議處理**:可保留但需弱化措辭(例如改為「首度」改標示為作者推論而非逐字引述,或改寫成「新增的 T1D nsMRA 建議」,移除「首度」這個無法逐字驗證的強斷言),或在文中以編輯註記標示此為根據上下文的合理推論。

### 3. 【待議】「KDIGO eGFR×UACR 風險分層(low/moderate/high/very-high)在 2026 草案中不變」— 無法以 grep 直接驗證,且與草案自述的更新範圍存在潛在張力

**文中原句(L251)**:
> 「惟本主題所倚賴的 **KDIGO eGFR×UACR 風險分層(low/moderate/high/very-high)在 2026 草案中不變**,故熱圖與絕對事件率梯度之判讀不受影響。」

草案中風險分層熱圖以圖片形式呈現(Figure 1,L797–799:"KDIGO heatmap with risk categories..."),**該圖片本身未被 OCR 成可 grep 的文字**,故無法用字串比對直接確認 2026 草案的 low/moderate/high/very-high 分級邊界與舊版完全相同。此外,草案自述(L293)本次更新**明確包含「新 Chapter 1(definitions, prevention, case-finding, **staging**, and cardiovascular risk assessment)」**——而風險分層熱圖正屬於 Chapter 1 的 staging 內容,與文中所稱「不變」存在語意張力(草案宣稱 Chapter 1 有更新,不代表分層邊界一定變動,但也不能反向推論「不變」)。

**建議處理**:此句屬無法以現有可搜尋文字 grep 證實或證偽的推論性陳述,應標記為推論/待確認,或改為更保守的措辭(如「本文未發現風險分層邊界變動之跡象,但因該圖為圖片格式無法逐字覆核」),不宜以確定語氣宣稱「不變」。

---

## 統計摘要

| Severity | 件數 |
|---|---|
| 必修 | 1(3.8.1 / 2A 前版編號與等級、指引名稱混淆) |
| 待議 | 2(「首度」推論用語;風險分層「不變」之無法grep驗證推論) |
| 通過 | 7 項核心 KDIGO 2026 事實(4.4.1/1A、4.4.2、4.4.3、4.4.7、4.7.1/2C、Work Group 判斷措辭、草案狀態標示) |

**總體結論**:KDIGO 2026 草案本身引用的建議條號、UACR 門檻、證據等級(1A/2C)與 SGLT2i 同步起始等核心事實**均逐字命中來源檔**,且「公開審查草案/尚未定稿」狀態標示落實到位。唯一的**必修**問題出在文中額外添加的「與 KDIGO 前版比較」細節(建議編號 3.8.1、等級 2A、指引名稱 KDIGO 2024/ADA-KDIGO 2022)——這段具體到編號與等級的比較性斷言在來源檔案中找不到任何逐字或語意對應,且指引名稱本身有錯置嫌疑,應視為 confabulated detail 予以刪除或降級處理。另有兩處推論性措辭(「首度」、風險分層「不變」)建議弱化為推論語氣,避免造成「逐字實證」的錯誤印象。
