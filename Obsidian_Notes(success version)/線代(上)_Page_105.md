# 第一章 矩陣 104

且

$$
\begin{bmatrix}
I & -B(C - B^T A^{-1}B)^{-1} \\
O & I
\end{bmatrix}
\begin{bmatrix}
A & B \\
O & C - B^T A^{-1}B
\end{bmatrix}
=
\begin{bmatrix}
A & O \\
O & C - B^T A^{-1}B
\end{bmatrix}.
$$

又

$$
\begin{bmatrix}
A^{-1} & O \\
O & (C - B^T A^{-1}B)^{-1}
\end{bmatrix}
\begin{bmatrix}
A & O \\
O & C - B^T A^{-1}B
\end{bmatrix}
=
\begin{bmatrix}
I & O \\
O & I
\end{bmatrix}.
$$

整理得

$$
\begin{bmatrix}
A^{-1} & O \\
O & (C - B^T A^{-1}B)^{-1}
\end{bmatrix}
\begin{bmatrix}
I & -B(C - B^T A^{-1}B)^{-1} \\
O & I
\end{bmatrix}
\begin{bmatrix}
I & O \\
-B^T A^{-1} & I
\end{bmatrix}
\begin{bmatrix}
A & B \\
B^T & C
\end{bmatrix}
=
\begin{bmatrix}
I & O \\
O & I
\end{bmatrix}.
$$

乘開得

$$
L^{-1}
=
\begin{bmatrix}
A^{-1} + A^{-1}B(C - B^T A^{-1}B)^{-1}B^T A^{-1} & (-A^{-1}B)(C - B^T A^{-1}B)^{-1} \\
-(C - B^T A^{-1}B)^{-1}B^T A^{-1} & (C - B^T A^{-1}B)^{-1}
\end{bmatrix}
=
\begin{bmatrix}
E & F \\
F^T & G
\end{bmatrix}.
$$

$\therefore E = A^{-1} + A^{-1}B(C - B^T A^{-1}B)^{-1}B^T A^{-1}$，$G = (C - B^T A^{-1}B)^{-1}$。

**Note：** 本題另需宣告 $A, C$ 為對稱矩陣，則可驗證
$(-(C - B^T A^{-1}B)^{-1}B^T A^{-1})^T = (-A^{-1}B)(C - B^T A^{-1}B)^{-1}$。

另外，因為題目先宣告 $L^{-1}$ 存在，即 $L$ 可逆，故由 $(*)$ 可推得 $C - B^T A^{-1}B$ 可逆。

> **試題 11**
>
> (10%) Let $A$, $B$, and $C$ are matrices and $\bar{x}, \bar{y}, \bar{z}$ are vectors. If $C^{-1} = A^{-1} + B^{-1}$ and $C^{-1}\bar{z} = A^{-1}\bar{x} + B^{-1}\bar{y}$, then show that $\bar{z} = \bar{x} + (I + AB^{-1})^{-1}(\bar{y} - \bar{x})$.
>
> 【105 政大統計】

**解**（本題題目有誤，應該是 $\bar{z} = \bar{x} + (I + BA^{-1})^{-1}(\bar{y} - \bar{x})$）

$$
A^{-1} + B^{-1} = B^{-1}BA^{-1} + B^{-1}AA^{-1} = B^{-1}(B + A)A^{-1}
$$

$$
\therefore C = (A^{-1} + B^{-1})^{-1} = (B^{-1}(B + A)A^{-1})^{-1} = A(A + B)^{-1}B，
$$

另外，

$$
A^{-1} + B^{-1} = A^{-1}BB^{-1} + A^{-1}AB^{-1} = A^{-1}(B + A)B^{-1}
$$

$$
\therefore C = (A^{-1} + B^{-1})^{-1} = (A^{-1}(B + A)B^{-1})^{-1} = B(A + B)^{-1}A。
$$

$$
\therefore \bar{z} = C(A^{-1}\bar{x} + B^{-1}\bar{y}) = CA^{-1}\bar{x} + CB^{-1}\bar{y}
$$

$$
= B(A + B)^{-1}AA^{-1}\bar{x} + A((A + B)^{-1}B)B^{-1}\bar{y}
$$

$$
= B(A + B)^{-1}\bar{x} + A(A + B)^{-1}\bar{y}
$$

$$
= (A + B)(A + B)^{-1}\bar{x} - A(A + B)^{-1}\bar{x} + A(A + B)^{-1}\bar{y}
$$

$$
= \bar{x} + A(A + B)^{-1}(\bar{y} - \bar{x})
$$

$$
= \bar{x} + (A^{-1})^{-1}(A + B)^{-1}(\bar{y} - \bar{x})
$$

$$
= \bar{x} + ((A + B)A^{-1})^{-1}(\bar{y} - \bar{x})
$$

$$
= \bar{x} + (I + BA^{-1})^{-1}(\bar{y} - \bar{x}).
$$