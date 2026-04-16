---
subject: Linear Algebra
tags: [矩陣, 定義, Chapter1]
status: finished
---

## 定義

> **Hermitian 矩陣**：$A^H = A$，即 $\overline{a_{ij}} = a_{ji}$
>
> **斜 Hermitian 矩陣 (skew-Hermitian)**：$A^H = -A$

Hermitian 矩陣是對稱矩陣在複數域上的推廣。

## 性質

- Hermitian 矩陣的對角項必為**實數**（因為 $\overline{a_{ii}} = a_{ii}$）
- 若 $A$ 為 Hermitian，則 $A^2$，$AA^H$，$A^H A$ 均為 Hermitian
- Hermitian 矩陣的特徵值必為**實數**（進階性質）

## 與對稱矩陣的關係

| 類型 | 條件 | 適用域 |
|------|------|--------|
| 對稱矩陣 | $A^T = A$ | 實數域 |
| Hermitian | $A^H = A$ | 複數域 |

## 相關連結

- [[共軛轉置矩陣]]
- [[對稱矩陣與斜對稱矩陣]]
