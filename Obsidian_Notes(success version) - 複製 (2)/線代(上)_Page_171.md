### 求行列式－Laplace 展開法

> **定義** 考慮方陣 $A$，$n \geq 2$：
>
> (1) 列展開：固定任意 $i$，$1 \leq i \leq n$，
>
> $$\det(A) = a_{i1} \cdot cof(a_{i1}) + a_{i2} \cdot cof(a_{i2}) + \cdots + a_{in} \cdot cof(a_{in}) = \sum_{k=1}^{n} a_{ik} \cdot cof(a_{ik})$$
>
> (2) 行展開：固定任意 $j$，$1 \leq j \leq n$，
>
> $$\det(A) = a_{1j} \cdot cof(a_{1j}) + a_{2j} \cdot cof(a_{2j}) + \cdots + a_{nj} \cdot cof(a_{nj}) = \sum_{k=1}^{n} a_{kj} \cdot cof(a_{kj})$$

例如：$A = \begin{bmatrix} a & b & c \\ d & e & f \\ g & h & i \end{bmatrix}$，對第一行展開：

$$cof(a_{11}) = (-1)^{1+1} \det\begin{bmatrix} e & f \\ h & i \end{bmatrix} = ei - fh，$$

$$cof(a_{21}) = (-1)^{2+1} \det\begin{bmatrix} b & c \\ h & i \end{bmatrix} = -(bi - ch) = ch - bi，$$

$$cof(a_{31}) = (-1)^{3+1} \det\begin{bmatrix} b & c \\ e & f \end{bmatrix} = bf - ce，$$

故 $\det(A) = a(ei - fh) + d(ch - bi) + g(bf - ce) = aei + dch + gbf - afh - dbi - ceg$。
