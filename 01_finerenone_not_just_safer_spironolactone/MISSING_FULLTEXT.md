# MISSING FULLTEXT — 主題候選一

僅取得 abstract / metadata（📌），未對其內容做具體數字斷言，僅引用試驗設計 / 基線特徵。

| Paper | DOI | Reason | Note |
|-------|-----|--------|------|
| （本輪已無僅 abstract 的 FINEARTS-HF 文獻） | — | — | Solomon 2024 與 Vaduganathan 2024 已升級為本地全文，見下方「已補全文」小節 |

## 已補全文（本輪升級）

本輪由使用者上傳之本地 PDF，經 LlamaParse 轉為 Markdown 全文（status: full_text），可 grep 稽核。以下文獻由 📌（abstract-only）升級為 📄（本地全文）：

| Paper | DOI | 本地全文檔 | 已驗證/落地內容 |
|-------|-----|-----------|----------------|
| Solomon SD et al. FINEARTS-HF baseline characteristics. Eur J Heart Fail. 2024. | 10.1002/ejhf.3266 | `hf_finearts_Solomon_2024.md` | 主文第 4.3 節「竇性心律者 NT-proBNP ≥300 pg/mL」「基線中位 NT-proBNP 1041 pg/mL」兩數字已 grep 命中並改標 📄；References 第 21 條同步改 📄 |
| Vaduganathan M et al. FINEARTS-HF rationale/design. Eur J Heart Fail. 2024. | 10.1002/ejhf.3253 | `hf_finearts_Vaduganathan_2024.md` | 試驗設計全文可 grep（隨機 6001 人、37 國、竇性心律 NT-proBNP ≥300 pg/ml 納入門檻等）；本文僅引用其試驗設計，References 第 22 條改 📄 |

**新增本地全文檔（先前無此檔／stub）：**

| Paper | DOI | 本地全文檔 | 說明 |
|-------|-----|-----------|------|
| Filippatos G et al. ARTS-HF：finerenone vs. eplerenone（HFrEF + DM/CKD，phase 2b）。Eur Heart J. 2016. | 10.1093/eurheartj/ehw132 | `arts_hf_Filippatos_2016.md` | 先前於「fetch 失敗（內容過濾）」欄記載遭 content-filtering 攔下未落地；**現已由使用者上傳之本地 PDF 經 LlamaParse 補全全文**。第 6 節「誠實承認的限制」新增此唯一 finerenone-vs-eplerenone 直接對頭之描述（90 天 phase 2b；主終點 NT-proBNP 下降 >30% 兩組相近，eplerenone 37.2% vs finerenone 30.9–38.8%，P=0.42–0.88；探索性臨床複合終點僅 10 mg 組 HR 0.56, 95% CI 0.35–0.90, nominal P=0.02），並強調其非長期腎臟硬終點對頭。已加入 References 第 23 條，標 📄 |

## 誠實限制

本地全文語料中**無** finerenone 對類固醇型 MRA 的**長期腎臟硬終點** head-to-head 數據（第 6 節已載明）。新補之 ARTS-HF 雖為 finerenone-vs-eplerenone 直接對頭，但屬 90 天 phase 2b、以 NT-proBNP 下降比例為主終點之短期研究，不構成長期腎臟硬終點對頭證據，故此限制仍成立。
