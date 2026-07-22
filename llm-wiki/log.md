# 操作日誌

> 記錄知識庫的所有變更歷史

---

## 2026-07-22 — 初始化

- **操作**：建立知識庫
- **主題**：nsMRA / Finerenone 心腎代謝文獻知識庫
- **語言**：中文（繁體）
- **狀態**：完成

## 2026-07-22 batch-ingest | deep-research 專案 40 篇回顧稿

- **素材來源**：`/Users/ander/Documents/medical/diabetes/nsmra/deep-research/` 七大主題資料夾的實質內容檔
- **納入 40 檔**：母體研究報告 1、KDIGO 2026 草案 1、主題一 4、主題二 4、主題三 7、主題四 7、主題五 12、主題六 2、主題七 3（含英文投稿稿 `manuscript_clean.md`）
- **刻意排除**：`_audit_*.md`、`MISSING_FULLTEXT.md`、`撰寫方法論.md`、`PA_SOURCE_INVENTORY.md`（流程稽核檔，留在母專案）
- **未納入**：436 個 `原始PDF/*.md` 全文轉檔（作為 grep 稽核語料留在母專案，未來可分批消化）

**新增頁面**：

- 素材摘要 40 頁（`wiki/sources/2026-07-22-*.md`）
- 實體頁 147 頁（初建 128 + 補漏 19）（`wiki/entities/`）——臨床試驗 34、藥物 19、方法學概念 19、生物標記 9、統計指標 8、臨床現象 7、族群概念 6、指引 6，其餘為策略、機轉、分子標的類
- 主題頁 16 頁（`wiki/topics/`）——由 9 組 ingest 提出的 60 個零散主題收斂而成

**更新頁面**：

- `purpose.md`——寫入六個關鍵問題、研究範圍與證據分級約定
- `.wiki-schema.md`——別名詞表換成本領域 20 組實際用詞（nsMRA、UACR、ASI、PA、K binder 等）
- `index.md`——全量重建，實體頁依九大類分組
- `wiki/overview.md`——重寫知識地圖

**處理管線**：9 個平行 ingest agent（依主題分工）產出 source 頁與實體／主題候選 JSON → 正規化合併（138 個原始實體名 → 128 個標準實體）→ 6 個平行 agent 寫實體頁、2 個寫主題頁 → 索引重建。分階段的用意是避免平行寫入時在 `index.md` 與實體頁上互相覆蓋。

**證據紀律**：沿用母專案規則，所有數字、試驗名、HR/CI 須能 grep 回 `raw/notes/` 原檔；推論性關係以 `<!-- confidence: INFERRED -->` 標記，原文含糊處以 `<!-- confidence: AMBIGUOUS -->` 標記。

## 2026-07-22 graph | 知識圖譜

- `wiki/graph-data.json`——203 節點、2400 條關聯，Louvain 分出 11 個社群
- `wiki/knowledge-graph.html`（2.4 MB）——互動式圖譜，離線雙擊可開
- `wiki/knowledge-graph.md`——Mermaid 靜態圖（度數前 30 節點）＋ 社群與樞紐節點說明
- 圖譜洞察（surprising connections / bridge nodes）因圖規模超出腳本預算（203 節點 / 2400 邊，上限 250 / 1000）而**降級**，僅保留基礎權重與社群偵測

## 2026-07-22 lint | 健康檢查與斷鏈修復

- 首次 lint：87 條斷鏈
- 修復三類：source 頁連結漏日期前綴（36 處）、正規化前的舊實體名（如 `Acute dip`→`eGFR dip`、`可逆性`→`停藥可逆性`）、描述性片語映射到既有頁（如 `早期聯用`→`同步起始`）
- 剩餘 19 個確為新實體，補建頁面（BrigHTN、Launch-HTN、Target-HTN、BaxPA、HALO、LCI699、EMPA-KIDNEY、Semaglutide、NT-proBNP、ENaC、CYP11B1、HSD11B2、Kcnk1、KDIGO 2024、ADA-KDIGO 2022 consensus、GRADE 證據等級、心律不整複合終點、心房顫動、排鉀利尿劑）
- 最終狀態：**0 孤立頁、0 斷鏈、index 雙向一致**，實體頁 147、主題頁 16、素材頁 40
