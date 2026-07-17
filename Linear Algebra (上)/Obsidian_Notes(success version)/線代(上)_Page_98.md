# 第一章 矩陣 97

## PAQ 分解

> **定義**
>
> 給定矩陣 $A \in F^{m \times n}$，
>
> 則 $PAQ = \begin{bmatrix} I & O \\ O & O \end{bmatrix}$ 稱為 $A$ 的 PAQ 分解。
>
> 其中，$P$ 為 $m \times m$ 的可逆矩陣；$Q$ 為 $n \times n$ 的可逆矩陣，$I$ 為 $r \times r$ 的單位矩陣，$r$ 為 $A$ 化成列梯形矩陣後的非零列數。
>
> 【91 成大統計】

> **Note**
>
> (1) 將 $A$ 做列運算成列梯矩陣後，再做行運算使其成為簡化列梯矩陣。
>
> (2) 將各個列基本矩陣相乘即 $P$，將各個行基本矩陣相乘即 $Q$。

> **例題**
>
> Let $A = \begin{bmatrix} 1 & 1 & 0 & -1 \\ 3 & 2 & 1 & 1 \\ 1 & 0 & 1 & 3 \end{bmatrix}$. Find invertible $P$ and $Q$ that satisfy $PAQ = \begin{bmatrix} I & O \\ O & O \end{bmatrix}$.

**解**

$$\begin{bmatrix} 1 & 1 & 0 & -1 \\ 3 & 2 & 1 & 1 \\ 1 & 0 & 1 & 3 \end{bmatrix} \xrightarrow{r_2^{(-3)}, r_3^{(-1)}} \begin{bmatrix} 1 & 1 & 0 & -1 \\ 0 & -1 & 1 & 4 \\ 0 & -1 & 1 & 4 \end{bmatrix} \xrightarrow{r_3^{(-1)}} \begin{bmatrix} 1 & 1 & 0 & -1 \\ 0 & -1 & 1 & 4 \\ 0 & 0 & 0 & 0 \end{bmatrix}$$

$$\xrightarrow{c_{12}^{(1)}, c_{14}^{(-1)}} \begin{bmatrix} 1 & 0 & 0 & 0 \\ 0 & 1 & -1 & -4 \\ 0 & 0 & 0 & 0 \end{bmatrix} \xrightarrow{c_{13}^{(1)}, c_{14}^{(4)}} \begin{bmatrix} 1 & 0 & 0 & 0 \\ 0 & 1 & 0 & 0 \\ 0 & 0 & 0 & 0 \end{bmatrix}$$

故得

$$R_{32}^{(-1)} R_{31}^{(-1)} R_{21}^{(-3)} AC_{12}^{(1)} C_{14}^{(-1)} C_{13}^{(1)} C_{14}^{(4)} = \begin{bmatrix} I & O \\ O & O \end{bmatrix}$$

則得 $P = \begin{bmatrix} 1 & 0 & 0 \\ -3 & 1 & 0 \\ 2 & -1 & 1 \end{bmatrix}$，

$$Q = \begin{bmatrix} 1 & -1 & -1 & -3 \\ 0 & 1 & 1 & 4 \\ 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & 1 \end{bmatrix}$$