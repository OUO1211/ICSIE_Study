# 第 1 章 矩陣

27

## 行展開與行切割

> **定理**
>
> 設 $A^{(j)}$ 為矩陣 $A=[a_{ij}]_{m\times n}$ 的第 $j$ 個行向量；$x$ 為行向量
>
> $$x=\begin{bmatrix}x_1\\x_2\\ \vdots \\x_n\end{bmatrix}.$$
>
> 行展開法則：
>
> $$Ax\ \text{可表成}\ \begin{bmatrix}a_{11}&a_{12}&\cdots&a_{1n}\\a_{21}&a_{22}&\cdots&a_{2n}\\ \vdots & \vdots & & \vdots \\a_{m1}&a_{m2}&\cdots&a_{mn}\end{bmatrix}\begin{bmatrix}x_1\\x_2\\ \vdots \\x_n\end{bmatrix}=\begin{bmatrix}A^{(1)}&A^{(2)}&\cdots&A^{(n)}\end{bmatrix}\begin{bmatrix}x_1\\x_2\\ \vdots \\x_n\end{bmatrix}$$
>
> $$=A^{(1)}x_1+A^{(2)}x_2+\cdots+A^{(n)}x_n$$
>
> 行切割法則：
>
> 若 $A=[a_{ij}]_{m\times n},\ B=[b_{ij}]_{n\times p},\ C=[c_{ij}]_{m\times p}$，則
>
> $$AB=C\ \text{可表成}\ A\begin{bmatrix}B^{(1)}&B^{(2)}&\cdots&B^{(p)}\end{bmatrix}=\begin{bmatrix}C^{(1)}&C^{(2)}&\cdots&C^{(p)}\end{bmatrix}\ \text{或}\ AB^{(j)}=C^{(j)},\ \forall j=1,2,\ldots,p。$$

行展開：

$$\begin{bmatrix}1&2&3\\4&5&6\end{bmatrix}\begin{bmatrix}a\\b\\c\end{bmatrix}=\begin{bmatrix}a+2b+3c\\4a+5b+6c\end{bmatrix}$$

$$=a\begin{bmatrix}1\\4\end{bmatrix}+b\begin{bmatrix}2\\5\end{bmatrix}+c\begin{bmatrix}3\\6\end{bmatrix}$$

行切割：

$$\begin{bmatrix}1&2&3\\4&5&6\end{bmatrix}\begin{bmatrix}a&x\\b&y\\c&z\end{bmatrix}=\begin{bmatrix}a+2b+3c&x+2y+3z\\4a+5b+6c&4x+5y+6z\end{bmatrix}$$

若有 $A\cdot B=C$

則 $AB^{(i)}=C^{(i)}$

列展開/切割亦相同