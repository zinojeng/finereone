# MR 受體的解離動力學與駐留時間：finerenone vs spironolactone / eplerenone 的微觀物理機制

> 本檔回答一個受體層級的微觀問題：**當一個 MR 拮抗劑「結合」到受體上之後，它在受體上「待多久」才鬆手？這個「駐留時間（residence time）」由什麼決定？三種藥（finerenone / spironolactone / eplerenone）的解離動力學與拮抗『型態』為何不同、其結構根源何在？** 這是「藥物在受體上待多久」（受體端）而非「藥物在血中待多久」（PK 端）的故事——後者與臨床 hold-restart 的耦合請見姊妹檔 `pk_pd_hysteresis_offrate_hold_restart.md`，本檔**不重複**臨床解毒流程，專注**分子結合的物理**。
>
> **引用標記慣例**：📄 = 本地全文可 grep 稽核；📌 = 僅取得 abstract（不對其未載內容作具體數字斷言）。每個數字句末以 `[本地MD檔名]` 標註來源供 grep 回溯。LLM 僅負責組織、改寫與**藥理詮釋**；所有數字（half-life、Kd、IC50、EC50、koff 對應量）均出自本地 MD，詮釋可延伸，數字不可杜撰。
>
> **證據分層**：🟢 已確立共識／實測值｜🟡 in-vitro 動力學／結構模型／機轉外推｜🔴 假說、尚無定量 published data 的缺口。
>
> **一句話結論**：受體佔據的持久度由**解離速率常數 koff**決定（residence time ≈ 1/koff），與血中濃度是兩回事。finerenone 在本地語料中有明確的量化錨點——**解離半衰期 ~50 min**、Kd 1.52 nM；其「bulky passive」拮抗在結構上塞不緊（helix 12 被撐開、複合體不穩定），動力學上正對應「放得快」。spironolactone / eplerenone 的**逐一 koff／residence time 定量值本地並不存在**（🔴），僅能以結構型態、prodrug 代謝物延長效應與 Fagart 對「passive 拮抗劑 dissociate quickly」的定性描述作**方向性**推論，不杜撰其具體 off-rate。

---

## 一、開場：residence time 的藥理框架——「待多久」不等於「血中有多少」🟡

藥效學裡有一個常被臨床端忽略的分離：**受體被佔據的持久度，取決於藥物從受體「鬆手」的速度（off-rate，koff），而非血中游離濃度的高低**。以最簡框架寫：

- **駐留時間 residence time ≈ 1 / koff**——koff 越小（鬆手越慢），藥物在受體上「駐留」越久。
- 這是一個**藥理框架**（可詮釋）；框架本身不帶數字。任何具體的解離半衰期、Kd、IC50 都必須來自本地實測（下節逐一標源）。

為什麼要把它從 PK 拆開？因為兩者計時完全不同：血中藥物濃度由代謝清除（CYP、腎排）決定；受體佔據由分子在結合口袋裡「卡得緊不緊」決定。一個血中半衰期很短的藥，若 koff 極小，仍可長時間佔據受體；反之亦然。本檔關心的正是後者——**受體口袋裡的微觀物理**。

> **白話比喻**：把 MR 想成一把鎖，拮抗劑是插進去的鑰匙。PK 半衰期問的是「櫃檯（血液）還有幾把備用鑰匙」；residence time 問的是「已經插進鎖孔的這把鑰匙，卡得多緊、多久會自己滑出來」。兩個問題的答案可以完全不同。

---

## 二、finerenone 的解離動力學（唯一可量化者）：~50 min 與 bulky-passive 的動力學對應 🟡

本地語料對 finerenone 給了三個互相扣合的錨點（皆出自同一篇分子藥理原著）：

