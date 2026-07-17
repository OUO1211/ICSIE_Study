### 伴隨矩陣的性質與應用

> **定義** 令 $A$ 為 $n$ 階方陣，則：
>
> (1) $A \cdot adj(A) = (adj(A)) \cdot A = \det(A) I_n$
>
> (2) 若 $A$ 可逆，則 $A^{-1} = \dfrac{1}{\det(A)} adj(A)$，且 $\det(A^{-1}) = \dfrac{1}{\det(A)}$。
>
> (3) 若 $A$ 可逆，則 $\det(adj(A)) = (\det A)^{n-1}$。【106 中正數學】

【證明】

(1) 令 $A = [a_{ij}]$，$adj(A) = [d_{ij}]$，$A \cdot adj(A) = [c_{ij}]$，

則由矩陣乘法可得：$c_{ij} = \sum_{k=1}^{n} a_{ik} d_{kj} = \sum_{k=1}^{n} cof(a_{jk}) a_{ik} = \begin{cases} \det(A) & \text{if } i = j \\ 0 & \text{if } i \neq j \end{cases}$，

故 $A \cdot adj(A) = diag(\det(A), \det(A), \ldots) = \det(A) I_n = \det(A) I$，同理可得 $adj(A) \cdot A = \det(A) I_n$。

（**注**：這是用行列式性質的結果。）

(2) 由(1)得 $A \cdot \dfrac{1}{\det(A)} adj(A) = \left(\dfrac{1}{\det(A)} adj(A)\right) \cdot A = I_n$，$\therefore A^{-1} = \dfrac{1}{\det(A)} adj(A)$。

又，$\det(A \cdot A^{-1}) = \det(I) = 1$，$\therefore \det(A)\det(A^{-1}) = 1$，$\therefore \det(A^{-1}) = \dfrac{1}{\det(A)}$。

(3) 由(1)得 $A \cdot adj(A) = (\det A) I_n$，得 $\det(A \cdot adj(adj(A))) = (\det A)^n$，

若 $A$ 可逆，即 $\det(A) \neq 0$，故得 $\det(adj(A)) = (\det A)^{n-1}$。

> **例題 2**
>
> $A = \begin{bmatrix} 1 & 4 & 3 \\ -1 & -2 & 0 \\ 2 & 2 & 3 \end{bmatrix}$，$A^{-1} = ?$

**解** $\det(A) = \begin{vmatrix} 1 & 4 & 3 \\ -1 & -2 & 0 \\ 2 & 2 & 3 \end{vmatrix} = \begin{vmatrix} 1 & 4 & 3 \\ 0 & 2 & 3 \\ 0 & -6 & -3 \end{vmatrix} = \begin{vmatrix} 0 & 1 & 6 \end{vmatrix} = 12$，

$cof(a_{11}) = (-1)^{1+1}\begin{vmatrix} -2 & 0 \\ 2 & 3 \end{vmatrix} = -6$，$cof(a_{12}) = (-1)^{1+2}\begin{vmatrix} -1 & 0 \\ 2 & 3 \end{vmatrix} = 3$，

$cof(a_{13}) = (-1)^{1+3}\begin{vmatrix} -1 & -2 \\ 2 & 2 \end{vmatrix} = 2$，$cof(a_{21}) = (-1)^{2+1}\begin{vmatrix} 4 & 3 \\ 2 & 3 \end{vmatrix} = -6$，

$cof(a_{22}) = (-1)^{2+2}\begin{vmatrix} 1 & 3 \\ 2 & 3 \end{vmatrix} = -3$，$cof(a_{23}) = (-1)^{2+3}\begin{vmatrix} 1 & 4 \\ 2 & 2 \end{vmatrix} = 6$，
