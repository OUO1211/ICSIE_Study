> **三角矩陣(triangular matrix)**
>
> 若方陣 $A = [a_{ij}]$ 滿足對角線上或下全為 $0$，則稱之為三角矩陣。又可細分成：
>
> (1) 上三角(upper triangular)矩陣：即當 $i > j$ 時 $a_{ij} = 0$
>
> (2) 下三角(lower triangular)矩陣：即當 $i < j$ 時 $a_{ij} = 0$
>
> (3) 嚴格上三角(strictly upper triangular)矩陣：即當 $i \geq j$ 時 $a_{ij} = 0$
>
> (4) 嚴格下三角(strictly lower triangular)矩陣：即當 $i \leq j$ 時 $a_{ij} = 0$

例如：
$$A = \begin{bmatrix} 1 & 1 & 1 \\ 0 & 1 & 0 \\ 0 & 0 & 2 \end{bmatrix}, \quad B = \begin{bmatrix} 1 & 1 & 0 \\ 0 & 0 & 0 \\ 0 & 0 & 2 \end{bmatrix}, \quad C = \begin{bmatrix} 0 & 1 & 1 \\ 0 & 0 & 0 \\ 0 & 0 & 0 \end{bmatrix}$$

，均為上三角矩陣，其中，$C$ 亦為嚴格上三角

$$D = \begin{bmatrix} 1 & 0 & 0 \\ 1 & 1 & 0 \\ 0 & 0 & 2 \end{bmatrix}, \quad E = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 0 & 0 \\ 0 & 0 & 2 \end{bmatrix}, \quad F = \begin{bmatrix} 0 & 0 & 0 \\ 0 & 0 & 0 \\ 1 & 0 & 0 \end{bmatrix}$$

，均為下三角矩陣，其中，$F$ 亦為嚴格下三角