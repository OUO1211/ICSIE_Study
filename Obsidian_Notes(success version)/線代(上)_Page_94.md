# 第一章 矩陣 93

## LDU 分解(LDU-decomposition)

> **定義**
>
> 給定 $n$ 階方陣 $A$，若存在下三角矩陣 $L$、對角矩陣 $D$、上三角矩陣 $U$，使得 $A=LDU$，則稱此為 $A$ 的一個 LDU 分解，其中 $L$ 與 $U$ 的對角項均為 $1$。
>
> 【92 成大統計】

> **Note**
>
> (1) 作 LDU 分解的步驟：
>
> Step 1　做 $LU$ 分解使 $A=LU$，且 $L$ 的對角均為 $1$。
>
> Step 2　令 $A=LU=LDD^{-1}U$，其中 $D=\operatorname{diag}(u_{11},u_{22},\cdots,u_{nn})$，$u_{ii}$ 為 $U$ 的對角項元素。
>
> Step 3　計算 $D^{-1}U$ 得 $U_1$，
>
> 得 $A=LDU_1$ 為所求
>
> (2) 不是每個矩陣都可做 LDU 分解。
>
> (3) 可應用解線性方程組。

> **例題 6**
>
> 請對 $A=\begin{bmatrix} 2 & 3 & 1 \\ 4 & 1 & 4 \\ 3 & 4 & 6 \end{bmatrix}$ 完成 LDU 分解。

**解**

$$
A=\begin{bmatrix}
1 & 0 & 0\\
2 & 1 & 0\\
\frac{3}{2} & \frac{1}{10} & 1
\end{bmatrix}
\begin{bmatrix}
2 & 3 & 1\\
0 & -5 & 2\\
0 & 0 & \frac{43}{10}
\end{bmatrix}
$$

$$
=
\begin{bmatrix}
1 & 0 & 0\\
2 & 1 & 0\\
\frac{3}{2} & \frac{1}{10} & 1
\end{bmatrix}
\begin{bmatrix}
2 & 0 & 0\\
0 & -5 & 0\\
0 & 0 & \frac{43}{10}
\end{bmatrix}
\begin{bmatrix}
1 & \frac{3}{2} & \frac{1}{2}\\
0 & 1 & -\frac{2}{5}\\
0 & 0 & 1
\end{bmatrix}
$$

$$
=
\begin{bmatrix}
1 & 0 & 0\\
2 & 1 & 0\\
\frac{3}{2} & \frac{1}{10} & 1
\end{bmatrix}
\begin{bmatrix}
2 & 0 & 0\\
0 & -5 & 0\\
0 & 0 & \frac{43}{10}
\end{bmatrix}
\begin{bmatrix}
1 & \frac{3}{2} & \frac{1}{2}\\
0 & 1 & -\frac{2}{5}\\
0 & 0 & 1
\end{bmatrix}
$$