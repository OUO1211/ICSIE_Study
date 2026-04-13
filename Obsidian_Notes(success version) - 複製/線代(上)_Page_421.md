> **例題 3**
>
> Let $B=\begin{bmatrix} -1 & 2 \\ 2 & -2 \end{bmatrix}$, $C=\begin{bmatrix} -3 & 4 \\ 2 & -2 \end{bmatrix}$ be two ordered bases for $R^2$.
>
> (1) (10%) Find the transition matrix from $C$ to $B$ (i.e., Find a matrix $A$ such that $A[v]_C=[v]_B$ for all $v\in R^2$).
>
> (2) (4%) Let $[v]_C=\begin{bmatrix} 1 \\ -1 \end{bmatrix}$, find $[v]_B$ and $v$.
>
> 【96,98,99 師大資工、93 成大資工、99,103 台科工概、105 海洋資工】

解：

(1)
$$
-1\begin{bmatrix} -1 \\ 2 \end{bmatrix}-2\begin{bmatrix} 2 \\ -2 \end{bmatrix}=\begin{bmatrix} -3 \\ 2 \end{bmatrix}
$$

$$
2\begin{bmatrix} -1 \\ 2 \end{bmatrix}+3\begin{bmatrix} 2 \\ -2 \end{bmatrix}=\begin{bmatrix} 4 \\ -2 \end{bmatrix}
$$

故所求為
$$
A=\begin{bmatrix} -1 & 2 \\ -2 & 3 \end{bmatrix}
$$

(2)
$$
[v]_B=\begin{bmatrix} -1 & 2 \\ -2 & 3 \end{bmatrix}\begin{bmatrix} 1 \\ -1 \end{bmatrix}=\begin{bmatrix} -3 \\ -5 \end{bmatrix}
$$

$$
v=-3\begin{bmatrix} -1 \\ 2 \end{bmatrix}-5\begin{bmatrix} 2 \\ -2 \end{bmatrix}=\begin{bmatrix} -7 \\ 4 \end{bmatrix}
$$

> **例題 4**
>
> (15%) Let $B_1=\{(1,0,1),(1,1,1),(-1,0,0)\}$ and $B_2=\{(0,3,-2),(-1,10,-7),(1,-8,6)\}$ be two bases of $R^3$. What is the matrix that converts $B_1$-coordinates to $B_2$-coordinates in $R^3$?
>
> 【105 台科資工】

解：

$$
\left[
\begin{array}{ccc|ccc}
0 & -1 & 1 & 1 & 1 & -1 \\
3 & 10 & -8 & 0 & 1 & 0 \\
-2 & -7 & 6 & 1 & 1 & 0
\end{array}
\right]
\xrightarrow{\text{列運算}}
\left[
\begin{array}{ccc|ccc}
1 & 0 & 0 & 2 & 1 & -4 \\
0 & 1 & 0 & 1 & 3 & 2 \\
0 & 0 & 1 & 2 & 4 & 1
\end{array}
\right]
$$

$$
\therefore P_{B_1\to B_2}=\begin{bmatrix}
2 & 1 & -4 \\
1 & 3 & 2 \\
2 & 4 & 1
\end{bmatrix}
$$