212
離散數學（上）

則很明顯 $\bigcup_{i \in N} A_i \sim N \times N \sim N$ ，所以 $\bigcup_{i \in N} A_i$ 為可數集。
而若 $\left\{A_i\right\}_{i \in N}$ 中的元素不全相異或 $A_i$ 為有限集合時，cardinality 顯然要比上述狀況的元素還要少，故亦為可數集。
（7）$Q^{-}=\left\{-x \mid x \in Q^{+}\right\}$為所有負有理數所成集合，則 $\left|Q^{-}\right|=\left|Q^{+}\right|$，且 $Q^{+}$為可數集，所以 $Q=Q^{-} \cup\{0\} \cup Q^{+}$為可數集。
（8）$R=Q \cup \bar{Q}$ ，其中， $\bar{Q}$ 為所有無理數所成集合。
已知 $Q$ 為可數集，若 $\bar{Q}$ 亦為可數集，則由（5）知 $R$ 亦為可數集，但此與（9）矛盾。故 $\bar{Q}$ 為不可數集。
（9）設 $(0,1)$ 為可數集，則因為 $(0,1)$ 不為有限集，故必為可列舉的，即存在 $f: N \xrightarrow{1-1, \text { onto }}(0,1)$ 如下：
$$
\begin{aligned}
& f(1)=0 . a_{11} a_{12} a_{13} \ldots \\
& f(2)=0 . a_{21} a_{22} a_{23} \ldots \\
& \quad \vdots \quad, \quad \text { 其中, } a_{i j} \in\{0, \ldots, 9\}, \quad \forall i, j, \\
& f(n)=0 . a_{n 1} a_{n 2} a_{n 3} \ldots \\
& \quad \vdots \\
& \text { 令 } s=0 . s_1 s_2 \ldots, \text { 其中 } s_i=\left\{\begin{array}{lll}
1 & \text { if } & a_{i i} \neq 1 \\
2 & \text { if } & a_{i i}=1
\end{array} \forall i=1,2, \ldots\right.
\end{aligned}
$$

則 $s \in(0,1)$ 且 $s \neq f(j), \forall j=1,2, \ldots$
即找到了一個介於 0 到 1 中間的實數，但卻沒有被 $f$ 映到，與 $f$ 為 onto 矛盾，故得 $(0,1)$ 不為可數集合。
（10）已知 $(0,1)$ 為不可數集，而 $(0,1) \subset R$ ，故實數集 $R$ 為不可數集。