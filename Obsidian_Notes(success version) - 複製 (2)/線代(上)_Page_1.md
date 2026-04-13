# 第 1 章　矩陣


## 1-1　矩陣的定義與運算

> **定義** 矩陣(matrix)
>
> 一個係於體(field) $F$ 的 $m\times n$ 矩陣
>
> $$
 A=[a_{ij}]=
 \begin{bmatrix}
 a_{11} & a_{12} & \cdots & a_{1n}\\
 a_{21} & a_{22} & \cdots & a_{2n}\\
 \vdots & \vdots & \ddots & \vdots\\
 a_{m1} & a_{m2} & \cdots & a_{mn}
 \end{bmatrix}
 \in F^{m\times n},
 $$
>
> 記為一 $m$ 列(row)、$n$ 行(column) 的二維陣列，其中 $a_{ij}\in F$。

**Note**

(1) 以後的章節所用的體，大都是以實數體（例如：實數($R$)或複數($C$)）來作。而若沒特別強調，就會以 $F$ 來表示。若 $F$ 為實數，則稱 $A$ 為實矩陣；若 $F$ 為複數，就稱 $A$ 為複矩陣。

(2) $a_{ij}$ 也稱為 $A$ 的元素(entry)。

(3) 有些版本記做 $A\in Mat_{m\times n}(F)$ 或 $A\in M_{m\times n}(F)$。

(4) 若一 $m\times n$ 矩陣元素全為零，則稱之為零矩陣(zero matrix)，也記成 $(O_{m\times n}$ 或 $0_{m\times n})$；當 $m=n$ 時，又把 $O_{n\times n}$ 記做 $O_n$。

例如：

$$
A=
\begin{bmatrix}
2 & \sqrt{2}\\
0 & 1
\end{bmatrix}
\in R^{2\times 2},\quad
B=
\begin{bmatrix}
1 & 1\\
-1 & 5\\
i & 0
\end{bmatrix}
\in C^{3\times 2},\quad
D=[1\ 2\ 1\ 0]\in R^{1\times 4}
$$

$$
O_2=
\begin{bmatrix}
0 & 0\\
0 & 0
\end{bmatrix},
\quad
O_{1\times 3}=[0\ 0\ 0]
$$

> **定義** 列矩陣(row matrix)、行矩陣(column matrix)、方陣(square matrix)
>
> 若矩陣 $A$ 只有一列，則稱 $A$ 為列矩陣。
>
> 若矩陣 $A$ 只有一行，則稱 $A$ 為行矩陣。
>
> 若矩陣 $A$ 列數手行數相同，則稱 $A$ 為方陣。

例如：

$$
A=[1\ 1\ 0]\in R^{1\times 3},\quad
B=[1\ 2]\in R^{2\times 1}
$$

都是列矩陣；