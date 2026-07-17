530
離散數學（上）

二項式定理（Binomial Theorem）
設 $x, y$ 為變數，$n$ 為正整數，則
$$
(x+y)^n=\binom{n}{0} x^0 y^n+\binom{n}{1} x^1 y^{n-1}+\ldots+\binom{n}{n} x^n y^0=\sum_{k=0}^n\binom{n}{k} x^k y^{n-k}
$$

【證明】
本定理可用歸納法得證，此處以組合證明討論：
考慮 $\overbrace{(x+y)(x+y) \ldots(x+y)}^n$ 之展開式中 $x^k y^{n-k}$ 之係數 $(0 \leq k \leq n)$ ，
因為 $x^k y^{n-k}$ 是從這 $n$ 個 $(x+y)$ 中選出 $k$ 個提供 $x$ ，另 $n-k$ 個提供 $y$ 所對乘而得，
因其選法有 $\binom{n}{k}$ 種，故知 $x^k y^{n-k}$ 係數為 $\binom{n}{k}$ ，
∴ 此二項式定理成立。

例如：
$$
\begin{aligned}
& (x+y)^3=\binom{3}{0} y^3+\binom{3}{1} x^1 y^2+\binom{3}{2} x^2 y^1+\binom{3}{3} x^3 \\
& (x+2 y)^4=\binom{4}{0} 16 y^4+\binom{4}{1} x^1 8 y^3+\binom{4}{2} x^2 4 y^2+\binom{4}{3} x^3 2 y+\binom{4}{4} x^4
\end{aligned}
$$