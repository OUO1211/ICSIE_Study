又因 $V_1 \cap V_2 = \{0\}$，即 $w_1 = w_2 = 0$，$w_3 = w_2 = 0$。
即得 $w_1 = w_2 = w_3 = w_4 = 0$，且 $V_1 \cap V_2 = \{0\}$，故矩陣法一一。

(3) False.

考慮 $\beta^2$，令 $V_1 = \text{span}(\{1,0\})$，$V_2 = \text{span}(\{1,1\})$，
則 $V_1 \cap V_2 = \{0\}$，$V_1 + V_2 = V_1 \oplus V_2$。

固為 $(1,1) = 1(1,0) + 0(0,1) = 0(1,0) + 1(1,1)$，故 $(1,1)$ 在 $V_1 \cup V_2$ 中的表達法不唯一。

---

> **試題 18**
>
> Define $W_1 = \{A \in M_{2\times 2} \mid A_{ij} = 0, \text{ for } i \leq j\}$ and $W_2$ to be the set of all symmetric $n$ by $n$ matrices with entries from $R$. Both $W_1$ and $W_2$ are subspaces of $M_{n\times n}(R)$.
>
> 先證 $F = M_{2\times 2}(R)$
>
> 【97 政大光電】

> **解**
>
> 令 $F = M_{2\times 2}(R)$
>
> 已知 $W_1 + W_2 \subseteq F$，又 $A = \begin{bmatrix} a & b \\ c & d \end{bmatrix} \in F$，令
>
> $$A = \begin{bmatrix} 0 & 0 \\ c-b & 0 \end{bmatrix} + \begin{bmatrix} a & b \\ b & d \end{bmatrix} \in W_1 + W_2$$
>
> 以此 $F \subseteq W_1 + W_2$。
>
> 再證 $W_1 \cap W_2 = \{0\}$：
>
> $\forall A \in W_1 \cap W_2$，$\because A \in W_1$ 得上三角元素為 $0$；$A \in W_2$ 得 $A$ 為對稱矩陣，$\therefore A = O$，
>
> 故 $W_1 \cap W_2 = \{0\}$，得證 $F = W_1 \oplus W_2$。

---

> **試題 19**
>
> Let $F$ be a vector space and let $W_1$ and $W_2$ be two subspaces such that $V = W_1 \oplus W_2$. If $\beta_1$ and $\beta_2$ are disjoint bases for the subspaces $W_1$ and $W_2$, respectively, such that $\beta_1 \cup \beta_2$ is linearly independent, then $V = W_1 \oplus W_2$.
>
> 【100 中興應數】

> **解**
>
> Let $F$ be a vector space，$\beta_1$ 生成 $W_1$，$\beta_2$ 生成 $W_2$，因為 $\beta_1 \cup \beta_2$ 為線性獨立集合，故 $\dim(W_1 \cap W_2) = 0$，
>
> 故 $W_1 \cap W_2 = \{0\}$，故 $V = W_1 \oplus W_2$。
