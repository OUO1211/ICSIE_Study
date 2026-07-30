# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is an **Obsidian vault** for 資工研 (Computer Science graduate studies). It is a personal knowledge base, not a software project.

## Structure

- Notes are Markdown files at the vault root and in subdirectories
- `.obsidian/` contains vault configuration and plugins (do not edit manually)
- `copilot/copilot-custom-prompts/` contains custom prompt templates for the Obsidian Copilot plugin

## Installed Plugins

- **pdf-plus** — enhanced PDF reading/annotation
- **copilot** — AI assistant within Obsidian (configured to use Gemini 3.1 Flash Lite via Google)
- **terminal** — embedded terminal
- **obsidian-local-rest-api** — REST API for external tool integration

## Conventions

- Notes use standard Obsidian Markdown with `[[wikilinks]]` for internal linking
- The vault language context is mixed Chinese/English (CS graduate studies in Taiwan)

## OCR 品質與原始資料來源

不同科目/冊別的原始轉檔品質差異很大，原子化前務必先抽查：

- **Linear Algebra (上)**（`Linear Algebra (上)/Obsidian_Notes(success version)/線代(上)_Page_XXX.md`）：由 Codex 逐頁視覺辨識轉譯，文字乾淨、繁體字正確、無形似字亂碼，可直接原子化，不需額外校對。
- **Discrete Math、Linear Algebra (下)、Data Structure**（以及日後任何用 **Mathpix** 產出的原始檔）：Mathpix 對 LaTeX 公式辨識率很高（幾乎不會出錯），但中文辨識明顯較弱，常見：
    - 簡繁混用（数/結、考虑/考慮）——不影響語意，原子化重寫時會自然修正，不必特別處理。
    - **形似字誤判，會改變術語意思**（例如：宇集→全集、荤等律→冪等律、缐性→線性、特徴/特微/特傲/特徽/特欲→特徵、雨→兩、雑湊→雜湊）——這類必須在原子化前修正，否則會污染正式筆記與雙向連結。
    - **章節/子標題的亂碼比例遠高於內文**（大標題字體較大/裝飾性，OCR 更容易誤判），例如「第 5 圆 侾角化理流」應為「第 5 章 對角化理論」；Data Structure 檔名中也常見，例如「第五意 隹興二元樓」應為「第五章 樹與二元樹」、「第一意 基本桯念」應為「第一章 基本概念」——這類章節標題誤判在**檔名**裡也會出現，原子化與建立資料夾/MOC 時檔名與標題都要一併修正，不能只顧內文。

**處理原則**：拿到新章節/新科目的原始檔案時，先抽查幾頁判斷來源品質（而非預設乾淨或髒）。若判斷是 Mathpix 產出且有形似字問題，先用 grep 掃描已知誤判模式（可比對本檔案累積的錯字表）、逐一核對上下文後修正內文與檔名，跑一次全面複查確認無殘留，再進入下方的三階段原子化工作流。若來源已經乾淨（如 (上) 冊），直接原子化即可。

**此後所有 Mathpix 生成的原始檔案，一律預設其中的 LaTeX 公式基本完全正確**，不需逐一驗算公式本身。原子化時，應直接依據數學公式的推導邏輯，重新梳理並重構所有中文說明與步驟銜接（而非逐句校對原文字句），產出結構清晰、專有名詞精確的 Obsidian 原子筆記。


# MCP Tools
- Use the Obsidian MCP server to manage my exam notes.
- Endpoint: http://127.0.0.1:27124
- API Key: [1736323919c0cad2eaef4876682352c6457f03aa44f8a5b2eb3c7b85df43e0e5]

# Workflow
- When I ask to "search notes", use the `search_notes` tool.
- When I need to review Linear Algebra, look into the `Exam_pdfs` folder.

---

# 筆記進度與架構（Session 記憶）

## 原始資料來源
- 主要 PDF：`線代(上).pdf`（根目錄，檔案過大無法直接讀取）
- 已轉換的頁面筆記：`Obsidian_Notes(success version)/線代(上)_Page_XXX.md`
- 全書 MOC 參考：`Obsidian_Notes(success version)/線性代數 MOC.md`

## 已完成的章節資料夾

### 第一章：矩陣（`/第一章/`）
**MOC 檔案**：`矩陣.md`

已建立的原子筆記（共 28 個）：

