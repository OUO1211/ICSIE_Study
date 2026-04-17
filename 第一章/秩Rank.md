---
subject: Linear Algebra
tags: [矩陣, 定義, Chapter1, Chapter2]
status: finished
---

## 定義

> **矩陣的秩 (rank)**
>
> 考慮矩陣 $A \in F^{m \times n}$，將 $A$ 以[[基本列運算]]化為[[RREF簡化列梯陣|列梯陣（REF）]]，若剩下 $k$ 個非零列，則稱 $A$ 的秩為 $k$，記作：
>
> $$\operatorname{rank}(A) = k$$

## 例子

$$A = \begin{bmatrix} 1 & 1 & 1 \\ 1 & 1 & 2 \end{bmatrix} \xrightarrow{r_{12}^{(-1)}} \begin{bmatrix} 1 & 1 & 1 \\ 0 & 0 & 1 \end{bmatrix} \implies \operatorname{rank}(A) = 2$$

$$B = \begin{bmatrix} 1 & 0 & -2 & 3 \\ 2 & 2 & 0 & 4 \\ 2 & 0 & -4 & 6 \\ 1 & 1 & 1 & 1 \end{bmatrix} \xrightarrow{\text{列運算}} \begin{bmatrix} 1 & 0 & -2 & 3 \\ 0 & 1 & 2 & -1 \\ 0 & 0 & 1 & -1 \\ 0 & 0 & 0 & 0 \end{bmatrix} \implies \operatorname{rank}(B) = 3$$

## 性質

- $\operatorname{rank}(A) \leq \min(m, n)$
- $\operatorname{rank}(A)$ = [[RREF簡化列梯陣]] 中 **pivot 的個數**
- $\operatorname{rank}(A) = \operatorname{rank}(A^T)$（列秩 = 行秩）
- $A$ [[可逆矩陣|可逆]] $\Leftrightarrow$ $\operatorname{rank}(A) = n$（$n$ 階方陣）
- $\operatorname{rank}(AB) \leq \min(\operatorname{rank}(A),\, \operatorname{rank}(B))$
- 與 [[PAQ分解]]：$PAQ = \begin{bmatrix} I_r & O \\ O & O \end{bmatrix}$，$r = \operatorname{rank}(A)$

## 與線性方程組 $Ax = b$ 的關係

> $A$ 為 $m \times n$ 矩陣

| 條件 | 結論 |
|------|------|
| $\operatorname{rank}(A) \neq \operatorname{rank}([A \mid b])$ | **無解** |
| $\operatorname{rank}(A) = \operatorname{rank}([A \mid b]) = n$ | **唯一解** |
| $\operatorname{rank}(A) = \operatorname{rank}([A \mid b]) < n$ | **無限多解**，有 $n - \operatorname{rank}(A)$ 個自由變數 |
| $\operatorname{rank}(A) = m$（對所有 $b$）| 方程組**必相容**（至少有一解）|

## 經典考題

〔94 台大資工〕**以下何者為真？**

- $\operatorname{rank}(A) = m$ $\Rightarrow$ $Ax=b$ 對任意 $b$ 至少有一解 ✓
- $\operatorname{rank}(A) = n$ $\Rightarrow$ $A$ 的行向量線性獨立 ✓
- $m > n$ 且 $\operatorname{rank}(A) = n$ $\Rightarrow$ $Ax=b$ 對任意 $b$ 有解 ✗（行不夠多覆蓋所有 $b$）

〔101 政大統計〕**$A$ 為非奇異 $n \times n$ 矩陣，$Ax=b$ 是否有唯一解？**

True。$A$ 可逆 $\Rightarrow$ $\operatorname{rank}(A) = n$，故唯一解為 $x = A^{-1}b$。

〔101 台科資工〕**$\operatorname{rank}(A) < n$ 是否代表 $Ax=b$ 對任意 $b$ 有無限多解？**

False。$\operatorname{rank}(A) < n$ 只說明若有解則無限多解，但不保證有解（可能無解）。

## 相關連結

- [[RREF簡化列梯陣]]
- [[基本列運算]]
- [[PAQ分解]]
- [[可逆矩陣]]

---

> **第三章延伸**：本筆記為 rank 的操作性定義（以 RREF 非零列計算）。
> 第三章從子空間維度的角度嚴格證明「列秩 = 行秩」，並引入 Sylvester 定理：
> → [[矩陣的秩]]（第三章，含完整性質與 Sylvester 不等式）
> → [[秩與線性系統]]（第三章，以行空間語言重述解的條件）
