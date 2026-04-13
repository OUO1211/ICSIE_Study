> **試題 9**
>
> 代換定理 令 $S=\{v_1,\ldots,v_n\}$ 為向量空間 $V$ 的一個生成集，則對任意 $V$ 中的獨立集 $S_0=\{u_1,\ldots,u_m\}$，其中 $m<n$，存在 $S$ 的 $n-m$ 的子集 $S_1$，使 $S_0\cup S_1$ 生成 $V$。

解：對 $m$ 作歸納法，

$m=0$ 時 $S_0=\varnothing$，取 $S_1=S$，則 $S_1$ 含有 $n$ 個向量，且 $S_1\cup S_0=S$ 生成 $V$。

設 $m=k$，此命題成立。

則 $m=k+1$ 時，

因為 $S_0=\{u_1,u_2,\ldots,u_k,u_{k+1}\}$ 為線性獨立集，故 $\{u_1,u_2,\ldots,u_k\}$ 為線性獨立集，

而由歸納假設知存在 $v_{i_1},v_{i_2},\ldots,v_{i_{n-k}}\in S$，使 $\{u_1,u_2,\ldots,u_k\}\cup\{v_{i_1},v_{i_2},\ldots,v_{i_{n-k}}\}$ 生成 $V$。

因 $u_{k+1}\in V$，故存在 $\alpha_1,\alpha_2,\ldots,\alpha_k,\beta_1,\beta_2,\ldots,\beta_{n-k}\in F$ 使得
$$
u_{k+1}=\alpha_1u_1+\alpha_2u_2+\cdots+\alpha_ku_k+\beta_1v_{i_1}+\beta_2v_{i_2}+\cdots+\beta_{n-k}v_{i_{n-k}}.
$$

（其中 $\beta_1,\beta_2,\ldots,\beta_{n-k}$ 不全為 $0$，否則 $u_{k+1}$ 為 $u_1,u_2,\ldots,u_k$ 的線性組合，矛盾）

設 $\beta_1\neq 0$，則
$$
v_{i_1}=\frac{1}{\beta_1}\left(-\alpha_1u_1-\alpha_2u_2-\cdots-\alpha_ku_k-\beta_2v_{i_2}-\cdots-\beta_{n-k}v_{i_{n-k}}+u_{k+1}\right),
$$

即 $v_{i_1}\in span(\{u_1,u_2,\ldots,u_{k+1}\}\cup\{v_{i_2},v_{i_3},\ldots,v_{i_{n-k}}\})$，

故取 $S_1=\{v_{i_2},v_{i_3},\ldots,v_{i_{n-k}}\}$，則 $S_1$ 中有 $n-(k+1)$ 個向量，且滿足 $S_0\cup S_1$ 生成 $V$。

即 $m=k+1$ 時，命題亦成立。

> **試題 10**
>
> (10%) Let $W$ be a subspace of a vector space $V$. Show that if $\beta$ is a basis for $W$ and $v\in V\backslash \beta$, then $\beta\cup\{v\}$ is linearly independent if and only if $v\notin W$. 

解：假設 $\beta\cup\{v\}$ 線性獨立，若 $v\in W$，則因為 $\beta$ 是 $W$ 的一組基底，故 $v$ 可被 $\beta$ 線性組合而而得 $\beta\cup\{v\}$ 為一相依集。矛盾，故 $v\notin W$。

假設 $v\notin W$，若 $v$ 若可被 $\beta$ 線性組合，則 $v\in W$，故得 $\beta\cup\{v\}$ 為一線性獨立集。