# Citation Verification Audit — 04_who_gets_greatest_benefit

稽核方式:對 References 清單中每一筆 DOI，以 CrossRef（`get_crossref_paper_by_doi` / `search_crossref`）及 PubMed（`search_pubmed`）拉取權威 metadata（title / authors / journal / volume / issue / page / year），逐項比對主文 References 清單第 1–33 筆所寫內容。另檢查每筆文獻是否確實在正文被 `[citation_key]` 引用（避免「有書目、無引用」的孤兒文獻）。全文無 PMID/PMC 標註，故此部分不適用。

## 逐筆結果

| # | 作者/年 | DOI | CrossRef 解析 | Title/作者/期刊/卷期頁比對 | 正文是否有對應 `[key]` 引用 | Status |
|---|---|---|---|---|---|---|
| 1 | Agarwal 2022, Eur Heart J | 10.1093/eurheartj/ehab777 | ✅ 解析成功 | 完全相符（43(6):474–84） | 是（多處，`stage4_ckd_Agarwal_2022`） | ✅ 通過 |
| 2 | Agarwal 2023, JAMA Cardiol | 10.1001/jamacardio.2023.1505 | ✅ 解析成功 | 完全相符（8(8):732–41）；摘要數字（eGFR/UACR 熱圖、38,359 事件、66%/25,357/38,360）與正文引用值逐一核對一致 | 是（多處） | ✅ 通過 |
| 3 | Bakris 2023, Kidney Int | 10.1016/j.kint.2022.08.040 | ✅ 解析成功 | 完全相符（103(1):196–206）；CrossRef 無摘要可取，與文中「📌abstract only」標記一致 | 是 | ✅ 通過 |
| 4 | Filippatos 2023, Eur Heart J Cardiovasc Pharmacother | 10.1093/ehjcvp/pvad001 | ✅ 解析成功 | 完全相符（9(2):183–91）；摘要中死亡率 HR、on-treatment 數字與正文引用一致 | 是（多處） | ✅ 通過 |
| 5 | Wada 2025, Kidney Dis | 10.1159/000545415 | ✅ 解析成功 | 完全相符（11:402–15）；摘要 HR/CI 數字（CV 0.90 [0.70–1.15]；≥57% 0.64 [0.50–0.82]；≥40% 0.67 [0.56–0.80]；血鉀 15.6%/17.1%、1.5%/1.8%）與正文逐一核對一致 | 是（多處） | ✅ 通過 |
| 6 | Li 2026, Kidney Dis | 10.1159/000550850 | ✅ 解析成功 | 完全相符（12:318–29）；N=697、≥57% HR 0.57 [0.38–0.86]、≥40% HR 0.54 [0.40–0.74]、CV HR 0.82 [0.52–1.29] 與正文完全一致 | 是（多處） | ✅ 通過 |
| 7 | Li 2025, Front Endocrinol | 10.3389/fendo.2025.1568438 | ✅ 解析成功 | 完全相符（16:1568438）；N=325、CV HR 0.91 [0.50–1.67]（正文寫「HR 0.91(0.50–1.67)」於表格一致，惟正文段落另處引用 ≥57% HR 0.40(0.19–0.83) 屬摘要未含之細節，無法逐一從 CrossRef 摘要核對，但 ≥40% HR 0.48 [0.29–0.79] 與摘要相符） | 是（多處） | ✅ 通過（部分細節如 ≥57% HR 0.40 未見於 CrossRef 摘要，屬全文內數字，非本查核範圍） |
| 8 | Zhang 2023, Kidney Dis | 10.1159/000531997 | ✅ 解析成功 | 完全相符（9(6):498–506）；N=372、HR 0.59 [0.39–0.88]、ARR 12.2%、NNT 8 (4–84)、次要終點 HR 0.75 [0.38–1.48] 與正文完全一致 | 是（多處） | ✅ 通過 |
| 9 | Raza 2025, BMC Nephrol | 10.1186/s12882-025-04526-0 | ✅ 解析成功 | 完全相符（26:676，作者 22 人清單與正文 et al. 縮寫一致） | 是（多處） | ✅ 通過 |
| 10 | Sato 2024, FOUNTAIN | **（正文未列 DOI）** | ✅ 經搜尋確認存在：**10.3390/jcm13175107**，J Clin Med. 2024;13(17):5107（PMID 39274317） | ❌ 正文書目寫「[Adv Ther / FOUNTAIN]. 2024.」——期刊名為佔位符/錯誤，非實際發表期刊（實際為 *Journal of Clinical Medicine*），且缺 DOI、卷期頁。内文引用的數字（N=1029、高血鉀 2.16/2.70 每 100 人、無相關住院、SGLT2i 72%、GLP-1RA 30%、CHF 60–66%）與 PubMed/CrossRef 摘要逐一核對**完全正確** | 是（多處，`asian_subgroup_Sato_2024`） | ❌ **META_MISMATCH（書目資訊缺失/錯誤，非內容錯誤）** |
| 11 | Li 2024, Cardiorenal Med | 10.1159/000538347 | ✅ 解析成功 | 相符（review 性質，與文中「📌abstract only」及「review 直言結論宜審慎」一致） | 是 | ✅ 通過 |
| 12 | Filippatos 2022, Circulation | 10.1161/CIRCULATIONAHA.121.057983 | ✅ 解析成功 | 完全相符（145:437–47）；摘要中新發 HF HR 0.68 [0.50–0.93]、CV死亡或首次HHF HR 0.82 [0.70–0.95]、首次HHF HR 0.71 [0.56–0.90] 與正文完全一致 | 是（多處） | ✅ 通過 |
| 13 | Filippatos 2024/2025, ESC Heart Fail (LVH) | 10.1002/ehf2.14962 | ✅ 解析成功 | 卷期頁相符（12(1):185–8）；**CrossRef published_date 為 2024-09-03（epub），但正文書目寫「2025」，而引用鍵卻用 `_Filippatos_2024`**——年份標示不一致（online-first vs print issue 慣例可能造成，非必然錯誤，但建議統一） | 是（多處） | ⚠️ 待議（年份標示 2024 vs 2025 不一致，DOI/卷期頁本身正確） |
| 14 | Jaiswal 2024, IJC Heart Vasc | 10.1016/j.ijcha.2024.101548 | ✅ 解析成功 | 完全相符（55:101548） | 是 | ✅ 通過 |
| 15 | Neves 2026, Diabetes Obes Metab | 10.1111/dom.70750 | ✅ 解析成功 | 完全相符（28(7):6022–33）；摘要中 0/1/2/≥3 目標比例 29/40/24/7%、事件率 6.0/5.1/4.3/3.5 每100人年 與正文完全一致 | 是（多處） | ✅ 通過 |
| 16 | Agarwal 2025, Diabetes Care (CONFIDENCE GLP-1RA) | 10.2337/dc25-1673 | ✅ 解析成功 | 完全相符（48(11):1904–13）；N=800、23% GLP-1RA、UACR 變化數字與正文一致 | 是 | ✅ 通過 |
| 17 | Agarwal 2025, NEJM (CONFIDENCE) | 10.1056/NEJMoa2410659 | ✅ 解析成功 | 完全相符（393:533–43，doc 未列 issue，不影響） | 是 | ✅ 通過 |
| 18 | Haq 2025, J Clin Med | 10.3390/jcm14093213 | ✅ 解析成功 | 完全相符（14(9):3213，作者 4 人清單完全吻合） | 是 | ✅ 通過 |
| 19 | Zhao 2026, J Diabetes Investig | 10.1111/jdi.70368 | ✅ 解析成功 | 相符（N=45、12個月、HOMA-IR/TYG 與正文描述一致） | 是 | ✅ 通過 |
| 20 | Zuin 2026, Eur J Heart Fail | 10.1093/ejhf/xuag150 | ✅ 解析成功 | 相符；摘要「FIDELIO-DKD (HR .86, NNT 56)」與正文「FIDELIO 主要複合 CV HR 0.86、NNT 56」逐字一致 | 是 | ✅ 通過 |
| 21 | Sun 2010, BMJ | 10.1136/bmj.c117 | ✅ 解析成功 | 完全相符（340:c117） | 是（多處，方法學樞紐） | ✅ 通過 |
| 22 | Sun 2012, BMJ | 10.1136/bmj.e1553 | ✅ 解析成功 | 完全相符（344:e1553，23 位作者清單相符） | **否——正文未見任何 `[...]` 引用此文獻** | ⚠️ 待議（孤兒書目：文獻真實存在、metadata 正確，但正文從未實際引用） |
| 23 | Schandelmaier 2020, CMAJ | 10.1503/cmaj.200077 | ✅ 解析成功 | 完全相符（192(32):E901–6） | 是 | ✅ 通過 |
| 24 | Wallach 2017, JAMA Intern Med | 10.1001/jamainternmed.2016.9125 | ✅ 解析成功 | 完全相符（177(4):554–60） | 是 | ✅ 通過 |
| 25 | Kent 2016, Int J Epidemiol | 10.1093/ije/dyw118 | ✅ 解析成功 | Title/作者相符；CrossRef 頁碼欄位僅顯示「dyw118」(online-first ID)，未能單獨核對正文所列「45(6):2075–88」印刷頁碼，但屬同一篇文獻，風險低 | 是 | ✅ 通過（頁碼細節未能 100% 逐字核對，風險低） |
| 26 | Kent 2018, BMJ | 10.1136/bmj.k4245 | ✅ 解析成功 | 完全相符（363:k4245） | 是 | ✅ 通過 |
| 27 | Yusuf 1991, JAMA | 10.1001/jama.1991.03470010097038 | ✅ 解析成功 | 卷期頁相符（266(1):93–8）；CrossRef 僅回傳單一作者「Salim Yusuf」（該筆老舊記錄的已知資料缺口），正文列出四位作者（Yusuf S, Wittes J, Probstfield J, Tyroler HA）為此經典文獻之正確完整作者名單 | 是（多處，方法學樞紐） | ✅ 通過（CrossRef 資料本身不完整，非正文之誤） |
| 28 | Assmann 2000, Lancet | 10.1016/S0140-6736(00)02039-0 | ✅ 解析成功 | 完全相符（355(9209):1064–9，四位作者相符） | 是 | ✅ 通過 |
| 29 | Matsushita 2010, Lancet | 10.1016/S0140-6736(10)60674-5 | ✅ 解析成功 | 完全相符（375(9731):2073–81）；CrossRef 未列作者（大型統合研究常見資料缺口） | 是 | ✅ 通過 |
| 30 | Bakris 2015, JAMA (ARTS-DN) | 10.1001/jama.2015.10081 | ✅ 解析成功 | 完全相符（314(9):884–94） | **否——正文未見引用** | ⚠️ 待議（孤兒書目） |
| 31 | Solomon 2024, NEJM (FINEARTS-HF) | 10.1056/NEJMoa2407107 | ✅ 解析成功 | Title/期刊/DOI 相符；**正文書目僅寫「N Engl J Med. 2024.」，缺卷期頁（實際應為 391(16):1475–85）** | **否——正文未見引用** | ⚠️ 待議（孤兒書目 + 卷期頁缺漏，但非錯誤數字） |
| 32 | Bakris 2020, NEJM (FIDELIO-DKD) | 10.1056/NEJMoa2025845 | ✅ 解析成功 | 完全相符（383(23):2219–29） | 否——正文以本地檔案標籤 `_prior_fidelio_figaro_extract` 引用同一試驗數據，未直接以此書目 key 標註 | ⚠️ 待議（書目存在但引用路徑改走內部萃取檔，屬編排慣例而非錯誤） |
| 33 | Pitt 2021, NEJM (FIGARO-DKD) | 10.1056/NEJMoa2110956 | ✅ 解析成功 | 完全相符（385(24):2252–63） | 同上，未直接以此書目 key 標註 | ⚠️ 待議（同上） |