- **解離半衰期 ~50 min**：kinetic 實驗測得 finerenone–MR 複合體的 dissociation half-life of ~50 min [molecular_Amazit_2015.md] 📄。
- **Kd = 1.52 ± 0.01 nM**：與 in vitro 轉譯之全長 MR 高親和力結合 [molecular_Amazit_2015.md] 📄。
- **功能性 IC50 = 58 ± 9 nM** [molecular_Amazit_2015.md] 📄。

把三者一起讀，出來的圖像是：finerenone **結合得夠緊**（奈莫耳級 Kd，足以有效拮抗），但**解離並不慢**（~50 min），並非「一結合就長期黏死」。這與它的拮抗型態一致——finerenone 屬 **bulky-passive（被動）拮抗**：Fagart 把 passive 拮抗劑歸為「會快速從受體解離的小分子」，並以 **BR-4628 從 MR 的快速解離**（原檔關鍵詞 `quickdissociation`，因 PDF 轉檔字元黏連）佐證 MR·BR-4628 複合體無法形成穩定構型 [r2_Fagart_2010.md] 📄。

**本檔的核心動力學洞見**：「複合體不穩定（bulky passive）」在動力學上正對應「解離快」——結構上塞不緊 → koff 較大 → residence time 較短。這是把 Amazit 的 ~50 min 與 Fagart 的快速解離（`quickdissociation`）放在同一條因果線上的合理詮釋（🟡，機轉外推）。

> **📌 邊界提醒**：~50 min 是 **in-vitro kinetic** 值，描述分子從受體鬆手的速度，**不等於**人體停藥後生理回正的時間。它的正確用途是：告訴我們「受體黏滯」不是下游 PD lag 的主因（詳見姊妹檔 `pk_pd_hysteresis_offrate_hold_restart.md` 第三、五節）。

---

## 三、對比 spironolactone：等效量級的 IC50，但 prodrug＋長效代謝物延長「有效受體暴露」，且在 S810L 上轉為 agonist 🟡🔴

spironolactone 的**受體端親和力**與 finerenone 屬同一量級：功能性 IC50 **74.0 ± 15 nM**（對照 finerenone 58 ± 9 nM）[molecular_Amazit_2015.md] 📄；在另一結構研究的 transactivation 體系中，spironolactone IC 為 **50.0 nM**（同體系 BR-4628 33.5 nM）[r2_Fagart_2010.md] 📄。也就是說，**「結合有多緊」兩者相近**，真正拉開差距的是三件受體端以外／型態上的事：

1. **prodrug + 長效活性代謝物**：spironolactone 本身血漿半衰期短，但代謝出三個長效活性代謝物——canrenone（16.5 h）、TMS（13.8 h）、HTMS（15.0 h），穩態下以 TMS 為主 [molecular_Kolkhof_2017.md] 📄。**分子層面的意義**：即使母藥從受體鬆手（passive 型態本身 koff 不算小），血中仍源源不絕地供應「活性分子」回頭佔據 MR——**「有效受體暴露」被代謝物在時間軸上拉長**，而非單一分子的 residence time 變長。這是 spironolactone「受體端更黏」的錯覺來源：黏的不是某一顆分子，是**代謝物接力**。
2. **S810L 上的型態反轉（機轉危險性）**：在 S810L 突變 MR（早發性高血壓致病突變）上，spironolactone **轉為 agonist**（EC50 = 25 ± 2 × 10⁻¹¹ M）；而 finerenone 維持**嚴格拮抗**（IC50 = 16.1 ± 3.1 × 10⁻⁶ M，不活化該突變體）[molecular_Amazit_2015.md] 📄。這說明兩者與受體的接觸型態在結構上本質不同（詳見第五節）。
3. **不招募 co-repressor**：ChIP/相互作用實驗顯示 spironolactone 與 BR-4628 一樣，**不促使 MR 招募 NCoR（co-repressor）**，且會抑制 NCoR 與 MR-aldosterone 複合體的結合 [r2_Fagart_2010.md] 📄；同時 spironolactone 在 SCNN1A 上表現為 **partial agonist**（促進 SRC-1 招募，程度低於 aldosterone），與 finerenone 的 inverse-agonist 相反 [molecular_Kolkhof_2017.md] 📄。

