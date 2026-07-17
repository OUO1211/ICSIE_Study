## 線性獨立(linearly independent)與線性相依(linearly dependent)

> 考慮向量空間的一子集 $S$。  
> 若存在 $S$ 中的向量 $v_1 \sim v_k$，其純量係數 $c_1 \sim c_k$ 不全為零，滿足
> $$c_1 v_1 + c_2 v_2 + \cdots + c_k v_k = 0,$$
> 則稱 $S$ 為線性相依集，否則稱之為線性獨立集。 【105 中興統計】

> 例如：
>
> $$\left\{
> \begin{bmatrix} 1 \\ 1 \\ 1 \end{bmatrix},
> \begin{bmatrix} 1 \\ 0 \\ 1 \end{bmatrix},
> \begin{bmatrix} 0 \\ 1 \\ 0 \end{bmatrix}
> \right\}$$
>
> 為線性相依集，因為 $v_1 = v_2 + v_3$；
>
> 但
>
> $$\left\{
> \begin{bmatrix} 1 \\ 0 \end{bmatrix},
> \begin{bmatrix} 0 \\ 1 \end{bmatrix}
> \right\}$$
>
> 則為線性獨立集。

> **Note**
>
> (1) $V$ 的任何子集 $S$，不是線性獨立，就是線性相依。
>
> (2) 線性相依集的直觀看法：  
> $S$ 為線性相依集，即表示 $S$ 中存在有某向量，可表為其他向量的線性組合。
>
> (3) 線性獨立集的等價定義：  
> 對任意 $S$ 中之向量 $v_1 \sim v_k$，任意純量係數 $c_1 \sim c_k$，  
> 若 $c_1 v_1 + \cdots + c_k v_k = 0$ 則 $c_1 = \cdots = c_k = 0$，  
> 則稱 $S$ 為線性獨立集。
>
> (4) 令 $A$ 為 $B$ 的子集合，則  
> (i) 若在 $A$ 為相依集，則 $B$ 為相依集；(ii) 若 $B$ 為獨立集，則 $A$ 為獨立集。
>
> (5) $\{0\}$ 為相依集。
>
> (6) 若 $S$ 含零向量，則 $S$ 為相依集；反之，若 $S$ 為獨立集，則必不含零向量。
>
> (7) 空集合 $\emptyset$ 為獨立集。
>
> (8) 集合 $S$ 是否獨立要與其作為 $V$ 之下有關。例如取 $S=\{(1,0),(i,0)\}$，則在討論複係數時 $S$ 為相依集（因為 $i(1,0)=(i,0)$）；但討論實係數時 $S$ 為獨立集。 【97.105 台北統計，102 交大資工】
>
> (9) $A=[v_1,\ldots,v_n]$ 為方陣，則向量 $v_1,\ldots,v_n$ 為 $\mathbb{R}^n$ 的一獨立集 $\Leftrightarrow A$ 可逆  
> （當 $m=n$ 時，此也等同於方陣 $A$ 行列式 $\ne 0 \Leftrightarrow A$ 可逆）
>
> (10) 若 $\{v_1,\ldots,v_n\}$ 為 $\mathbb{R}^n$ 的一獨立集且 $A$ 可逆，則 $\{Av_1,\ldots,Av_n\}$ 亦為 $\mathbb{R}^n$ 的一獨立集。 【99 交大資工，107 中山應數】