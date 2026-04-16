---
subject: Linear Algebra
tags: [矩陣, 定義, Chapter1]
status: finished
---

## 定義

> **列梯陣 (REF, Row Echelon Form)**：矩陣滿足：
> 1. 所有零列在非零列的下方
> 2. 每個非零列的第一個非零元素（**領導元素 pivot**）位於上一列 pivot 的右邊

> **簡化列梯陣 (RREF, Reduced Row Echelon Form)**：在 REF 基礎上，另要求：
> 3. 每個 pivot 為 $1$
> 4. pivot 所在行的其他元素均為 $0$

## 例子

$$\text{REF: } \begin{bmatrix} 1 & 2 & 0 \\ 0 & 1 & 3 \\ 0 & 0 & 0 \end{bmatrix}, \quad \text{RREF: } \begin{bmatrix} 1 & 0 & -6 \\ 0 & 1 & 3 \\ 0 & 0 & 0 \end{bmatrix}$$

## 性質

- 任意矩陣都可以透過**基本列運算**化為 RREF
- RREF 是唯一的（對於給定矩陣，RREF 形式唯一）
- RREF 中非零列的數量 = $\operatorname{rank}(A)$

## 應用

- 求[[秩 Rank|矩陣的秩]]
- 解線性方程組（高斯-喬登消去法）
- 判斷[[可逆矩陣|矩陣可逆]]性（$A$ 可逆 $\Leftrightarrow$ RREF 為 $I$）

## 相關連結

- [[基本列運算]]
- [[PAQ分解]]
- [[利用列運算求反矩陣]]
