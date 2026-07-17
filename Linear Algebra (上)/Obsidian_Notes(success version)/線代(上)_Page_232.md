(1) $adj(A) = \begin{bmatrix} 12 & 4 & 12 \\ 6 & 2 & -10 \\ -16 & 16 & 16 \end{bmatrix}$，(2) $A^{-1} = \dfrac{1}{64}\begin{bmatrix} 12 & 4 & 12 \\ 6 & 2 & -10 \\ -16 & 16 & 16 \end{bmatrix}$【104 中央資工】

**解** (1) True. (2) True.

> 3. Find the inverse of:

(1) $\begin{bmatrix} k & 0 & 0 & 0 & 0 \\ 1 & k & 0 & 0 & 0 \\ 0 & 1 & k & 0 & 0 \\ 0 & 0 & 1 & k & 0 \\ 0 & 0 & 0 & 1 & k \end{bmatrix}$，(2) $\begin{bmatrix} 1 & 1 & 0 & 0 \\ 0 & 1 & 1 & 0 \\ 0 & 0 & 1 & 1 \\ 0 & 0 & 0 & 1 \end{bmatrix}$

**解** (1) $\dfrac{1}{k^5}\begin{bmatrix} k^4 & 0 & 0 & 0 & 0 \\ -k^3 & k^4 & 0 & 0 & 0 \\ k^2 & -k^3 & k^4 & 0 & 0 \\ -k & k^2 & -k^3 & k^4 & 0 \\ 1 & -k & k^2 & -k^3 & k^4 \end{bmatrix}$，(2) $\begin{bmatrix} 1 & -1 & 1 & -1 \\ 0 & 1 & -1 & 1 \\ 0 & 0 & 1 & -1 \\ 0 & 0 & 0 & 1 \end{bmatrix}$。

> 4. Given $A = \begin{bmatrix} x^2 & x & 1 \\ y^2 & y & 1 \\ z^2 & z & 1 \end{bmatrix}$，(1) What conditions must $x, y, z$ satisfy in order for $A$ to be nonsingular? (2) Let $x = 3$, $y = 2$, $z = -1$. Find the (3, 2)-entry of $A^{-1}$ by computer a quotient of two determinants.

**解** (1) $x, y, z$ 兩兩相異時。(2) 1。

> 5. (6%) Find $\det(A)$, $A$, $\det(3A^{-1}A^T)$. Where $adj(A) = \begin{bmatrix} 2 & 1 & 0 \\ 4 & 3 & 2 \\ -2 & -1 & 2 \end{bmatrix}$。【96 交大資工】

**解** 先計算得 $\det(adj(A)) = 4$，

$\because A(adj(A)) = \det(A)I_3$，

$\therefore \det(A)\det(adj(A)) = \det(A)^3$，$\therefore \det(adj(A)) = \det(A)^2$，故知 $\det(A) = \pm 2$，

又 $A = \det(A)(adj(A))^{-1} = \pm 2\begin{bmatrix} 2 & -1/2 & 1/2 \\ -3 & 1 & -1 \\ 1/2 & 0 & 1/2 \end{bmatrix}$。

又 $\det(3A^{-1}A^T) = 3^3 \det(A^{-1})\det(A^T) = 3^3 \det(A)^{-1}\det(A) = 27$。