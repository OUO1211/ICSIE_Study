# 3-2　生成與獨立

## 線性組合(linear combination)

> 考慮體系 $F$ 的向量空間 $V/F$，
>
> (1) 設向量 $v_1, v_2, \ldots, v_k \in V$，純量 $a_1, a_2, \ldots, a_k \in F$，
>
> 則稱 $v = v_1a_1 + v_2a_2 + \cdots + v_ka_k = \displaystyle\sum_{i=1}^{k} v_i a_i$ 為 $v_1, v_2, \ldots, v_k$ 的線性組合。
>
> (2) 設 $S \subseteq V$，任取向量 $v_1, v_2, \ldots, v_k \in S$，純量 $a_1, a_2, \ldots, a_k \in F$，
>
> 則稱 $v = v_1a_1 + v_2a_2 + \cdots + v_ka_k = \displaystyle\sum_{i=1}^{k} v_i a_i$ 為 $S$ 的一組線性組合。

例如：

$v_1 = \begin{bmatrix} 1 \\ 0 \\ 0 \end{bmatrix}$，$v_2 = \begin{bmatrix} 0 \\ 2 \\ 0 \end{bmatrix}$，$v_3 = \begin{bmatrix} 2 \\ 6 \\ 0 \end{bmatrix}$，則因為 $v_3 = 2v_1 + 3v_2$，故可稱 $v_3$ 為 $v_1, v_2$ 的一線性組合。

$v_1 = 5x$，$v_2 = 7x^2$，$v_3 = 10x + x^2$，則因為 $v_3 = 2v_1 + \dfrac{1}{7}v_2$，故可稱 $v_3$ 為 $v_1, v_2$ 的一線性組合。

$v_1 = \begin{bmatrix} 0 & 0 \\ 0 & 4 \end{bmatrix}$，$v_2 = \begin{bmatrix} 5 & 0 \\ 0 & 0 \end{bmatrix}$，$v_3 = \begin{bmatrix} 0 & 0 \\ 0 & 0 \end{bmatrix}$，則因為 $v_3 = 0v_1 + 0v_2$，

故可稱 $v_3$ 為 $v_1, v_2$ 的一線性組合。