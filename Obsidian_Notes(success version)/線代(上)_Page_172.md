> **例 1**
>
> Find determinant.
>
> (1) $A=\begin{bmatrix}2&1&3&4\\1&5&2&0\\1&0&0&3\\2&0&0&1\end{bmatrix}$（挑 0 較多的列/行）【107 中興統計】
>
> (2) $B=\begin{bmatrix}0&1&0&4&0&-2\\37&20&7&2&1&4\\0&1&0&1&0&0\\0&1&-10&-1&0&-2\\2&-5&-94&0&0&4\\0&-1&0&0&0&0\end{bmatrix}$
>
> (3) $C=\begin{bmatrix}7&1&23&0&0&1\\1&2&101&-5&-2&0\\3&-4&0&1&0&0\\3&9&2&0&0&0\\7&6&0&0&0&0\\1&0&0&0&0&0\end{bmatrix}$【109 台師電機】

**解**

(1)
$$
\det(A)=2\cdot(-1)^{4+1}\begin{vmatrix}1&3&4\\5&2&0\\0&0&3\end{vmatrix}+1\cdot(-1)^{4+4}\begin{vmatrix}2&1&3\\1&5&2\\1&0&0\end{vmatrix}
$$
$$
=-2\cdot3\cdot(-1)^{3+3}\begin{vmatrix}1&3\\5&2\end{vmatrix}+1\cdot(-1)^{3+1}\begin{vmatrix}1&3\\5&2\end{vmatrix}
$$
$$
=78-13=65
$$

(2)
$$
\det(B)=1\cdot(-1)^{2+5}\begin{vmatrix}0&1&0&4&-2\\0&1&0&1&0\\0&1&-10&-1&-2\\2&-5&-94&0&4\\0&-1&0&0&0\end{vmatrix}
$$
$$
=(-1)\cdot2\cdot(-1)^{4+1}\begin{vmatrix}1&0&4&-2\\1&0&1&0\\1&-10&-1&-2\\-1&0&0&0\end{vmatrix}
$$
$$
=2\begin{vmatrix}0&4&-2\\0&1&0\\-10&-1&-2\end{vmatrix}-20\cdot(-1)^{3+1}\begin{vmatrix}4&-2\\1&0\end{vmatrix}=-40
$$

(3)
$$
\det(C)=24
$$