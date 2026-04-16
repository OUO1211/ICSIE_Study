---
subject: Linear Algebra
tags: [矩陣, 定義, Chapter1, Chapter2]
status: finished
---

## 定義

> **矩陣的秩 (rank)**
>
> 將矩陣 $A$ 做基本列運算化為列梯陣（REF），剩下 $k$ 個非零列，則稱：
>
> $$\operatorname{rank}(A) = k$$

## 例子

$$A = \begin{bmatrix} 1 & 1 & 1 \\ 1 & 1 & 2 \end{bmatrix} \xrightarrow{r_{21}^{(-1)}} \begin{bmatrix} 1 & 1 & 1 \\ 0 & 0 & 1 \end{bmatrix} \implies \operatorname{rank}(A) = 2$$

## 性質

- $\operatorname{rank}(A) \leq \min(m, n)$（$A$ 為 $m \times n$ 矩陣）
- $\operatorname{rank}(A) = $ [[RREF簡化列梯陣]] 中 pivot 的個數
- $A$ 可逆 $\Leftrightarrow$ $\operatorname{rank}(A) = n$（方陣）
- $\operatorname{rank}(AB) \leq \min(\operatorname{rank}(A),\, \operatorname{rank}(B))$

## 與線性方程組的關係

考慮 $Ax = b$（$A$ 為 $m \times n$）：

| 條件 | 結論 |
|------|------|
| $\operatorname{rank}(A) \neq \operatorname{rank}([A \mid b])$ | **無解** |
| $\operatorname{rank}(A) = \operatorname{rank}([A \mid b]) = n$ | **唯一解** |
| $\operatorname{rank}(A) = \operatorname{rank}([A \mid b]) < n$ | **無限多解**（$n - \operatorname{rank}(A)$ 個自由變數）|

## 經典考題

〔94 台大資工〕以下何者為真？

- `rank(A) = m` $\Rightarrow$ $Ax=b$ 至少有一解 ✓
- `rank(A) = n` $\Rightarrow$ $A$ 的行向量線性獨立 ✓
- `rank(A) = n` 且 $A$ 為 $m \times n$，$m > n$ $\Rightarrow$ $Ax=b$ 不一定有解

## 與 PAQ 分解的關係

$$PAQ = \begin{bmatrix} I_r & O \\ O & O \end{bmatrix}, \quad r = \operatorname{rank}(A)$$

## 相關連結

- [[RREF簡化列梯陣]]
- [[基本列運算]]
- [[PAQ分解]]
- [[可逆矩陣]]
