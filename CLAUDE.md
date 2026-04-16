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
