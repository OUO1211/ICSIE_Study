### 行列式與直線方程

> **問題 8**
>
> (7%) Prove that $(x_1, y_1)$, $(x_2, y_2)$, $(x_3, y_3)$ are colinear if and only if $\begin{vmatrix} x_1 & y_1 & 1 \\ x_2 & y_2 & 1 \\ x_3 & y_3 & 1 \end{vmatrix} = 0$.
>
> 【101 中正資工】

**解** 三點共線

$\Leftrightarrow$ 存在 $a, b, c$ 不全為零，直線 $ax + by + c = 0$，通過三點

$\Leftrightarrow$ 存在 $a, b, c$ 不全為零，滿足：$\begin{cases} ax_1 + by_1 + c = 0 \\ ax_2 + by_2 + c = 0 \\ ax_3 + by_3 + c = 0 \end{cases}$

$\Leftrightarrow$ 存在 $a, b, c$ 不全為零，滿足：$\begin{bmatrix} x_1 & y_1 & 1 \\ x_2 & y_2 & 1 \\ x_3 & y_3 & 1 \end{bmatrix} \begin{bmatrix} a \\ b \\ c \end{bmatrix} = \begin{bmatrix} 0 \\ 0 \\ 0 \end{bmatrix}$，

（即此齊次方程式有非零解）

$\Leftrightarrow \begin{bmatrix} x_1 & y_1 & 1 \\ x_2 & y_2 & 1 \\ x_3 & y_3 & 1 \end{bmatrix}$ 不可逆

$\Leftrightarrow \det\begin{pmatrix} \begin{bmatrix} x_1 & y_1 & 1 \\ x_2 & y_2 & 1 \\ x_3 & y_3 & 1 \end{bmatrix} \end{pmatrix} = 0$。
