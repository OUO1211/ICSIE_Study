> **試題 4**
>
> Let $U = \{p(t): p(t) = a_0 + a_1t\}$ defined on $[-1,1]$ for some $a_0, a_1 \in R$ and $W = \{q(t): q(t) = b_0 + b_1t + b_2t^2\}$ defined on $[-1,1]$ for some $b_0, b_1, b_2 \in R$. Note $U$ and $W$ are vector spaces and having natural bases $S = \{p_1(t), p_2(t)\}$ and $T = \{q_1(t), q_2(t), q_3(t)\}$, where $T = \{q_1(t) = 1, q_2(t) = t, q_3(t) = t^2\}$ and $S = \{p_1(t) = 1, p_2(t) = t\}$, respectively. Let the linear mapping $L: U \to W$ be defined by $L(p(t)) = \int_{-1}^{t} p(x)dx$.
>
> (1) (12%) Please find $[L(p_1(t))]_T$ and $[L(p_2(t))]_T$, the coordinate vectors of $L(p_1(t))$ and $L(p_2(t))$ with respect to the ordered bases $S$ and $T$.
>
> (2) (6%) Find the matrix $L$ representing $L$ with respect to the bases $S$ and $T$.
>
> 【107 政大大昌】

> **解**
>
> (1) $L(p_1(t)) = L(1) = \int_{-1}^{t} 1\, dx = t - (-1) = t + 1 = 1 + t + 0 \cdot t^2$，$\therefore [L(p_1(t))]_T = \begin{bmatrix} 1 \\ 1 \\ 0 \end{bmatrix}$
>
> $\therefore [L(p_2(t))]_T = \begin{bmatrix} -0.5 \\ 0 \\ 0.5 \end{bmatrix}$
>
> (2) $[L]_S^T = \begin{bmatrix} 1 & -0.5 \\ 1 & 0 \\ 0 & 0.5 \end{bmatrix}$
