> **例 11**
>
> True or false:
>
> (1) Let $A$ be an $n \times n$ matrix such that $A^k = I$ for some positive integer $k$, then $A$ is invertible.
>
> 【105 成大數學】
>
> (2) If $A$ and $B$ are $n \times n$ matrices. If $n$ is odd and $AB = -BA$, then either $A$ or $B$ is not invertible.
>
> 【邱政文機數、100 台北聯】
>
> (3) If the entries of $A$ and $A^{-1}$ are all integers, then $\det(A)$ is 1 or $-1$.
>
> 【88 中央資工、93 師大資工、98 政大統計】

**解**

(1) True.

$1 = \det(I) = \det(A^k) = \det(A)^k$，$\therefore \det(A) \neq 0$，故 $A$ 可逆。

(2) True.

$\because \det(A)\det(B) = \det(AB) = \det(-BA) = (-1)^n\det(BA) = -\det(B)\det(A)$，

$\therefore \det(A)\det(B) = 0$，故 $\det(A) = 0$ 或 $\det(B) = 0$。

(3) True.

$\because 1 = \det(I) = \det(A \cdot A^{-1}) = \det(A)\det(A^{-1})$，又 $A \in \mathbb{Z}^{n \times n}$，$\det(A) \in \mathbb{Z}$，

故 $\det(A) = 1$ 或 $\det(A) = -1$（即 $\det(A^{-1}) = \det(A^{-1})$）。
