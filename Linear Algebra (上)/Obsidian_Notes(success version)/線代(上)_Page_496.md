> **試題 9**
>
> (12%) Let $B_1 = \{(1,1), (1,-1)\}$ and $B_2 = \{(1,1,0), (0,1,1), (1,0,1)\}$ be bases of $R^2$ and $R^3$ respectively, and $A = \begin{bmatrix} 2 & 1 \\ -1 & 3 \\ 1 & 1 \end{bmatrix}$ be the matrix of a linear transformation $T: R^2 \to R^3$ with respect to $B_1$ and $B_2$. Find the matrix of $T$ with respect to the standard bases of $R^2$ and $R^3$.
>
> 【104 台科資工】

> **解**
>
> 令 $\beta_1 = \{(1,0), (0,1)\}$，則 $B_1$ 到 $\beta_1$ 的座標變換矩陣 $[I_{B_1}]_{\beta_1}^{B_1} = \begin{bmatrix} 1 & 1 \\ 1 & -1 \end{bmatrix}$。
>
> 令 $\beta_2 = \{(1,0,0), (0,1,0), (0,0,1)\}$，則 $\beta_2$ 到 $B_2$ 的座標變換矩陣 $[I_{B_2}]_{\beta_2}^{B_2} = \begin{bmatrix} 1 & 0 & 1 \\ 1 & 1 & 0 \\ 0 & 1 & 1 \end{bmatrix}$。
>
> $$\therefore [T]_{\beta_1}^{\beta_2} = [I_{B_2}]_{\beta_2}^{B_2} [T]_{B_1}^{B_2} ([I_{B_1}]_{\beta_1}^{B_1})^{-1}$$
>
> $$= [I_{B_2}]_{\beta_2}^{B_2} [T]_{B_1}^{B_2} [I_{\beta_1}]_{B_1}^{\beta_1}$$
>
> $$= \begin{bmatrix} 1 & 0 & 1 \\ 1 & 1 & 0 \\ 0 & 1 & 1 \end{bmatrix} \begin{bmatrix} 2 & 1 \\ -1 & 3 \\ 1 & 1 \end{bmatrix} \begin{bmatrix} 1 & 1 \\ 1 & -1 \end{bmatrix}^{-1} = \frac{1}{2}\begin{bmatrix} 5 & 1 \\ 5 & -3 \\ 4 & -4 \end{bmatrix}$$