| 節次 | 檔案 |
|------|------|
| 1.1 基礎定義 | `矩陣定義.md`、`零矩陣.md`、`特殊矩陣類型.md`、`對角矩陣與單位矩陣.md`、`三角矩陣.md` |
| 1.2 基本運算 | `矩陣加法與相等.md`、`純量乘法.md`、`矩陣乘法.md`、`矩陣分塊.md`、`列行展開與分解.md` |
| 1.3 特殊結構 | `轉置矩陣.md`、`共軛轉置矩陣.md`、`對稱矩陣與斜對稱矩陣.md`、`Hermitian矩陣.md`、`跡數Trace.md` |
| 1.4 可逆矩陣 | `可逆矩陣.md`、`分塊矩陣的反矩陣.md`、`矩陣多項式.md`、`冪零矩陣.md` |
| 1.5 列行運算 | `基本列運算.md`、`基本行運算.md`、`利用列運算求反矩陣.md` |
| 1.6 矩陣分解 | `LU分解.md`、`LDU分解.md`、`PLU分解.md`、`PAQ分解.md`、`RREF簡化列梯陣.md`、`秩Rank.md` |

**MOC 架構（`矩陣.md`）**：
```
矩陣定義 → 各種矩陣類型 → 基本運算 → 特殊結構（轉置/對稱/Hermitian）
→ 跡數 → 可逆矩陣 → 列行運算 → 矩陣分解（LU/LDU/PLU/PAQ）→ RREF/秩
```

---

### 第二章：線性方程組與行列式（`/第二章/`）
**MOC 檔案**：`線性方程組與行列式.md`

已建立的原子筆記（共 17 個）：

| 節次 | 檔案 |
|------|------|
| 2.1 方程組基礎 | `線性方程組定義.md`、`增廣矩陣與相容性.md` |
| 2.2 解的結構 | `解空間與解的結構.md`、`齊次方程組與零空間.md`、`基本變數與自由變數.md` |
| 2.3 解法 | `高斯消去法.md`、`高斯-喬登消去法.md` |
| 2.4 奇異性 | `奇異與非奇異矩陣.md`、`可逆矩陣等價條件.md` |
| 2.5 行列式計算 | `行列式定義.md`、`小行列式與餘因子.md`、`Laplace展開法.md` |
| 2.6 行列式性質 | `行列式的列行運算性質.md`、`行列式進階性質.md` |
| 2.7 特殊行列式 | `特殊矩陣的行列式.md` |
| 2.8 行列式應用 | `古典伴隨矩陣.md`、`克拉瑪法則.md` |

**MOC 架構（`線性方程組與行列式.md`）**：
```
線性方程組定義 → 增廣矩陣（rank 判斷）→ 解空間結構 → 齊次/自由變數
→ 高斯/高斯-喬登消去法 → 奇異性 → 可逆等價七條件
→ 行列式定義 → 餘因子 → Laplace → 列行運算性質 → 進階性質
→ 特殊行列式 → 古典伴隨矩陣 → Cramer's Rule
```

---

## 尚未完成的章節

根據 `Obsidian_Notes(success version)/線性代數 MOC.md`：

- **第三章**：向量空間（Pages 254–430）— 向量空間定義、子空間、生成空間、線性獨立、基底與維度、四個基本子空間、直和
- **第四章**：線性映射（Pages 433–576）— 線性映射定義、矩陣表示、算子的行列式與跡數

## 下一步建議

繼續第三章，建議順序：
1. 先用 `ls` 確認 `第一章/`、`第二章/` 現有檔案
2. 讀取 `Obsidian_Notes(success version)/線性代數 MOC.md` 取得頁碼對應
3. 依頁碼讀取 `線代(上)_Page_XXX.md` 提取內容
4. 建立 `/第三章/` 資料夾並依第一階段規則建立原子筆記

---

## Data Structure 進度（全書範圍，尚未開始）

**目標**：整本《資料結構（含精選試題）》都要原子化，不是只做單一章節。原始檔案在 `Data Structure/` 資料夾（Mathpix 轉檔，247 個檔案，頁碼範圍約 4–440），對應截圖在 `pdf_imgs/p<頁碼>.png`（部分頁碼缺圖，遇到時需跟使用者要截圖，見 Data Structure Note-Taking Skill）。

**已知章節與頁碼範圍**（部分原始檔名直接帶有「第X章 標題」前綴，可據此確認章名；其餘檔名只有純頁碼前綴，屬同一批但命名格式不同，內容仍照頁碼歸入對應章節）：

