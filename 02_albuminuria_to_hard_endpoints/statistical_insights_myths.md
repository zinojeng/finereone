# 統計迷思與深度解讀 · 主題二（surrogate validation 的統計核心）

> 本檔為主題 02〈從白蛋白尿到硬終點〉的**統計深度解讀**，把主文散落的 R²、mediation %、trial-level 關聯抽出來，用「臨床醫師最容易踩的統計陷阱」重新組織。全題庫中本主題的統計密度最高——因為 finerenone 的適應症擴張正在從「數事件」轉向「看 biomarker 軌跡」，讀懂 surrogate validation 的統計就是讀懂未來十年的證據等級。
>
> **引用標記慣例**：📄 = 本地全文可 grep 稽核；📌 = 僅取得 abstract（不對其未載內容作具體斷言，數字維持原樣不擴張）。每個數字句末以 `[本地MD檔名]` 標註來源供 grep 回溯。**LLM 只做組織、改寫與統計詮釋；詮釋可以延伸，數字一律 grep 回本地全文，不杜撰。**
>
> **證據分層**：🟢 已確立的統計／監管共識｜🟡 post hoc／mediation／模型推估｜🔴 abstract-only 或方法學上仍不穩定的估計。
>
> **經典錨點——相對 vs 絕對**：所有 surrogate 迷思的母題，都是「相對 vs 絕對」這條老陷阱的變形。臨床醫師習慣把「相對關聯」直接讀成「絕對可替代」。例如 Coresh 個體層級資料裡，UACR 下降 30% 對應 ESKD 的 HR 是 0.78——這是**相對**風險比；但它換算到**絕對**尺度時，在 baseline ACR >30 mg/g 者才「confer >1% absolute reduction in 10-year ESKD risk」[egfr_slope_surrogate_Coresh_2019] 📄。同一個 HR，低風險族群的絕對意義小得多。下面五個迷思，本質上都是「哪一個尺度、哪一個層級」被偷換了。

---

## 迷思一：「病人身上 UACR 與腎衰相關」＝「治療降 UACR 就會保腎」

這是 surrogate validation **最核心、最致命**的混淆——把 individual-level 關聯偷換成 trial-level 有效性。

**❌ 常見誤解**
門診看到「這個病人 UACR 降了 30%，文獻說 UACR 降相關腎衰風險降」，就直接推論「所以這個藥有效、可以停止追硬終點」。把「病人身上的預後關聯」當成「治療效應的替代」。

**✅ 統計正解**
這是兩個完全不同的層級，證據也來自不同研究：
- **個體層級（observational）**：Coresh 的 28 個世代、693,816 人分析，2 年內 ACR 下降 30% 對應後續 ESKD 的校正 HR 0.83（95% CI 0.74–0.94），校正 regression dilution 後 0.78（0.66–0.92）[egfr_slope_surrogate_Coresh_2019] 📄。這回答的是「**同一個人** UACR 變化預不預測他的結局」。
- **試驗層級（trial-level R²）**：Heerspink 2025 的 48 個 RCT、85,681 人分析，問的是完全不同的問題——「一個**治療**對 UACR 的效應，能不能預測這個**治療**對硬終點的效應」，答案是每 30% UACR 降幅對應 clinical endpoint 風險平均降 19%（95% BCI 5–30%），median R²=0.66（0.06–0.98）[r2_Heerspink_2025] 📄。
- 監管採信的是**後者**。Coresh 自己在文中就把兩者分開：「clinical trials compare groups of individuals and how average albuminuria reduction is related to risk」——個體關聯只是 surrogacy criteria 的**其中一條**，不能單獨定案 [egfr_slope_surrogate_Coresh_2019] 📄。

**💡 臨床亮點**
床邊看到病人 UACR 下降，正確的解讀是「這是一個**良好的治療反應標記**（response marker）」，而不是「腎臟保護已經兌現、可以鬆手」。個體關聯強（HR 0.78）給你「值得繼續」的信心；但唯有 trial-level R² 才是「這個 biomarker 能代替硬終點」的執照——而那張執照（下一則）其實遠沒有想像中乾淨。