> **🔴 誠實邊界**：本地語料**沒有** spironolactone 自身的解離半衰期／koff／residence time 定量值。上述「有效受體暴露被拉長」是**代謝物 PK ＋型態**的合理推論，**不可**回填成 spironolactone 的具體 off-rate 數字。

---

## 四、對比 eplerenone：對 MR 親和力低、選擇性優於 spironolactone、效價顯著低於 bulky-passive 類 🟡

eplerenone 在受體端的定位很清楚：**對 MR 親和力低**。Fagart 記載其 transactivation IC 為 **2000 nM**（同體系 spironolactone 50.0 nM、BR-4628 33.5 nM）——即 BR-4628 與 spironolactone 效價相當，但顯著強於 eplerenone（原檔關鍵詞 `morepotentthaneplerenone`）[r2_Fagart_2010.md] 📄；Kolkhof 進一步量化 eplerenone 對 MR 的 in vitro 親和力「約比 spironolactone 低 **40-fold lower**」[molecular_Kolkhof_2017.md] 📄。

但 eplerenone 的存在理由是**選擇性**：其環氧修飾使分子更凹、降低對 AR/PR 的親和 → 選擇性優於 spironolactone（後者有抗雄性素等 off-target）[r2_Fagart_2010.md] 📄。in vivo 上 eplerenone 以較高的游離比例（血漿蛋白結合約 50%，spironolactone 則 94%）部分補償其低親和力 [molecular_Kolkhof_2017.md] 📄。finerenone 對 MR 的選擇性再進一階——**至少 500-fold 相對於 eplerenone 更選擇性 MR**、且效價至少等同 spironolactone [molecular_Kolkhof_2017.md] 📄。

> **🔴 誠實邊界**：eplerenone 亦**無**本地可查的 koff／residence time 定量值。低親和力（高 IC、40-fold lower）**在框架上暗示** koff 偏大／駐留較短，但這是由親和力推型態的**定性**推論，不等於實測 off-rate。

---

## 五、結構基礎：為何 off-rate 與拮抗型態不同？helix 12 protrusion 與 Asn770 接觸 🟡

三者的動力學差異，根在**結合口袋裡的立體化學**：

- **bulky 側鏈 → 撐開 helix 12（H12）**：bulky 非類固醇 MRA（BR-4628、finerenone）的 5-acetyl、C6-methyl 等基團向 H12 螺旋方向突出（原檔關鍵詞 `protrude toward the H12 helix`），使 H12 無法回到 agonist 位 [r2_Fagart_2010.md] 📄。Kolkhof 綜述進一步總結 bulky MRA「probably cause a **protrusion of helix 12** … and as a consequence, an **unstable receptor–ligand complex, which is unable to recruit coregulators**」[molecular_Kolkhof_2017.md] 📄。**動力學後果**：構型被剛化/撐開、無法收攏成穩定共構 → 複合體壽命短 → 解離快。
- **docking 於 agonist conformation、但反而致不穩定**：BR-4628 docking 到 MR 配體結合域的 agonist conformation，卻因與 D-ring 錨定區（Thr945）無接觸而**無法形成穩定複合體**；Fagart 以其**快速解離**（`quickdissociation`）與**對蛋白酶分解的低抵抗力**佐證此複合體不穩定 [r2_Fagart_2010.md] 📄。
- **Asn770 接觸與否 = agonist vs passive antagonist 的分子開關**：mutagenesis 指出 spironolactone/progesterone **無法與 Asn770 建立強接觸**是其被動拮抗特徵之源；BR-4628 則**強烈接觸 Asn770**。同時 Amazit 以突變體鎖定 **Ser-810 與 Ala-773** 為 finerenone 高選擇性的關鍵殘基 [molecular_Amazit_2015.md] 📄、[r2_Fagart_2010.md] 📄。S810L 上 spironolactone 反轉為 agonist（第三節），正說明這幾個接觸點的擾動足以把「拮抗」翻成「促效」。