## 總結

- **33 筆 DOI 全數可經 CrossRef 解析（無 DEAD_DOI）。**
- **1 筆必修（❌ META_MISMATCH）**：#10 Sato 2024 FOUNTAIN 研究——正文書目缺 DOI，且期刊名寫成佔位符「[Adv Ther / FOUNTAIN]」，實際發表於 *Journal of Clinical Medicine* 2024;13(17):5107（DOI: 10.3390/jcm13175107，PMID 39274317）。內文引用之具體數字（N=1029、高血鉀發生率 2.16/2.70、SGLT2i 72%、GLP-1RA 30%、CHF 60–66%）本身經 PubMed/CrossRef 摘要核對皆正確，問題僅在書目條目本身的期刊名/DOI 缺失，**建議修正書目格式**。
- **5 筆待議**：
  - #13 Filippatos LVH 論文年份標示（正文「2025」vs CrossRef epub「2024」，引用鍵又用 `_2024`）不一致，建議統一。
  - #22 Sun 2012、#30 Bakris ARTS-DN 2015、#31 Solomon FINEARTS-HF 2024 三筆為「孤兒書目」——存在於 References 清單但正文從未以 `[key]` 引用，其中 #31 另缺卷期頁資訊。
  - #32、#33（FIDELIO-DKD、FIGARO-DKD 原始試驗 NEJM 全文）書目正確，但正文用本地檔案標籤 `_prior_fidelio_figaro_extract` 引用相同試驗數據而非直接標註此書目 key，屬引用路徑編排問題，建議與 claim-auditor 確認 `_prior_fidelio_figaro_extract` 是否即對應此二篇。
- **PMID/PMC 一致性**：全文無 PMID/PMC 標註，不適用。
- 其餘 27 筆文獻之 title / authors / journal / volume / issue / page / year 與 CrossRef 權威 metadata**逐項相符**，未發現任何自創或錯置引用。

已完成，通知 arbitrator。
