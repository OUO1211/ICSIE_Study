28
資料結構（含精選試題）
Data Structure

例題 1－37
$\mathrm{T}(\mathrm{n})=\mathrm{n}+4 \mathrm{~T}\left(\frac{\mathrm{n}}{2}\right)$ 之 Time Complexity
解 $\mathrm{T}(\mathrm{n})=\mathrm{n}+4 \mathrm{~T}\left(\frac{\mathrm{n}}{2}\right)$
$$
\begin{aligned}
& =n+4\left(\frac{n}{2}+4 T\left(\frac{n}{4}\right)\right) \\
& =n+4\left(\frac{n}{2}+4\left(\frac{n}{4}+4 T\left(\frac{n}{8}\right)\right)\right) \\
& =n+2 n+4 n+\cdots+4^{\log n} T(1) \\
& =n+2 n+4 n+\cdots+\theta\left(n^2\right) \\
& =n\left(\sum_{k=0}^{\log n-1} 2^k\right)+\theta\left(n^2\right) \\
& =n\left(\frac{2^{\log n}-1}{2-1}\right)+\theta\left(n^2\right) \\
& =\theta\left(n^2\right)+\theta\left(n^2\right) \\
& =\theta\left(n^2\right)
\end{aligned}
$$

Exercise
改用 Master Theorem 求解
解 $n^{\log _b a}=n^2$
而 $\mathrm{f}(\mathrm{n})=\mathrm{n} \quad \therefore$ case 1
$$
\therefore \theta\left(\mathrm{n}^2\right)
$$

例題 1－38
$\mathrm{T}(\mathrm{n})=2 \mathrm{~T}\left(\frac{\mathrm{n}}{2}\right)+\mathrm{n} \log \mathrm{n}$
解 $\because \mathrm{a}=2, \mathrm{~b}=2, \mathrm{f}(\mathrm{n})=\mathrm{n} \log \mathrm{n}$
而 $n^{\log _b a}=n^{\log _2 2}=n$
$$
\begin{aligned}
& \frac{f(n)}{n^{\log _b a}}=\frac{n \log n}{n}=\log n=\log ^k n, \quad \mathrm{k}=1 \\
& T(n)=\theta\left(n^{\log _b a} \log ^{k+1} n\right)=\theta\left(n \log ^2 n\right)
\end{aligned}
$$