---

## 迷思二：R²=0.66 就是「六成的病可以用 UACR 替代」

**❌ 常見誤解**
把 trial-level R² 讀成「這個 surrogate 有 66% 的準確度／可信度」，或「六成病人可以只看 UACR」。R² 一高就當它是「臨床可替代性」的分數。

**✅ 統計正解**
Trial-level R² 是「**各試驗的治療效應點，被那條 meta-regression 迴歸線解釋的比例**」——它描述的是「跨試驗的治療效應點散得多齊」，不是「病人層級的替代率」，更不是「可信度百分比」。三個關鍵細節：
- **UACR 的 R²=0.66（95% BCI 0.06–0.98）**[r2_Heerspink_2025] 📄。這個 credible interval 從 0.06 一路開到 0.98——幾乎橫跨「毫無替代力」到「近乎完美」。作者直言「The wide BCIs decrease our certainty about the strength of the association」，並拆解出**只有 45.2% 機率**達到「strong surrogate（R²>0.72）」，還有 28.0% 機率落在 low（R²<0.49）[r2_Heerspink_2025] 📄。
- **R² 會隨資料集移動**：更早的 Heerspink 2019（41 comparisons、29,979 人）median R² 只有 0.47（0.02–0.96），限制在 baseline ACR >30 mg/g 才升到 0.72（0.05–0.99）[editorial_endpoints_Heerspink_2019] 📄。同一個 biomarker，換個資料集、換個族群，R² 就從 0.47 跳到 0.72。
- **R² 依藥物機轉而異**：RAASi/ETA 這類走白蛋白尿路徑的藥，UACR 可解釋 82%；SGLT2i 僅 45%、免疫抑制劑僅 41% [editorial_endpoints_Matyjek_2026] 📄。R² 不是「這個 biomarker」的固有屬性，是「這個 biomarker × 這類藥 × 這種族群」的聯合屬性。

**💡 臨床亮點**
把「R²=0.66」翻譯成床邊語言：不是「六成準」，而是「**在白蛋白尿族群、對走白蛋白尿路徑的藥，UACR 是個合理但不確定的替代終點**」。Matyjek 給出最實用的非對稱判讀——**陰性預測**很強（「absence of UACR reduction is associated with a very low probability of subsequent clinical benefit」），但正向的 UACR 反應「do not replace long-term outcome follow-up and eGFR monitoring」[editorial_endpoints_Matyjek_2026] 📄。所以：UACR 沒降，幾乎可以放棄期待；UACR 降了，仍要繼續盯 eGFR。

---

## 迷思三：「finerenone 84% 的腎益處來自降 UACR」

這是 mediation % 被最常過度解讀的一句話——把統計歸因讀成機轉佔比。

**❌ 常見誤解**
「UACR mediated 84% of the kidney effect」→「finerenone 護腎主要（84%）就是靠降蛋白尿」→「只要把 UACR 壓下去，腎臟就保住了」。把一個 post hoc 的 mediation 百分比當成穩定的機轉分解。

