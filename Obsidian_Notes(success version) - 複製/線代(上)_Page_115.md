# 第二章 線性方程組與求解 116

## 解線性系統－高斯消去法 (Gauss elimination)、高斯喬丹消去法 (Gauss-Jordan elimination)

高斯消去法：將增廣矩陣利用列運算，化成列梯陣，再做方程組。

高斯喬丹消去法：將增廣矩陣利用運算成簡化列梯陣，再解方程組。

> **例題 1**
>
> (5%) Solve the following system:
>
> $$\begin{cases} 2x_1 + x_2 + x_3 = 2 \\ -x_1 + 2x_2 = 1 \\ x_1 - x_2 + 2x_3 = -2 \end{cases}$$
>
> 【110 台大材】

**解**

$$\begin{bmatrix} 2 & 1 & 1 & 2 \\ -1 & 2 & 0 & 1 \\ 1 & -1 & 2 & -2 \end{bmatrix}
\xrightarrow{\cdots}
\begin{bmatrix} 1 & -1 & 2 & -2 \\ -1 & 2 & 0 & 1 \\ 2 & 1 & 1 & 2 \end{bmatrix}
\xrightarrow{\cdots}
\begin{bmatrix} 1 & -1 & 2 & -2 \\ 0 & 1 & 2 & -1 \\ 0 & 3 & -3 & 6 \end{bmatrix}
\xrightarrow{\cdots}
\begin{bmatrix} 1 & 0 & 4 & -3 \\ 0 & 1 & 2 & -1 \\ 0 & 0 & -9 & 9 \end{bmatrix}
\xrightarrow{\cdots}
\begin{bmatrix} 1 & 0 & 0 & 1 \\ 0 & 1 & 0 & 1 \\ 0 & 0 & 1 & -1 \end{bmatrix}$$

故得 $x_1 = 1$，$x_2 = 1$，$x_3 = -1$。

> **例題 2**
>
> Use Gaussian elimination to solve the given system
>
> $$\begin{bmatrix} 1 & 3 & 1 & 2 \\ 2 & 6 & 4 & 8 \\ 0 & 0 & 2 & 4 \end{bmatrix}\begin{bmatrix} w \\ x \\ y \\ z \end{bmatrix}=\begin{bmatrix} 1 \\ 3 \\ 1 \end{bmatrix}$$
>
> 【99.100 台大資工‧98.101 彰師資工題】

**解**

$$\begin{bmatrix} 1 & 3 & 1 & 2 & 1 \\ 2 & 6 & 4 & 8 & 3 \\ 0 & 0 & 2 & 4 & 1 \end{bmatrix}
\xrightarrow{\text{消去}}
\begin{bmatrix} 1 & 3 & 0 & 0 & 0.5 \\ 0 & 0 & 1 & 2 & 0.5 \\ 0 & 0 & 0 & 0 & 0 \end{bmatrix}$$

解為

$$\left\{\begin{bmatrix} w \\ x \\ y \\ z \end{bmatrix}\,\middle|\,\begin{matrix} w+3x=0.5 \\ y+2z=0.5 \end{matrix}\right\}
=
\left\{\begin{bmatrix} 0.5-3t \\ t \\ 0.5-2s \\ s \end{bmatrix},\, s,t\in\mathbb{R}\right\}
=
\begin{bmatrix} 0.5 \\ 0 \\ 0.5 \\ 0 \end{bmatrix}
+
\begin{bmatrix} -3t \\ t \\ -2s \\ s \end{bmatrix},\ s,t\in\mathbb{R}$$