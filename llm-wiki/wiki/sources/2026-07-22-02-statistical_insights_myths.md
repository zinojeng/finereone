---
tags: [素材摘要, 統計方法學, 替代終點, 中介分析, 統計迷思]
created: 2026-07-22
updated: 2026-07-22
sources: []
source_type: 筆記
source_path: raw/notes/02-statistical_insights_myths.md
images: 0
image_paths: []
---

# 統計迷思與深度解讀 · 主題二（surrogate validation 的統計核心）

> 五個 surrogate 統計陷阱的母題都是同一句話：relative ≠ absolute、individual-level ≠ trial-level、R² 高 ≠ 臨床可替代、mediation % ≠ 機轉佔比、slope ≠ slope。

## 基本資訊
- **來源類型**：本地 Markdown 回顧稿（主題二的統計深度解讀專檔，撰寫日期基準 2026-07-11）
- **原文位置**：raw/notes/02-statistical_insights_myths.md
- **消化日期**：2026-07-22

## 核心觀點

1. **母題錨點：相對 vs 絕對。** Coresh 個體層級資料中 UACR 下降 30% 對應 ESKD 的 HR 0.78 是**相對**風險比；換到**絕對**尺度時，只有 baseline ACR >30 mg/g 者才「confer >1% absolute reduction in 10-year ESKD risk」📄。同一個 HR，在低風險族群的絕對意義小得多——後續五個迷思本質都是「哪一個尺度、哪一個層級被偷換了」。

2. **迷思一：把「病人身上 UACR 與腎衰相關」讀成「治療降 UACR 就會保腎」。** 這是把 individual-level 關聯偷換成 trial-level 有效性。個體層級（Coresh 28 世代、693,816 人）回答的是「同一個人 UACR 變化預不預測他的結局」：2 年 ACR 降 30% → ESKD 校正 HR 0.83（0.74–0.94），校正 regression dilution 後 0.78（0.66–0.92）📄。試驗層級（Heerspink 2025, 48 RCT、85,681 人）問的是完全不同的問題——「一個**治療**對 UACR 的效應能否預測該**治療**對硬終點的效應」：每 30% 降幅對應風險降 19%（95% BCI 5–30%），median R²=0.66（0.06–0.98）📄。**監管採信的是後者。** 床邊解讀：UACR 下降是良好的**治療反應標記**，不是「腎臟已保住、可以鬆手」的證明。

3. **迷思二：R²=0.66 就是「六成的病可以用 UACR 替代」。** trial-level R² 描述的是「各試驗的治療效應點被那條 meta-regression 迴歸線解釋的比例」，不是病人層級的替代率或可信度百分比。三個細節：(a) 95% BCI 0.06–0.98 幾乎橫跨「毫無替代力」到「近乎完美」，作者直言「The wide BCIs decrease our certainty about the strength of the association」，並拆出**只有 45.2% 機率**達 strong（R²>0.72）、還有 **28.0% 機率**落在 low（R²<0.49）📄；(b) R² 會隨資料集移動——Heerspink 2019（41 comparisons、29,979 人）median R² 僅 0.47（0.02–0.96），限 baseline ACR >30 mg/g 才升到 0.72（0.05–0.99）📄；(c) R² 依藥物機轉而異：RAASi/ETA 82%、SGLT2i 45%、免疫抑制劑 41% 📄。**R² 不是 biomarker 的固有屬性，是「biomarker × 藥物類別 × 族群」的聯合屬性。**

4. **Matyjek 的非對稱判讀是最實用的一條。** 陰性預測很強（「absence of UACR reduction is associated with a very low probability of subsequent clinical benefit」），但正向的 UACR 反應「do not replace long-term outcome follow-up and eGFR monitoring」📄。所以：**UACR 沒降，幾乎可以放棄期待；UACR 降了，仍要繼續盯 eGFR。**

5. **迷思三：「finerenone 84% 的腎益處來自降 UACR」。** Agarwal 2023 以「基線→月 4 log UACR 變化」為 mediator：連續變項 mediated kidney 84%、CV 37%；改用 ≥30% 二元門檻則掉到 64% 與 26% 📌。這個百分比至少四重不穩定：(a) 連續 vs 二元就差一大截，同一真實機轉不會因 mediator 切法改變——會變的是**估計**；(b) 測量誤差會**低估**中介比例（UACR 測量變異極大，Coresh 全篇在處理 regression dilution）；(c) mediator→outcome 那一段是**觀察性**的，Agarwal 2026 自算 joint UACR+SBP 的 natural indirect effect E-value 僅 **1.29（confidence limit 1.19）**——一個中等強度的未測混淆就可能把中介效應解釋掉 📄；(d) 作者自陳「The current findings are not readily extendable to other drugs.」📌。

6. **迷思四：eGFR slope 已驗過，所以「用哪種 slope 都一樣硬」。** 同樣叫 slope，trial-level R² 差近一倍：total slope（基線→3 年，含 acute dip）R²=0.97（Inker 2023, 66 studies/186,312 人，95% BCI 0.82–1.00；Inker 2019, 47 RCT/60,620 人亦為 0.97, 0.78–1.00）📄；chronic slope（3 個月後、剔除 acute dip）**僅 R²=0.55（0.25–0.77）**，被歸類為 moderate 📄。

