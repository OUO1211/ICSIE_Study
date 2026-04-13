

# 線性代數（上）

[ ]  
$C=\begin{bmatrix}1\\3\end{bmatrix}\in \mathbb{R}^{2\times 1},\ D=\begin{bmatrix}1\\1\\0\\1\end{bmatrix}\in \mathbb{R}^{4\times 1}$ 都是列矩陣。

$E=\begin{bmatrix}1&1\\0&2\end{bmatrix}$ 為 $2$ 階方陣，$F=\begin{bmatrix}3&0&2\\0&4&2\\1&0&5\end{bmatrix}$ 為 $3$ 階方陣。

且 $1、2$ 為 $E$ 的對角項；$3、4、5$ 為 $F$ 的對角項。

> **定義** 對角矩陣(diagonal matrix)、單位矩陣(identity matrix)
>
> 若一 $n$ 階方陣的非對角項均為 $0$，則稱之為一對角矩陣，也記成 $\operatorname{diag}(d_1,\ldots,d_n)$，其中 $d_i$ 為第 $i$ 對角項。
>
> 若一 $n$ 階對角矩陣滿足對角項全 $1$，則稱之為一單位矩陣，記成 $I_n$。

> **定義** Note
>
> 若為 $n$ 階方陣且元素全 $1$，則記成 $1_n$ 或 $J_n$。

例如：

$A=\begin{bmatrix}1&0\\0&2\end{bmatrix}=\operatorname{diag}(1,2),\ B=\begin{bmatrix}1&0&0&0\\0&0&0&0\\0&0&1&0\\0&0&0&-1\end{bmatrix}=\operatorname{diag}(1,0,1,-1).$

$I_1=\begin{bmatrix}1\end{bmatrix},\ I_2=\begin{bmatrix}1&0\\0&1\end{bmatrix},\ I_3=\begin{bmatrix}1&0&0\\0&1&0\\0&0&1\end{bmatrix},\ I_4=\begin{bmatrix}1&0&0&0\\0&1&0&0\\0&0&1&0\\0&0&0&1\end{bmatrix}$

$J_3=\begin{bmatrix}1&1&1\\1&1&1\\1&1&1\end{bmatrix}$