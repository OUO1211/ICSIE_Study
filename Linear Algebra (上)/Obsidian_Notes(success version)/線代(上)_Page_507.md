> **試題 11**
>
> (10%) Let $A = \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix}$, $B = \begin{bmatrix} 5 & 6 \\ 7 & 8 \end{bmatrix}$. Find the trace of the linear operator $X \mapsto AXB$ on $R^{2\times 2}$.
>
> 【110 成大應數】

> **解**
>
> 令線性映射 $T: X \mapsto AXB$
>
> 取標準基底 $\beta = \left\{\begin{bmatrix} 1 & 0 \\ 0 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 1 \\ 0 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 0 \\ 1 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 0 \\ 0 & 1 \end{bmatrix}\right\}$
>
> $T\begin{bmatrix} 1 & 0 \\ 0 & 0 \end{bmatrix} = A\begin{bmatrix} 1 & 0 \\ 0 & 0 \end{bmatrix}B = \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix}\begin{bmatrix} 1 & 0 \\ 0 & 0 \end{bmatrix}\begin{bmatrix} 5 & 6 \\ 7 & 8 \end{bmatrix} = \begin{bmatrix} 5 & 6 \\ 15 & 18 \end{bmatrix}$
>
> $T\begin{bmatrix} 0 & 1 \\ 0 & 0 \end{bmatrix} = \begin{bmatrix} 7 & 8 \\ 21 & 24 \end{bmatrix}$
>
> $T\begin{bmatrix} 0 & 0 \\ 1 & 0 \end{bmatrix} = \begin{bmatrix} 10 & 12 \\ 20 & 24 \end{bmatrix}$
>
> $T\begin{bmatrix} 0 & 0 \\ 0 & 1 \end{bmatrix} = \begin{bmatrix} 14 & 16 \\ 28 & 32 \end{bmatrix}$
>
> $$\therefore [T]_\beta = \begin{bmatrix} 5 & 7 & 10 & 14 \\ 6 & 8 & 12 & 16 \\ 15 & 21 & 20 & 28 \\ 18 & 24 & 24 & 32 \end{bmatrix}$$
>
> $\therefore \mathrm{trace}(T) = 5 + 8 + 20 + 32 = 65$