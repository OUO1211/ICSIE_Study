## 對稱矩陣(symmetric matrix)與斜對稱矩陣(skew symmetric matrix)

> **考慮 \(n\) 階方陣 \(A\)，**
>
> (1) 若 \(A^T = A\)，則稱 \(A\) 為對稱矩陣。即 \(A = [a_{ij}]_{n \times n}\)，滿足 \(a_{ij} = a_{ji}\)。
>
> (2) 若 \(A^T = -A\)，則稱 \(A\) 為斜對稱矩陣。即若 \(A = [a_{ij}]_{n \times n}\)，滿足 \(a_{ij} = -a_{ji}\)，必有 \(a_{ii} = 0,\ \forall i\)。

例如：

$$(A=\begin{bmatrix}1&2\\2&3\end{bmatrix})，(B=\begin{bmatrix}1&2&3\\2&0&4\\3&4&5\end{bmatrix})，均為對稱矩陣，(C=\begin{bmatrix}0&-4&5\\4&0&-2\\-5&2&0\end{bmatrix}) 為斜對稱矩陣。$$

**Note**

(1) 有些版本將「斜對稱」稱為「反對稱」。

(2) 任一 \(n\) 階方陣可表為一對稱矩陣與斜對稱矩陣之和。

【110 台大資工】

## 厄米特矩陣(Hermitian matrix)與斜厄米特矩陣(skew Hermitian matrix)

> **考慮 \(n\) 階方陣 \(A\)，**
>
> (1) 若 \(A^H = A\)，則稱 \(A\) 為 Hermitian 矩陣。
>
> (2) 若 \(A^H = -A\)，則稱 \(A\) 為斜 Hermitian 矩陣。

例如：

$$
A=\begin{bmatrix}
1&i&6+3i\\
-i&4&-7\\
6-3i&-7&8
\end{bmatrix}
\text{ 為 Hermitian matrix,}
$$

$$
B=\begin{bmatrix}
i&0&3-i\\
0&-i&5i\\
-3-i&5i&0
\end{bmatrix}
\text{ 為 skew-Hermitian matrix.}
$$

> **例題 6**
>
> $$Let (A=\begin{bmatrix}1&-1\\-1&2\end{bmatrix}), (B=\begin{bmatrix}2&1\\0&1\end{bmatrix}), (C=\begin{bmatrix}2&i\\-i&1\end{bmatrix}), (D=\begin{bmatrix}i&1\\-1&i\end{bmatrix}), and (E=\begin{bmatrix}i&0\\0&2i\end{bmatrix}).$$
>
> (1) List matrices that are symmetric. (2) List matrices that are Hermitian.

**解**

(1) \(A\), \(D\), \(E\) 都是 symmetric。

(2) \(A\), \(C\) 都是 Hermitian。

【109 交大資工】