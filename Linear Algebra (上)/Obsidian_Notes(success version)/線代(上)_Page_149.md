# 第二章 線性方程組與求解 149

> **例題 4**
>
> Let $A$ be a $7 \times 5$ matrix with $\operatorname{rank}(A) = 5$.
>
> (1) For any $b \in R^7$, $Ax = b$ has infinite number of solution.
>
> (2) For any $b \in R^7$, $Ax = b$ has a unique solution.
>
> 【110 文大資工】

**解**

(1) False. 反例可取
$$
A=\begin{bmatrix}
1 & 0 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 & 0 \\
0 & 0 & 1 & 0 & 0 \\
0 & 0 & 0 & 1 & 0 \\
0 & 0 & 0 & 0 & 1 \\
0 & 0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 & 0
\end{bmatrix},
\quad
Ax=\begin{bmatrix}
1 \\
1 \\
1 \\
1 \\
1 \\
2 \\
3
\end{bmatrix}
$$
無解。

(2) False. 反例同 (1)。

> **例題 5**
>
> Consider the linear equation $Ax = b$ with $A \in R^{m \times n}$. Which of the following statements are true?
>
> (1) If $\operatorname{rank}(A) = m$, then there exists at least one solution.
>
> (2) If $\operatorname{rank}(A) = n$, then there exists exactly one solution.
>
> (3) If $\operatorname{rank}(A) = n$, then the column vectors of $A$ are linearly independent.
>
> (4) If $n > m$, then there exists at least one solution.
>
> (5) If $m > n$, then there exists at most one solution.
>
> 【94 台大資工】
>
> 【109 中山電機】

**解**

True. (1), (3).

(2) False. 可取反例：
$$
A=\begin{bmatrix}
1 & 0 \\
0 & 1 \\
0 & 0
\end{bmatrix}
$$
，1 行獨立，但
$$
Ax=\begin{bmatrix}
2 \\
3 \\
4
\end{bmatrix}
$$
無解。

(4) False. 可取反例：
$$
A=\begin{bmatrix}
1 & 0 & 0 \\
0 & 0 & 0
\end{bmatrix}
$$
，但
$$
Ax=\begin{bmatrix}
1 \\
1
\end{bmatrix}
$$
無解。

(5) False. 可取反例：
$$
A=\begin{bmatrix}
1 & 0 \\
0 & 0 \\
0 & 0
\end{bmatrix}
$$
，但
$$
Ax=\begin{bmatrix}
1 \\
0 \\
0
\end{bmatrix}
$$
無限多解。