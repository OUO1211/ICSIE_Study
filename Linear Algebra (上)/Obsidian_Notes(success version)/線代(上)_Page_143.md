# 第二章 線性方程組與求解 143

> **例題 3**
>
> For which $k$ does $\begin{cases} kx + y + z = 1 \\ x + ky + z = 1 \\ x + y + kz = 1 \end{cases}$ have no solution, one solution or infinite many solutions? If it has solutions, find them.
>
> 【99 師大數學・96 清大統計】

**解**

其增廣矩陣 $[A \mid b] = \begin{bmatrix} k & 1 & 1 & \mid & 1 \\ 1 & k & 1 & \mid & 1 \\ 1 & 1 & k & \mid & 1 \end{bmatrix} \xrightarrow{r_{31}^{(-k)},\ r_{32}^{(-1)}} \begin{bmatrix} 0 & 1-k & 1-k^2 & \mid & 1-k \\ 0 & k-1 & 1-k & \mid & 0 \\ 1 & 1 & k & \mid & 1 \end{bmatrix} = B.$

(1) 若 $k = 1$，$B = \begin{bmatrix} 0 & 0 & 0 & \mid & 0 \\ 0 & 0 & 0 & \mid & 0 \\ 1 & 1 & 1 & \mid & 1 \end{bmatrix}$，即 $x + y + z = 1$，此時有無限多解，

解集合可表為
$$
\left\{
\begin{bmatrix}
1\\
0\\
0
\end{bmatrix}
+
s\begin{bmatrix}
-1\\
1\\
0
\end{bmatrix}
+
t\begin{bmatrix}
-1\\
0\\
1
\end{bmatrix},
\ s,t\text{ 為任意數}
\right\}.
$$

(2) 若 $k \ne 1$，$\frac{r_1^{(1)}}{1-k},\ \frac{r_2^{(1)}}{k-1} \to \begin{bmatrix} 0 & 1 & 1+k & \mid & 1 \\ 0 & -1 & 1 & \mid & 0 \\ 1 & 1 & k & \mid & 1 \end{bmatrix} \xrightarrow{r_{21}^{(1)},\ r_{23}^{(-1)}} \begin{bmatrix} 0 & 0 & 2+k & \mid & 1 \\ 0 & -1 & 1 & \mid & 0 \\ 1 & 0 & k+1 & \mid & 1 \end{bmatrix} = C.$

此時若 $k = -2$，則 $C = \begin{bmatrix} 0 & 0 & 0 & \mid & 1 \\ 0 & -1 & 1 & \mid & 0 \\ 1 & 0 & -1 & \mid & 1 \end{bmatrix}$，即得 $0x + 0y + 0z = 1$，故此時無解

(3) 若 $k \ne 1$，$k \ne -2$，$C \xrightarrow{r_1^{(1/(2+k))},\ r_2^{(-1)},\ r_3^{(1-k)}} \begin{bmatrix} 0 & 0 & 1 & \mid & \dfrac{1}{2+k} \\ 0 & 1 & 0 & \mid & \dfrac{1}{2+k} \\ 1 & 0 & 0 & \mid & \dfrac{1}{2+k} \end{bmatrix}.$

即得唯一解
$$
\begin{bmatrix}
x\\
y\\
z
\end{bmatrix}
=
\frac{1}{2+k}
\begin{bmatrix}
1\\
1\\
1
\end{bmatrix}.
$$