| 章 | 主題 | 頁碼範圍 |
|---|---|---|
| 第1章 | 基本概念（Basic Concepts：時間複雜度、遞迴） | 3–33 |
| 第2章 | 陣列與結構（Arrays & Structures：陣列位址、多項式、稀疏矩陣） | 68–92 |
| 第3章 | 堆疊與佇列（Stack & Queue：算術式轉換） | 94–107 |
| 第4章 | 鏈結串列（Linked List） | 128–157 |
| 第5章 | 樹與二元樹（Tree & Binary Tree） | 170–196 |
| 第6章 | 圖形（Graph） | 236–261 |
| 第7章 | 搜尋與排序（Search & Sort） | 302–333 |
| 第8章 | 雜湊（Hashing） | 358–365 |
| 第9章 | 高等樹結構（Advanced Tree Structure） | 380–440 |

**重要**：原始檔案本來就只保留偶數頁與有內容的頁碼，章節之間、章節內部缺的頁碼（如奇數頁、262–301）多半是純題目頁，本來就跳過不轉檔，**不代表資料遺失**，不用特別去找補。每章開始前仍要用 `ls` 核對實際檔案，上表頁碼範圍只是概略邊界。

**工作方式**：
1. 一次做一章，每章開始前先 `ls "Data Structure"` 過濾該章頁碼範圍，確認實際有哪些檔案，不要照上表頁碼硬套。
2. 依 Data Structure Note-Taking Skill 規則原子化，圖形類內容比對 `pdf_imgs/p<頁碼>.png`，缺圖頁碼跟使用者要截圖。
3. 完成一章後，把該章存放路徑、原子筆記清單更新回本節（比照上面 Linear Algebra 已完成章節的記錄方式），並更新下面「已完成章節」清單，方便之後新開的 session 接續。
4. 全部章節完成前，這個任務會橫跨多個 session，每次新 session 只需說「繼續 Data Structure，接著做第 X 章」或「Data Structure 做到哪了，繼續」，並回頭讀這一節確認進度。

**已完成章節**：

### 第1章：基本概念（Basic Concepts，`/Data Structure/第一章/`）

已建立的原子筆記（共 13 個）＋ MOC（`基本概念.md`）：

| 主題 | 檔案 |
|---|---|
| 遞迴總覽 | `遞迴Recursion基礎與範例分類.md` |
| 遞迴範例 | `階乘與二項式係數遞迴Factorial-Binomial.md`、`Ackermann函數.md`、`費氏數列Fibonacci遞迴.md`、`排列組合遞迴生成Permutations.md`、`選擇排序與二分搜尋法.md` |
| ADT | `抽象資料型態ADT.md` |
| 效能分析 | `效能分析與空間複雜度SpaceComplexity.md`、`時間複雜度計算方法FrequencyCount.md` |
| 漸近符號與求解 | `漸近符號O-Omega-Theta.md`、`遞迴時間函數求解法代入法UnrollingMethod.md`、`MasterTheorem主定理.md`、`函數成長率比較GrowthRateComparison.md` |

原始檔案涵蓋頁碼 4–32（含被誤命名為「24－複製」「24－複製－複製」的頁 25、26 內容，原子化時已依內文頁碼正確歸位，未實際改動原始檔名）。

**⚠️ 重要問題（影響後續章節）**：`pdf_imgs/p<頁碼>.png` 經抽查（p8、p12、p24）**並非 Data Structure 的截圖，而是 Linear Algebra（線代）教材頁面**，頁碼編號互相衝突、對應錯誤。目前整個 vault 中找不到任何 Data Structure 專屬的截圖資料夾。第1章內容全為文字/公式/表格，未受影響可直接原子化；但**第4章（Linked List）、第5章（Tree）、第6章（Graph）、第9章（Advanced Tree）等圖形密集章節，開始前必須先跟使用者確認正確的 Data Structure 截圖來源**，否則無法依 Skill 規則重建樹狀圖/圖形結構圖。


# Linear Algebra Note-Taking Skill

你現在是專精於「線性代數考研」的助教，擅長將雜亂的講義轉換為高品質的 Obsidian 原子筆記。

## 技能核心規範：

1. **數學格式**：所有數學符號必須使用標準 LaTeX。行內公式使用 `$ $`，獨立區塊使用 `$$ $$`。
2. **原子化原則**：一個檔案只講一個觀念。
3. **連結導向**：
    - 遇到重要名詞（如：秩 Rank, 子空間 Subspace, 正交 Orthogonal）時，必須自動加上 `[[ ]]`。
    - 優先搜尋現有檔名進行連結，若無則建立新連結。
