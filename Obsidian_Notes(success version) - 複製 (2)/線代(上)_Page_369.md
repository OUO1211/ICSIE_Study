> **例題 20**
>
> (10%) Let $A = [a_1, a_2, a_3, a_4]$ be a $4 \times 4$ matrix with reduced row echelon form given by
>
> $$U = \begin{bmatrix} 1 & 0 & 2 & 1 \\ 0 & 1 & 1 & 4 \\ 0 & 0 & 0 & 0 \\ 0 & 0 & 0 & 0 \end{bmatrix}.$$
>
> If $a_1 = \begin{bmatrix} -3 \\ 5 \\ 2 \\ 1 \end{bmatrix}$ and $a_2 = \begin{bmatrix} 4 \\ -3 \\ 7 \\ -1 \end{bmatrix}$.
>
> (1) Find the rank of $A$.
>
> (2) Find a basis of null space of $A$.
>
> (3) Find $a_3$ and $a_4$.
>
> 【99 交大資工，106 佑大資工類組，109 交大資工】

**解**

(1) $rank(A) = rank(U) = 2$。

(2) $$null(A) = null(U) = \left\{ \begin{bmatrix} a \\ b \\ c \\ d \end{bmatrix} \middle| \begin{array}{l} a + 2c + d = 0 \\ b + c + 4d = 0 \end{array} \right\} = \left\{ \begin{bmatrix} -2c - d \\ -c - 4d \\ c \\ d \end{bmatrix} \middle| c, d \in \mathbb{R} \right\} = span\left\{ \begin{bmatrix} -2 \\ -1 \\ 1 \\ 0 \end{bmatrix}, \begin{bmatrix} -1 \\ -4 \\ 0 \\ 1 \end{bmatrix} \right\}.$$

又 $S$ 為獨立集，故可取 $S$ 為 $null(A)$ 的一組基底。

(3) $$U^{(3)} = 2U^{(1)} + 1U^{(2)}, \therefore a_3 = 2a_1 + a_2 = \begin{bmatrix} -2 \\ 7 \\ 11 \\ 1 \end{bmatrix}$$

$$U^{(4)} = U^{(1)} + 4U^{(2)}, \therefore a_4 = a_1 + 4a_2 = \begin{bmatrix} 13 \\ -7 \\ 30 \\ -3 \end{bmatrix}$$