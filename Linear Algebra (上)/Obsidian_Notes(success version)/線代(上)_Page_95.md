# 第一章 矩陣 94

## PLU 分解

> 
>
 給定 階方陣 $A$，若 $A$ 無法做 $LU$ 分解，但 $A$ 完成列交換後可做 $LU$ 分解，則存在置換矩陣 (permutation) $P$、下三角矩陣 $L$、上三角矩陣 $U$，使得 $A=P^TLU$，並稱此為 $A$ 的一個 $P^TLU$ 分解。

> **Note**
>
> (1) 做 $P^TLU$ 分解的步驟：
>
> Step1 對 $A$ 列交換，直到 $A$（或成為 $B$）的各領導主子行列式均非零。
>
> Step2 對 $B$ 做 $LU$ 分解。
>
> Step3 對 $A$ 做的各列運算所對應的基本矩陣乘積合為 $P$。
>
> Step4 由 $PA=B=LU$，得 $A=P^TLU$。
>
> (2) $P$ 為正交矩陣，滿足 $P^{-1}=P^T$。
>
> (3) $P$ 不一定唯一。
>
> (4) 也可討論 $P^TLDU$ 分解。

> **例題 7**
>
> Find the $PA=LU$ factorization for
> $A=\begin{bmatrix} 1 & 1 & 1 \\ 1 & 1 & 3 \\ 2 & 5 & 8 \end{bmatrix}$。
>
> 【104 台大工材】

**解**

$$
A=\begin{bmatrix} 1 & 1 & 1 \\ 1 & 1 & 3 \\ 2 & 5 & 8 \end{bmatrix}
\to
\underbrace{\begin{bmatrix} 1 & 1 & 1 \\ 2 & 5 & 8 \\ 1 & 1 & 3 \end{bmatrix}}_{PA}
\xrightarrow{r_{12}^{(-2)},\ r_{13}^{(-1)}}
\begin{bmatrix} 1 & 1 & 1 \\ 0 & 3 & 6 \\ 0 & 0 & 2 \end{bmatrix}
=U,
$$

即

$$
(R_{13}^{(-1)}R_{12}^{(-2)})PA=U
$$

$$
\therefore\ PA=R_{12}^{(2)}R_{13}^{(1)}U
=
\begin{bmatrix} 1 & 0 & 0 \\ 2 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix}
\begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 1 & 0 & 1 \end{bmatrix}
\begin{bmatrix} 1 & 1 & 1 \\ 0 & 3 & 6 \\ 0 & 0 & 2 \end{bmatrix}
=
\underbrace{\begin{bmatrix} 1 & 0 & 0 \\ 2 & 1 & 0 \\ 1 & 0 & 1 \end{bmatrix}}_{L}
\underbrace{\begin{bmatrix} 1 & 1 & 1 \\ 0 & 3 & 6 \\ 0 & 0 & 2 \end{bmatrix}}_{U}
$$

且

$$
P=R_{23}=
\begin{bmatrix}
1 & 0 & 0 \\
0 & 0 & 1 \\
0 & 1 & 0
\end{bmatrix}
$$