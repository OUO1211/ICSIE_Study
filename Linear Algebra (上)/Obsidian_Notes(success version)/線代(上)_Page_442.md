（接上頁試題 15 的後半）

設 $u \in N(AB)$，則 $ABu = 0$，則 $Bu \in N(A)$，又 $Bu \in R(B)$，且 $R(B) \cap N(A) = \{0\}$，

故 $Bu = 0$，則 $u \in N(B)$，故得 $N(AB) \subseteq N(B)$，

故得 $N(AB) = N(B)$。

> **試題 16**
>
> (10%) Given $A \in M_{m \times n}$ with $m \neq n$, prove that the set $\{B \in M_{n \times m} \mid AB = I_m\}$ is either empty or an infinite set.
>
> 【101 師大數學】

解：令 $S = \{B \in M_{n \times m} \mid AB = I_m\}$，

若 $S = \varnothing$，則得證；

否則令 $B \in S$，使 $AB = I_m$，故 $\operatorname{rank}(I_m) \leq \operatorname{rank}(A) \leq m$，即 $\operatorname{rank}(A) = m$，

且由 $\dim(\ker(A)) = n - \operatorname{rank}(A) > 0$，故可取任意 $(4)$ 中的向量 $u^1, \cdots, u^m$，由

$$
AB^{(1)} =
\begin{bmatrix}
1 \\
0 \\
\vdots \\
0
\end{bmatrix},
\ldots,
AB^{(m)} =
\begin{bmatrix}
0 \\
\vdots \\
0 \\
1
\end{bmatrix},
$$

得 $$A(B^{(1)} + u_1) =
\begin{bmatrix}
1 \\
0 \\
\vdots \\
0
\end{bmatrix},
\ldots,
A(B^{(m)} + u_m) =
\begin{bmatrix}
0 \\
\vdots \\
0 \\
1
\end{bmatrix}$$，

即存在無限多個 $C = [B^{(1)} + u_1, \cdots, B^{(m)} + u_m]$，使 $AC = I_m$，得證。

> **試題 17**
>
> Let $V_1, \ldots, V_m$ be nonzero subspaces of $R^n$.
>
> (1) What is the meaning of saying that $V_1 + \cdots + V_m$ is a direct sum?
>
> (2) Show that $V_1 + V_2$ is a direct sum if and only if $V_1 \cap V_2 = \{0\}$.
>
> (3) If $V_1 \cap V_2 = V_2 \cap V_3 = V_3 \cap V_1 = \{0\}$, is the sum $V_1, \ldots, V_m$ direct? Either give a proof or a counterexample.
>
> 【93 交大應數】

解：

(1) 若 $\forall v \in V_1 + V_2 + \cdots + V_m$，$v$ 可唯一表為 $v = v_1 + v_2 + \cdots + v_m$，其中 $v_i \in V_i$，$\forall i$，

則稱 $V_1 + V_2 + \cdots + V_m$ 為一個 direct sum。

(2) ($\Rightarrow$)：任取 $v \in V_1 \cap V_2$，則 $v \in V_1$ 且 $v \in V_2$，

而 $v = v + 0 = 0 + v \in V_1 + V_2$，且 $V_1 + V_2$ 中的向量表達法唯一，

故得 $v = 0$，即 $V_1 \cap V_2 = \{0\}$。

($\Leftarrow$)：取 $v \in V_1 + V_2$，設 $v = u_1 + u_2 = v_1 + v_2$，其中 $u_1, v_1 \in V_1$，$u_2, v_2 \in V_2$，

故 $u_1 - v_1 = v_2 - u_2 \in V_1 \cap V_2 = \{0\}$，故 $u_1 = v_1$，$u_2 = v_2$，

故 $V_1 + V_2$ 為 direct sum。