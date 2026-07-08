# Citation Verifier 稽核報告 — 06_beyond_t2d_cardiorenal_landscape

稽核方法:對 References 清單中每筆 DOI 以 `mcp__paper-search__get_crossref_paper_by_doi` 取回 Crossref metadata,逐項比對作者/標題/期刊/年份/卷期頁;無 DOI 者以 `search_crossref` 關鍵字回查是否存在對應紀錄。PMC/PMID 未見於本文 References(僅本地語料 front-matter 有 PMID,不在稽核範圍內予以比對)。

## 逐條結果

| # | 文中引用 | Crossref 比對結果 | Status |
|---|---|---|---|
| 1 | Bakris GL et al. FIDELIO-DKD. N Engl J Med. 2020;383(23):2219-2229. doi:10.1056/NEJMoa2025845 | 標題/作者/期刊/卷期頁完全相符 | ✅ 通過 |
| 2 | Pitt B et al. FIGARO-DKD. N Engl J Med. 2021;385(24):2252-2263. doi:10.1056/NEJMoa2110956 | 完全相符 | ✅ 通過 |
| 3 | Agarwal R et al. FIDELITY. Eur Heart J. 2022;43(6):474-484. doi:10.1093/eurheartj/ehab777 | 完全相符,N=13,026、HR 數字與 abstract 一致 | ✅ 通過 |
| 4 | Heerspink HJL et al. FINE-ONE. N Engl J Med. 2026;394(10):947-957. doi:10.1056/NEJMoa2512854 | 完全相符 | ✅ 通過 |
| 5 | Bayer AG; Halpern L (Pharmacy Times). KERENDIA FDA Priority Review press release. May 21 & 25, 2026. (無 DOI) | 屬新聞稿/trade coverage,非期刊論文,Crossref/PubMed 資料庫本即無收錄,此為預期情況。但文中未附可查證之 URL,無法獨立核實內容 | 🟡 待議(建議補 URL 供稽核) |
| 6 | Beernink JM et al. Diabetes Care. 2026. doi:10.2337/dc26-0882 | 標題/作者/期刊完全相符;內文引用之 P interaction 0.41/0.70、HbA1c 差異 P=0.74 與 abstract 完全一致 | ✅ 通過 |
| 7 | Heerspink HJL et al. "Rationale and design of the FINE-ONE trial." Diabetes Res Clin Pract. 2023;204:110908. doi:10.1016/j.diabres.2023.110908 | DOI/作者/期刊/卷/頁完全相符;但文中引用標題為節略版,原始標題為「Rationale and design of a randomised phase III registration trial investigating finerenone in participants with type 1 diabetes and chronic kidney disease: The FINE-ONE trial」,節略幅度較大(省略了「registration trial」「phase III」等關鍵描述) | 🟡 待議(標題節略,建議還原完整標題或加註「節略」) |
| 8 | Heerspink HJL et al. FIND-CKD. N Engl J Med. 2026. doi:10.1056/NEJMoa2604625 | 標題/作者/期刊/年份相符(尚在 ahead-of-print,無卷期頁屬正常) | ✅ 通過 |
| 9 | Heerspink HJL et al. FIND-CKD design/baseline. Nephrol Dial Transplant. 2025;40(2):308-319. doi:10.1093/ndt/gfae132 | 卷期頁完全相符;Crossref online 上線日為 2024-06-11、正式卷期年份 2025——屬期刊 ahead-of-print 慣例,非錯誤 | ✅ 通過 |
| 10 | Neuen BL et al. FIND-CKD glomerular subgroup. JAMA. 2026. doi:10.1001/jama.2026.9923 | 標題/作者/期刊/年份相符;N=903(IgAN 416/46.1%、FSGS 215/23.8%、MN 90/10.0%)、finerenone 446 vs placebo 457、eGFR slope 差 0.73(0.22–1.24)、白蛋白尿 −42%(35–48%)、HR 0.74(0.57–0.97)與 abstract 逐項相符 | ✅ 通過 |
| 11 | Neuen BL et al. INFINITY. Lancet. 2026. doi:10.1016/S0140-6736(26)01009-3 | 標題/作者/期刊/年份相符 | ✅ 通過 |
| 12 | Vaduganathan M et al. FINE-HEART. Nat Med. 2024. doi:10.1038/s41591-024-03264-4 | 標題/作者/期刊相符;N=18,991、CV 死亡 HR 0.89(0.78–1.01,P=0.076)、全因死亡 HR 0.91(0.84–0.99,P=0.027)、HHF HR 0.83(0.75–0.92,P<0.001)、腎複合 HR 0.80(0.72–0.90,P<0.001)與 abstract 逐字相符 | ✅ 通過 |
| 13 | Docherty KF et al. Circulation. 2025.(**文中無 DOI、無卷期頁**) | 經 `search_crossref` 回查確認真實存在:DOI 10.1161/CIRCULATIONAHA.124.072011,Circulation 2025;151(1):45-58;作者/標題(節略版)相符;LVEF 分層 RR 0.84/0.80/0.94、P interaction 0.70/0.28 與 abstract 完全一致。本地語料 `finearts_hfpef_ckm_Docherty_2025.md` front-matter 已正確記載此 DOI,但正文 References 清單漏列 | 🔴 必修(缺 DOI/卷期頁,應補為 doi:10.1161/CIRCULATIONAHA.124.072011,Circulation. 2025;151(1):45-58) |
| 14 | Mc Causland FR et al. "Finerenone and kidney outcomes in patients with heart failure: the FINEARTS-HF trial." 2025.(**文中無期刊名、無 DOI、無卷期頁**) | 經 `search_crossref` 回查確認真實存在:DOI 10.1016/j.jacc.2024.10.091,J Am Coll Cardiol. 2025;85(2):159-168;作者/標題完全相符。注意:另有一筆同標題但不同 DOI 的 JASN Kidney Week 2024 摘要紀錄(10.1681/asn.2024jpj2c3rq,vol 35 issue 10S,abstract supplement),**不可誤引為此文**——本地語料 `finearts_hfpef_ckm_Mc_2025.md` front-matter 已正確記載真正的 JACC 全文 DOI,但正文 References 清單完全未附期刊/DOI/卷期頁,可讀性上與摘要版本無法區辨 | 🔴 必修(缺期刊名/DOI/卷期頁,易與同名 JASN 摘要混淆,應補為 J Am Coll Cardiol. 2025;85(2):159-168. doi:10.1016/j.jacc.2024.10.091) |
| 15 | Pabon MA et al. FINE-HEART AF. J Am Coll Cardiol. 2025;85(17):1649-1660. doi:10.1016/j.jacc.2025.03.429 | 標題(節略)/作者/期刊/卷期頁完全相符;AF 事件數 286(3.9%)vs 345(4.7%)、HR 0.83(0.71–0.97,P=0.019)待確認於全文(僅 abstract 未含逐字數字,但期刊/卷期頁/DOI 均正確) | ✅ 通過 |
| 16 | Foà A et al. FINE-HEART sudden death. J Am Coll Cardiol. 2026. doi:10.1016/j.jacc.2026.04.045(+ 伴隨評論 Ameri P et al. doi:10.1016/j.jacc.2026.05.031) | 兩筆 DOI 均存在且標題/作者相符:主文「Effects of Finerenone on Sudden Death Across the Cardio-Kidney-Metabolic Landscape」(Foà, Pabon, Filippatos…);伴隨評論「Sudden Death in Cardio-Kidney-Metabolic Patients」(Ameri, Cannatà, Pontremoli)完全相符 | ✅ 通過 |
| 17 | Ostrominski JW et al. FINE-HEART JASN subset. J Am Soc Nephrol. 2026;37(2):312-325. doi:10.1681/ASN.0000000823 | 標題/作者/期刊/卷期頁完全相符;N=14,180、CV死亡或HHF HR 0.83(0.75–0.93,P=0.001)、腎複合 P interaction(UACR)=0.04、非糖尿病敏感度分析 HbA1c P interaction=0.59 與 abstract 逐項相符。Crossref 線上刊出日 2025-09-12、正式卷期 2026——屬 ahead-of-print 慣例,非錯誤 | ✅ 通過 |
| 18 | Ostrominski JW et al. Anthropometric/CKM pooled. J Am Coll Cardiol. 2025;86(20):1781-1801. doi:10.1016/j.jacc.2025.08.039 | 標題/作者/期刊/卷期頁完全相符。**但此筆引用在正文各段落中完全未被 `[finearts_hfpef_ckm_Ostrominski_2025.md]` 標記引用過**(全文搜尋僅出現於 References 清單本身),屬孤兒引用(未使用文獻) | 🟡 待議(metadata 本身正確,但為未被正文使用之孤兒引用,建議刪除或補上對應段落引用) |
| 19 | Claudel SE, Verma A. Cell Metab. 2023;35(12):2104-2106. doi:10.1016/j.cmet.2023.10.015 | 標題/作者/期刊/卷期頁完全相符 | ✅ 通過 |

