> **例 4**
>
> Solve the following equations using determinant:
>
> (1) $\begin{cases} 3y + 2x = z + 1 \\ 3x + 2z = 8 - 5y \\ 3z - 1 = x - 2y \end{cases}$，$\begin{cases} 4x_1 + 5x_2 = 2 \\ 11x_1 + x_2 + x_3 = 3 \\ x_1 + 5x_2 + x_3 = 1 \end{cases}$

**解**

(1) 整理得 $\begin{cases} 2x + 3y - z = 1 \\ 3x + 5y + 2z = 8 \\ x - 2y - 3z = -1 \end{cases}$，$A = \begin{bmatrix} 2 & 3 & -1 \\ 3 & 5 & 2 \\ 1 & -2 & -3 \end{bmatrix}$，

$\Delta = \begin{vmatrix} 2 & 3 & -1 \\ 3 & 5 & 2 \\ 1 & -2 & -3 \end{vmatrix} = 22$，

$\Delta_1 = \begin{vmatrix} 1 & 3 & -1 \\ 8 & 5 & 2 \\ -1 & -2 & -3 \end{vmatrix} = 66$，$\Delta_2 = \begin{vmatrix} 2 & 1 & -1 \\ 3 & 8 & 2 \\ 1 & -1 & -3 \end{vmatrix} = -22$，$\Delta_3 = \begin{vmatrix} 2 & 3 & 1 \\ 3 & 5 & 8 \\ 1 & -2 & -1 \end{vmatrix} = 44$，

$\therefore x = \dfrac{\Delta_1}{\Delta} = 3$，$y = \dfrac{\Delta_2}{\Delta} = -1$，$z = \dfrac{\Delta_3}{\Delta} = 2$

(2) $A = \begin{bmatrix} 4 & 5 & 0 \\ 11 & 1 & 1 \\ 1 & 5 & 1 \end{bmatrix}$，$\Delta = -66$，

$\Delta_1 = \begin{vmatrix} 2 & 5 & 0 \\ 3 & 1 & 1 \\ 1 & 5 & 1 \end{vmatrix} = -18$，$\Delta_2 = \begin{vmatrix} 4 & 2 & 0 \\ 11 & 3 & 1 \\ 1 & 1 & 1 \end{vmatrix} = -12$，$\Delta_3 = \begin{vmatrix} 4 & 5 & 2 \\ 11 & 1 & 3 \\ 1 & 5 & 1 \end{vmatrix} = 12$，

$\therefore x = \dfrac{\Delta_1}{\Delta} = \dfrac{3}{11}$，$y = \dfrac{\Delta_2}{\Delta} = \dfrac{2}{11}$，$z = \dfrac{\Delta_3}{\Delta} = -\dfrac{2}{11}$

---

> **問題 5**
>
> Consider the linear system $\begin{cases} ax + y + z = 1 \\ x + ay + z = 0 \\ x + y + az = 0 \end{cases}$. Find what values of $a$ does the linear system have a unique solution? Also, use Cramer's rule to find the solution.

**解** 係數矩陣 $A = \begin{bmatrix} a & 1 & 1 \\ 1 & a & 1 \\ 1 & 1 & a \end{bmatrix}$，求得 $\det(A) = (a-1)^2(a+2)$。

故 $Ax = b$ 有唯一解，欲使 $(a-1)^2(a+2) \neq 0$，即 $a \neq 1$ 且 $a \neq -2$。

又 $\Delta_1 = \begin{vmatrix} 1 & 1 & 1 \\ 0 & a & 1 \\ 0 & 1 & a \end{vmatrix} = a^2 - 1 = (a-1)(a+1)$，$\Delta_2 = \begin{vmatrix} a & 1 & 1 \\ 1 & 0 & 1 \\ 1 & 0 & a \end{vmatrix} = 1-a = -(a-1)$，$\Delta_3 = \begin{vmatrix} a & 1 & 1 \\ 1 & a & 0 \\ 1 & 1 & 0 \end{vmatrix} = 1-a = -(a-1)$，

$$x = \dfrac{\Delta_1}{\det A} = \dfrac{(a-1)(a+1)}{(a-1)^2(a+2)} = \dfrac{a+1}{(a-1)(a+2)}$$

$$y = \dfrac{\Delta_2}{\det A} = \dfrac{-(a-1)}{(a-1)^2(a+2)} = \dfrac{-1}{(a-1)(a+2)}$$

$$z = \dfrac{\Delta_3}{\det A} = \dfrac{-(a-1)}{(a-1)^2(a+2)} = \dfrac{-1}{(a-1)(a+2)}$$