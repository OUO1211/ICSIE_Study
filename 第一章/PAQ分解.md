---
subject: Linear Algebra
tags: [矩陣, 分解, Chapter1]
status: finished
core_mapping: "列+行運算化標準形 [Ir O; O O]，直接讀出 rank"
mantra: "PAQ 化標準形，左右夾出秩"
pattern_signal_strong:
  - condition: "題目要求求矩陣標準形或找 P、Q 使 PAQ=[Ir O;O O]"
    weight: 3
  - condition: "題目要用列/行運算同時化簡求 rank"
    weight: 3
pattern_signal_weak:
  - condition: "題目僅求秩（rank），可只做列運算到 REF）"
    weight: 1
  - condition: "出現非方陣（PAQ 分解對 m×n 矩陣均適用）"
    weight: 1
anti_signal:
  - condition: "P 和 Q 必須可逆（列/行基本矩陣的乘積），不可任意取"
  - condition: "PAQ 分解非唯一，P 和 Q 的選取方式有多種"
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
- 可用來求[[秩Rank|矩陣的秩]]

## 相關連結

- [[基本列運算]]
- [[基本行運算]]
- [[RREF簡化列梯陣]]
