## 2-4 行列式的應用

本節討論行列式的兩項重要應用：
一、求反矩陣。
二、線性系統的另一種解法 Cramer's rule。

### 古典伴隨矩陣（adjoint matrix）

> **定義** 考慮方陣 $A = [a_{ij}]$，稱 $adj(A) = [cof(a_{ij})]^T$ 為 $A$ 的古典伴隨矩陣。

> **Note**
>
> $cof(a_{ij}) = (-1)^{i+j}\det(M_{ij})$ 為 $a_{ij}$ 的餘因子（cofactor），$M_{ij}$ 為把 $A$ 去掉第 $i$ 列，第 $j$ 行所得。

> **例題 1**
>
> 給定 $A = \begin{bmatrix} 3 & -2 & 1 \\ 5 & 6 & 2 \\ 1 & 0 & -3 \end{bmatrix}$，求 $adj(A)$。

**解**

$cof(a_{11}) = (-1)^{1+1}\begin{vmatrix} 6 & 2 \\ 0 & -3 \end{vmatrix} = -18$，$cof(a_{12}) = (-1)^{1+2}\begin{vmatrix} 5 & 2 \\ 1 & -3 \end{vmatrix} = 17$，

$cof(a_{13}) = (-1)^{1+3}\begin{vmatrix} 5 & 6 \\ 1 & 0 \end{vmatrix} = -6$，

$cof(a_{21}) = (-1)^{2+1}\begin{vmatrix} -2 & 1 \\ 0 & -3 \end{vmatrix} = -6$，$cof(a_{22}) = (-1)^{2+2}\begin{vmatrix} 3 & 1 \\ 1 & -3 \end{vmatrix} = -10$，$cof(a_{23}) = (-1)^{2+3}\begin{vmatrix} 3 & -2 \\ 1 & 0 \end{vmatrix} = -2$，

$cof(a_{31}) = (-1)^{3+1}\begin{vmatrix} -2 & 1 \\ 6 & 2 \end{vmatrix} = -10$，$cof(a_{32}) = (-1)^{3+2}\begin{vmatrix} 3 & 1 \\ 5 & 2 \end{vmatrix} = -1$，$cof(a_{33}) = (-1)^{3+3}\begin{vmatrix} 3 & -2 \\ 5 & 6 \end{vmatrix} = 28$，

故 $adj(A) = \begin{bmatrix} -18 & -6 & -10 \\ 17 & -10 & -1 \\ -6 & -2 & 28 \end{bmatrix}$。