---
tags: [主題, CONFIDENCE, over-additive, 試驗方法學]
created: 2026-07-22
updated: 2026-07-22
sources: [wiki/sources/2026-07-22-03-confidence_trial_deep_dive.md, wiki/sources/2026-07-22-03-confidence_over_additive_and_offtreatment_reversibility.md, wiki/sources/2026-07-22-03-statistical_insights_myths.md, wiki/sources/2026-07-22-03-discussion_controversies_endpoint_hyperkalemia_cost.md, wiki/sources/2026-07-22-05-uacr_rebound_reversibility_mechanism.md, wiki/sources/2026-07-22-00-KDIGO_2026_Diabetes_CKD_draft.md]
---

# CONFIDENCE 與 over-additive 效應

> 回答 purpose.md 關鍵問題三的後半段：CONFIDENCE 的 over-additive 效應該怎麼解讀，停藥後還剩多少？

## 為什麼重要

CONFIDENCE 是第一個隨機化直接檢驗「同步起始」的試驗，也是 KDIGO 2026 草案 Practice Point 4.4.2 的唯一依據，所以它的每一個限制都會被指引繼承。它在替代終點上給了乾淨的答案（UACR 降幅幾乎完整相加、不見天花板），卻同時戳破一個流行假說（同步加 SGLT2i 能抵消 finerenone 的高血鉀），並在停藥 30 天後推翻另一個假說（結構性殘餘防護）。而「over-additive」這個詞本身承載了超過設計能提供的意涵——它是三臂平行試驗、不是 2×2 factorial，從來沒有做過超加成的正式交互檢定。這一頁把可說的與不可說的分開。

## 素材匯總

| 素材 | 對本主題的貢獻 | 證據層級 |
|------|----------------|----------|
| [[2026-07-22-03-confidence_trial_deep_dive]] | 設計、族群、終點階層、CONSORT 流向與所有次分析的原始數字 | 尚待驗證（Phase 2、UACR 主終點） |
| [[2026-07-22-03-confidence_over_additive_and_offtreatment_reversibility]] | over-additive 的精確語意、eGFR dip 疊加機制、停藥反彈的假說判決 | 尚待驗證（30 天洗脫窗） |
| [[2026-07-22-03-statistical_insights_myths]] | 拆解「additive vs over-additive vs synergy」三層次與「沉默不是清白」 | 可外推（方法學） |
| [[2026-07-22-03-discussion_controversies_endpoint_hyperkalemia_cost]] | 爭議定位：正反方其實不矛盾，差在比較臂與終點層級 | 尚待驗證 |
| [[2026-07-22-05-uacr_rebound_reversibility_mechanism]] | 用腎絲球內壓解釋 UACR 反彈與 eGFR dip 回復的同源性 | 可外推（機制整合） |
| [[2026-07-22-00-KDIGO_2026_Diabetes_CKD_draft]] | 指引如何引用 CONFIDENCE 並兩度標註其限制 | 已核准（指引草案） |

## 核心觀點

1. **設計「乾淨」在 double-dummy**：NCT05254002，隨機、雙盲、double-dummy、國際多中心、三臂平行、Phase 2，1:1:1 分入 finerenone+empagliflozin／finerenone+安慰劑／empagliflozin+安慰劑，治療 180 天。double-dummy 讓單藥臂也吞下對應安慰劑，是全盲與無偏比較的設計核心。隨機化依 eGFR（<60 vs ≥60）與 UACR（≤850 vs >850 mg/g）分層，訪視 Day 14、30、90、180，停藥後 Day 210 再測一次評估可逆性 📄（來源：[[2026-07-22-03-confidence_trial_deep_dive]]）。

2. **族群與 CONSORT**：2022/7–2024/8，14 國 143 站點，隨機 818 人，FAS 800（combination 269、finerenone 264、empagliflozin 267）。基線 mean eGFR 54.2 ± 17.1、中位 UACR 583（IQR 292–1140）mg/g、HbA1c 7.3 ± 1.2%、血鉀 4.48 ± 0.42 mmol/L；ACEi/ARB 788（98.4%）。關鍵排除包含血鉀 >4.8、T1D、篩選前 8 週內用過 SGLT2i 或鉀結合劑 📄（來源：[[2026-07-22-03-confidence_trial_deep_dive]]）。

