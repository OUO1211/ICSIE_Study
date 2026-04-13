## 第 3 章　向量空間

## 矩陣的四大基本子空間 (fundamental subspaces)

> 考慮 $m \times n$ 矩陣 $A$，
>
> (1) $RS(A) = \{A$ 的列向量的線性組合$\}$，稱為 $A$ 的列空間 (row space)，又可表為
>
> $$\{a_1 A_{(1)} + \cdots + a_m A_{(m)} \mid a_i \text{ 為純量係數}\}$$
>
> $$= \{xA \mid x : n \times 1\}。$$
>
> (2) $CS(A) = \{A$ 的行向量的線性組合$\}$，稱為 $A$ 的行空間 (column space)，又可表為
>
> $$\{a_1 a^{(1)} + \cdots + a_n a^{(n)} \mid a_i \text{ 為純量係數}\}$$
>
> $$= \{Ax \mid x : n \times 1\}。$$
>
> (3) $\ker(A) = \{x_{n \times 1} \mid Ax = 0\}$，稱為 $A$ 的核空間 (kernel)，即為齊次方程的解集合。
>
> (4) $L\ker(A) = \{y_{1 \times m} \mid yA = 0\}$，稱為 $A$ 的左核空間 (left kernel)

> **Note**
>
> 例如，考慮矩陣
>
> $$A = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 1 & 0 & 0 \end{bmatrix}，$$
>
> 則
>
> 其列空間 $RS(A) = \{a(1,0,0) + b(0,1,0) + c(1,0,0) \mid a,b,c \in R\} = \{(x,y,0) \mid x,y \in R\}$；
>
> 其行空間 $CS(A) = \left\{ a\begin{bmatrix} 1 \\ 0 \\ 1 \end{bmatrix} + b\begin{bmatrix} 0 \\ 1 \\ 0 \end{bmatrix} + c\begin{bmatrix} 0 \\ 0 \\ 0 \end{bmatrix} \mid a,b,c \in R \right\} = \left\{ \begin{bmatrix} x \\ y \\ x \end{bmatrix} \mid x,y \in R \right\}$；
>
> 核空間 $\ker(A) = \left\{ \begin{bmatrix} x \\ y \\ z \end{bmatrix} \,\middle|\, \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 1 & 0 & 0 \end{bmatrix}\begin{bmatrix} x \\ y \\ z \end{bmatrix} = \begin{bmatrix} 0 \\ 0 \\ 0 \end{bmatrix} \right\} = \left\{ \begin{bmatrix} x \\ y \\ z \end{bmatrix} \,\middle|\, \begin{array}{l} x = 0 \\ y = 0 \end{array} \right\} = \left\{ \begin{bmatrix} 0 \\ 0 \\ z \end{bmatrix} \mid z \in R \right\}$；
>
> 左核空間 $L\ker(A) = \left\{ [x\ y\ z] \,\middle|\, [x\ y\ z]\begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 1 & 0 & 0 \end{bmatrix} = [0\ 0\ 0] \right\} = \left\{ [x\ y\ z] \,\middle|\, \begin{array}{l} x + z = 0 \\ y = 0 \end{array} \right\} = \{[a\ 0\ {-}a] \mid a \in R\}$。