*若 $E$ 為列交換矩陣，則由(i)得遞性質成立。

*若 $E = R_i^{(k)}$，則

$$\delta\!\left(\begin{bmatrix} \vdots \\ e_i \\ \vdots \\ e_j + ke_i \\ \vdots \end{bmatrix}\right) = \delta\!\left(\begin{bmatrix} \vdots \\ e_i \\ \vdots \\ e_j \\ \vdots \end{bmatrix}\right) + k\delta\!\left(\begin{bmatrix} \vdots \\ e_i \\ \vdots \\ e_i \\ \vdots \end{bmatrix}\right) = 1 + k \cdot 0 = 1 = \det(R_i^{(k)})$$

*若 $E = R_i^{(k)}$，$\delta(ke_i) = k\delta(e_i) = k = \det(R_i^{(k)})$

故得證。

---

> **試題 8**
>
> Let $C = \begin{bmatrix} -x & 1 & 3 & 1 & 2 \\ -2 & 0 & x & 2 & 2 \\ x & 0 & -2 & -3 & -1 \\ 0 & 0 & 0 & -1 & 0 \\ 1 & 0 & 0 & 0 & x \end{bmatrix}$. Find an integer $x$ such that all entries of the inverse of $C$ are integers. Find such $x$. 【104 台大數學】

**解** $x = -1$。

$\because C \in Z^{5\times5}$，故 $C$ 的每個位置的餘因子 (cofactor) 均為整數，

故 $C$ 的伴隨矩陣 $(\text{adj}) \in Z^{5\times5}$；

又因 $C^{-1} = \dfrac{1}{\det(C)} \text{adj}(C)$，

計算得 $\det(C) = 2x^2 - x - 4$，可取 $x = -1$，則 $\det(C) = -1$，

如此可使 $C^{-1} \in Z^{5\times5}$。

並可代入 $x = -1$ 高斯消去法後求出 $C^{-1} = \begin{bmatrix} 0 & -4 & 2 & -9 & -5 \\ 1 & -1 & 2 & -6 & -1 \\ 0 & 3 & -2 & 8 & 4 \\ 0 & 0 & 0 & -1 & 0 \\ 0 & -2 & 1 & -4 & -3 \end{bmatrix}$