3. **主要療效**：combo 較 finerenone 多降 29%（LSMR 0.71；0.61–0.82；P<0.001）、較 empagliflozin 多降 32%（0.68；0.59–0.79；P<0.001）。自基線降幅 combo 約 −52%、finerenone 約 −32%、empagliflozin 約 −29%；自基線 LSMR 為 0.48（0.44–0.54）／0.68（0.61–0.76）／0.71（0.64–0.79）。Day 14 combo UACR 已較基線降 >30%、Day 90 已 >40% 📄（來源：[[2026-07-22-03-confidence_trial_deep_dive]]、[[2026-07-22-03-confidence_over_additive_and_offtreatment_reversibility]]）。

4. **[[over-additive 效應]] 的精確語意**：在 CONFIDENCE 是「≈ 全加成、不見天花板」，即相對於「只加一藥」的增益，作者明言 52% 與「32% + 29% 的 full additive effect 預期」相符。它**不是**統計上超越加成模型的協同（synergy）📄（來源：[[2026-07-22-03-confidence_over_additive_and_offtreatment_reversibility]]）。

5. **不撞天花板有機制根據**：eGFR-mediation 分析顯示把 empagliflozin 加到 finerenone 上急性 eGFR 中介 28%（P=0.07），反過來僅中介 5.2%（P=0.23）；作者結論句是 finerenone 的加成效應「is nonhemodynamic」，可能源自其直接的抗發炎與抗纖維化效應。兩把鑰匙開兩把不同的鎖，所以效應相加而不互相排擠 📄（來源：[[2026-07-22-03-confidence_over_additive_and_offtreatment_reversibility]]）。

6. **[[eGFR dip]] 疊加但安全**：急性 eGFR 變化（基線→Day 14）combination −26.6、finerenone −22.1、empagliflozin −24.8 mL/min/1.73 m²（三組差異 P<0.001）；Day 30「>30% eGFR 下降」combo 17 人（6.3%）vs finerenone 10 人（3.8%）vs empagliflozin 3 人（1.1%）。機轉是 empagliflozin 增加遠端鈉氯輸送、強化 [[管球回饋]]、收縮入球小動脈，finerenone 經 MR 阻斷降低容量／血壓與 [[腎絲球內壓]]——兩者方向相同故 dip 相加。NEJM 主文載 eGFR 在初期下降後穩定，combo 的 AKI 僅 1.9% 📄（來源：[[2026-07-22-03-confidence_over_additive_and_offtreatment_reversibility]]、[[2026-07-22-03-confidence_trial_deep_dive]]）。

7. **誰會 dip 大，恰是最禁得起的人**：決定因子為 baseline eGFR 越高（每高 10 mL/min OR 1.24；1.11–1.39）與 baseline 使用利尿劑（OR 1.96；1.32–2.91）。與 KDIGO 分層一致——combo 的 >30% eGFR 下降反而集中在 low/moderate（12.1%）與 high（8.2%），very high 最少（4.4%），因後者可壓縮的 hyperfiltration 空間小。>30% eGFR 下降是血流動力學可逆現象、非腎損傷，不應觸發停藥 📄（來源：[[2026-07-22-03-confidence_trial_deep_dive]]）。

8. **跨 KDIGO 風險層一致（prespecified）**：781 名有資料者中 11.3% low/moderate、29.6% high、462（59.2%）very high。combo 降幅 low/mod −61.7%、high −60.7%、very high −52.4%，各層皆優於單藥；very high 層 combo vs finerenone LSMR 0.72（0.59–0.89）、vs empagliflozin 0.75（0.61–0.91），各層 P_interaction >.05 📄（來源：[[2026-07-22-03-confidence_trial_deep_dive]]）。

9. **關鍵反直覺：同步起始並未抵消 [[高血鉀]]**：以中央實驗室 K >5.5 定義，combination 與 finerenone 單藥在血鉀平均變化（P=0.91）與高血鉀 odds（P=0.85）均無顯著差異；整體 113 人（14.5%）＝ combination 40/265（15.1%）、finerenone 48/255（18.8%）、empagliflozin 25/259（9.7%）。以 empagliflozin 單藥為參照的 adjusted OR：combination 2.69（1.46–4.96）、finerenone 2.56（1.42–4.59）——幾乎重疊 📄（來源：[[2026-07-22-03-confidence_trial_deep_dive]]、[[2026-07-22-03-discussion_controversies_endpoint_hyperkalemia_cost]]）。

