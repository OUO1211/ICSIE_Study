# 第二章 線性方程組與求解 131

> **例題 5**
>
> 設 $A = \begin{bmatrix} 2 & -1 & 0 \\ -1 & 2 & -1 \\ 0 & -1 & 2 \end{bmatrix}$，$b = \begin{bmatrix} 6 \\ 0 \\ -6 \end{bmatrix}$。
>
> (1) 試求出下三角矩陣 $L$、上三角矩陣 $U$、及對角矩陣 $D$，使得 $A = LDU$。
>
> (2) 求 $x$ 使得 $Ax = b$。

**解**

$$A = \begin{bmatrix} 1 & 0 & 0 \\ -1/2 & 1 & 0 \\ 0 & -2/3 & 1 \end{bmatrix} \begin{bmatrix} 2 & 0 & 0 \\ 0 & 3/2 & 0 \\ 0 & 0 & 4/3 \end{bmatrix} \begin{bmatrix} 1 & -1/2 & 0 \\ 0 & 1 & -2/3 \\ 0 & 0 & 1 \end{bmatrix}$$

$$Ax = b \Rightarrow LDUx = b$$，令 $Ux = y$，$Dy = z$，則 $Lz = b$。

由 $\begin{bmatrix} 1 & 0 & 0 \\ -1/2 & 1 & 0 \\ 0 & -2/3 & 1 \end{bmatrix} \begin{bmatrix} z_1 \\ z_2 \\ z_3 \end{bmatrix} = \begin{bmatrix} 6 \\ 0 \\ -6 \end{bmatrix}$，解得 $z = \begin{bmatrix} 6 \\ 3 \\ -4 \end{bmatrix}$。

再由 $\begin{bmatrix} 2 & 0 & 0 \\ 0 & 3/2 & 0 \\ 0 & 0 & 4/3 \end{bmatrix} \begin{bmatrix} y_1 \\ y_2 \\ y_3 \end{bmatrix} = \begin{bmatrix} 6 \\ 3 \\ -4 \end{bmatrix}$，得 $y = \begin{bmatrix} 3 \\ 2 \\ -3 \end{bmatrix}$。

最後由 $\begin{bmatrix} 1 & -1/2 & 0 \\ 0 & 1 & -2/3 \\ 0 & 0 & 1 \end{bmatrix} \begin{bmatrix} x_1 \\ x_2 \\ x_3 \end{bmatrix} = \begin{bmatrix} 3 \\ 2 \\ -3 \end{bmatrix}$，解得 $x = \begin{bmatrix} 0 \\ 0 \\ -3 \end{bmatrix}$。
