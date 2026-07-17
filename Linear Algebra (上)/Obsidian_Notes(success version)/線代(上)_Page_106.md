# 第一章 矩陣 105

> **試題 12**
>
> (20%) Let $J$ be the $n \times n$ matrix each of whose entries is 1.
>
> (1) Find $(I + aJ)^{-1}$ for the real number $a$ for which the inverse exists.
>
> (2) Show that $(I + aJ)^{-1}$ is of the form $(I + bJ)$, and find $b$.
>
> 【87 政大統計‧91 成大統計計題‧98 交大統計】

**解**

(1) $I-\dfrac{a}{1+na}J$  (2) $b=\dfrac{-a}{1+na}$

令 $x=\begin{bmatrix}a&\cdots&a\end{bmatrix}^T，\ y=\begin{bmatrix}1&\cdots&1\end{bmatrix}^T，\ M=I+xy^T$。

$$
\because\ M^2=(I+xy^T)^2=I+2xy^T+xy^Tyx^T=I+2xy^T+(y^Tx)xy^T
$$

$$
=I+(2+na)xy^T=(2+na)(I+xy^T)-(1+na)I。
$$

即得 $M^2=(2+na)M-(1+na)I$，

$$
\therefore\ I=\frac{1}{1+na}\left[(2+na)I-M\right]M。
$$

$$
\therefore\ M^{-1}=\frac{1}{1+na}\left[(2+na)I-M\right]
=\frac{1}{1+na}\left[(1+na)I-xy^T\right]
=I-\frac{a}{1+na}J。
$$

> **試題 13**
>
> The following is the pseudo code for $LU$ Decomposition.
>
> ```
> for i = 1,2,3,...,n
>     L_{i1} = A_{i1}
> for j = 1,...,n
>     U_{1j} = A_{1j} / L_{11}
> for j = 2,3,...,n-1
> {
>     for i = j, j+1,...,n
>         L_{ij} = A_{ij} - \sum_{k=1}^{j-1} L_{ik} U_{kj}
>     for k = j, j+1,...,n
>         U_{jk} = \left( A_{jk} - \sum_{i=1}^{j-1} L_{ji} U_{ik} \right) / L_{jj}
> }
> ```