10. **高血鉀的決定因子與時序無關**：基線血鉀每高 1 mmol/L aOR 9.23（5.07–16.81）、eGFR 每低 5 mL/min aOR 1.11（1.03–1.20）。後果輕微：僅 3 名（每臂 1 名）因高血鉀永久停藥。且高血鉀不在 UACR 下降的因果路徑上——percent mediation 僅 0.2%，這同時拿掉「療效靠升鉀」與「同步 SGLT2i 讓 finerenone 更安全」兩個說法 📄（來源：[[2026-07-22-03-confidence_trial_deep_dive]]、[[2026-07-22-03-discussion_controversies_endpoint_hyperkalemia_cost]]）。

11. **停藥 30 天：反彈是主導訊號**：UACR 回升 LSMR combination 1.63（1.49–1.78）、finerenone 1.45（1.32–1.59）、empagliflozin 1.44（1.32–1.58），全部 >1，combo 反彈幅度最大。血鉀、血壓、eGFR 同步回復。「結構性殘餘防護使 UACR 持續維持顯著低於基線」的假說就此 30 天窗而言不成立 📄（來源：[[2026-07-22-03-confidence_over_additive_and_offtreatment_reversibility]]、[[2026-07-22-05-uacr_rebound_reversibility_mechanism]]）。

12. **臨床框架**：CONFIDENCE 的益處是持續用藥才維持的可逆功能效應——像持續按住彈簧，手一放，UACR、血壓、血鉀、eGFR 一起彈回；combo 只是把彈簧一開始按得更低。這正是 disease-modifying 療法不宜輕易停的生理理由（來源：[[2026-07-22-03-confidence_over_additive_and_offtreatment_reversibility]]）。

13. **安全綜覽**：SAE combination 19/268（7.1%）、finerenone 16/264（6.1%）、empagliflozin 17/266（6.4%）；因不良事件永久停藥整體 30 名（3.8%）；symptomatic hypotension 於 low/moderate 與 high 層無人發生、僅 very high 層 2 名 📄（來源：[[2026-07-22-03-confidence_trial_deep_dive]]）。

## 尚有爭議或未解之處

1. **主終點是 UACR，不是硬腎終點**：這是 surrogate-based 的結論，不是硬終點證據。正方論證硬終點 Phase 3 估計需隨機化約 41,000 人，並引 2019 年 41 試驗、29,979 人 patient-level 統合（前 6 個月 ≥30% albuminuria 下降對應長期複合腎終點風險降 27%，HR 0.73；0.67–0.81）；保留方 Wen 統合顯示相較 SGLT2i 單藥，combination 在 mortality（OR 0.73；0.47–1.13）、MACE（0.77；0.55–1.08）、MAKE（0.87；0.58–1.31）均無顯著額外益處。雙方其實不矛盾，引用時務必標明比較臂與終點層級（來源：[[2026-07-22-03-discussion_controversies_endpoint_hyperkalemia_cost]]）。**尚待驗證（surrogate-based）**

2. **「超加成」從未被正式檢定**：統計上的超加成需 2×2 factorial 設計檢定「合併效果 > 兩單藥效果的加總／相乘」；CONFIDENCE 是三臂平行、並非為 super-additivity 的正式 [[交互作用檢定]] 而設計，也沒有報這個 interaction P 值。站得住的說法是「明確優於任一單藥、且跨風險層一致」，不是「協同 synergy」——那個詞的最強證據仍在動物模型（來源：[[2026-07-22-03-statistical_insights_myths]]）。**尚待驗證**

3. **文獻裡的 P_interaction 檢定的是別的東西**：Vaduganathan 測的是「combination 相對益處在 KDIGO 風險層間是否一致」，且該分析明載未做多重比較校正（來源：[[2026-07-22-03-statistical_insights_myths]]）。<!-- confidence: INFERRED -->

