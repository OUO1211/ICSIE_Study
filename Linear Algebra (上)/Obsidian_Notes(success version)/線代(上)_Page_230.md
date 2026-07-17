$cof(a_{31}) = (-1)^{3+1}\begin{vmatrix} 4 & 3 \\ -2 & 0 \end{vmatrix} = 6$；$cof(a_{32}) = (-1)^{3+2}\begin{vmatrix} 1 & 3 \\ -1 & 0 \end{vmatrix} = -3$；

$cof(a_{33}) = (-1)^{3+3}\begin{vmatrix} 1 & 4 \\ -1 & -2 \end{vmatrix} = 2$；$\therefore A^{-1} = \dfrac{1}{12}\begin{bmatrix} -6 & -6 & 6 \\ 3 & -3 & -3 \\ 2 & 6 & 2 \end{bmatrix}$

---

> **例題 3**
>
> Let $A$ be the $4 \times 4$ matrix, if $adj(A) = \begin{bmatrix} 2 & 0 & 0 & 0 \\ 0 & 2 & 1 & 0 \\ 0 & 4 & 3 & 2 \\ 0 & -2 & -1 & 2 \end{bmatrix}$, find $A$.
>
> 【94,96 彰師資工】

**解** $\because A \cdot adj(A) = \det(A) \cdot I_4$，

故 $\det(A)\det(adj(A)) = \det(A)^4$，

得 $\det(adj(A)) = \det(A)^3$。

由題目得

$$
\det\begin{bmatrix}
2 & 0 & 0 & 0 \\
0 & 2 & 1 & 0 \\
0 & 4 & 3 & 2 \\
0 & -2 & -1 & 2
\end{bmatrix}
= 2 \cdot \begin{vmatrix}
2 & 1 & 0 \\
4 & 3 & 2 \\
-2 & -1 & 2
\end{vmatrix}
= 2 \cdot 2 \cdot \begin{vmatrix}
2 & 1 \\
4 & 3
\end{vmatrix}
= 8
$$

$\therefore \det(A) = \sqrt[3]{8} = 2$。

故 $A$ 可逆，且 $adj(A)$ 可逆，又：$A \cdot adj(A) = \det(A) \cdot I_4$，

故 $A = \det(A) \cdot I_4 \cdot (adj(A))^{-1}$。

先求得 $(adj(A))^{-1} = \begin{bmatrix} \dfrac{1}{2} & 0 & 0 & 0 \\ 0 & 2 & -1 & 1 \\ 0 & -\dfrac{3}{2} & 1 & -\dfrac{1}{2} \\ 0 & \dfrac{1}{2} & 0 & \dfrac{1}{2} \end{bmatrix}$，而後得 $A = \begin{bmatrix} 1 & 0 & 0 & 0 \\ 0 & 4 & -1 & 1 \\ 0 & -6 & 2 & -2 \\ 0 & 1 & 0 & 1 \end{bmatrix}$