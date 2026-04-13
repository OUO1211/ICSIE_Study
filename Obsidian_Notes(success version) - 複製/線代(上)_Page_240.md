**解** (1) False.

反例如 $A=\begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}$，$B=\begin{bmatrix} 0 & 1 \\ -1 & 0 \end{bmatrix}$，$AB=\begin{bmatrix} -1 & 0 \\ 0 & 1 \end{bmatrix}$，$BA=\begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix}$

(2) True.

$\because \det(A+B)=\det(A+BA^{-1}A)=\det[(I+BA^{-1})A]=\det(I+BA^{-1})\det(A)$，

又 $\det(A)\neq 0$，所以 $\det(A+B)=0 \Leftrightarrow \det(I+BA^{-1})=0$。

> **試題 5**
>
> Let $A^2=I=B^2$，$\det(A)+\det(B)=0$. Prove that $\det(A+B)=0$.
>
> **解** $A(A+B)=A^2+AB=I+AB；\ (A+B)B=AB+B^2=AB+I；$
>
> $\therefore A(A+B)=(A+B)B。$
>
> $\therefore \det(A)\det(A+B)=\det(A+B)\det(B)，$
>
> 若 $\det(A+B)\neq 0$，則得 $\det(A)=\det(B)$，
>
> 又由題意 $\det(A)+\det(B)=0$，得 $\det(A)=\det(B)=0$，即 $A$ 不可逆；
>
> 但 $A^2=I$，故 $A$ 可逆，矛盾。
>
> 故得證。

> **試題 6**
>
> If $P_1$ is an even permutation matrix and $P_2$ is an odd permutation matrix, deduce from $P_1+P_2=P_1(P_1^T+P_2^T)P_2$ that $\det(P_1+P_2)=0$. 【99 台大土木】
>
> **解** $P_1$ 是偶排列矩陣，是指 $P_1$ 是由 $I$ 經偶次列交換所得的矩陣，所以 $\det(P_1)=(-1)^{\text{偶次}}=1；$
>
> $P_2$ 是奇排列矩陣，是指 $P_2$ 是由 $I$ 經奇次列交換所得的矩陣，所以 $\det(P_2)=(-1)^{\text{奇次}}=-1；$
>
> 因為 $P_1+P_2=P_1(P_1^T+P_2^T)P_2$
>
> $\therefore \det(P_1+P_2)=\det[P_1(P_1^T+P_2^T)P_2]=\det(P_1)\det(P_1^T+P_2^T)\det(P_2)=-\det(P_1+P_2)^T$
>
> $\therefore \det(P_1+P_2)=0。$