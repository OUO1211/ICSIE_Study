## 矩陣的相等與加減法

> **考慮 $m \times n$ 的矩陣 $A = [a_{ij}]$，$B = [b_{ij}]$，則**
>
> (1) $A = B \Leftrightarrow a_{ij} = b_{ij}$ 對所有 $1 \leq i \leq m$，$1 \leq j \leq n$。
>
> (2) $A + B = [a_{ij} + b_{ij}]$。
>
> (3) $A - B = [a_{ij} - b_{ij}]$。

> **例如：**
>
> 若 $\begin{bmatrix} 1 & 0 \\ 2 & 4 \\ x & 5 \end{bmatrix} = \begin{bmatrix} 1 & y \\ 2 & 4 \\ 0 & 5 \end{bmatrix}$，則 $x = 0$，$y = 0$。

$$A = \begin{bmatrix} 1 & 0 \\ 2 & 4 \\ 3 & 5 \end{bmatrix}, \quad B = \begin{bmatrix} 0 & 0 \\ 1 & 0 \\ 0 & 2 \end{bmatrix}, \quad A + B = \begin{bmatrix} 1 & 0 \\ 3 & 4 \\ 3 & 7 \end{bmatrix}$$

$$C = \begin{bmatrix} 1 & 2 & 3 \\ 1 & 2 & 0 \end{bmatrix}, \quad D = \begin{bmatrix} 0 & 1 & 0 \\ 0 & 1 & 3 \end{bmatrix}, \quad C - D = \begin{bmatrix} 1 & 1 & 3 \\ 1 & 1 & -3 \end{bmatrix}$$

**Note**

(1) 兩矩陣需階數相同才能做加減法。  
(2) 矩陣的加法運算滿足結合性：對任意矩陣 $A、B、C$，$(A + B) + C = A + (B + C)$。  
(3) 矩陣的加法運算滿足交換性：對任意矩陣 $A、B$，$A + B = B + A$。  
(4) 給定 $m \times n$ 矩陣 $A$，若 $m \times n$ 矩陣 $B$ 滿足 $A + B = B + A = 0$，則稱 $B$ 為 $A$ 的一個負矩陣，記做 $B = -A$。

> **例如：**

$$A = \begin{bmatrix} 1 & -2 & -4 \\ 0 & 3 & 0.5 \end{bmatrix}, \quad -A = \begin{bmatrix} -1 & 2 & 4 \\ 0 & -3 & -0.5 \end{bmatrix}$$