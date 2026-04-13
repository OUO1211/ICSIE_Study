# 第一章 矩陣 88

## 線性代數（上）

> **例題**
>
> (10%) Let $A = \begin{bmatrix} 2 & 1 & 1 \\ 6 & 4 & 5 \\ 4 & 1 & 3 \end{bmatrix}$.
>
> (1) Find elementary matrices $F_1, F_2$ and $F_3$ such that $F_3 F_2 F_1 A = U$, where $U$ is an upper triangular matrix.
>
> (2) Determine the inverses of $F_1, F_2$ and $F_3$ and set $L = F_1^{-1} F_2^{-1} F_3^{-1}$. What type of matrix is $L$? Verify that $A = LU$.
>
> 【97-98 政大統計‧97 中興資料‧107 中興統計類題‧109 交大資工】

**解**

$A = \begin{bmatrix} 2 & 1 & 1 \\ 6 & 4 & 5 \\ 4 & 1 & 3 \end{bmatrix} \xrightarrow{r_{12}^{(-3)},\ r_{13}^{(-2)}} \begin{bmatrix} 2 & 1 & 1 \\ 0 & 1 & 2 \\ 0 & -1 & 1 \end{bmatrix} \xrightarrow{r_{23}^{(1)}} \begin{bmatrix} 2 & 1 & 1 \\ 0 & 1 & 2 \\ 0 & 0 & 3 \end{bmatrix} = U$，故 $R_{23}^{(1)} R_{13}^{(-2)} R_{12}^{(-3)} A = U$。

> (1) 取 $F_1 = R_{12}^{(-3)} = \begin{bmatrix} 1 & 0 & 0 \\ -3 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix}$，$F_2 = R_{13}^{(-2)} = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ -2 & 0 & 1 \end{bmatrix}$，$F_3 = R_{23}^{(1)} = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 1 & 1 \end{bmatrix}$。
>
> (2) $(F_1)^{-1} = R_{12}^{(3)} = \begin{bmatrix} 1 & 0 & 0 \\ 3 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix}$，$(F_2)^{-1} = R_{13}^{(2)} = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 2 & 0 & 1 \end{bmatrix}$，$(F_3)^{-1} = R_{23}^{(-1)} = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & -1 & 1 \end{bmatrix}$。
>
> $L = R_{12}^{(3)} R_{13}^{(2)} R_{23}^{(-1)} = \begin{bmatrix} 1 & 0 & 0 \\ 3 & 1 & 0 \\ 2 & -1 & 1 \end{bmatrix}$ 為下三角矩陣，
>
> $$LU = \begin{bmatrix} 1 & 0 & 0 \\ 3 & 1 & 0 \\ 2 & -1 & 1 \end{bmatrix} \begin{bmatrix} 2 & 1 & 1 \\ 0 & 1 & 2 \\ 0 & 0 & 3 \end{bmatrix} = \begin{bmatrix} 2 & 1 & 1 \\ 6 & 4 & 5 \\ 4 & 1 & 3 \end{bmatrix} = A$$