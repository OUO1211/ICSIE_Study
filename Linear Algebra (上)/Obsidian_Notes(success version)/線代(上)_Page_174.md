### 行列式基本性質・由定義

> **定義**
>
> (1) $A$ 的某行（列）均為零，則其行列式值為零。
>
> (2) $A$ 的某兩行（列）相同，則其行列式值為零。
>
> (3) $A$ 的某行（列）可表為兩行（列）向量的和，則其行列式值等於由此兩分量分出之兩矩陣的行列式的和。
>
> 【110 台大資工】
>
> $$\det\begin{pmatrix} A^{(1)}, \cdots, A^{(i-1)}, A^{(i)} + B^{(i)}, A^{(i+1)}, \cdots, A^{(n)} \end{pmatrix} = \det\begin{pmatrix} A^{(1)}, \cdots, A^{(i-1)}, A^{(i)}, A^{(i+1)}, \cdots, A^{(n)} \end{pmatrix} + \det\begin{pmatrix} A^{(1)}, \cdots, A^{(i-1)}, B^{(i)}, A^{(i+1)}, \cdots, A^{(n)} \end{pmatrix}$$
>
> (4) $A$ 的某行（列）可為其他行（列）的線性組合，則其行列式值為零。
>
> (5) $A$ 為上三角、下三角或對角矩陣時，$\det(A)$ 為主對角元素積。

例如：

$$\det\begin{bmatrix} 1 & 4 & 3 \\ 0 & 0 & 0 \\ \sqrt{5} & \pi & 10^5 \end{bmatrix} = 0,$$

$$\det\begin{bmatrix} 1 & 4 & 3 \\ \sqrt{5} & \pi & 10^5 \\ \sqrt{5} & \pi & 10^5 \end{bmatrix} = 0,$$

$$\det\begin{bmatrix} 1 & 4 & 3 \\ \sqrt{5} & \pi & 10^5 \\ 2 + \sqrt{5} & 8 + \pi & 6 + 10^5 \end{bmatrix} = 0,$$

$$\det\begin{bmatrix} a & b & c \\ 1+10 & 2+15 & 3+20 \\ d & e & f \end{bmatrix} = \det\begin{bmatrix} a & b & c \\ 1 & 2 & 3 \\ d & e & f \end{bmatrix} + \det\begin{bmatrix} a & b & c \\ 10 & 15 & 20 \\ d & e & f \end{bmatrix},$$

$$\det\begin{bmatrix} 2 & \pi & \sqrt{5} \\ 0 & 3 & 10^5 \\ 0 & 0 & 4 \end{bmatrix} = \det\begin{bmatrix} 2 & 0 & 0 \\ 0 & 3 & 0 \\ 0 & 0 & 4 \end{bmatrix} = 2 \cdot 3 \cdot 4 = 24.$$

> **Note**
>
> 設 $A = [a_{ij}]_{n \times n}$，則
>
> (1) $\displaystyle\sum_{k=1}^{n} a_{jk} cof(a_{ik}) = \begin{cases} \det(A) & \text{if } i = j \\ 0 & \text{if } i \neq j \end{cases}$
>
> (2) $\displaystyle\sum_{k=1}^{n} a_{ki} cof(a_{kj}) = \begin{cases} \det(A) & \text{if } i = j \\ 0 & \text{if } i \neq j \end{cases}$