> **白話比喻**：MR 的 H12 像一道要「喀」一聲扣上才會啟動下游的門閂。類固醇型（spiro/eple）體積合身、不去頂那道門閂，屬「被動不啟動」；bulky 非類固醇（fine/BR-4628）則像塞了一個過大的楔子，把門閂**頂歪**——門關不上（無法招募 coregulator），而且楔子本身塞不穩、容易滑出（解離快）。

---

## 六、功能後果：passive antagonism、核轉位延遲、cofactor 招募抑制 🟡

結合型態的差異，向下游投射成三層可觀察的功能差別：

- **passive vs 型態差異的 coregulator 後果**：finerenone 與 BR-4628 為 bulky-passive，不主動招募 co-repressor；而 finerenone 在 SCNN1A 上更進一步表現 **inverse agonism**——連 basal 狀態的 MR 與 SRC-1 招募都被壓低，spironolactone 則為 partial agonist [molecular_Amazit_2015.md] 📄、[molecular_Kolkhof_2017.md] 📄。
- **核轉位延遲**：aldosterone 單獨誘導最大 translocation index **3.11 ± 0.02**；拮抗劑單獨（1 h）僅輕度上升（spironolactone 1.84 ± 0.01、finerenone 1.76 ± 0.01），且 finerenone **比 spironolactone 更有效延遲** aldosterone 誘導的 MR 核輸入 [molecular_Amazit_2015.md] 📄。
- **cofactor recruitment 抑制**：finerenone 抑制 MR、SRC-1、RNA Pol II 於 SCNN1A 調控序列的招募 [molecular_Amazit_2015.md] 📄——這條「型態 → cofactor → 下游轉錄」的鏈，正是姊妹檔 `pk_pd_hysteresis_offrate_hold_restart.md` 第四節所述 PD 效應的分子起點。

**交叉連結（不重複）**：本節止於「受體型態如何決定 cofactor 招募」；至於 cofactor/ENaC 下游重建的**時間常數**與停藥後 PD 回復速率，屬臨床 PK–PD 耦合，見姊妹檔第四、五節（該檔明示其定量半衰期為缺口）。

---

## 七、三藥並列對比表 🟡

| 維度 | finerenone | spironolactone | eplerenone | 來源 |
|---|---|---|---|---|
| 功能性 IC50 / 效價 | **58 ± 9 nM**（另體系 BR-4628 類 33.5 nM） | **74.0 ± 15 nM**（另體系 50.0 nM） | 親和力低（IC 2000 nM；約 40-fold lower vs spiro） | `molecular_Amazit_2015` / `r2_Fagart_2010` / `molecular_Kolkhof_2017` 📄 |
| Kd（全長 MR） | **1.52 ± 0.01 nM** | 本地無並列 Kd 定量 | 本地無並列 Kd 定量 | `molecular_Amazit_2015` 📄 |
| **解離動力學（koff / residence time）** | **解離半衰期 ~50 min**（實測；bulky-passive「quick dissociation」） | **本地無定量**（prodrug＋代謝物 canrenone 16.5 / TMS 13.8 / HTMS 15.0 h 延長「有效受體暴露」） | **本地無定量**（低親和力→框架上推測 koff 偏大，非實測） | `molecular_Amazit_2015` / `r2_Fagart_2010` / `molecular_Kolkhof_2017` 📄；🔴 spiro/eple 無 koff |
| 拮抗型態 | bulky **passive**（非類固醇），複合體不穩定 | 類固醇型 passive／SCNN1A 上 **partial agonist** | 類固醇型（低親和力弱拮抗） | `r2_Fagart_2010` / `molecular_Kolkhof_2017` 📄 |
| S810L 突變體上行為 | **維持拮抗**（IC50 16.1 ± 3.1 × 10⁻⁶ M） | **轉為 agonist**（EC50 25 ± 2 × 10⁻¹¹ M） | 本地未給 eple S810L 定量（Kolkhof 述 steroidal MRA 悖論性活化 S810L） | `molecular_Amazit_2015` / `molecular_Kolkhof_2017` 📄 |
| NCoR / coregulator 招募 | 不招募 co-repressor；**inverse agonist**（壓 basal SRC-1） | 不招募 NCoR、抑制 NCoR–MR-aldo 結合；SCNN1A 上 **partial agonist** | 本地未給 eple 之 NCoR 數據 | `r2_Fagart_2010` / `molecular_Amazit_2015` 📄 |
| 活性代謝物 | 無（見姊妹檔：inactive metabolites） | **有且長效**：canrenone 16.5 / TMS 13.8 / HTMS 15.0 h | 本地未特別列長效活性代謝物 | `molecular_Kolkhof_2017` 📄 |
| 選擇性 / off-target | 最選擇性（≥500-fold vs eplerenone） | 有 off-target（抗雄性素、PR 促效） | 選擇性優於 spironolactone，但親和力低 | `molecular_Kolkhof_2017` / `r2_Fagart_2010` 📄 |
| 組織分布 | 心／腎 balanced distribution | 代謝物主導、心組織放射性低 | 腎累積 ≥3-fold 高於心 | `molecular_Kolkhof_2017` 📄 |

