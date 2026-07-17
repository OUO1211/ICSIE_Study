$$= \{a + (-4c - 12d - 32e)x + cx^2 + dx^3 + ex^4 \mid a, c, d, e \in \mathbb{R}\}$$

$\therefore S = \{1, (-4x + x^2), (-12x + x^3), (-32x + x^4)\}$ 為線性獨立集，

$\therefore$ 取 $S$ 可為 $W$ 的一組基底。

> **例題 13**
>
> (12%) Let $C[-1,1]$ be the vector space over $\mathbb{R}$ of all continuous functions defined on the interval $[-1,1]$. Let $V = \{f \in C[-1,1] \mid f(x) = ae^x + be^{2x} + ce^{3x}, a, b, c \in \mathbb{R}\}$.
>
> (1) Prove that $B = \{e^x, e^{2x}, e^{3x}\}$ is a basis of $V$。 【99 彰師數學教組】
>
> (2) Prove that $B' = \{e^x - 2e^{2x}, e^x + 2e^{2x} + 2e^{3x}, 3e^{3x}\}$ is a basis of $V$。 【108 交大資工】

**解**

(1) Wronskian $\{e^x, e^{2x}, e^{3x}\}$：

$$= \det \begin{bmatrix} e^x & e^{2x} & e^{3x} \\ e^x & 2e^{2x} & 3e^{3x} \\ e^x & 4e^{2x} & 9e^{3x} \end{bmatrix} = -2e^{6x} \ne 0$$，$\forall x \in \mathbb{R}$，

故以是線性獨立的，

又 $B$ 生成 $V$，故 $B$ 為 $V$ 的一個一組基底。

(2) 設 $\alpha(e^x - 2e^{2x}) + \beta(e^x + 2e^{2x} + 2e^{3x}) + \gamma(3e^{3x}) = 0$，

則 $(\alpha + \beta)e^x + (-2\alpha + 2\beta)e^{2x} + (2\beta + 3\gamma)e^{3x} = 0$，

由 $\{e^x, e^{2x}, e^{3x}\}$ 是線性獨立，$\therefore \begin{cases} \alpha + \beta = 0 \\ -2\alpha + 2\beta = 0 \\ 2\beta + 3\gamma = 0 \end{cases}$

可解得 $\alpha = \beta = \gamma = 0$，

$\therefore B' = \{e^x - 2e^{2x}, e^x + 2e^{2x} + 2e^{3x}, 3e^{3x}\}$ 是線性獨立集，

又由(1)可得 $\dim(V) = 3$，故 $B'$ 為 $V$ 的一組基底。
