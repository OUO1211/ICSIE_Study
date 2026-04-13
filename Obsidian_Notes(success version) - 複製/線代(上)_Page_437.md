（接上頁試題 6 的後半）

則存在 $u \in U$，$v \in V \cap W$，使 $x = u + v$，

由 $u \in U$，$v \in V$，故 $u + v \in (U + V)$，

由 $U \subseteq W$，故 $u \in W$，又由 $v \in V \cap W$，故 $v \in W$，$\therefore u + v \in W$，

$\therefore x = u + v \in (U + V) \cap W$。

> **試題 7**
>
> 生成集局部裁減定理 一令 $S$ 為向量空間 $V$ 的一個子集合，若 $S$ 不為獨立集，則存在 $u \in S$ 使 $\operatorname{span}(S - \{u\}) = V$。

解 因為 $S$ 為線性相依，故存在 $v_1, v_2, \ldots, v_k \in S$，$\alpha_1, \alpha_2, \ldots, \alpha_k \in F$ 不全為 $0$，

使得 $\alpha_1 v_1 + \alpha_2 v_2 + \cdots + \alpha_k v_k = 0$，設 $\alpha_1 \neq 0$，

則得 $v_1 = \dfrac{-\alpha_2}{\alpha_1} v_2 + \cdots + \dfrac{-\alpha_k}{\alpha_1} v_k$，則取 $u = v_1$，得 $u \in \operatorname{span}(S - \{u\})$，

又因 $S$ 生成 $V$，故 $S - \{u\}$ 亦生成 $V$。

> **試題 8**
>
> 獨立集局部擴增定理 一令 $S$ 為向量空間 $V$ 的一個獨立子集合，若 $S$ 不生成 $V$，則存在 $u \in V - S$ 使 $S \cup \{u\}$ 仍為獨立集。

解

因為 $S$ 不生成 $V$，故存在 $u \in V - \operatorname{span}(S)$，

欲證得 $S \cup \{u\}$ 為線性獨立，

任取 $S \cup \{u\}$ 中的有限個向量 $v_1, v_2, \ldots, v_k$，設 $\alpha_1 v_1 + \alpha_2 v_2 + \cdots + \alpha_k v_k = 0$，

若 $u \neq v_i$，$\forall i = 1, 2, \ldots, k$，

$\because S$ 為線性獨立，則 $\alpha_i = 0$，$\forall i = 1, 2, \ldots, k$。

若 $u = v_i$，for some $i = 1, 2, \ldots, k$，（設為 $v_1$）

則 $\alpha_1$ 必為 $0$，（否則 $u = v_1 = \dfrac{-\alpha_2}{\alpha_1} v_2 + \cdots + \dfrac{-\alpha_k}{\alpha_1} v_k \in \operatorname{span}(S)$，矛盾）

即 $\alpha_2 v_2 + \cdots + \alpha_k v_k = 0$，又因 $v_2, \ldots, v_k$ 為線性獨立集，故 $\alpha_2 = \cdots = \alpha_k = 0$，故 $\alpha_1 = \alpha_2 = \cdots = \alpha_k = 0$，故 $S \cup \{u\}$ 為線性獨立集。