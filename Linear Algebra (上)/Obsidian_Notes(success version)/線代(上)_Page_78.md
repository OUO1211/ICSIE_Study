## 可逆與列運算

> **定理：可逆與列運算**
>
> 考慮 $n$ 階方矩陣 $A$，則
>
> $A$ 可逆 $\Leftrightarrow$ $A$ 可以由若干列基本矩陣的乘積。
>
> 〔103 暨南資工、110 政大應數〕

**【證明】**

設 $A$ 可逆，則 $A$ 可列運算至 $I_n$。

設對應的列基本矩陣為 $E_1, \ldots, E_k$，使得 $(E_k \cdots E_1)A = I$。

即 $A = (E_k \cdots E_1)^{-1} = E_1^{-1} \cdots E_k^{-1}$ 為列基本矩陣的乘積。

反之，列基本矩陣的均可逆，故列基本矩陣的乘積亦可逆，故 $A$ 可逆。

**Note**

以上結論若以行運算描述，則可改為：

$n$ 階方陣 $A$ 可逆 $\Leftrightarrow$ $A$ 可表為若干行基本矩陣的乘積。

> **例題 3**
>
> Consider the matrix $A = \begin{bmatrix} 1 & 2 \\ 2 & 3 \end{bmatrix}$.
>
> (1) Find the elementary matrix $E_1$, $E_2$ such that $E_1 E_2 A = I$.
>
> (2) Write $A^{-1}$ as product of elementary matrices.
>
> (3) Write $A$ as product of elementary matrices.
>
> 〔99 高科電通、100 中央資工頻道、92 海洋資料〕
>
> **解：**
>
> (1) $A = \begin{bmatrix} 1 & 2 \\ 2 & 3 \end{bmatrix} \xrightarrow{r_{21}^{(-2)}} \begin{bmatrix} 1 & 2 \\ 0 & -1 \end{bmatrix} \xrightarrow{r_2^{(-1)}} \begin{bmatrix} 1 & 2 \\ 0 & 1 \end{bmatrix} \xrightarrow{r_{12}^{(-2)}} \begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix} = I$
>
> 即 $E_1 = R_{21}^{(-2)} = \begin{bmatrix} 1 & 0 \\ -2 & 1 \end{bmatrix}$，$E_2 = R_2^{(-1)} = \begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix}$
>
> (2) 由 (1) 得 $A^{-1} = R_{12}^{(-2)} R_2^{(-1)} R_{21}^{(-2)} = \begin{bmatrix} 1 & -2 \\ 0 & 1 \end{bmatrix} \begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix} \begin{bmatrix} 1 & 0 \\ -2 & 1 \end{bmatrix}$
>
> (3) 由 (1) 得 $A = (R_{21}^{(-2)})^{-1}(R_2^{(-1)})^{-1}(R_{12}^{(-2)})^{-1} = R_{21}^{(2)} R_2^{(-1)} R_{12}^{(2)} = \begin{bmatrix} 1 & 0 \\ 2 & 1 \end{bmatrix} \begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix} \begin{bmatrix} 1 & 2 \\ 0 & 1 \end{bmatrix}$
