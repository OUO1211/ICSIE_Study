> **例題 8**
>
> Determine which of the following are bases for the vector space of $2 \times 2$ matrices.
>
> (1) $\left\{ \begin{bmatrix} 1 & 2 \\ 0 & 1 \end{bmatrix}, \begin{bmatrix} 3 & 4 \\ 1 & 1 \end{bmatrix}, \begin{bmatrix} 1 & 2 \\ 1 & 1 \end{bmatrix}, \begin{bmatrix} 0 & 2 \\ 1 & 2 \end{bmatrix} \right\}$
> (2) $\left\{ \begin{bmatrix} 1 & 0 \\ 0 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 1 \\ 0 & 0 \end{bmatrix}, \begin{bmatrix} 1 & 2 \\ 3 & 0 \end{bmatrix}, \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix} \right\}$
>
> 【95 中興資料】

**解**

(1) 考慮以其 entry 排成列向量所成矩陣 $\begin{bmatrix} 1 & 2 & 0 & 1 \\ 3 & 4 & 1 & 1 \\ 1 & 2 & 1 & 1 \\ 0 & 2 & 1 & 2 \end{bmatrix}$，

列運算後可得 $\begin{bmatrix} 1 & 2 & 0 & 1 \\ 0 & -2 & 1 & -2 \\ 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & 0 \end{bmatrix}$，

即此四向量為線性相依，故不為基底。

(2) 考慮以其 entry 排成列向量所成矩陣 $\begin{bmatrix} 1 & 0 & 0 & 0 \\ 0 & 1 & 0 & 0 \\ 1 & 2 & 3 & 0 \\ 1 & 2 & 3 & 4 \end{bmatrix}$，

$\because \det = 24$，

$\therefore$ 此四個向量為線性獨立，又因 $\dim(M_{2\times2}) = 4$ 為 $M_{2\times2}$ 的基底。

> **例題 9**
>
> $L=\left\{ \begin{bmatrix} a & b \\ c & d \end{bmatrix} \in M_2(R) \mid a+d=0 \right\}$. Find the dimension of $L$.

**解**

$L=\left\{ \begin{bmatrix} a & b \\ c & -a \end{bmatrix} \mid a,b,c \in R \right\}=span\left\{ \begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix}, \begin{bmatrix} 0 & 1 \\ 0 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 0 \\ 1 & 0 \end{bmatrix} \right\}$，

又因為顯即可得 $\begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix}, \begin{bmatrix} 0 & 1 \\ 0 & 0 \end{bmatrix}, \begin{bmatrix} 0 & 0 \\ 1 & 0 \end{bmatrix}$ 為線性獨立集，

故 $S$ 可為 $L$ 一組基底且 $\dim(L)=3$。