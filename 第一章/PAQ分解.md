---
subject: Linear Algebra
tags: [矩陣, 分解, Chapter1]
status: finished
---

## 定義

> **PAQ 分解**：給定矩陣 $A \in F^{m \times n}$，存在可逆矩陣 $P$（$m \times m$）和 $Q$（$n \times n$），使：
>
> $$PAQ = \begin{bmatrix} I_r & O \\ O & O \end{bmatrix}$$
>
> 其中 $r = \operatorname{rank}(A)$。

〔91 成大統計〕

## 步驟

1. 對 $A$ 做**列運算**，化為列梯形矩陣
2. 再做**行運算**，化為簡化列梯矩陣（含 $I_r$ 塊）
3. $P$ = 所有列基本矩陣之乘積
4. $Q$ = 所有行基本矩陣之乘積

## 例子

$$A = \begin{bmatrix} 1 & 1 & 0 & -1 \\ 3 & 2 & 1 & 1 \\ 1 & 0 & 1 & 3 \end{bmatrix}$$

經列運算→行運算，得 $PAQ = \begin{bmatrix} I_2 & O \\ O & O \end{bmatrix}$，即 $r = 2$。

## 性質

- PAQ 分解等價於 $\operatorname{rank}(A) = r$
- 可用來求[[秩 Rank|矩陣的秩]]

## 相關連結

- [[基本列運算]]
- [[基本行運算]]
- [[RREF簡化列梯陣]]
