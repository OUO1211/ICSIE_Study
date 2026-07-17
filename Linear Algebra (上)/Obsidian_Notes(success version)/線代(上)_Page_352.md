> **例題 16**
>
> Given a matrix $A = \begin{bmatrix} 2 & 3 & 1 & 5 \\ 2 & 1 & 0 & 4 \\ 0 & 0 & 1 & 1 \end{bmatrix}$，which of the following statements are TRUE？
>
> (1) $A$ has a column space of dimension 3.
>
> (2) The column space of $A$ is identical to the column space of matrix $\begin{bmatrix} 1 & 1 & 5 \\ 1 & 0 & 4 \\ 0 & 1 & 1 \end{bmatrix}$。
>
> (3) The left nullspace of $A$ is a line in $\mathbb{R}^3$。 【102 交大資工】

**解**

(1) False. 對 $A$ 做行運算可知 $CS(A) = span\left\{ \begin{bmatrix} 1 \\ 1 \\ 0 \end{bmatrix}, \begin{bmatrix} 1 \\ 0 \\ 1 \end{bmatrix} \right\}$，$\dim(CS(A)) = 2$。

(2) True. $CS\left( \begin{bmatrix} 1 & 1 & 5 \\ 1 & 0 & 4 \\ 0 & 1 & 1 \end{bmatrix} \right) = span\left\{ \begin{bmatrix} 1 \\ 1 \\ 0 \end{bmatrix}, \begin{bmatrix} 1 \\ 0 \\ 1 \end{bmatrix} \right\}$。

(3) True. $\dim(\text{left nullspace}(A)) = \dim(N(A^T)) = \dim(CS(A^T)^\perp) = 3 - \dim(CS(A)) = 3 - 2 = 1$。

> **例題 17**
>
> Given the system: $x_1 + 2x_2 - x_3 + x_4 = 0$，$-x_1 - 2x_2 + 3x_3 + 5x_4 = 0$，$-x_1 - 2x_2 - x_3 - 7x_4 = 0$. Which vectors form a basis for the solutions to the system？
>
> (1) $\begin{bmatrix} -2 \\ 1 \\ 0 \\ 0 \end{bmatrix}$ (2) $\begin{bmatrix} -1 \\ -2 \\ -1 \\ -7 \end{bmatrix}$ (3) $\begin{bmatrix} 1 \\ 2 \\ -1 \\ 1 \end{bmatrix}$ (4) $\begin{bmatrix} -1 \\ -2 \\ 3 \\ 5 \end{bmatrix}$ (5) $\begin{bmatrix} -4 \\ 0 \\ -3 \\ 1 \end{bmatrix}$
>
> 【100 彰師統計類題，107 中央資工】

**解** (1), (5).

考慮其係數矩陣 $\begin{bmatrix} 1 & 2 & -1 & 1 \\ -1 & -2 & 3 & 5 \\ -1 & -2 & -1 & -7 \end{bmatrix}$，可列運算成 $\begin{bmatrix} 1 & 2 & 0 & 4 \\ 0 & 0 & 1 & 3 \\ 0 & 0 & 0 & 0 \end{bmatrix}$。