**✅ 統計正解**
Agarwal 2023 對 FIDELIO+FIGARO 的 mediation：以「基線→第 4 個月 log UACR 變化」為 mediator，UACR（連續變項）mediated kidney 效應的 **84%**、CV 效應的 **37%**；改用「是否達 ≥30% 門檻」的**二元變項**，則掉到 **64%** 與 **26%** [albuminuria_mediation_Agarwal_2023] 📌。這個百分比至少有四重不穩定：
1. **連續 vs 二元就差一大截**：同一份資料，kidney 從 84% 掉到 64%、CV 從 37% 掉到 26% [albuminuria_mediation_Agarwal_2023] 📌。同一個真實機轉不會因為你把 mediator 切成連續或門檻就改變——會變的是**估計**，這本身就說明 point estimate 不該被當精確值讀。
2. **測量誤差會衰減中介比例**：mediator（UACR）本身測量變異極大（Coresh 全篇都在處理 regression dilution [egfr_slope_surrogate_Coresh_2019] 📄）；mediator 測得越不準，估到的中介比例通常被**低估**。Agarwal 2026 因此必須專門跑 measurement-error 敏感度分析（見迷思五）。
3. **mediator–outcome 殘餘混淆**：mediation 的「效應→mediator→結局」路徑，其 mediator 到 outcome 那一段是**觀察性**的。Agarwal 2026 自算 E-value：joint UACR+SBP 的 natural indirect effect E-value 僅 1.29（confidence limit 1.19）[albuminuria_mediation_Agarwal_2026] 📄——意思是只要有一個中等強度的未測混淆因子，這個中介效應就可能被解釋掉。
4. **作者自陳不可外推**：Agarwal 2023 的 Limitation 白紙黑字——「The current findings are not readily extendable to other drugs.」[albuminuria_mediation_Agarwal_2023] 📌。finerenone 的 84% 不代表任何降 UACR 的藥都有等量腎保護，這與 Matyjek 的 82% vs 45% vs 41% 藥物類別差異完全呼應 [editorial_endpoints_Matyjek_2026] 📄。

**💡 臨床亮點**
把「84%」讀成「UACR 是 finerenone 效應鏈上一個**重要中繼站**」，而不是「機轉的 84% 配額」。實務三條線：(1) UACR 是很好的**腎臟端**反應指標（中介比例高），但 CV 端只捕捉到約四分之一到三分之一——**UACR 沒大降的病人不等於 CV 沒獲益**；(2) 不要把 finerenone 的 mediation 數字外推到別的藥；(3) mediation 是統計歸因，不是機轉證明，抗發炎／抗纖維化的直接效應這些 biomarker 根本沒測到。

---

## 迷思四：eGFR slope 是驗過的 surrogate，所以「用哪種 slope 都一樣硬」

**❌ 常見誤解**
「FDA/EMA 已接受 eGFR slope 當 primary endpoint」→ 把所有 slope 版本一視同仁，看到「slope 改善」就當它等價於硬終點益處。忽略 total slope 與 chronic slope 是兩個強度天差地遠的 surrogate。

**✅ 統計正解**
同樣叫「eGFR slope」，trial-level R² 差了將近一倍：
- **Total slope（基線→3 年，含 acute dip）**：Inker 2023（66 studies、186,312 人）R²=0.97（95% BCI 0.82–1.00）[egfr_slope_surrogate_Inker_2023] 📄；Inker 2019（47 RCT、60,620 人）亦為 0.97（0.78–1.00）[egfr_slope_surrogate_Inker_2019] 📄。
- **Chronic slope（3 個月後，剔除 acute dip）**：同一份 Inker 2023 只有 **R²=0.55（95% BCI 0.25–0.77）**——被歸類為僅「moderate」[egfr_slope_surrogate_Inker_2023] 📄。
- **為什麼剔掉 acute dip 反而變差？** 因為 acute dip 本身帶資訊。Greene 2025（66 comparisons）用多變量 Bayesian meta-regression 一次拆解 acute 與 chronic：兩者**各自獨立**預測硬終點（joint R²=0.95，0.79–1.00）；固定 chronic slope 下，每多 1 ml/min/1.73 m²/3 個月的急性下降，硬終點 HR 上升 **11.4%（7.9–15.0%）**[egfr_slope_surrogate_Greene_2025] 📄。
- **監管採信 total slope 的統計根據**：Greene 算出 acute 對 chronic 的**最佳權重比 0.078（0.055–0.105）**，恰與「3 個月 / 33 個月 = 0.09」的 3-year total slope 定義吻合 [egfr_slope_surrogate_Greene_2025] 📄。也就是說，total slope 不是隨手取的平均，而是「以接近最佳權重同時納入 acute 與 chronic」的那個 slope；Levey 的 NKF-FDA-EMA workshop 也定調：用 slope 當終點時「必須排除藥物急性效應的干擾」[egfr_slope_surrogate_Levey_2020] 📄。

