## 矩陣的乘法

> **設矩陣乘積的定義如下：**
>
> 設 $A = [a_{ij}]_{m \times n}$，
> $$
 A = \begin{bmatrix}
 a_{11} & \cdots & \cdots & a_{1n} \\
 \vdots & \ddots & & \vdots \\
 a_{i1} & a_{i2} & a_{i3} & \cdots & a_{in} \\
 \vdots & & \ddots & \vdots \\
 a_{m1} & \cdots & \cdots & a_{mn}
 \end{bmatrix}_{m \times n}, \quad
 B = [b_{ij}]_{n \times p} =
 \begin{bmatrix}
 b_{11} & \cdots & b_{1j} & \cdots & b_{1p} \\
 \vdots & & \vdots & & \vdots \\
 b_{i1} & \cdots & b_{ij} & \cdots & b_{ip} \\
 \vdots & & \vdots & & \vdots \\
 b_{n1} & \cdots & b_{nj} & \cdots & b_{np}
 \end{bmatrix}_{n \times p}
 $$
>
> 則 $AB = [c_{ij}]_{m \times p} =$
> $$
 \begin{bmatrix}
 c_{11} & \cdots & c_{1p} \\
 \vdots & \ddots & \vdots \\
 c_{i1} & \cdots & c_{ip} \\
 \vdots & & \vdots \\
 c_{m1} & \cdots & c_{mp}
 \end{bmatrix}_{m \times p}
 $$
>
> 其中，$c_{ij} = a_{i1}b_{1j} + a_{i2}b_{2j} + a_{i3}b_{3j} + \cdots + a_{in}b_{nj} = \sum_{k=1}^{n} a_{ik}b_{kj}$，$1 \leq i \leq m$，$1 \leq j \leq p$。

例如：$2 \times 2$

$$
A = \begin{bmatrix} 1 & 3 \\ 2 & 4 \end{bmatrix}, \quad
B = \begin{bmatrix} 10 & 30 & 50 \\ 20 & 40 & 60 \end{bmatrix}
$$

設 $AB = C = [c_{ij}]_{2 \times 3}$，則

$c_{11} = 1 \times 10 + 3 \times 20 = 70$，$c_{12} = 1 \times 30 + 3 \times 40 = 150$，$c_{13} = 1 \times 50 + 3 \times 60 = 230$。

$c_{21} = 2 \times 10 + 4 \times 20 = 100$，$c_{22} = 2 \times 30 + 4 \times 40 = 220$，$c_{23} = 2 \times 50 + 4 \times 60 = 340$。

故
$$
C = \begin{bmatrix} 70 & 150 & 230 \\ 100 & 220 & 340 \end{bmatrix}
$$

**Note**

(1) 需在“$A$”的行數 =“$B$”的列數時，才可做 $AB$ 的運算。  
(2) 對方陣 $A$，定義 $A^0 = I$，且對正整數 $k$，$A^{k+1} = A^k A = A A^k$。