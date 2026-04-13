# 第二章 線性方程組與求解 150

## 線性代數（上）

> **例題 6**
>
> True or false: let $A$ be an $m \times n$ matrix and $b$ be a vector in $R^m$.
>
> (1) Let $m > n$ and $\text{rank}(A) = n$, then $Ax = b$ is consistent for any $b$. 【103 台科資工】
>
> (2) If $Ax = b$ has a unique solution, then $m \geq n$. 【106 台大電信】
>
> (3) If $Ax = b$ is consistent for every $b$, then $A$ has pivot column. 【106 中山通訊】
>
> (4) If $A$ has a pivot positions in every row, then $Ax = b$ has a unique solution for each $b$. 【105 中山通訊】

**解**

(1) False. 因為 $m > n$ 且 $\text{rank}(A)=n<m$，故 $A$ 不可能每一列都有 pivot，無法任意 $b$ 均使 $Ax=b$ 都有解。

(2) False. 可取反例為
$$
A=\begin{bmatrix}
1 & 0 \\
0 & 1 \\
1 & 1
\end{bmatrix},\quad
b=\begin{bmatrix}
2 \\
3 \\
5
\end{bmatrix}。
$$

(3) True.

(4) False. 可取反例為
$$
A=\begin{bmatrix}
1 & 0 & 0 \\
0 & 1 & 0
\end{bmatrix},\quad
b=\begin{bmatrix}
1 \\
1
\end{bmatrix}，
$$
有多解：
$$
\begin{bmatrix}
1 \\
1 \\
0
\end{bmatrix},
\begin{bmatrix}
1 \\
1 \\
1
\end{bmatrix}
\ldots
$$

> **例題 7**
>
> True or false:
>
> (1) (5%) If $\text{rank}(A) < n$, then $Ax = b$ has infinitely many solutions for any $b \in R^m$.
>
> 【101 台科資工】
>
> (2) Let $A$ be a nonsingular $n \times n$ matrix. Then for any $b$, $Ax = b$ has a unique solution.
>
> 【101 政大統計】
>
> (3) Let
> $$
 A=\begin{bmatrix}
 1 & 3 & 4 \\
 -4 & 2 & -6 \\
 -3 & -2 & -7
 \end{bmatrix}
 $$
> and
> $$
 b=\begin{bmatrix}
 b_1 \\
 b_2 \\
 b_3
 \end{bmatrix}。
 $$
> Is $Ax = b$ consistent for all possible $b_1, b_2, b_3$?

**解**

(1) False. 反例可取
$$
\begin{bmatrix}
1 & 1 \\
0 & 0
\end{bmatrix}
\begin{bmatrix}
x_1 \\
x_2
\end{bmatrix}
=
\begin{bmatrix}
1 \\
1
\end{bmatrix}，
$$
無解。

(2) True. 此時 $A$ 可逆。有唯一解 $x=A^{-1}b$。

(3) False.
$$
\because\ A \sim \begin{bmatrix}
1 & 3 & 4 \\
0 & 5 & 0 \\
0 & 0 & 0
\end{bmatrix}，\quad \therefore\ \text{rank}(A)=2。
$$