**💡 臨床亮點**
用一個比喻：chronic slope 像「只看下半場比分」，acute dip 像「上半場的一次戰術性換血」——把上半場整段剪掉，反而看不懂整場走勢。臨床上有兩層意義：(1) 對 finerenone/RASi 這種**會製造 acute dip** 的藥，chronic slope 會**高估**真實持續益處（把不利的初期成分剪掉了），total slope 才誠實；(2) 讀一篇用 slope 當 primary 的擴張試驗時，先問「它用的是 total 還是 chronic」——R² 0.97 與 0.55 是兩個完全不同等級的證據，不能混為一談。

---

## 迷思五：「4 個月的 UACR 中介了後續事件」——時序其實對不上

**❌ 常見誤解**
把 mediation 的因果箭頭想當然爾地讀成「早期 UACR 下降 → 造成 → 後續所有益處」，並假設 CV 益處與腎益處走同一條、同一個時間軸的路。

**✅ 統計正解**
Finerenone 的 CV 益處與腎益處**時序錯開**，這對「4 個月 mediator → 後續事件」的框架是個弔詭：
- Agarwal 2026 明載：CV 益處「emerges within months, before measurable kidney protection」，而腎保護「requires approximately 18 months to become statistically apparent」[albuminuria_mediation_Agarwal_2026] 📄。CV 益處早於**可測得**的腎保護出現——若腎保護是 CV 益處的中介路徑，時序就不對。
- 這正是為何單看 UACR 只 mediated CV 益處的一小塊。Agarwal 2026 的多 mediator 模型：第 4 個月 finerenone 降 UACR 32.2%、降 SBP 3.6 mmHg、降體重 0.23 kg、升血鉀 0.19 mEq/L；但只有 **UACR（mediated 39%，95% CI 7–71）與 SBP（21%，3–40）**顯著，體重與血鉀**不**中介；UACR+SBP 合計 mediated CV 益處的 **50%（95% CI 21–100）**[albuminuria_mediation_Agarwal_2026] 📄。上界頂到 100、下界到 21，本身就說明估計的不確定。
- mediation 的「比例」在某些次群甚至**失去意義**：Agarwal 2026 指出當 treatment 與 mediator 效應方向相反時，proportion-mediated 這個指標「uninformative」[albuminuria_mediation_Agarwal_2026] 📄。
- 心衰場景更極端：Mc 2025（FINEARTS-HF，基線 median UACR 僅 17 mg/g）中，UACR 變化連續分析 mediated composite 的 34%（95% CI 16–132）、首次 HF 事件 29%（14–82）；二元化 >30% 則只剩 15% 與 11% [albuminuria_mediation_Mc_2025] 📌。CI 上界 132% 這種數字，直接提醒「別把 point estimate 當真值」。

**💡 臨床亮點**
床邊心智模型要從「單一路徑、單一時鐘」升級成「**至少兩條路、兩個時鐘**」：CV 益處走得快（數月、部分經 SBP 與血流動力學），腎益處走得慢（約 18 個月、高度經白蛋白尿路徑）。實務上這解釋了為什麼——起始 finerenone 後短期內先看到的可能是血壓與 UACR 反應，而腎功能曲線的「分岔」要更久才顯著；不能因為前幾個月 eGFR 沒有明顯好轉（甚至有 acute dip）就判定無效。**「4 個月 mediator」是個方便的觀測窗，不是完整的因果時序。**

---

## 統計素養檢查表（查房／簡報用一頁）

讀任何一個 surrogate 數字前，先過這八題：

