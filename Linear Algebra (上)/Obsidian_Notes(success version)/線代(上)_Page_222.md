由(a)得 $\det\begin{bmatrix} A & B \\ C & D \end{bmatrix} = \det A \cdot \det(D - CA^{-1}B) = \det(AD - ACA^{-1}B)$

$= \det(AD - CAA^{-1}B) = \det(AD - CB)$。

> **例 14**
>
> Compute the determinant of each of the following matrices:
>
> $$A = \begin{bmatrix} 1 & -1 & -2 & 0 & 2 \\ 0 & 1 & 0 & 4 & 1 \\ 1 & 1 & 5 & 0 & 0 \\ 0 & 0 & 0 & 3 & -1 \\ 0 & 0 & 0 & 1 & 1 \end{bmatrix} \text{【104 雲科資工】} \quad B = \begin{bmatrix} 1 & 0 & 0 & 2 & 9 \\ 7 & 2 & 0 & 3 & 7 \\ 3 & 7 & 1 & 5 & -9 \\ 0 & 0 & 0 & -4 & 3 \\ 0 & 0 & 0 & 2 & 1 \end{bmatrix} \text{【109 台聯電機】}$$
>
> $$C = \begin{bmatrix} 3a & -7 & 8 & 9 & -6 \\ 0 & 2 & -5 & 7 & 7 \\ 0 & 0 & 1 & 5 & 0 \\ 0 & 0 & 2 & 4 & -1 \\ 0 & 0 & 0 & -2 & 0 \end{bmatrix} \text{【106 中山通訊】}$$

**解**

$$\det(A) = \begin{vmatrix} 1 & -1 & -2 \\ 0 & 1 & 0 \\ 1 & 1 & 5 \end{vmatrix} \cdot \begin{vmatrix} 3 & -1 \\ 1 & 1 \end{vmatrix} = 1 \cdot \begin{vmatrix} 1 & -2 \\ 3 & -1 \end{vmatrix} \cdot \begin{vmatrix} 5 & 1 \\ 1 & 1 \end{vmatrix} = 28$$

$$\det(B) = \begin{vmatrix} 1 & 0 & 0 \\ 7 & 2 & 0 \\ 3 & 7 & 1 \end{vmatrix} \cdot \begin{vmatrix} -4 & 3 \\ 2 & 1 \end{vmatrix} = 1 \cdot 2 \cdot 1 \cdot (-10) = -20$$

$$\det(C) = \begin{vmatrix} 3a & -7 \\ 0 & 2 \end{vmatrix} \cdot \begin{vmatrix} 1 & 5 & 0 \\ 2 & 4 & -1 \\ 0 & -2 & 0 \end{vmatrix} = 6a \cdot (-1) \cdot (-1)^{2+3} \begin{vmatrix} 1 & 5 \\ 0 & -2 \end{vmatrix} = -12a$$