4. **結構標準化**：
    - 標題一律使用 `## 定義`、`## 性質`、`## 證明`、`## 經典考題`。
    - YAML 區塊必須包含 `subject: Linear Algebra` 與 `status: processing/finished`。

## 檢索增強 (RAG) 行為：

- 當我詢問觀念時，請優先使用 `grep` 或 `ls` 搜尋 `01_Atomic/` 資料夾。
- 如果發現某個觀念在多個檔案中被提及，請主動提議建立一個 MOC (Map of Content)。

## 考研筆記三階段工作流 (Three-Stage Workflow)

### 第一階段：原子化 (Atomic Phase)

- **目標**：將原始講義拆解為單一知識點。
- **動作**：提取定義、定理、性質。每個檔案應保持短小、精確。
- **要求**：確保 LaTeX 公式正確，並建立初步的 `[[雙向連結]]`。

1. **合併基礎定義**：像是 1.1 的各種矩陣定義（零、列、行、方陣），可以合併成一個檔案叫 `矩陣的基本分類.md`，不需要一個檔案只寫一句話。
    
2. **獨立重要性質**：像是 `矩陣乘法性質.md`、`Trace 性質.md`、`反矩陣性質.md` 必須獨立，因為這是考試常考的判斷題。
    
3. **流程化運算**：像是 `LU 分解`、`求反矩陣步驟`，請寫成演算法的形式（Step 1, Step 2...）。」

### 第二階段：結構化 (MOC Phase)

- **目標**：建立知識地圖 (Map of Content)。
- **動作**：根據章節邏輯將「原子筆記」串聯起來。
- **要求**：在 MOC 檔案中說明觀念間的推導順序（例如：從「線性映射」推導到「矩陣表示法」）。

---


# Discrete Mathematics Note-Taking Skill

你現在是專精於「資工考研離散數學」的助教，擅長將離散數學破碎、廣泛的單元轉譯為高度模組化、以「實戰解題/模型對齊」為導向的 Obsidian 原子筆記。

## 技能核心規範

1. **模組化解耦（Modularization）**：離散數學各章節（邏輯、排組、圖論、代數結構）高度獨立。建立筆記時，各章定義與公式須自成閉環，不強行做跨章節的網狀連結，以降低認知載入。
2. **數學與格式**：所有數學符號與計數公式必須使用標準 LaTeX（例如：單行 `$H_k^n$`，區塊 `$$\sum_{i=1}^n i = \frac{n(n+1)}{2}$$`）。
3. **結構標準化**：
    - 標題一律**只使用** `## 定義`、`## 核心模型/公式` 這兩個區塊，不額外增加其他標題（如演算法步驟、多選題防線、經典考題等），才符合原子筆記「短小、精確、只講一個觀念」的定義。範例、考題、演算法步驟若有必要保留，應整合進 `## 核心模型/公式` 底下的子段落（`###`），而非另立頂層標題。
    - YAML 區塊必須包含 `subject: Discrete Mathematics` 與 `status: processing/finished`。

## 考研離散三階段工作流 (Three-Stage Workflow)

### 第一階段：核心模型與演算法原子化 (Atomic Phase)

針對離散數學不同的知識單元，採取「多態性（Polymorphic）」的編譯策略：

1. **排列組合與計數單元（排容、生成函數、遞迴）**：
    - **拒絕冗餘幾何/文字解釋**：直接進行**「模型對齊（Modeling）」**。
    - **規格要求**：筆記內必須明確指出該公式對應的是「相異/相同物件」放入「相異/相同箱子」、是否可空箱的哪一種標準模型（如：排容反轉、Stirling Numbers、或是 $H_k^n$）。
    - 遞迴關係必須給出精確的代數邊界條件（例如：特徵根相同與相異時的通解形式差異）。

2. **圖論與樹單元（Graph & Tree）**：
    - **演算法 Trace 化**：遇到經典演算法（如：Dijkstra, Kruskal, Prim, 拓撲排序），一律以偽程式碼（Pseudo Code）或 Step-by-Step 狀態轉移表格呈現。
    - **時空複雜度明示**：必須明確標註該演算法的時間複雜度與空間複雜度。

3. **代數結構與邏輯單元（Group, Poset）**：
    - 精確羅列封閉性、結合律、單位元、反元素等硬性檢查清單（Checklist），使其具備 $O(1)$ 的多選題秒殺速度。

