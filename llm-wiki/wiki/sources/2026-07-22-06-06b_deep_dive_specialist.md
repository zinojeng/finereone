---
tags: [素材摘要, finerenone, 臨床試驗方法學, 替代終點, 跨藥類對讀]
created: 2026-07-22
updated: 2026-07-22
sources: []
source_type: 筆記
source_path: raw/notes/06-06b_deep_dive_specialist.md
images: 0
image_paths: []
---

# 主題六 companion：專科醫師版深度解析——六篇關鍵 finerenone 試驗的單篇深挖與跨藥類對讀

> 用「acute dip vs chronic slope」這一條方法學主線，把 FINE-ONE 的替代終點註冊、FIND-CKD 的 slope 設計、FINEARTS-HF 那個 HR 1.33 的反向訊號與兩個「三試驗合池」的詮釋限制，串成一套可教學的臨床試驗解讀。

## 基本資訊
- **來源類型**：本地 Markdown 回顧稿（主文 06-06 的 companion）
- **原文位置**：raw/notes/06-06b_deep_dive_specialist.md
- **消化日期**：2026-07-22

## 核心觀點

1. **卡 A｜[[FINE-ONE]] 的監理創新**。N=242，6 個月 UACR 相對變化為 primary；UACR 降 34%（GMR 0.66，0.60–0.73）vs placebo 12%（GMR 0.88，0.79–0.98），安慰劑校正多降 25%（GMR 0.75，0.65–0.87，P<0.001）；高血鉀 10.1% vs 3.3%，因高血鉀停藥 1.7% vs 0；6 個月 eGFR −5.6 vs −2.7（差 −2.9，−5.1 至 −0.7），washout 後回基線 📌。**本卡數字均來自 abstract／結構式摘要（NEJM 全文付費牆），不作全文級斷言**——與主文對同批數字標 📄 的取得層級不同。<!-- confidence: AMBIGUOUS -->

2. **[[Lewis 1993 captopril 試驗]] 對讀凸顯世代差異**。captopril 試驗 N=409（captopril 207／placebo 202），IDDM+糖尿病腎病、蛋白尿 ≥500 mg/d、Cr ≤2.5，**硬終點**為血清肌酸酐加倍：25 vs 43 例（P=0.007），風險降 48%，死亡／透析／移植複合降 50% 📌。原文判讀：FINE-ONE 在同族群只用 6 個月、UACR 替代終點、N=242 完成註冊路徑，**不是試驗品質退步，而是 surrogate endpoint 三十年成熟的結果**；且 finerenone 定位為 RASi 基石**之上的加藥**，非取代 ACEi。

3. **卡 B｜[[FIND-CKD]] 為何選 total eGFR slope**。因在高 eGFR、慢進展的非糖尿病 CKD，ESKD 事件太稀少。[[Inker 2019]]（47 RCT／60,620 人）顯示 total slope 對硬終點 R²=0.97，且 **≥0.75 mL/min/yr 的 slope 效應以 ≥96% 機率預測臨床獲益** 📄——FIND-CKD 觀察到的 0.7 差值恰在此門檻附近，是「剛好夠格」的替代終點證據。基線 mean eGFR 46.7；病因學慢性腎絲球腎炎 57.0%（IgAN 26.3%、FSGS 13.6%）、高血壓／缺血性腎病 29.0% 📄。

4. **兩段式 spline 與 ≥57% 門檻是同一防禦動作**。[[Greene 2019]] 模擬明言：**有急性效應的藥，total slope 可能造成偽結論**，必須分段解讀 📄；FIND-CKD 以 month 3 為 change point 防這一手，並改用 ≥57% eGFR 下降（而非 FIDELIO 的 ≥40%）定義複合腎終點，目的是讓急性血流動力學下降不被誤計為疾病進展 📄。基線→month 3 finerenone 比 placebo 相差 1.2 mL/min/1.73m²，month 3 之後慢性下降較緩，停藥後 eGFR 回升 📄。

