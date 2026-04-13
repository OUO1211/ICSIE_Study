# 3-5 座標化

## 座標表示

> 令 $\beta = \{b_1, \ldots, b_n\}$ 為向量空間 $V$ 之一有序基底，
>
> 則對 $\forall v \in V$，存在唯一一組純量 $c_1, \ldots, c_n$，滿足 $v = c_1 b_1 + \cdots + c_n b_n$，
>
> 並稱：
>
> $\begin{bmatrix} c_1 \\ \vdots \\ c_n \end{bmatrix}$
>
> 為 $v$ 相對於 $\beta$ 的座標向量，記成 $[v]_\beta$。

> **Note**
>
> (1) 有序基底(ordered basis)：若改變基底中的向量順序，則當成不同的基底。
>
> (2) 給定 $\beta$ 為 $V$ 之一有序基底，則
>
> (i) $\forall v \in V$，$[v]_\beta$ 存在且唯一。
>
> (ii) $\forall a, b \in F$，$\forall u, v \in V$，$[au + bv]_\beta = a[u]_\beta + b[v]_\beta$。
>
> (iii) $u = v \Leftrightarrow [u]_\beta = [v]_\beta$。
>
> (iv) $\forall x \in F^{n \times 1}$，存在唯一一 $v \in V$，使得 $[v]_\beta = x$。

例如

$\beta = \left\{ \begin{bmatrix} 0 \\ 1 \end{bmatrix}, \begin{bmatrix} 2 \\ 0 \end{bmatrix} \right\}$ 為 $\mathbb{R}^2$ 的一組基底，向量 $v = \begin{bmatrix} 1 \\ 2 \end{bmatrix} = 2 \begin{bmatrix} 0 \\ 1 \end{bmatrix} + \frac{1}{2} \begin{bmatrix} 2 \\ 0 \end{bmatrix}$，

故 $[v]_\beta = \begin{bmatrix} 2 \\ 1/2 \end{bmatrix}$。