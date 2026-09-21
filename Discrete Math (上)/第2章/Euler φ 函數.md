---
subject: Discrete Mathematics
status: finished
---

# Euler φ 函數

## 定義

對正整數 $n>1$，Euler φ 函數定義為不超過 $n$ 且與 $n$ 互質的正整數個數：

$$
\phi(n)=|\{m\mid 1\le m\le n,\ \gcd(m,n)=1\}|.
$$

## 核心模型/公式

若 $n=p_1^{e_1}p_2^{e_2}\cdots p_k^{e_k}$，$p_1,\ldots,p_k$ 為相異質因數，則：

$$
\phi(n)=n\prod_{i=1}^k\left(1-\frac1{p_i}\right).
$$

### 排容模型

令 $U=\{1,\ldots,n\}$，令 $A_i$ 為 $U$ 中可被 $p_i$ 整除的數。與 $n$ 不互質恰為 $\bigcup_iA_i$；所求是 $\left|\bigcap_i\bar A_i\right|$。對各相異質因數的倍數集合套用 [[排容原理]]，可得乘積公式。

### 特例

$$
\phi(p)=p-1\quad(p\text{ 為質數}),
$$

$$
\phi(pq)=(p-1)(q-1)\quad(p,q\text{ 為相異質數}).
$$