5. **卡 B/C 的跨藥類效應量落差**。[[DAPA-CKD]] 非糖尿病亞群主要複合 **HR 0.50（0.35–0.72）**、腎絲球腎炎 0.43（0.26–0.71）📄；[[EMPA-KIDNEY]]／Herrington IPD meta 慢性 eGFR 下降減緩 **64%**、kidney failure HR 0.66（0.55–0.79）📌；finerenone 的 FIND-CKD 走 slope 路線（差 0.7、複合 HR 0.77）較溫和。原文歸因為**終點哲學不同**（事件驅動 vs slope 驅動）而非藥效優劣，並指出兩者機轉互補、FIND-CKD 設計即把 SGLT2i 使用列為分層因子（17% 已在 SGLT2i）📄。

6. **卡 C｜IgAN 的三藥對讀，比較效應量務必辨明分母**。FIND-CKD glomerular 亞群 UACR −42%（12mo）、KF/≥40% HR 0.74（0.57–0.97）📌；[[PROTECT]]（sparsentan）慢性 slope −2.7 vs −3.8（差 1.1，p=0.037）、UPCR −42.8% vs −4.4%（GLSM 0.60）、複合腎衰 RR 0.7（0.4–1.2）📌；DAPA-CKD IgAN 亞群 −3.5 vs −4.7、UACR −26%、主要複合 4% vs 15%，**HR 0.29（0.12–0.73）但事件僅 6 vs 20、CI 寬** 📌。關鍵警告：PROTECT 用 **active comparator（irbesartan）**，其 −42.8% 是相對於已最大化 ARB 的額外降幅；finerenone／dapagliflozin 則是相對 placebo（於 RASi 之上）。

7. **白蛋白尿在 IgAN 特別站得住腳**。[[Heerspink 2019]] 顯示替代性在**基線白蛋白尿高**時最強（基線 >30 mg/g 時 R² 0.72）📄；IgAN 族群基線 UACR ~840 mg/g，正落在替代終點最可信的區間。

8. **卡 D｜HR 1.33 反向訊號的三因子拆解（本 companion 最核心的教學點）**。[[FINEARTS-HF]] 腎族群基線 mean eGFR 62±20、**median UACR 僅 18（7–67）mg/g**；複合腎終點 75 vs 55 事件、HR 1.33（0.94–1.89），≥57% 版本 41 vs 31、HR 1.28（0.80–2.05）📄。拆解為：(a) acute dip −2.9（−3.4 至 −2.4）被計入複合腎終點；(b) 低白蛋白尿、低事件背景使短期 dip 被過度計數；(c) total-based 終點框架。**反證**：chronic slope +0.2（−0.1 至 +0.4）無差異、UACR 6 個月降 30%（25–34%）、新發 macroalbuminuria HR 0.62（0.53–0.73）／microalbuminuria HR 0.76（0.68–0.83）📄。結論是統計假象而非傷腎。

9. **卡 D｜[[TOPCAT]] 的區域異質是「類固醇型 MRA 在 HFpEF equivocal」的關鍵解釋**。Pfeffer 2015 區域分析顯示俄／喬 vs 美洲事件率差約 4 倍，spironolactone 僅在美洲（n=1767）顯著，俄／喬（n=1678）無效且**無鉀／肌酐反應**（暗示未實際服藥）📌。TOPCAT 主試驗（Pitt 2014）與 EMPEROR-Preserved（Anker 2021）**本地僅 metadata，標 ❌、完全不引數字**，僅作定性背景。FINEARTS-HF 主試驗主要複合 RR 0.84（0.74–0.95，P=0.007）、worsening HF RR 0.82、CV 死亡 8.1% vs 8.7%（HR 0.93，0.78–1.11）📌；[[DELIVER]] HR 0.82（0.73–0.92，P<0.001）、CV 死亡 0.88（0.74–1.05）📌。