---

## 八、誠實邊界 🔴：三者並列的 koff / residence time 表在本地並不存在

必須明確揭露本檔最重要的缺口，避免製造「排序幻覺」：

- **只有 finerenone 有實測解離半衰期（~50 min）** [molecular_Amazit_2015.md] 📄。**spironolactone 與 eplerenone 各自的解離半衰期／koff／residence time，本地與已檢索學術來源（含 Consensus／PubMed 檢索）未提供定量值**。
- **不存在三者並列的 kon/koff 表**；本檔第七節表中 spiro/eple 的解離動力學欄位一律標「本地無定量」。
- 因此任何「residence time 排序」只能作**定性**描述：finerenone 有已知的 ~50 min ＋ bulky-passive「quick dissociation」型態；spironolactone 的「受體端更持久」實為**代謝物接力延長有效暴露**而非單分子 koff 變小；eplerenone 由低親和力**框架推測** koff 偏大。**不杜撰** spiro/eplerenone 的具體 off-rate 數字。
- Fagart 的英文逐字引句因 PDF 轉檔字元黏連（多處單字連寫），本檔對該檔多採中文概念改寫，僅保留可 grep 命中之關鍵詞（如 `passive`、`quickdissociation`、`agonist conformation`、`33.5nM`、`50.0nMforspironolactone`、`2000nMfor`、`morepotentthaneplerenone`），未硬填無法 grep 的 verbatim 長引號。

---

## 證據分層小結

| 論點 | 等級 | 主要本地全文來源 |
|---|---|---|
| finerenone–MR 解離半衰期 ~50 min、Kd 1.52 nM、IC50 58 nM | 🟡 in-vitro kinetic | `molecular_Amazit_2015.md` 📄 |
| spironolactone IC50 74 nM（另體系 50.0 nM）、S810L 轉 agonist、partial agonist | 🟡 in-vitro | `molecular_Amazit_2015.md` / `r2_Fagart_2010.md` / `molecular_Kolkhof_2017.md` 📄 |
| bulky-passive「dissociate quickly / quick dissociation」、helix 12 protrusion、Asn770 接觸 | 🟡 結構/動力學 | `r2_Fagart_2010.md` / `molecular_Kolkhof_2017.md` 📄 |
| eplerenone 低親和力（IC 2000 nM、40-fold lower）、選擇性優於 spironolactone | 🟡 in-vitro | `r2_Fagart_2010.md` / `molecular_Kolkhof_2017.md` 📄 |
| spironolactone prodrug＋長效代謝物（canrenone 16.5 / TMS 13.8 / HTMS 15.0 h） | 🟢 藥動學綜述 | `molecular_Kolkhof_2017.md` 📄 |
| NCoR 不招募、抑制 NCoR–MR-aldosterone 結合、inverse vs partial agonist | 🟡 相互作用/ChIP | `r2_Fagart_2010.md` / `molecular_Amazit_2015.md` 📄 |
| **spironolactone / eplerenone 各自 koff / residence time 定量值、三者並列 kon/koff 表** | 🔴 尚無 published 數據 | —（誠實揭露，第八節） |

