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

### 第三階段：模式化 (Pattern Match Phase)

- **目標**：題型與解法解構（考研衝刺核心）。
- **動作**：建立「題型模式筆記」。
- **要求**：
    - 辨識題目特徵（如：看到 $A^k$、看到 $tr(A)$）。
    - 匹配對應工具（如：對角化、特徵值性質）。
    - 格式：`## 題目特徵` -> `## 聯想工具` -> `## 解題陷阱`。
