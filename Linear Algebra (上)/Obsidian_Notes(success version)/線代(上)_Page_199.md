> **例 9**
>
> Let $A = \begin{bmatrix} a & b & c \\ p & q & r \\ u & v & w \end{bmatrix}$, $B = \begin{bmatrix} 2p & -a+u & 3u \\ 2q & -b+v & 3v \\ 2r & -c+w & 3w \end{bmatrix}$, and assume that $\det A = 3$. Compute the following determinants: (1) $\det(-A^4)$, (2) $\det(A^{-1})$, (3) $\det(A^T)$, (4) $\det(2B^{-1})$.
>
> 【98,99 台大資工、106 高師應數離散、108 成大數學】

**解**

(1) $\det(-A^4) = (-1)^3 \det(A)^4 = -81$。

(2) $\det(A^{-1}) = \dfrac{1}{\det(A)} = \dfrac{1}{3}$。

(3) $\det(A^T) = \det(A) = 3$。

(4) $\det(B) = 2 \cdot 3 \cdot \begin{vmatrix} p & -a+u & u \\ q & -b+v & v \\ r & -c+w & w \end{vmatrix} = 6 \begin{vmatrix} p & -a & u \\ q & -b & v \\ r & -c & w \end{vmatrix} = -6 \begin{vmatrix} p & a & u \\ q & b & v \\ r & c & w \end{vmatrix} = 6 \begin{vmatrix} a & p & u \\ b & q & v \\ c & r & w \end{vmatrix} = 6 \begin{vmatrix} a & b & c \\ p & q & r \\ u & v & w \end{vmatrix} = 18$，

$\therefore \det(2B^{-1}) = 2^3 \det(B)^{-1} = \dfrac{8}{18}$。

---

> **例 10**
>
> $A = \begin{bmatrix} 0 & 1 & 2 & 0 \\ 0 & 5 & 0 & -1 \\ 2 & 0 & 3 & 4 \\ 0 & -1 & 1 & 0 \end{bmatrix}$. Compute the following determinants:
>
> (1) $(4\%)$ $\det(A)$, (2) $(4\%)$ $\det(2A^{-1})$, (3) $(4\%)$ $\det(A^T A)$, (4) $(8\%)$ $\det(A^T - A)$.
>
> 【110 台北工工】

**解**

(1) $\det(A) = 6$。

(2) $\det(2A^{-1}) = 2^4 \det(A^{-1}) = 16/6$。

(3) $\det(A^T A) = \det(A^T)\det(A) = \det(A)\det(A) = 36$。

(4) $\det(A^T - A) = \det\left(\begin{bmatrix} 0 & 0 & 2 & 0 \\ 1 & 5 & 0 & -1 \\ 2 & 0 & 3 & 1 \\ 0 & -1 & 4 & 0 \end{bmatrix} - \begin{bmatrix} 0 & 1 & 2 & 0 \\ 0 & 5 & 0 & -1 \\ 2 & 0 & 3 & 4 \\ 0 & -1 & 1 & 0 \end{bmatrix}\right) = \begin{vmatrix} 0 & -1 & 0 & 0 \\ 1 & 0 & 0 & 0 \\ 0 & 0 & 0 & -3 \\ 0 & 0 & 3 & 0 \end{vmatrix} = 9$。