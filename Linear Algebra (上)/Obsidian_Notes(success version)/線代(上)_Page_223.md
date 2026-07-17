> **例 15**
>
> (10%) Solve for $t$ if $\det\begin{bmatrix} 3-t & 2 & 0 & 0 & 0 \\ 1 & 4-t & 0 & 0 & 0 \\ 0 & 0 & 3-t & 1 & 0 \\ 0 & 0 & 1 & 3-t & 0 \\ 0 & 0 & 0 & 0 & 4-t \end{bmatrix} = 0$.
>
> 【110 台大資工】

**解**

$$0 = \begin{vmatrix} 3-t & 2 & 0 & 0 & 0 \\ 1 & 4-t & 0 & 0 & 0 \\ 0 & 0 & 3-t & 1 & 0 \\ 0 & 0 & 1 & 3-t & 0 \\ 0 & 0 & 0 & 0 & 4-t \end{vmatrix} = \begin{vmatrix} 3-t & 2 \\ 1 & 4-t \end{vmatrix} \cdot \begin{vmatrix} 3-t & 1 \\ 1 & 3-t \end{vmatrix} \cdot (4-t)$$

$$= (t-2)(t-5)(t-2)(t-4)(4-t),$$

$$\therefore t = 2, 4, 5.$$