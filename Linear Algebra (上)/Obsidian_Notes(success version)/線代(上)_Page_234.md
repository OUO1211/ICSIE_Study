### 求解線性系統－克拉瑪法則（Cramer's rule）

> **定義** 考慮線性方程組：
>
> $$\begin{cases} a_{11}x_1 + a_{12}x_2 + \cdots + a_{1n}x_n = b_1 \\ a_{21}x_1 + a_{22}x_2 + \cdots + a_{2n}x_n = b_2 \\ \vdots \\ a_{n1}x_1 + a_{n2}x_2 + \cdots + a_{nn}x_n = b_n \end{cases}$$，以 $Ax = b$ 表達。
>
> 其中 $A = \begin{bmatrix} a_{11} & a_{12} & \cdots & a_{1n} \\ a_{21} & a_{22} & \cdots & a_{2n} \\ \vdots & & & \vdots \\ a_{n1} & a_{n2} & \cdots & a_{nn} \end{bmatrix}$，$x = \begin{bmatrix} x_1 \\ x_2 \\ \vdots \\ x_n \end{bmatrix}$，$b = \begin{bmatrix} b_1 \\ b_2 \\ \vdots \\ b_n \end{bmatrix}$，
>
> 定義 $\Delta = \det(A)$，$\Delta_j = \begin{vmatrix} a_{11} & \cdots & b_1 & \cdots & a_{1n} \\ a_{21} & \cdots & b_2 & \cdots & a_{2n} \\ \vdots & & \vdots & & \vdots \\ a_{n1} & \cdots & b_n & \cdots & a_{nn} \end{vmatrix}$，$\Delta_j$ 第 $j$ 行以 $b$ 取代
>
> 若 $\Delta \neq 0$，則此聯立方程組只有一解：$x_1 = \dfrac{\Delta_1}{\Delta}$，$x_2 = \dfrac{\Delta_2}{\Delta}$，……，$x_n = \dfrac{\Delta_n}{\Delta}$。

【證明】

因為 $A$ 可逆，故 $x = A^{-1}b = \dfrac{adj(A)}{\det(A)} b$ 為此線性系統的解。

令 $adj(A) = [d_{ij}]$，則

對任意 $i$：

$$\therefore x_i = \dfrac{1}{\det(A)} \sum_{k=1}^{n} d_{ik} b_k = \dfrac{1}{\det(A)} \sum_{k=1}^{n} cof(a_{ki}) b_k = \dfrac{\Delta_i}{\Delta}$$