## 本地全文語料（可 grep 稽核）

📄 全文：`molecular_Amazit_2015.md`（解離半衰期 ~50 min、Kd 1.52±0.01 nM、IC50 58±9 / 74.0±15 nM、translocation index 3.11±0.02、spiro 1.84 / fine 1.76、S810L：spiro EC50 25±2×10⁻¹¹ M / fine IC50 16.1±3.1×10⁻⁶ M / aldo EC50 4.2±0.4×10⁻¹⁰ M、Ser-810/Ala-773、inverse agonism）、`r2_Fagart_2010.md`（BR-4628 IC 33.5nM / spironolactone 50.0nM / eplerenone 2000nM、160-fold、agonist conformation、passive「dissociatequickly」/「quickdissociation」、NCoR 不招募、H12/Asn770/protrusion、複合體不穩定 unable to recruit co-regulator）、`molecular_Kolkhof_2017.md`（prodrug <2h、canrenone 16.5 / TMS 13.8 / HTMS 15.0 h、eplerenone 40-fold lower、蛋白結合 94% / ~50%、finerenone ≥500-fold 選擇性、bulky-passive helix 12 protrusion unstable complex unable to recruit coregulators、balanced distribution、eplerenone 腎累積 3-fold）。

---

## References（Vancouver 風格，含本地檔）

1. Amazit L, Le Billan F, Kolkhof P, et al. Finerenone impedes aldosterone-dependent nuclear import of the mineralocorticoid receptor and prevents genomic recruitment of steroid receptor coactivator-1. J Biol Chem. 2015;290(36):21876-21889. 📄 [molecular_Amazit_2015.md]
2. Fagart J, Hillisch A, Huyet J, et al. A new mode of mineralocorticoid receptor antagonism by a potent and selective nonsteroidal molecule (BR-4628). J Biol Chem. 2010;285(39):29932-29940. 📄 [r2_Fagart_2010.md]
3. Kolkhof P, Bärfacker L. 30 years of the mineralocorticoid receptor: MRAs — 60 years of research and development. J Endocrinol. 2017;234(1):T125-T140. 📄 [molecular_Kolkhof_2017.md]

---
*此檔為主題一之「MR 受體解離動力學／駐留時間」微觀機制深度解讀，為 `pk_pd_hysteresis_offrate_hold_restart.md` 之姊妹深挖（該檔談三時鐘的臨床耦合，本檔專注受體結合物理，不重複 hold-restart 臨床流程）。所有具體數字（~50 min、Kd 1.52 nM、IC50 58/74 nM、BR-4628 33.5 / spiro 50.0 / eple 2000 nM、40-fold、500-fold、S810L EC50 25×10⁻¹¹ M / IC50 16.1×10⁻⁶ M、canrenone 16.5 / TMS 13.8 / HTMS 15.0 h、translocation 3.11 / 1.84 / 1.76）均可 grep 回上列本地全文 MD。residence time ≈ 1/koff 為藥理框架、bulky-passive↔解離快之對應為機轉詮釋。明示缺口：spironolactone / eplerenone 各自的 koff / residence time 定量值與三者並列 kon/koff 表，本地與已檢索學術來源全無，標為 🔴、不賦予數字。撰寫日期基準 2026-07-12。*
