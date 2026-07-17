## 526 線性代數(上)

**5.** (18%) Let $T$ be the linear operator on $R^2$ defined by $T(a,b,c) = (3a+c, -2a+b, -a+2b+4c)$.

(1) What is the matrix of $T$ in the standard ordered basis for $R^2$?

(2) What is the matrix of $T$ in the ordered basis $\{v_1 = (1,0,1),\ v_2 = (-1,2,1),\ v_3 = (2,1,1)\}$?

(3) Give a rule for $T^{-1}$ like the one which defines $T$. 【99 交大統計所、101 中正統計】

> **例**
>
> (1) 方法一：$\ker(L) = \ker(A)$，行標準形矩陣：
>
> $$\begin{bmatrix} 3 & 0 & 1 \\ -2 & 1 & 0 \\ -1 & 2 & 4 \end{bmatrix} \rightarrow \begin{bmatrix} 17 & 35 & 22 \\ -3 & 15 & -6 \\ 0 & -2 & -14 & 0 \end{bmatrix}$$
>
> (3) $T^{-1}(x_1, x_2, x_3) = \frac{1}{4}(4x_1 + 2x_2 - x_3,\ 8x_1 + 13x_2 - 2x_3,\ -3x_3 - 6x_2 + 3x_3)$

**6.** (15%) Find linear transformations $U,\ T: R^2 \to R^2$ such that $UT = T_0$ (the zero transformation) but $TU \neq T_0$. 【110 成大應數】

> **例** 例如取
>
> $$T\begin{pmatrix}x\\y\end{pmatrix} = \begin{bmatrix}1 & 0\\0 & 0\end{bmatrix}\begin{pmatrix}x\\y\end{pmatrix},\quad U\begin{pmatrix}x\\y\end{pmatrix} = \begin{bmatrix}0 & 0\\1 & 0\end{bmatrix}\begin{pmatrix}x\\y\end{pmatrix}$$
>
> $$(UT)\begin{pmatrix}x\\y\end{pmatrix} = \begin{bmatrix}0 & 0\\1 & 0\end{bmatrix}\begin{bmatrix}1 & 0\\0 & 0\end{bmatrix}\begin{pmatrix}x\\y\end{pmatrix} = \begin{bmatrix}0 & 0\\0 & 0\end{bmatrix}\begin{pmatrix}x\\y\end{pmatrix} = T_0\begin{pmatrix}x\\y\end{pmatrix}$$
>
> $$(TU)\begin{pmatrix}x\\y\end{pmatrix} = \begin{bmatrix}1 & 0\\0 & 0\end{bmatrix}\begin{bmatrix}0 & 0\\1 & 0\end{bmatrix}\begin{pmatrix}x\\y\end{pmatrix} \neq T_0\begin{pmatrix}x\\y\end{pmatrix}$$