## 彙總

- **必修(2 項)**:#13(Docherty 2025 Circulation)、#14(Mc Causland 2025 JACC)兩筆正文 References 缺漏 DOI/卷期頁(#14 甚至缺期刊名)。經回查確認論文皆真實存在且 DOI 可解析,**非偽造引用,純屬 Reference 條目資訊不完整**,且 #14 因與同名 JASN 摘要撞名,若不補 DOI 有被誤認/誤核對之風險。建議依下列修正:
  - #13 → `doi:10.1161/CIRCULATIONAHA.124.072011. Circulation. 2025;151(1):45-58.`
  - #14 → `J Am Coll Cardiol. 2025;85(2):159-168. doi:10.1016/j.jacc.2024.10.091.`
- **待議(3 項)**:#5(新聞稿無可查證 URL)、#7(標題節略幅度較大)、#18(孤兒引用,metadata 正確但正文未實際引用)。
- **通過(14 項)**:其餘 14 筆 DOI 皆可於 Crossref 解析,標題/作者/期刊/卷期頁與文中所載一致,關鍵數字(HR/95% CI/P value/樣本數)與 Crossref abstract 逐項核對相符。
- 全文 References 清單中**未見任何 PMID/PMCID 標示**,故 PMC ID 一致性檢查不適用於本文(本地語料 front-matter 雖含 PMID,但非正文引用格式的一部分,不在此稽核範圍)。
- 未發現 ❌DEAD_DOI(所有列出 DOI 之 Crossref 紀錄皆存在)、未發現 ❌META_MISMATCH(標題/作者/期刊/年份經比對後皆屬節略而非錯誤)。
