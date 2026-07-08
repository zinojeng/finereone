# Citation Audit — DOI 存活 + Metadata 比對

稽核對象：`01_finerenone_not_just_safer_spironolactone.md` References 區塊(22 筆)
稽核方法：`mcp__paper-search__get_crossref_paper_by_doi`(逐一比對 title/作者/期刊/年份/頁碼)+ 對高風險項目(未來年份、缺 DOI)以 `WebFetch` 直接 resolve `https://doi.org/{doi}` 驗證存活;FIND-CKD 另以 `search_pubmed` 交叉核對。
稽核範圍聲明：僅檢查「論文是否存在 + metadata 是否對得上」,不重複 claim-auditor 的內容數字 grep 工作。

| # | 文中引用(簡) | DOI | Crossref/PubMed 比對結果 | Status |
|---|---|---|---|---|
| 1 | Amazit L et al. J Biol Chem 2015;290(36):21876-89 | 10.1074/jbc.M115.657957 | Title/作者/期刊/卷期頁碼/年份全部相符 | ✅ 通過 |
| 2 | Kolkhof P, Bärfacker L. J Endocrinol 2017;234(1):T125-40 | 10.1530/JOE-16-0600 | 全部相符 | ✅ 通過 |
| 3 | Agarwal R et al. Eur Heart J 2021;42(2):152-61 | 10.1093/eurheartj/ehaa736 | 全部相符;abstract 確認 finerenone 心腎平衡分布、MR 發炎纖維化等文中引用內容存在於原文 | ✅ 通過 |
| 4 | Kolkhof P et al. Int J Mol Sci 2022;23(16):9243 | 10.3390/ijms23169243 | 全部相符 | ✅ 通過 |
| 5 | Pitt B et al. (ARTS) Eur Heart J 2013;34(31):2453-63 | **文中未列 DOI** | Crossref 搜尋確認真實 DOI 為 `10.1093/eurheartj/eht187`,title/作者(Pitt, Kober, Ponikowski, Gheorghiade, Filippatos, Krum 等)/期刊/卷期頁碼與文中所述完全相符,論文存在且可查;WebFetch 確認該 DOI 302 導向 Oxford Academic 頁面,存活 | ❌ **必修**(DOI 缺漏 = 查無):文中此筆參考文獻未附 DOI,違反「含 DOI」的格式要求,應補上 `doi:10.1093/eurheartj/eht187` |
| 6 | Bakris GL et al. (FIDELIO-DKD) NEJM 2020;383:2219-29 | 10.1056/NEJMoa2025845 | Title/作者/期刊/卷/頁碼相符(2020-12-03 出版,383(23):2219-2229;文中僅寫 383:2219-2229 未含 issue,無誤) | ✅ 通過 |
| 7 | Pitt B et al. (FIGARO-DKD) NEJM 2021;385:2252-63 | 10.1056/NEJMoa2110956 | 全部相符(385(24):2252-2263) | ✅ 通過 |
| 8 | Agarwal R et al. (FIDELITY) Eur Heart J 2022;43(6):474-84 | 10.1093/eurheartj/ehab777 | 全部相符;abstract 內 N=13,026、CV HR 0.86 (0.78-0.95, P=0.0018)、腎臟 HR 0.77 (0.67-0.88, P=0.0002) 與文中數字一致 | ✅ 通過 |
| 9 | Agarwal R et al. JAMA Cardiol 2023;8(8):732-741 | 10.1001/jamacardio.2023.1505 | Title/作者/期刊/卷期相符;Crossref extra 欄位頁碼僅顯示起始頁「732」(API 顯示慣例,非文獻本身錯誤),abstract 確認為 FIDELITY 心血管風險可修飾性分析(eGFR/UACR 分層、HR 0.86、交互作用 P=.66) | ✅ 通過(頁碼顯示為 API 截斷,非引用錯誤) |
| 10 | Rossing P et al. Diabetes Care 2022;45(12):2991-98 | 10.2337/dc22-0294 | 全部相符;abstract 確認 SGLT2i 交互作用 P=0.46(CV)/0.29(腎臟)與文中數字一致 | ✅ 通過 |
| 11 | Filippatos G et al. Eur Heart J Cardiovasc Pharmacother 2023;9(2):183-91 | 10.1093/ehjcvp/pvad001 | 全部相符;abstract 確認全因死亡 HR 0.82 (0.70-0.96, P=0.014)、心血管死亡 HR 0.82 (0.67-0.99, P=0.040)、猝死 HR 0.75 (0.57-0.996, P=0.046) 與文中數字一致 | ✅ 通過 |
| 12 | Verma A, Upadhyay A. Diabetes Obes Metab 2026 | 10.1111/dom.70464 | Title/作者相符;Crossref 顯示已分配正式卷期頁(28(4):2582-2593),出版日期 2026-01-19,與「2026」年份標示相符;WebFetch 確認 302 導向 Wiley 頁面,存活 | ✅ 通過 |
| 13 | Docherty KF et al. Circulation 2025 | 10.1161/CIRCULATIONAHA.124.072011 | Title/作者相符;Crossref 顯示正式出版日期 2025-01-07,卷期 151(1):45-58,與文中「2025」相符 | ✅ 通過 |
| 14 | Van Spall HGC, Vardeny O. Heart Fail Rev 2026 | 10.1007/s10741-026-10636-0 | Title/作者相符;Crossref 顯示卷期 31(1),出版日期 2026-05-26,與「2026」相符;WebFetch 確認 302 導向 Springer 頁面,存活 | ✅ 通過 |
| 15 | Lu H et al. JAMA Cardiol 2026 | 10.1001/jamacardio.2026.0682 | Title/作者相符(JAMA 頁面二次確認完整標題與文中一致:"Biomarker, Functional Status, and Quality-of-Life Trajectories Before Modes of Death in Heart Failure: Post Hoc Analysis of the FINEARTS-HF Randomized Clinical Trial");Crossref 卷期 11(6):574,出版 2026-06-01 | ✅ 通過 |
| 16 | Chimura M et al. JAMA Cardiol 2026 | 10.1001/jamacardio.2026.1049 | Title/作者相符;卷期 11(5):416,出版 2026-05-01;abstract 確認 EMPEROR-Preserved 風險模型於 FINEARTS-HF 6001 名患者中應用,與文中敘述一致 | ✅ 通過 |
| 17 | Geller DS et al. Science 2000;289(5476):119-23 | 10.1126/science.289.5476.119 | 全部相符;abstract 確認 S810L 突變、懷孕惡化高血壓、21-羥基缺失類固醇轉為致效劑等文中敘述存在於原文 | ✅ 通過 |
| 18 | Fagart J et al. J Biol Chem 2010;285(39):29932-40 | 10.1074/jbc.M110.131342 | 全部相符 | ✅ 通過 |
| 19 | Coresh J et al. Lancet Diabetes Endocrinol 2019;7(2):115-27 | 10.1016/S2213-8587(18)30313-9 | 全部相符;CKD Prognosis Consortium 作者群、期刊、卷期頁碼一致 | ✅ 通過 |
| 20 | Heerspink HJL et al. (FIND-CKD) **NEJM 2025** | 10.1056/NEJMoa2604625 | Title/作者/期刊相符,論文存在且存活(WebFetch 302 導向 nejm.org);但 **Crossref 與 PubMed 均顯示官方出版年份為 2026**(Crossref published_date = 2026-06-04;PubMed indexed date = 2026-01-01),而非文中標示的「2025」 | ❌ **必修**:出版年份應更正為 **2026**,而非 2025(文中「N Engl J Med. 2025」與資料庫記錄之 2026 不符) |
| 21 | Solomon SD et al. Eur J Heart Fail 2024 | 10.1002/ejhf.3266 | Title/作者/期刊相符;卷期 26(6):1334-46,出版 2024-05-11 | ✅ 通過 |
| 22 | Vaduganathan M et al. Eur J Heart Fail 2024 | 10.1002/ejhf.3253 | Title/作者/期刊相符;卷期 26(6):1324-33,出版 2024-05-14 | ✅ 通過 |