4. **「沉默不是清白」**：P=0.91／0.85 講的是「沒偵測到差異」，不是「證明同步聯用不會多出高血鉀」。原文自承三點 power 限制——finerenone 只讓血鉀升約 +0.18 mEq/L（約比 spironolactone 少三分之一），這個較小的鉀波動「may have limited the opportunity to detect a mitigating effect of empagliflozin」，因此「the absence of a demonstrable reduction in hyperkalemia risk should be viewed as hypothesis-generating rather than definitive」。Wen 統合印證：combination vs finerenone 高血鉀 OR 1.09（0.52–2.28、I²=95.1%），CI 寬到兩側都涵蓋 1（來源：[[2026-07-22-03-statistical_insights_myths]]）。**尚待驗證**

5. **床邊翻譯**：同步聯用時血鉀監測節奏照 finerenone 單藥的規格走，不能因為加了 SGLT2i 就鬆手（來源：[[2026-07-22-03-statistical_insights_myths]]）。

6. **時序假說仍是假說**：[[FIVE-STAR]] 次分析中，已慢性使用 SGLT2i 者再加 finerenone 血鉀僅升 0.13 mEq/L，未用者升 0.37 mEq/L（P-interaction 0.02）；機轉推測為 SGLT2i 需時間誘導遠端小管鉀處理適應。但 FIVE-STAR 的 SGLT2i 使用非隨機化、子組樣本小、未校正多重比較，Sinclair 呼籲三臂 sequencing RCT（finerenone-first／同步／SGLT2i-first）（來源：[[2026-07-22-03-discussion_controversies_endpoint_hyperkalemia_cost]]、[[2026-07-22-03-confidence_trial_deep_dive]]）。**尚待驗證（hypothesis-generating）**

7. **三套高血鉀數字不可混用**：NEJM 主文 investigator-reported 為 9.3%／11.4%／3.8%；JACC 中央實驗室為 15.1%／18.8%／9.7%；Cheng editorial 引 15.3% vs 18.6%——定義與分母不同（來源：[[2026-07-22-03-confidence_trial_deep_dive]]）。

8. **generalizability 有明文限制**：試驗「had stringent inclusion and exclusion criteria that may limit the generalizability of findings to broader, more diverse populations, especially those at low risk」，且治療僅 180 天；長期結構性殘餘保護是本試驗答不了的問題（來源：[[2026-07-22-03-discussion_controversies_endpoint_hyperkalemia_cost]]、[[2026-07-22-03-confidence_over_additive_and_offtreatment_reversibility]]）。**尚待驗證**

## 關鍵實體

- [[CONFIDENCE]] — 第一個隨機化直接檢驗同步起始的三臂試驗，也是本頁所有數字的來源
- [[over-additive 效應]] — 語意需精確界定為「≈ 全加成、不見天花板」，非統計協同
- [[Empagliflozin]] — 被隨機化的對照與聯用臂，其急性 eGFR 中介比例 28% 是機轉分工的量化證據
- [[Finerenone]] — 其加成 is nonhemodynamic（中介 5.2%），這是 over-additive 的機制根據
- [[eGFR dip]] — 疊加但可逆，且最深的 dip 出現在基線腎功能最好的人身上
- [[高血鉀]] — 同步起始未抵消，這是本試驗最反直覺的隨機化裁決
- [[UACR 反彈]] — 停藥 30 天的主導訊號，推翻結構性殘餘防護假說
- [[停藥可逆性]] — Day 180→210 的再測設計讓這個問題第一次有前瞻資料
- [[替代終點]] — 主終點的層級，決定整個結論的可外推邊界
- [[交互作用檢定]] — 分辨「跨層一致」與「超加成」的關鍵，本試驗只做了前者
- [[trial sequential analysis]] — 顯示相對 SGLT2i 單藥的證據量尚未跨越 monitoring boundary
- [[FIVE-STAR]] — 時序假說的來源，非隨機化、僅 hypothesis-generating
- [[管球回饋]] — empagliflozin 端 eGFR dip 的機轉，與 finerenone 端方向相同故相加
- [[腎絲球內壓]] — 統一 UACR 下降與 eGFR dip 的單一變因

## 相關頁面

- [[四大支柱與加藥策略]]
- [[PK-PD 解耦與停藥可逆性]]
- [[因果中介分析]]
- [[替代終點方法學]]
