## 2-3 行列式

對方陣 $A$，以 $\det(A)$ 或 $|A|$ 來表示 $A$ 的行列式（determinant），是一種為了求解線性方程組而引進的特定算式，計算方式如下：

1 階行列式：設 $A = [a]$，則 $A$ 的行列式 $\det(A) = a$。

2 階行列式：設 $A = \begin{bmatrix} a & b \\ c & d \end{bmatrix}$，則 $\det(A) = ad - bc$。

3 階行列式：設 $A = \begin{bmatrix} a & b & c \\ d & e & f \\ g & h & i \end{bmatrix}$，則 $\det(A) = aei + bfg + cdh - ceg - afh - bdi$。

而其實對於階數 $n \geq 2$ 的 $n \times n$ 矩陣的行列式，可以透過方式定義，合稱如後。

> **餘因子（cofactor）**
>
> 考慮矩陣 $A = \begin{bmatrix} a_{11} & a_{12} & \cdots & a_{1n} \\ \vdots & & & \vdots \\ & & a_{ij} & \\ \vdots & & & \vdots \\ a_{n1} & & \cdots & a_{nn} \end{bmatrix}$
>
> 令 $M_{ij}$ 表示刪去第 $i$ 列與第 $j$ 行之後的 $(n-1) \times (n-1)$ 方陣，
>
> 則 $A$ 的餘因子（cofactor）：$cof(a_{ij})$，定義為 $(-1)^{i+j} \det(M_{ij})$。

> **Note**
>
> 例如：$A = \begin{bmatrix} 1 & 2 & 3 \\ 3 & 4 & 5 \\ 4 & 5 & 6 \end{bmatrix}$，則
>
> $cof(a_{11}) = (-1)^{1+1} \det\begin{bmatrix} 4 & 5 \\ 5 & 6 \end{bmatrix} = 24 - 25 = -1$。
>
> $cof(a_{12}) = (-1)^{1+2} \det\begin{bmatrix} 3 & 5 \\ 4 & 6 \end{bmatrix} = -(18 - 20) = 2$。
