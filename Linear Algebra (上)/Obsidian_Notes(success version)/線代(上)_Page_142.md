# 第二章 線性方程組與求解 142

## 線性代數（上）

> **例題 1**
>
> (10%) In each part, use the information in the table to determine whether the linear system $Ax = b$ is consistent. If so, state the number of solutions it has.
>
> |  | (1) | (2) | (3) | (4) | (5) |
> |--|-----|-----|-----|-----|-----|
> | Size of $A$ | $3 \times 3$ | $3 \times 3$ | $3 \times 3$ | $5 \times 6$ | $5 \times 6$ |
> | $\mathrm{rank}(A)$ | 3 | 2 | 2 | 5 | 4 |
> | $\mathrm{rank}([A \mid b])$ | 3 | 3 | 2 | 5 | 5 |
>
> 解　(1) 恰一解． (2) 無解． (3) 無限多解． (4) 無限多解． (5) 無解．
>
> 【103 台南資工】

> **例題 2**
>
> (10%) Determine $h$ and $k$ such that the solution set of the system
>
> (i) is empty,
> (ii) contains a unique solution, and
> (iii) contains infinitely many solutions.
>
> (1) $\begin{cases} x_1 + 3x_2 = k \\ 4x_1 + hx_2 = 8 \end{cases} \qquad (2) \begin{cases} -2x_1 + hx_2 = 1 \\ 6x_1 + kx_2 = -2 \end{cases}$
>
> 【107 政大資科】

**解**

(1) $\mathrm{rank}\begin{bmatrix} 1 & 3 \mid k \\ 4 & h \mid 8 \end{bmatrix} = \mathrm{rank}\begin{bmatrix} 1 & 3 & \mid k  \\ 0 & h - 12 & \mid 8 - 4k \end{bmatrix}$

故

(i) $h = 12,\ k \ne 2$ 時，此系統無解．

(ii) $h \ne 12$ 時，此系統恰一解．

(iii) $h = 12,\ k = 2$ 時，此系統無限多解．

(2) $\mathrm{rank}\begin{bmatrix} -2 & h \mid 1 \\ 6 & k \mid -2 \end{bmatrix} = \mathrm{rank}\begin{bmatrix} -2 & h \mid 1 \\ 0 & k + 3h \mid 1 \end{bmatrix}$

故

(i) $k = -3h$ 時，此系統無解．

(ii) $k \ne -3h$ 時，此系統恰一解．

(iii) 此系統不會有無限多解．