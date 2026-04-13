## 線性算子的行列式與跡數

> **定義**
>
> 設 $T \in L(V, V)$，$\dim(V) < \infty$，任取 $V$ 的一組有序基底 $\beta$，
>
> 定義 $\det(T) = \det([T]_\beta)$ 為 $T$ 的**行列式**；
>
> 定義 $\text{tr}(T) = \text{tr}([T]_\beta)$ 為 $T$ 的**跡數**。

> **Note**
>
> 雖然一個線性算子矩陣表示會因選取的基底不同而不同，但因這些矩陣會彼此相似，而使得此線性算子的行列式與跡數都是固定值。

> **例如**
>
> 令 $T: R^2 \to R^2$ 定義為
> $$
> T\begin{bmatrix} a \\ b \end{bmatrix}
> =
> \begin{bmatrix} a+b \\ 2a-b \end{bmatrix},
> $$
> 則 $L$ 的標準矩陣表示為
> $$
> \begin{bmatrix} 1 & 1 \\ 2 & -1 \end{bmatrix}.
> $$
>
> 故 $\det(T) = -3$，$\text{trace}(T) = 0$。