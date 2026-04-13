> **例題 1**
>
> (4%) Let $B = \{3 + 2x + x^2,\,-x + 2x^2,\,1 + x^2\}$. Calculate $[1]_B$.
>
> 【109 台科資工】

解

設 $a(3 + 2x + x^2) + b(-x + 2x^2) + c(1 + x^2) = 1$，

得 $(3a + c) + (2a - b)x + (a + 2b + c)x^2 = 1$，

解
$$
\begin{cases}
3a + c = 1 \\
2a - b = 0 \\
a + 2b + c = 0
\end{cases}
\quad \text{得 } a = -\frac{1}{2},\ b = -1,\ c = \frac{5}{2}
$$

$\therefore [1]_B = \begin{bmatrix} -1/2 \\ -1 \\ 5/2 \end{bmatrix}$

> **例題 2**
>
> (6%) Find the coordinate vector of the matrix $A = \begin{bmatrix} 2 & -1 \\ 4 & 3 \end{bmatrix}$ relative to the ordered basis
>
> $$S = \left\{ \begin{bmatrix} 1 & 1 \\ 0 & -1 \end{bmatrix}, \begin{bmatrix} 0 & 0 \\ 1 & 1 \end{bmatrix}, \begin{bmatrix} 0 & 2 \\ 0 & -1 \end{bmatrix}, \begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix} \right\}.$$
>
> 【104 海洋資工】

解

令
$$
\begin{bmatrix} 2 & -1 \\ 4 & 3 \end{bmatrix}
= c_1 \begin{bmatrix} 1 & 1 \\ 0 & -1 \end{bmatrix}
+ c_2 \begin{bmatrix} 0 & 0 \\ 1 & 1 \end{bmatrix}
+ c_3 \begin{bmatrix} 0 & 2 \\ 0 & -1 \end{bmatrix}
+ c_4 \begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}
$$

$$
\begin{cases}
c_1 + 0c_2 + 0c_3 + 0c_4 = 2 \\
c_1 + 0c_2 + 2c_3 + c_4 = -1 \\
0c_1 + c_2 + 0c_3 + c_4 = 4 \\
-c_1 + c_2 - c_3 + 0c_4 = 3
\end{cases}
\quad \text{得 }
\begin{cases}
c_1 = 2 \\
c_2 = 1 \\
c_3 = -2 \\
c_4 = 1
\end{cases}
$$

即所求為
$$
[A]_S = \begin{bmatrix} 2 \\ 1 \\ -2 \\ 1 \end{bmatrix}.
$$