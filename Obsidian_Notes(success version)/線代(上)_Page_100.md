# 第一章 矩陣 99

## 1-3 進階試題練習

> **試題 1**
>
> Let $M_2(Z)$ be the set of all $2 \times 2$ matrices with integral entries. Is true that the equation $X^2 - 5X + 4I = O$ has at most two solutions in $M_2(Z)$?
>
> 【94 彰師數學】

**解**

$X^2 - 5X + 4I = O \Leftrightarrow (X - 4I)(X - I) = O$。

令 $X = \begin{bmatrix} a & b \\ c & d \end{bmatrix}$ 滿足所求，則需 $\begin{bmatrix} a-4 & b \\ c & d-4 \end{bmatrix} \begin{bmatrix} a-1 & b \\ c & d-1 \end{bmatrix} = \begin{bmatrix} 0 & 0 \\ 0 & 0 \end{bmatrix}$。

即：$\begin{cases} a^2 - 5a + 4 + bc = 0 \\ c(a+d-5) = 0 \\ b(a+d-5) = 0 \\ d^2 - 5d + 4 + bc = 0 \end{cases}$，而此方程組不止兩解，故原式不止兩解。

例如：$\begin{bmatrix} 0 & 2 \\ -2 & 5 \end{bmatrix}$，$\begin{bmatrix} 0 & -2 \\ 2 & 5 \end{bmatrix}$，$\begin{bmatrix} 0 & 1 \\ -4 & 5 \end{bmatrix}$ 都是解。

> **試題 2**
>
> (5%) Assume $A$, $B$, and $C$ are respectively $m \times p$, $p \times q$, and $q \times n$ matrices, and $M = ABC$. Let $M^{kl} = a_k c^l$ for $1 \leq k \leq p$ and $1 \leq l \leq q$ here $a_k$ and $c^l$ respectively denote the $k$-th column vector of $A$ and the $l$-th row vector of $C$. Prove that $M = \sum_{k=1}^{p} \sum_{l=1}^{q} b_{kl} M^{kl}$.
>
> 【104 交大資工】

**解**

$M = (AB)C = \left[\sum_{k=1}^{p} a_k b_k\right] C = \sum_{k=1}^{p} a_k [b_{k1}\ b_{k2}\ \ldots\ b_{kq}] C = \sum_{k=1}^{p} a_k \sum_{l=1}^{q} b_{kl} c^l = \sum_{k=1}^{p} \sum_{l=1}^{q} a_k b_{kl} c^l = \sum_{k=1}^{p} \sum_{l=1}^{q} b_{kl} M^{kl}$

> **試題 3**
>
> Let $A$, $B$ be $2 \times 2$ real matrices satisfying $AB = -BA$. Show that exists a real number $y$ such that $(AB)^2 = yI$.
>
> 【99 中正數學】