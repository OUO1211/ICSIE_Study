# 第二章 線性方程組與求解 130

## 解線性系統－用 LU 分解

先將係數矩陣 $A$ 化成 LU 分解，對 $Ax = b$ 或 $LUx = b$：

- Step 1：令 $Ux = y$，解式 $Ly = b$，用前代法。
- Step 2：解 $Ux = y$，用後代法。

> **Note**
>
> 也可以 $LA = LDU$ 分解法求解，此時用方程：

> **例題 4**
>
> (15%) Factor $A$ into $LU$; write down the upper triangular system $Ux = y$ which appears after elimination and solve $x$, for
>
> $$A = \begin{bmatrix} 2 & 3 & 3 \\ 0 & 5 & 7 \\ 6 & 9 & 8 \end{bmatrix}, \quad b = \begin{bmatrix} 2 \\ 2 \\ 5 \end{bmatrix}$$
>
> 【109 台工大資工】

**解**

$$A_{\text{aug}} = \begin{bmatrix} 2 & 3 & 3 \\ 0 & 5 & 7 \\ 6 & 9 & 8 \end{bmatrix} \xrightarrow{r_3^{(-3)}} \begin{bmatrix} 2 & 3 & 3 \\ 0 & 5 & 7 \\ 0 & 0 & -1 \end{bmatrix} = U$$，故 $R_{31}^{(-3)} A = U$。

$$A = [R_{31}^{(-3)}]^{-1} U = R_{31}^{(3)} U = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 3 & 0 & 1 \end{bmatrix} \begin{bmatrix} 2 & 3 & 3 \\ 0 & 5 & 7 \\ 0 & 0 & -1 \end{bmatrix}$$

故 $Ax = b \Rightarrow LUx = b$。

令 $Ux = y$，先解 $Ly = b$：

$$\begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 3 & 0 & 1 \end{bmatrix} \begin{bmatrix} y_1 \\ y_2 \\ y_3 \end{bmatrix} = \begin{bmatrix} 2 \\ 2 \\ 5 \end{bmatrix}$$，解得 $y = \begin{bmatrix} 2 \\ 2 \\ -1 \end{bmatrix}$。

再由 $\begin{bmatrix} 2 & 3 & 3 \\ 0 & 5 & 7 \\ 0 & 0 & -1 \end{bmatrix} \begin{bmatrix} x_1 \\ x_2 \\ x_3 \end{bmatrix} = \begin{bmatrix} 2 \\ 2 \\ -1 \end{bmatrix}$，得 $y_1 = 2$，$y_2 = 2$，$y_3 = -1$。

解 $Ux = y$：

$$\begin{bmatrix} 2 & 3 & 3 \\ 0 & 5 & 7 \\ 0 & 0 & -1 \end{bmatrix} \begin{bmatrix} v \\ x \\ w \end{bmatrix} = \begin{bmatrix} 2 \\ 2 \\ -1 \end{bmatrix}$$，解得 $x = \begin{bmatrix} 1 \\ -1 \\ 1 \end{bmatrix}$。
