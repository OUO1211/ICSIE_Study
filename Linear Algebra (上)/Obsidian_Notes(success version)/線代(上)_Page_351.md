> **例題 15**
>
> (20%) Give linearly independent sets of vectors that span each of the subspaces $R(A)$，$R(A^T)$，$N(A)$，and $N(A^T)$. $A = \begin{bmatrix} 1 & 1 & 0 \\ 2 & 1 & 1 \\ 1 & -1 & 2 \end{bmatrix}$。 【107 台大資工】
>
> 【100 政大資料，100 成大統計，99 成大統計，96.103.105 交大資工，101 成大資工 題組】

**解**

$A = \begin{bmatrix} 1 & 1 & 0 \\ 2 & 1 & 1 \\ 1 & -1 & 2 \end{bmatrix} \xrightarrow{\text{列運算}} \begin{bmatrix} 1 & 0 & 1 \\ 0 & 1 & -1 \\ 0 & 0 & 0 \end{bmatrix} = B$

(1) 因為 $A$ 的梯式矩陣的 pivot 在第一、二行，

故可取 $A$ 的第一、二行 $\begin{bmatrix} 1 \\ 2 \\ 1 \end{bmatrix}, \begin{bmatrix} 1 \\ 1 \\ -1 \end{bmatrix}$ 為 $R(A)$ 的一組基底。

(2) $R(A^T) = RS(A) = RS(B) = span\{(1,0,1),(0,1,-1)\}$，可取 $S$ 為 $R(A^T)$ 的一組基底。

(3) $N(A) = N(B) = \left\{ \begin{bmatrix} a \\ b \\ c \end{bmatrix} \middle| \begin{array}{l} a + c = 0 \\ b - c = 0 \end{array} \right\} = t\begin{bmatrix} -1 \\ 1 \\ 1 \end{bmatrix}$（$t \in \mathbb{R}$）= $span\left\{ \begin{bmatrix} -1 \\ 1 \\ 1 \end{bmatrix} \right\}$，

故可取 $\{(-1,1,1)^T\}$ 為 $N(A)$ 的一組基底。

(4) $N(A^T) = R(A)$ 的正交補，

$\left\{ \begin{bmatrix} a \\ b \\ c \end{bmatrix} \middle| A^T \begin{bmatrix} a \\ b \\ c \end{bmatrix} = 0 \right\} = \left\{ \begin{bmatrix} a \\ b \\ c \end{bmatrix} \middle| \begin{array}{l} a + 2b + c = 0 \\ 2a + 3b + 0 = 0 \\ a + b - c = 0 \end{array} \right\} = t\begin{bmatrix} 3 \\ -2 \\ 1 \end{bmatrix}$（$t \in \mathbb{R}$），

故可取 $\{(3,-2,1)^T\}$ 為 $N(A^T)$ 的一組基底。
