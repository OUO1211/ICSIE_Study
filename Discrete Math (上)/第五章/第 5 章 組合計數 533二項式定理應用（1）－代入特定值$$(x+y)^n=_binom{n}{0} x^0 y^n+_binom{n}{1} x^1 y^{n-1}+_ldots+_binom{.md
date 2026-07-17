第 5 章 組合計數 533

二項式定理應用（1）－代入特定值
$$
(x+y)^n=\binom{n}{0} x^0 y^n+\binom{n}{1} x^1 y^{n-1}+\ldots+\binom{n}{n} x^n y^0
$$

例如：
（1）以 $x=y=1$ 代入，可得係數總和，$\binom{n}{0}+\binom{n}{1}+\binom{n}{2}+\ldots+\binom{n}{n}=2^n$ 。
【重要】
（2）以 $x=-1, y=1$ 代入，得 $\binom{n}{0}-\binom{n}{1}+\binom{n}{2}-\ldots+(-1)^n\binom{n}{n}=0$ 。
【重要】
（3）以 $x=2, y=1$ 代入，得 $\binom{n}{0}+2\binom{n}{1}+2^2\binom{n}{2}+\ldots+2^n\binom{n}{n}=3^n$ 。
【98中山資エ】【104 台大資工】
（4）$\binom{n}{0}+\binom{n}{2}+\binom{n}{4}+\cdots=\binom{n}{1}+\binom{n}{3}+\binom{n}{5}+\cdots=2^{n-1}, n \geq 1$ 。
（5）$\binom{n}{0}+\binom{n}{1}+\binom{n}{2}+\cdots+\binom{n}{(n-1) / 2}=2^{n-1}$ ，其中，$n$ 為正奇數。
【104 交大應数】【106 台大資工】
$$
\text { 解 } \begin{aligned}
2^n & =\binom{n}{0}+\binom{n}{1}+\binom{n}{2}+\cdots+\binom{n}{(n-1) / 2}+\binom{n}{(n+1) / 2}+\ldots+\binom{n}{n-1}+\binom{n}{n}, \\
& =\binom{n}{0}+\binom{n}{1}+\binom{n}{2}+\cdots+\binom{n}{(n-1) / 2}+\binom{n}{(n-1) / 2}+\ldots+\binom{n}{1}+\binom{n}{0}, \\
& =2\left(\binom{n}{0}+\binom{n}{1}+\binom{n}{2}+\cdots+\binom{n}{(n-1) / 2}\right), \text { 故所求為 } 2^{n-1} 。
\end{aligned}
$$