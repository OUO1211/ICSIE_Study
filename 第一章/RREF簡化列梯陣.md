---
subject: Linear Algebra
tags: [矩陣, 定義, Chapter1]
status: finished
core_mapping: "pivot 化為 1 且所在行清零，非零列數等於 rank"
mantra: "梯形 pivot 要為 1，上下清空成 RREF"
pattern_signal_strong:
  - condition: "題目要求化為 RREF（簡化列梯陣）"
    weight: 3
  - condition: "題目問矩陣的 rank（數 RREF 非零列數）"
    weight: 3
pattern_signal_weak:
  - condition: "題目判斷矩陣是否可逆（RREF 是否為 I）"
    weight: 1
  - condition: "題目要找 pivot 列（基底行）與自由行"
    weight: 1
anti_signal:
  - condition: "REF 不等於 RREF（REF 中 pivot 不必為 1）"
  - condition: "RREF 唯一，但到達 RREF 的過程（列運算順序）不唯一"
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

- 求[[秩Rank|矩陣的秩]]
- 解線性方程組（高斯-喬登消去法）
- 判斷[[可逆矩陣|矩陣可逆]]性（$A$ 可逆 $\Leftrightarrow$ RREF 為 $I$）

## 相關連結

- [[基本列運算]]
- [[PAQ分解]]
- [[利用列運算求反矩陣]]
