---
subject: Discrete Mathematics
status: finished
---

# Vandermonde捲積

## 定義

Vandermonde 捲積描述從兩個不交集合合計選取元素的組合數。

## 核心模型/公式

$$
\sum_k\binom rk\binom s{n-k}=\binom{r+s}n.
$$

左側按「從第一群選 $k$ 個、第二群選 $n-k$ 個」分類；右側直接從總共 $r+s$ 個元素選 $n$ 個。

也可由比較 $(1+x)^r(1+x)^s=(1+x)^{r+s}$ 的 $x^n$ 係數得到。求和上下限可寫為所有整數 $k$，因為超出範圍的二項式係數視為 $0$。
