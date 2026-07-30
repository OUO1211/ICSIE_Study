第五章 樹與二元樹
195
Tree＆Binary Tree
$$
\begin{aligned}
& \rightarrow \quad B(x)-1=x \sum_{n=0}^{\infty}\left(b_0 b_n+b_1 b_{n-1}+\ldots+b_n b_0\right) x^n \\
& \rightarrow \quad B(x)-1=x \cdot B(x) \cdot B(x)
\end{aligned}
$$

【註】假設 $\mathrm{F}(\mathrm{x})=\sum_{\mathrm{n}=0}^{\infty} \mathrm{a}_{\mathrm{n}} \mathrm{x}^{\mathrm{n}}, \mathrm{G}(\mathrm{x})=\sum_{\mathrm{n}=0}^{\infty} \mathrm{b}_{\mathrm{n}} \mathrm{x}^{\mathrm{n}}$
$$
\begin{aligned}
& \rightarrow \quad F(x) \cdot G(x)=\sum_{n=0}^{\infty} C_n x^n \\
& C_n=\sum_{i=0}^{\infty} a_i b_{n-i}=a_0 b_n+a_0 b_n+a_1 b_{n-1}+\ldots+a_n b_0 \\
& x B^2(x)-B(x)+1=0 \\
& \therefore \quad B(x)=\frac{1-\sqrt{1-4 x}}{2 x}
\end{aligned}
$$
經由二項式定理：
$$
\begin{aligned}
(2 x+b)^n=\sum_{i=0}^{\infty} & \binom{n}{i}(a x)^i(b)^{n-1} \\
\rightarrow \quad(1-4 x)^{1 / 2} & =\sum_{n=0}^{\infty}\binom{1 / 2}{n}(1)^{1 / 2 n}(-4 x)^n \\
& =\sum_{n=0}^{\infty}\binom{1 / 2}{n}(-4 x)^n
\end{aligned}
$$
$$
\begin{aligned}
\therefore B(x) & =\frac{1}{2 x}\left[1-\sum_{n=0}^{\infty}\binom{1 / 2}{n}(-4 x)^n\right] \\
& =\frac{1}{2 x}-\sum_{n=0}^{\infty}\binom{1 / 2}{n}(-1)^n 2^{2 n} x^n \frac{1}{2 x} \\
& =\frac{1}{2 x}-\sum_{n=0}^{\infty}\binom{1 / 2}{n}(-1)^n 2^{2 n}+x^{n-1}
\end{aligned}
$$
令 $n-1=m$
$$
\rightarrow \mathrm{B}(\mathrm{x})=\frac{1}{2 \mathrm{x}}-\sum_{\mathrm{m}=-1}^{\infty}\binom{1 / 2}{\mathrm{~m}+1}(-1)^{\mathrm{n}-1} 2^{2 \mathrm{~m}-1} \mathrm{x}^{\mathrm{n}}
$$
而 $\mathrm{m}=-1$ 時，$\binom{1 / 2}{0}(-1)^0 2^{-1} \mathrm{x}^{-1}=\frac{1}{2 \mathrm{x}}$
$$
\therefore B(x)=\sum_{m=0}^{\infty}\binom{1 / 2}{m+1}(-1)^n 2^{2 n+1} x^n
$$

令 $n=m$