| # | 問題 | 為什麼要問 | 錨定數字 |
|---|---|---|---|
| 1 | 這是 **individual-level** 關聯還是 **trial-level** 有效性？ | 前者是預後、後者才是替代執照 | Coresh HR 0.78 vs Heerspink R²=0.66 [egfr_slope_surrogate_Coresh_2019]／[r2_Heerspink_2025] |
| 2 | R² 的 **credible interval** 有多寬？ | 寬 CI＝高不確定，別只讀 point estimate | UACR R²=0.66（0.06–0.98）[r2_Heerspink_2025] |
| 3 | 這個 surrogate 對**這一類藥**成立嗎？ | R² 依機轉而異 | RAASi 82% vs SGLT2i 45% [editorial_endpoints_Matyjek_2026] |
| 4 | mediation % 是**連續**還是**二元** mediator？ | 兩者常差一大截＝估計不穩 | 84%→64%（腎）、37%→26%（CV）[albuminuria_mediation_Agarwal_2023] |
| 5 | mediator–outcome 段有沒有**殘餘混淆**？ | E-value 小＝結論脆弱 | joint E-value 1.29 [albuminuria_mediation_Agarwal_2026] |
| 6 | 用的是 **total** 還是 **chronic** slope？ | R² 0.97 vs 0.55 是兩個等級 | Inker 2023 [egfr_slope_surrogate_Inker_2023] |
| 7 | **acute dip** 被剪掉了嗎？ | 剪掉會高估持續益處 | acute 每 1 單位→HR +11.4% [egfr_slope_surrogate_Greene_2025] |
| 8 | **相對**還是**絕對**？基線風險多高？ | 同一 HR 在低風險族群絕對意義小 | >1% 10-yr ARR 僅在 ACR>30 [egfr_slope_surrogate_Coresh_2019] |

一句話帶走：**relative ≠ absolute、individual-level ≠ trial-level、R² 高 ≠ 臨床可替代、mediation % ≠ 機轉佔比、slope ≠ slope。**

---

## 證據分層小結

| 統計論點 | 等級 | 主要本地全文來源 |
|---|---|---|
| individual-level 關聯（ESKD HR 0.78）≠ trial-level 有效性 | 🟢 | `egfr_slope_surrogate_Coresh_2019` 📄 |
| UACR trial-level R²=0.66（0.06–0.98）、寬 CI＝高不確定 | 🟢/🟡 | `r2_Heerspink_2025`、`editorial_endpoints_Heerspink_2019` 📄 |
| R² 依藥物類別而異（82/45/41%）、陰性預測強 | 🟢 | `editorial_endpoints_Matyjek_2026` 📄 |
| mediation 連續 vs 二元不穩（84/64、37/26） | 🔴 abstract | `albuminuria_mediation_Agarwal_2023` 📌 |
| joint 中介 50%、E-value 1.29、measurement-error 敏感度 | 🟡 | `albuminuria_mediation_Agarwal_2026` 📄 |
| total slope R²=0.97 vs chronic 0.55 | 🟢 | `egfr_slope_surrogate_Inker_2023`、`Inker_2019` 📄 |
| acute dip 帶資訊、最佳權重 0.078、每單位 HR +11.4% | 🟢/🟡 | `egfr_slope_surrogate_Greene_2025` 📄 |
| CV 益處早於腎保護（數月 vs ~18 月）之時序錯配 | 🟡 | `albuminuria_mediation_Agarwal_2026` 📄 |
| HF 低白蛋白尿族群中介比例（34/29、15/11） | 🔴 abstract | `albuminuria_mediation_Mc_2025` 📌 |
| slope 用作終點須排除 acute effect | 🟢 | `egfr_slope_surrogate_Levey_2020` 📄 |

## 本地全文語料（可 grep 稽核）

📄 全文：`egfr_slope_surrogate_Coresh_2019`（個體層級 ESKD HR）、`r2_Heerspink_2025`（UACR trial-level R²=0.66）、`editorial_endpoints_Heerspink_2019`（舊 trial-level R²=0.47/0.72）、`editorial_endpoints_Matyjek_2026`（藥物類別 82/45/41%、陰性預測）、`egfr_slope_surrogate_Inker_2019`／`Inker_2023`（total vs chronic slope R²）、`egfr_slope_surrogate_Greene_2025`（acute/chronic 拆解、權重 0.078）、`egfr_slope_surrogate_Levey_2020`（NKF-FDA-EMA workshop）、`albuminuria_mediation_Agarwal_2026`（FIDELITY UACR+SBP 多 mediator、E-value、時序）。
📌 abstract（數字不擴張）：`albuminuria_mediation_Agarwal_2023`（84/64、37/26 中介）、`albuminuria_mediation_Mc_2025`（FINEARTS-HF 中介）。