10. **卡 E｜[[FINE-HEART]] 為何把信心放在全因死亡**。N=18,991、中位追蹤 2.9 年；primary CV 死亡 4.4% vs 5.0%，HR 0.89（0.78–1.01），**P=0.076 未達顯著**；納入 undetermined death 之敏感度分析 6.6% vs 7.4%，HR 0.88（0.79–0.98），**P=0.025**；全因死亡 HR 0.91（0.84–0.99，P=0.027）📄。原文邏輯：當死因裁定的分類邊界能翻轉統計結論，**競爭風險較少、分類爭議較小的全因死亡反而更 robust**；「主要終點失手不等於無效」。合池限制：三試驗族群／終點定義不同（urgent HF visit 只在 FINEARTS 收集），腎益處幾乎全由 FIDELIO/FIGARO 驅動，未校正多重比較 📄。

11. **卡 F｜[[INFINITY]] 是 finerenone 版的「SGLT2i 大合池」對應物**。N=14,574（FIDELIO+FIGARO+FIND-CKD），PROSPERO CRD420251269149；腎複合 HR 0.76（0.68–0.86）降 24%、kidney failure alone 0.85（0.74–0.99）、CV 複合 0.80（0.70–0.91）、HHF 0.78（0.66–0.92）、**CV 死亡 0.82（0.67–0.999）擦邊顯著**、全因死亡 0.88（0.79–0.99）📌。與 SGLT2i 的 Herrington 2025（23,340 人 IPD meta）殊途同歸地把各自藥類定位為跨病因 foundational therapy，且都強調效果不隨 SGLT2i 背景使用而異，為合併使用（CONFIDENCE 型設計）鋪路。

12. **兩個「三試驗合池」不可混為一談**。INFINITY 是**純 CKD**三試驗（含非糖尿病 FIND-CKD）、以腎終點為主軸；FINE-HEART 是**含 HF 的 CKM**三試驗（含 FINEARTS）、以 CV 死亡為主軸；兩者共用 FIDELIO/FIGARO 但問的問題不同。另：**一致性 ≠ 同質效應量**——HTE 檢定「不顯著」只代表未偵測到交互作用，受各次族群 power 限制。

## 關鍵概念

[[Finerenone]]、[[eGFR dip]]、[[eGFR slope]]、[[eGFR slope]]、[[橋接生物標記]]、[[替代終點]]、[[治療效應異質性]]、[[FINE-ONE]]、[[FIND-CKD]]、[[FINEARTS-HF]]、[[FINE-HEART]]、[[INFINITY]]、[[TOPCAT]]、[[PROTECT]]、[[DAPA-CKD]]、[[Inker 2019]]、[[Greene 2019]]、[[Heerspink 2019]]

## 與其他素材的關聯

- 本文為 [[2026-07-22-06-06_beyond_t2d_cardiorenal_landscape]] 的 companion，不重述主文架構而做單篇深挖；主文的「證據階梯表」對應本文的「六張卡」。
- **取得層級標記存在版本差異**：主文對 FINE-ONE 系列、glomerular 亞群、INFINITY 標 📄（部分為版本記錄全文），companion 對同批數字標 📌 並明言僅 abstract 級。引用時應採較保守的 📌。<!-- confidence: AMBIGUOUS -->
- 與主題二（替代終點方法學）高度重疊：Inker 2019／Greene 2019／Heerspink 2019 三篇是本文與主題二共用的方法學靠山。<!-- confidence: INFERRED -->
- 與主題五（安全工程）相連：acute dip 的可逆性判讀直接決定「eGFR 下降要不要停藥」的門診決策。<!-- confidence: INFERRED -->

## 原文精彩摘錄

> Lewis 1993 用「三年、硬終點」證明 ACEi；FINE-ONE 在同一族群卻只用「6 個月、UACR 替代終點、N=242」就完成註冊路徑——這不是試驗品質退步，而是 **surrogate endpoint 30 年成熟的結果**。

> **結論**：HR 1.33 是 acute dip × 低事件背景 × total-based 終點三者交互的產物；chronic slope 無害 + 白蛋白尿改善，共同排除真實腎損傷。這是「同一數字在不同終點框架下講出相反故事」的經典教材。

> 當死因裁定的分類邊界會翻轉統計結論時，**competing-risk 較少、分類爭議較小的全因死亡反而更 robust**——這是作者明文選擇 all-cause death 作為可信訊號的邏輯。

## 相關頁面

- [[2026-07-22-06-06_beyond_t2d_cardiorenal_landscape]]
