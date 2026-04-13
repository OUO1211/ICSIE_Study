### 行列式基本性質－列運算與行運算

> **定義**
>
> (1) 任意對調 $A$ 的某兩行（列），所得行列式值與原行列式值，正負號相反。
>
> (2) $A$ 的某行（列）乘以非零實數 $k$，所得行列式值為原行列式值的 $k$ 倍。
>
> (3) $A$ 的某行（列）乘以非零實數 $k$ 加到另一行（列），所得行列式值不變。
>
> (4) $\det(kA)=k^n\det(A)$，$A:n\times n$。
>
> 【重要】

例如：

$$
\det\begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \\ 1 & 1 & 1 \end{bmatrix}
=
-\det\begin{bmatrix} 1 & 1 & 1 \\ 4 & 5 & 6 \\ 1 & 2 & 3 \end{bmatrix}。
$$

$$
\det\begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \\ 1 & 1 & 1 \end{bmatrix}
=
\frac{1}{10}\det\begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \\ 10 & 10 & 10 \end{bmatrix}。
$$

$$
\det\begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \\ 1 & 1 & 1 \end{bmatrix}
=
\det\begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \\ 1+10 & 1+20 & 1+30 \end{bmatrix}
=
\det\begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \\ 11 & 21 & 31 \end{bmatrix}。
$$

$$
\det\begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix}=-2；\quad
\det\begin{bmatrix} 10 & 20 \\ 30 & 40 \end{bmatrix}=-200。
$$

> **Note**
>
> 考慮 $n$ 階方陣 $A$，上述性質的一般化所表達的就是：
>
> (1) $\det(r_{ij}(A))=-\det(A)$；$\det(r_i^{(k)}(A))=k\det(A)$，$k\neq 0$；$\det(r_{ij}^{(k)}(A))=\det(A)$。
>
> （同理 $\det(c_{ij}(A))=-\det(A)$；$\det(c_i^{(k)}(A))=k\det(A)$，$k\neq 0$；$\det(c_{ij}^{(k)}(A))=\det(A)$。）
>
> (2) $\det(R_{ij})=-1$，$\det(R_i^{(k)})=k$，$k\neq 0$，$\det(R_{ij}^{(k)})=1$。
>
> （同理 $\det(C_{ij})=-1$，$\det(C_i^{(k)})=k$，$k\neq 0$，$\det(C_{ij}^{(k)})=1$。）
>
> (3) 設 $P$ 為列基本矩陣，$Q$ 為行基本矩陣，則
>
> $$
> \det(PA)=\det(P)\det(A)
> $$
>
> $$
> \det(AQ)=\det(A)\det(Q)
> $$