## 第 4 章 線性映射 585

> **試題 12**
>
> Let $T$ be the linear operator on $R^2$, the matrix of which in the standard ordered basis is $\begin{bmatrix}2&1\\0&2\end{bmatrix}$. Let $W_1$ be the subspace of $R^2$ spanned by the vector $e_1=(1,0)$.
>
> (1) Show that $W_1$ is invariant under $T$.
>
> (2) Prove that there is no subspace $W_2$ which is invariant under $T$ and which is complementary to $W_1$, (i.e., no subspace $W_2$ satisfying $R=W_1\oplus W_2$.)
>
> 【90 成大應數】

**解**

(1) 設 $\beta=\{e_1,e_2\}=\{(1,0),(0,1)\}$ 為 $R^2$ 的標準基底，即 $[T]_\beta=\begin{bmatrix}2&1\\0&2\end{bmatrix}$。

則得 $T(e_1)=2e_1=(2,0)$，$T(e_2)=e_1+2e_2=(1,2)$，

即 $T(xe_1+ye_2)=xT(e_1)+yT(e_2)=(2x+y,2y)$，

$\because W_1=\operatorname{span}\{e_1\}$，設 $v\in W_1$，則 $v=ae_1$，for some $a\in R$，

則 $T(v)=T(ae_1)=aT(e_1)=(2a,0)=2ae_1\in W_1$，故 $T(W_1)\subseteq W_1$。

(2) 若存在 $T$ 不變子空間 $W_2$ 使得 $R^2=W_1\oplus W_2$，

則因 $\dim(R^2)=\dim(W_1)+\dim(W_2)=1+\dim(W_2)$，得 $\dim(W_2)=1$。

令 $W_2$ 的一組基底向量為 $(a,b)\in R^2$，

則因 $R^2=W_1\oplus W_2$，得 $W_1\cap W_2=\{0\}$，$\therefore b\neq 0$。

又因若 $b=0$，則 $v\in W_1$，則得 $v\in W_1\cap W_2$，得 $v=0$，與「$v$ 為 $W_2$ 的一組基底」矛盾。

因 $T(W_2)\subseteq W_2$，$\therefore T(v)=\alpha v=\alpha(a,b)\in W_2$，for some $\alpha\in R$，

又 $T(v)=T(a,b)=(2a+b,2b)$，所以由
$$
\begin{cases}
\alpha a=2a+b\\
\alpha b=2b
\end{cases}
$$
得 $\alpha=2$，$b=0$，而得矛盾。

故不存在 $T$ 不變子空間 $W_2$ 使得 $R^2=W_1\oplus W_2$。