---

## 必修項目彙總

1. **Ref #5(ARTS, Pitt 2013)缺 DOI**:文中引用格式聲稱「含 DOI」,但此筆遺漏。真實 DOI 已查得為 `10.1093/eurheartj/eht187`(Eur Heart J. 2013;34(31):2453-2463,已用 WebFetch 確認存活),建議補上。
2. **Ref #20(FIND-CKD, Heerspink)出版年份錯誤**:文中標示「N Engl J Med. 2025」,但 Crossref(published_date 2026-06-04)與 PubMed(indexed 2026-01-01)均顯示正式出版年份為 **2026**。建議更正為「N Engl J Med. 2026」。此筆同時被本地檔名 `FIND-CKD_NEJMoa2604625.md` 與正文多處引用(第 2、7 節),年份標示應一併留意但不影響其論文本身存在性與內容真實性。

## 待議項目

無其他待議項目 — 除上述兩筆必修外,其餘 20 筆 DOI 均可正常 resolve,且 title/作者/期刊/年份/卷期頁碼與文中標示完全相符。

## PMC ID 一致性

文中 References 區塊未使用 PMC ID(僅用 DOI 標註),故無 PMC ID 一致性問題需檢查。

## 通知

已完成全部 22 筆引用之 DOI 存活與 metadata 比對,結果通知 arbitrator:2 筆必修(缺 DOI / 年份錯誤),0 筆死鏈,0 筆 metadata 實質內容(作者/期刊/題名)錯誤。
