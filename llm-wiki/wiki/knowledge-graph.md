# 知識圖譜

> 自動生成 | 2026-07-22 | 全庫共 203 個節點、2400 條關聯
> 下圖只畫**度數最高的 30 個節點**與其中權重最高的關聯，避免圖過密。完整互動版見 `wiki/knowledge-graph.html`。

```mermaid
graph LR
  N0["Finerenone"]
  N1["FIDELITY"]
  N2["高血鉀"]
  N3["UACR"]
  N4["CONFIDENCE"]
  N5["替代終點"]
  N6["2026-07-22-07-…"]
  N7["FINEARTS-HF"]
  N8["Spironolactone"]
  N9["eGFR dip"]
  N10["臨床統計素養與常見陷阱"]
  N11["SGLT2i"]
  N12["原發性醛固酮症"]
  N13["適應症版圖擴張"]
  N14["高血鉀安全工程"]
  N15["2026-07-22-06-…"]
  N16["FIDELIO-DKD"]
  N17["eGFR slope"]
  N18["中介分析"]
  N19["FIND-CKD"]
  N20["相對風險與絕對風險"]
  N21["KDIGO 2026 糖尿病…"]
  N22["2026-07-22-06-…"]
  N23["Empagliflozin"]
  N24["FIGARO-DKD"]
  N25["效益風險權衡與指引仿單框架"]
  N26["NNT"]
  N27["Baxdrostat"]
  N28["交互作用檢定"]
  N29["四大支柱"]
  N0 --> N1
  N0 --> N12
  N0 --> N16
  N0 --> N24
  N0 --> N3
  N0 --> N8
  N1 --> N0
  N1 --> N16
  N1 --> N24
  N1 --> N3
  N10 --> N20
  N10 --> N28
  N10 --> N9
  N12 --> N0
  N12 --> N27
  N12 --> N6
  N12 --> N8
  N13 --> N12
  N14 --> N2
  N14 --> N23
  N14 --> N25
  N16 --> N0
  N16 --> N1
  N16 --> N2
  N16 --> N24
  N16 --> N26
  N16 --> N3
  N17 --> N1
  N17 --> N19
  N17 --> N3
  N17 --> N5
  N19 --> N1
  N19 --> N17
  N19 --> N3
  N21 --> N29
  N23 --> N2
  N23 --> N9
  N24 --> N0
  N24 --> N1
  N24 --> N16
  N24 --> N26
  N24 --> N3
  N25 --> N14
  N25 --> N2
  N25 --> N29
  N25 --> N8
  N27 --> N0
  N27 --> N12
  N27 --> N6
  N29 --> N21
  N3 --> N1
  N3 --> N17
  N3 --> N19
  N5 --> N17
  N6 --> N12
  N6 --> N27
  N7 --> N1
  N8 --> N0
  N8 --> N12
  N9 --> N23
```

## 圖譜結構說明

Louvain 社群偵測把 203 個節點分成 11 個社群，社群名取自該群最具代表性的頁面：

| 社群 | 節點數 | 說明 |
|------|--------|------|
| 臨床統計素養與常見陷阱 | 41 | 橫切全庫的方法學與統計概念，是最大的一群——反映七個主題各有一份統計迷思檔 |
| 合成端 vs 受體端：ASI 與原發性醛固酮症 | 32 | 主題七自成一個相對獨立的知識塊 |
| 四大支柱與加藥策略 | 26 | CONFIDENCE、SGLT2i、序列 vs 同步起始 |
| 替代終點方法學 | 22 | UACR、eGFR slope、終點資格化 |
| 效益風險權衡與指引仿單框架 | 18 | NNT/NNH、KDIGO、仿單條文 |
| eGFR dip 與腎絲球血流動力學 | 16 | 血流動力學可逆性 |
| 適應症版圖擴張 | 14 | T1D、非糖尿病 CKD、HF |
| 受體藥理與 nsMRA 分野 | 12 | 受體選擇性、解離動力學 |
| 因果中介分析 | 9 | UACR/SBP/血鉀 三條中介路徑 |
| 高血鉀安全工程 | 9 | 場景別監測 |
| 低血鉀 | 4 | 電解質帳的另一端，目前素材最少 |

## 樞紐節點（度數前 10）

| 節點 | 度數 |
|------|------|
| Finerenone | 129 |
| FIDELITY | 94 |
| 高血鉀 | 75 |
| UACR | 59 |
| CONFIDENCE | 58 |
| 替代終點 | 58 |
| FINEARTS-HF | 55 |
| Spironolactone | 53 |
| eGFR dip | 50 |
| SGLT2i | 46 |

## 查看方式

- **互動式（推薦）**：雙擊 `wiki/knowledge-graph.html`（建議 Chrome / Firefox；Safari 若提示「已阻止指令碼」，可在 `wiki/` 下跑 `python3 -m http.server 8000` 再訪問）
- **Mermaid 靜態圖**：本檔，Obsidian / VS Code（Markdown Preview Enhanced）/ GitHub / Typora 皆可渲染

> 圖譜洞察（surprising connections、bridge nodes）因圖規模超出腳本預算（203 節點 / 2400 邊，上限 250 / 1000）而降級，僅保留基礎權重與社群偵測。