7. **剔掉 acute dip 反而變差，因為 acute dip 本身帶資訊。** Greene 2025（66 comparisons）多變量 Bayesian meta-regression：acute 與 chronic 各自獨立預測硬終點（joint R²=0.95, 0.79–1.00）；固定 chronic slope 下，每多 1 ml/min/1.73 m²/3 個月的急性下降，硬終點 HR 上升 **11.4%（7.9–15.0%）**；acute 對 chronic 的**最佳權重比 0.078（0.055–0.105）**恰與「3 個月/33 個月=0.09」的 3-year total slope 定義吻合 📄。Levey 的 NKF-FDA-EMA workshop 亦定調用 slope 當終點時「必須排除藥物急性效應的干擾」📄。臨床兩層意義：對會製造 acute dip 的藥（finerenone/RASi），**chronic slope 會高估真實持續益處**（把不利的初期成分剪掉了），total slope 才誠實；讀擴張試驗時先問「它用的是 total 還是 chronic」。

8. **迷思五：「4 個月的 UACR 中介了後續事件」——時序其實對不上。** Agarwal 2026 明載 CV 益處「emerges within months, before measurable kidney protection」，而腎保護「requires approximately 18 months to become statistically apparent」📄。若腎保護是 CV 益處的中介路徑，時序就不對。同一模型中月 4 finerenone 降 UACR 32.2%、降 SBP 3.6 mmHg、降體重 0.23 kg、升血鉀 0.19 mEq/L，但只有 UACR（39%, 7–71）與 SBP（21%, 3–40）顯著，體重與血鉀**不**中介，合計 50%（21–100）📄。另 proportion-mediated 在 treatment 與 mediator 效應方向相反時「uninformative」📄。心衰場景更極端：Mc 2025（FINEARTS-HF，基線 median UACR 僅 17 mg/g）連續分析 mediated composite 34%（95% CI 16–132）、首次 HF 事件 29%（14–82），二元化 >30% 只剩 15% 與 11% 📌——**CI 上界 132% 直接提醒別把 point estimate 當真值。**

9. **床邊心智模型要升級成「兩條路、兩個時鐘」。** CV 益處走得快（數月、部分經 SBP 與血流動力學），腎益處走得慢（約 18 個月、高度經白蛋白尿路徑）。這解釋了為何起始 finerenone 後短期先看到血壓與 UACR 反應，腎功能曲線的分岔要更久才顯著——不能因為前幾個月 eGFR 沒好轉（甚至有 acute dip）就判定無效。

10. **原文附一份「統計素養檢查表」（查房／簡報用一頁，八題）**：是 individual-level 還是 trial-level？R² 的 credible interval 多寬？這個 surrogate 對這一類藥成立嗎？mediation % 用連續還是二元 mediator？mediator–outcome 段有無殘餘混淆（看 E-value）？用 total 還是 chronic slope？acute dip 被剪掉了嗎？相對還是絕對、基線風險多高？每題都附錨定數字。

## 關鍵概念

- [[trial-level R²]]
- [[中介分析]]
- [[UACR]]
- [[eGFR slope]]
- [[eGFR dip]]
- [[E-value]]
- [[替代終點]]
- [[相對風險與絕對風險]]

## 與其他素材的關聯

- 本檔是主題二主文 `02-02_albuminuria_to_hard_endpoints.md` 的統計配套檔，由主文 §0 的方框明確指向；主文負責證據鏈敘事，本檔負責把散落的 R²、mediation %、trial-level 關聯抽出來重新組織成「臨床醫師最容易踩的陷阱」。<!-- confidence: EXTRACTED -->
- 與 `02-uacr_sbp_mediation_of_cv_benefit.md` 刻意分工：該檔明言「不重述 surrogate 驗證的方法學（trial-level R²、個體 vs 試驗層級、連續 vs 二元的統計陷阱），那些見本檔迷思一至五」；本檔迷思三／五則反向指向該檔的中介比例細節。<!-- confidence: EXTRACTED -->
- 迷思四（total vs chronic slope、acute dip 帶資訊）是主題五 `egfr_dip_hemodynamic_reversible.md` 的統計基礎。<!-- confidence: INFERRED -->
- 本檔把 `r2_Heerspink_2025` 標為 📄 本地全文，而 `02-endpoint_evolution_hard_to_surrogate.md` 經仲裁後標為 📌 abstract-only。<!-- confidence: AMBIGUOUS -->

## 原文精彩摘錄

> 「床邊看到病人 UACR 下降，正確的解讀是『這是一個**良好的治療反應標記**』，而不是『腎臟保護已經兌現、可以鬆手』。個體關聯強（HR 0.78）給你『值得繼續』的信心；但唯有 trial-level R² 才是『這個 biomarker 能代替硬終點』的執照。」

> 「用一個比喻：chronic slope 像『只看下半場比分』，acute dip 像『上半場的一次戰術性換血』——把上半場整段剪掉，反而看不懂整場走勢。」

> 「一句話帶走：**relative ≠ absolute、individual-level ≠ trial-level、R² 高 ≠ 臨床可替代、mediation % ≠ 機轉佔比、slope ≠ slope。**」

## 相關頁面

- [[trial-level R²]]
- [[中介分析]]
- [[替代終點]]
- [[eGFR slope]]
- [[eGFR dip]]
