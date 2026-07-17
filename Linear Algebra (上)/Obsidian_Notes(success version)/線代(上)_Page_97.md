$$
= \underbrace{\begin{bmatrix}
0 & 0 & 1 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 0 & 1 \\
1 & 0 & 0 & 0
\end{bmatrix}}_{P}
\underbrace{\begin{bmatrix}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & -1 & 1 & 0 \\
-1 & 0 & 2 & 1
\end{bmatrix}}_{L}
\underbrace{\begin{bmatrix}
1 & 0 & 0 & 1 \\
0 & 0 & 1 & -1 \\
0 & 0 & 0 & 1 \\
0 & 0 & 0 & 0
\end{bmatrix}}_{U}
$$

> **例題**
>
> (8%) Find the factorization $PA = LDU$ for $A = \begin{bmatrix} 1 & 1 & 1 \\ 5 & 5 & 8 \\ 3 & 4 & 10 \end{bmatrix}$.
>
> 【108 中山通訊】

**解**

$$
P = \begin{bmatrix}
1 & 0 & 0 \\
0 & 0 & 1 \\
0 & 1 & 0
\end{bmatrix}, \quad
L = \begin{bmatrix}
1 & 0 & 0 \\
3 & 1 & 0 \\
5 & 0 & 1
\end{bmatrix}, \quad
D = \begin{bmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 3
\end{bmatrix}, \quad
U = \begin{bmatrix}
1 & 1 & 1 \\
0 & 1 & 7 \\
0 & 0 & 1
\end{bmatrix}
$$