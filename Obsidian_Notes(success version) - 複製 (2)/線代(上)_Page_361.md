前面 $A$ 的行空間時，稍微用到，若 $A$ 與 $B$ 列等價，則 $B$ 的 pivot element 所在行，對應回 $A$，可為 $A$ 的 $CS(A)$ 的基底。（前面這個規律可由前述所行的（把舊式 $\#$ $A$ 的列轉換，且舊的 pivot 在 $B^{(1)}$，$B^{(2)}$，$B^{(k)}$（即 $A^{(1)}, A^{(2)}, A^{(k)}$ 可為 $CS(A)$ 的一組基底。））

【97 暨南資工】

> **例題 18**
>
> Let $U = \begin{bmatrix} 1 & 0 & 0 & 0 & 1 \\ 0 & 1 & 0 & -1 \\ 0 & 0 & 0 & 1 & 1 \\ 0 & 0 & 0 & 0 & 0 \end{bmatrix}$ be the row reduced echelon matrix of the matrix $A$. Prove or disprove that the first, second and the fourth columns of $A$ form a basis for the column space of $A$.
>
> 【91 中央數學】

**解**

令 $A$ 的行向量為：$A^{(1)}, A^{(2)}, A^{(3)}, A^{(4)}, A^{(5)}$，欲證明 $A^{(1)}, A^{(2)}, A^{(4)}$ 為線性獨立，

設 $\alpha A^{(1)} + b A^{(2)} + c A^{(4)} = 0$，即 $aA^{(1)} + bA^{(2)} + 0A^{(3)} + cA^{(4)} + 0A^{(5)} = 0$，

則 $\begin{bmatrix} a \\ b \\ 0 \\ c \\ 0 \end{bmatrix} \in \ker(A)$，

但 $A \sim U$，$\ker(A) = \ker(U)$，故得 $U \begin{bmatrix} a \\ b \\ 0 \\ c \\ 0 \end{bmatrix} = 0$，

設 $U$ 的行向量為：$U^{(1)}, U^{(2)}, U^{(3)}, U^{(4)}, U^{(5)}$，

得 $aU^{(1)} + bU^{(2)} + 0U^{(3)} + cU^{(4)} + 0U^{(5)} = 0$，

則 $a U^{(1)} + b U^{(2)} + c U^{(4)} = 0$，即 $a\begin{bmatrix} 1 \\ 0 \\ 0 \\ 0 \end{bmatrix} + b\begin{bmatrix} 0 \\ 1 \\ 0 \\ 0 \end{bmatrix} + c\begin{bmatrix} 0 \\ -1 \\ 1 \\ 0 \end{bmatrix} = 0$，得 $a = b = c = 0$，

又因 $\dim CS(A) = rank(A) = rank(U) = 3$，

故 $\{A^{(1)}, A^{(2)}, A^{(4)}\}$ 為 $CS(A)$ 的一組基底。
