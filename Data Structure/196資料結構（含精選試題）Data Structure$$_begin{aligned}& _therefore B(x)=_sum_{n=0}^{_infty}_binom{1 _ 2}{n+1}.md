196
資料結構（含精選試題）

Data Structure
$$
\begin{aligned}
& \therefore B(x)=\sum_{n=0}^{\infty}\binom{1 / 2}{n+1}(-1)^n 2^{2 n-1} x^n=\sum_{n=0}^{\infty} b_n x^n \\
& \begin{aligned}
\therefore b_n & =\binom{1 / 2}{n+1}(-1)^n 2^{2 n-1} \\
& =\frac{1 / 2(1 / 2-1) \cdots(1 / 2-(n+1)+1)}{(n+1)!} \cdot(-1)^n 2^{2 n-1} \\
& =\frac{1(-1)(-3) \cdots(1-2 n)}{(n+1)!} \cdot(-1)^n 2^{2 n} \\
& =\frac{1 \cdot 3 \cdot 5 \cdots 2 n-1}{(n+1)!} \cdot 2^n \\
& =\frac{1 \cdot 3 \cdot 5 \cdots(2 n-1)}{(n+1)!} \cdot \frac{2 \cdot 4 \cdot 6 \cdots(2 n)}{2 n \cdot n!} \\
& =\frac{(2 n)!}{n!(n+1)!}=\frac{1}{n+1} \cdot \frac{(2 n)!}{n!n!}=\frac{1}{n+1}\binom{2 n}{n} \\
\because\binom{m}{n} & =\frac{m!}{n!(m-n)!}
\end{aligned}
\end{aligned}
$$