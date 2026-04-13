> **試題 11**
>
> (15%) Consider $V = \{A \mid AX = XA, \text{ for any } X \in M_{n \times 1}\} \subseteq M_{n \times n}$. Show that $V$ is an one dimensional subspace of $M_{n \times n}$.
>
> 【107 台大數學】

解：對 $V$ 中任意元素 $A$，令 $X$ 只在第 $i$ 行有元素，其餘均為零行。

則 $AX = [0, \ldots, 0, A_{*i}, 0, \ldots, 0]$，$XA = [0, \ldots, 0, A_{i*}^T, 0, \ldots, 0]$，故 $AX = XA$ 時，

$A$ 的 $i$ 行等於 $A$ 的 $i$ 列轉置，$\therefore A = \text{diag}(c_1, c_2, \ldots, c_n)$，故均為對角陣。

又取 $A = \text{diag}(c_1, \ldots, c_n)$，$X$ 任意，則 $AX = \text{diag}(c_1, \ldots, c_n) X$，$(AX)_{ij} = c_i X_{ij}$，

$(XA)_{ij} = \sum_k X_{ik} A_{kj} = X_{ij} c_j$，

若 $AX = XA$，則 $c_i X_{ij} = X_{ij} c_j$，$\forall i, j$，即 $(c_i - c_j) X_{ij} = 0$，$\forall i, j, X$，

故 $c_i = c_j$，$\forall i, j$，即 $A = cI$，故 $V = \{cI \mid c \in R\}$，為一維子空間。

> **試題 12**
>
> (20%) Let $A \in R^{2 \times 2}$ and write $U = \{X \in R^{2 \times 2} : AX = XA\}$. Show that $\dim U \geq 2$.
>
> 【108 成大數學】

解：令 $A = \begin{bmatrix} a & b \\ c & d \end{bmatrix}$，則

$$U = \left\{ \begin{bmatrix} x & y \\ z & w \end{bmatrix} : \begin{bmatrix} a & b \\ c & d \end{bmatrix} \begin{bmatrix} x & y \\ z & w \end{bmatrix} = \begin{bmatrix} x & y \\ z & w \end{bmatrix} \begin{bmatrix} a & b \\ c & d \end{bmatrix} \right\}$$

$$= \left\{ \begin{bmatrix} x & y \\ z & w \end{bmatrix} : \begin{bmatrix} ax + bz & ay + bw \\ cx + dz & cy + dw \end{bmatrix} = \begin{bmatrix} ax + by & bx + dy \\ az + cw & bz + dw \end{bmatrix} \right\}$$

$$= \left\{ \begin{bmatrix} x & y \\ z & w \end{bmatrix} : \begin{matrix} bz - by = 0 \\ (a-d)y + b(w-x) = 0 \\ c(x-w) + (d-a)z = 0 \\ cy - cz = 0 \end{matrix} \right\}$$

$\therefore \dim(\ker(A)) = 4 - \text{rank}(B)$，

兩個 $0$ 是若干、$c$ 若干為零，分成 $0$ 種情形對應，故可得 $\text{rank}(B) \leq 2$，

$\therefore \dim(U) = 4 - 2 = 2$。