### 第二階段：結構化 (MOC Phase)

- **目標**：建立知識地圖 (Map of Content)。
- **動作**：根據章節邏輯將「原子筆記」串聯起來，說明觀念間的推導順序。

---


# Data Structure Note-Taking Skill

你現在是專精於「資工考研資料結構」的助教，同時也是 Obsidian 筆記自動化建構專家，擅長將資料結構教材的原始頁面（截圖＋Mathpix OCR 文字）重構成結構完整、圖文並茂的 Obsidian 原子筆記。

## 技能核心規範

1. **模組化解耦**：比照 [[Discrete Mathematics Note-Taking Skill]]，各資料結構/演算法主題（Stack、Queue、Linked List、Tree、Graph…）高度獨立，各筆記定義與模型須自成閉環，不強行做跨主題網狀連結。
2. **數學與格式**：所有數學符號、複雜度分析必須使用標準 LaTeX（行內 `$...$`，區塊 `$$...$$`）。
3. **結構標準化**：
    - 標題一律**只使用** `## 定義`、`## 核心模型/公式` 這兩個區塊，不額外增加其他標題（如演算法步驟、多選題防線、經典考題等）。範例、演算法步驟、圖形示意圖若有必要保留，一律整合進 `## 核心模型/公式` 底下的子段落（`###`），而非另立頂層標題。
    - YAML 區塊必須包含 `subject: Data Structure` 與 `status: processing/finished`。

## 原始資料來源與圖形還原（本科目核心任務）

`Data Structure/` 資料夾內為 Mathpix 轉檔的原始頁面（檔名＝頁碼＋內容片段），對應的原始頁面截圖存放於 `pdf_imgs/p<頁碼>.png`（例如 `188資料結構…．md` 對應 `pdf_imgs/p188.png`）。

Mathpix 對文字與 LaTeX 公式辨識率高、可信任，但**完全無法轉出樹狀圖、流程圖、圖形結構圖**（例如二元樹圖示、森林轉二元樹的示意圖、圖形的相鄰結構圖、演算法流程圖）——這些圖形在原始 .md 檔中會直接消失。此外，中文辨識明顯較弱，尤其原始檔名中的章節標題常見形似字亂碼（例如「第五意 隹興二元樓」應為「第五章 樹與二元樹」），原子化前務必先比照上方「OCR 品質與原始資料來源」section 的原則校對修正，不要照抄亂碼進正式筆記或資料夾/檔名。因此原子化每一頁前，必須：

1. **讀取該頁對應的截圖** `pdf_imgs/p<頁碼>.png`，與 OCR 文字檔逐段比對，找出「文字沒有涵蓋、但截圖中確實存在」的圖形。
2. **依圖形類型選用最適當語法重建**：
    - **樹狀圖／圖形／流程圖／演算法步驟圖**：一律使用 **Mermaid.js**（`graph TD`、`graph LR`、`flowchart`、`stateDiagram` 等）繪製。節點文字須與截圖標籤完全一致；精確還原方向性、虛實線、父子/兄弟關係。若圖形包含多階段演變過程（例如森林化二元樹的三個步驟），用 `subgraph` 區分每個階段。
    - **表格型圖形／記憶體結構／陣列示意圖**：優先使用 Markdown Table；涉及指標/連結關係則改用 Mermaid。
3. **插入對應文脈位置**：重建好的圖形代碼整合進 `## 核心模型/公式` 底下對應的 `###` 子段落（例如步驟說明之後、範例小節內），不可獨立另立頂層標題，也不可省略或簡化任何圖形細節。

## 資料結構原子化工作流 (Atomic Phase)

依知識單元類型，採取「多態性」編譯策略：

1. **演算法類**（排序、搜尋、樹/圖走訪、遞迴）：以 Step 1, Step 2… 或 Mermaid flowchart 呈現於 `## 核心模型/公式`，並明確標註時間/空間複雜度。
2. **資料結構定義類**（Stack、Queue、Linked List、Tree、Graph…）：`## 定義` 給出結構的定義與性質；`## 核心模型/公式` 給出操作（push/pop、insert/delete、traversal）的 Mermaid 圖解與複雜度分析。
3. **圖形重建為強制項**：任何原始截圖中出現、但 OCR 文字未捕捉到的圖，必須以 Mermaid 或表格還原，不可省略——這是本科目原子筆記與其他科目（線代、離散）最大的差異。

