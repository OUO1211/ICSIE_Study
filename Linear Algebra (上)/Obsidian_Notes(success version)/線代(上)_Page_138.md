# 第二章 線性方程組與求解 139

## 2-2 矩陣的秩

本小節先直觀定義 rank，探討線性系統解的個數，並進而得到方陣是否有解的等價條件，第三章會再正式給 rank 的定義。

> **定義：矩陣的秩 (rank)**
>
> 考慮矩陣 $A$，
>
> 將 $A$ 列運算成為列梯陣（或簡化列梯陣），若剩下 $k$ 個非零列，則稱 $A$ 的秩為 $k$，記作 $\text{rank}(A) = k$。

> **Note**
>
> $\text{rank}(A) \leq n$，$\text{rank}(A) \leq m$ 恆成立。

例如：

$$A = \begin{bmatrix} 1 & 1 & 1 \\ 1 & 1 & 2 \end{bmatrix} \xrightarrow{r_2^{(-1)}} \begin{bmatrix} 1 & 1 & 1 \\ 0 & 0 & 1 \end{bmatrix}$$

$\therefore \text{rank}(A) = 2$；

$$B = \begin{bmatrix} 1 & 0 & -2 & 3 \\ 2 & 2 & 0 & 4 \\ 2 & 0 & -4 & 6 \\ 1 & 1 & 1 & 1 \end{bmatrix} \xrightarrow{r_2^{(-2)}, r_3^{(-2)}, r_4^{(-1)}} \begin{bmatrix} 1 & 0 & -2 & 3 \\ 0 & 2 & 4 & -2 \\ 0 & 0 & 0 & 0 \\ 0 & 1 & 3 & -2 \end{bmatrix} \xrightarrow{r_{24}} \cdots \xrightarrow{r_{34}^{(-1/2)}} \begin{bmatrix} 1 & 0 & -2 & 3 \\ 0 & 2 & 4 & -2 \\ 0 & 0 & 1 & -1 \\ 0 & 0 & 0 & 0 \end{bmatrix}$$

$$\xrightarrow{r_3^{(0.5)}} \begin{bmatrix} 1 & 0 & -2 & 3 \\ 0 & 1 & 2 & -1 \\ 0 & 0 & 1 & -1 \\ 0 & 0 & 0 & 0 \end{bmatrix}$$

$\therefore \text{rank}(B) = 3$。
