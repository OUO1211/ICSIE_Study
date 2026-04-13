$$r_{12}(A) = \begin{bmatrix} 2 & 4 & 6 \\ 1 & 3 & 5 \end{bmatrix} \xrightarrow{r} \begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix} \begin{bmatrix} 1 & 3 & 5 \\ 2 & 4 & 6 \end{bmatrix} = R_{12} A$$

$$r_1^{(-2)}(A) = \begin{bmatrix} 1 & 3 & 5 \\ -4 & -8 & -12 \end{bmatrix} = \begin{bmatrix} 1 & 0 \\ 0 & -2 \end{bmatrix} \begin{bmatrix} 1 & 3 & 5 \\ 2 & 4 & 6 \end{bmatrix} = R_1^{(-2)} A$$

$$r_{12}^{(-2)}(A) = \begin{bmatrix} 1 & 3 & 5 \\ 0 & -2 & -4 \end{bmatrix} = \begin{bmatrix} 1 & 0 \\ -2 & 1 \end{bmatrix} \begin{bmatrix} 1 & 3 & 5 \\ 2 & 4 & 6 \end{bmatrix} = R_{12}^{(-2)} A$$

> **例題 1**
>
> (15%) Let $A = \begin{bmatrix} 1 & 2 & -1 & 0 \\ 0 & 0 & 1 & -3 \\ 2 & 4 & -1 & -2 \end{bmatrix}$ and $B = \begin{bmatrix} 1 & 2 & 0 & 0 \\ 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & 1 \end{bmatrix}$. It is known that $B$ is the reduced echelon form of $A$. Find a matrix $E$ such that $EA = B$.
>
> 〔99 師大資工頻道、108 中山應數〕
>
> **解：**
>
> $$\begin{bmatrix} 1 & 2 & -1 & 0 \\ 0 & 0 & 1 & -3 \\ 2 & 4 & -1 & -2 \end{bmatrix} \xrightarrow{r_{31}^{(-2)}} \begin{bmatrix} 1 & 2 & -1 & 0 \\ 0 & 0 & 1 & -3 \\ 0 & 0 & 1 & -2 \end{bmatrix} \xrightarrow{r_{23}^{(-1)}} \begin{bmatrix} 1 & 2 & -1 & 0 \\ 0 & 0 & 1 & -3 \\ 0 & 0 & 0 & 1 \end{bmatrix}$$
>
> $$\xrightarrow{r_{32}^{(3)}} \begin{bmatrix} 1 & 2 & -1 & 0 \\ 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & 1 \end{bmatrix} \xrightarrow{r_{21}^{(1)}} \begin{bmatrix} 1 & 2 & 0 & 0 \\ 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & 1 \end{bmatrix} = B$$
>
> $\therefore R_{21}^{(1)} R_{32}^{(3)} R_{23}^{(-1)} R_{31}^{(-2)} A = B$，即 $E$
>
> $$E = \begin{bmatrix} 1 & 1 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix} \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 3 \\ 0 & 0 & 1 \end{bmatrix} \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & -1 & 1 \end{bmatrix} \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ -2 & 0 & 1 \end{bmatrix} = \begin{bmatrix} -5 & -2 & 3 \\ -6 & -2 & 3 \\ -2 & -1 & 1 \end{bmatrix}$$