---

## References（Vancouver，含本地檔）

1. Coresh J, Heerspink HJL, Sang Y, et al. Change in albuminuria and subsequent risk of end-stage kidney disease: an individual participant-level consortium meta-analysis of observational studies. Lancet Diabetes Endocrinol. 2019;7(2):115–27. 📄 [egfr_slope_surrogate_Coresh_2019]
2. Heerspink HJL, Collier WH, Chaudhari J, et al. A meta-analysis of albuminuria as a surrogate endpoint for kidney failure. Nat Med. 2025. 📄 [r2_Heerspink_2025]
3. Heerspink HJL, Greene T, Tighiouart H, et al. Change in albuminuria as a surrogate endpoint for progression of kidney disease: a meta-analysis of treatment effects in randomised clinical trials. Lancet Diabetes Endocrinol. 2019;7(2):128–39. 📄 [editorial_endpoints_Heerspink_2019]
4. Matyjek A, Fernández-Fernández B. Validation of albuminuria as a surrogate endpoint in chronic kidney disease. Clin Kidney J. 2026;19(5):sfag054. 📄 [editorial_endpoints_Matyjek_2026]
5. Inker LA, Heerspink HJL, Tighiouart H, et al. GFR slope as a surrogate end point for kidney disease progression in clinical trials. J Am Soc Nephrol. 2019;30(9):1735–45. 📄 [egfr_slope_surrogate_Inker_2019]
6. Inker LA, Collier W, Greene T, et al. A meta-analysis of GFR slope as a surrogate endpoint for kidney failure. Nat Med. 2023;29(7):1867–76. 📄 [egfr_slope_surrogate_Inker_2023]
7. Greene T, Collier W, Haaland B, et al. Clinical implications of the slope of GFR in clinical trials of CKD progression. Clin J Am Soc Nephrol. 2025;20(5):632–41. 📄 [egfr_slope_surrogate_Greene_2025]
8. Levey AS, Gansevoort RT, Coresh J, et al. Change in albuminuria and GFR as end points for clinical trials in early stages of CKD (NKF-FDA-EMA workshop). Am J Kidney Dis. 2020;75(1):84–104. 📄 [egfr_slope_surrogate_Levey_2020]
9. Agarwal R, Pandey A, Solomon SD, Vaduganathan M, Zannad F. Systolic blood pressure and albuminuria reduction mediate cardiovascular benefits of finerenone in T2D and CKD. Nephrol Dial Transplant. 2026. 📄 [albuminuria_mediation_Agarwal_2026]
10. Agarwal R, Tu W, Farjat AE, et al. Impact of finerenone-induced albuminuria reduction on CKD outcomes in T2D: a mediation analysis. Ann Intern Med. 2023;176(12):1606–16. 📌 [albuminuria_mediation_Agarwal_2023]
11. Mc Causland FR, Vaduganathan M, Claggett BL, et al. Changes in albuminuria and the effect of finerenone on cardiovascular outcomes: insights from FINEARTS-HF (abstract #3019). Nephrol Dial Transplant. 2025;40(Suppl 3). 📌 [albuminuria_mediation_Mc_2025]

---
*此檔為主題二之統計深度解讀，撰寫日期基準 2026-07-11。所有具體數字均可 grep 回上列本地全文 MD。Agarwal 2023 與 Mc 2025 僅取得結構化 abstract，其中介百分比維持 📌 且不擴張；統計詮釋（相對vs絕對、層級混淆、R² 意義、mediation 過度解讀、時序錯配）為本檔之改寫與解讀工作，數字本身未經杜撰。*
