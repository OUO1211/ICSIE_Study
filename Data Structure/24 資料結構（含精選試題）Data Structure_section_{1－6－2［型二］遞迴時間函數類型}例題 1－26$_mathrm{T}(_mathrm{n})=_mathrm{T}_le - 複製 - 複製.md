26
資料結構（含精選試題）
Data Structure

Master Theorem 之例題
例題 1－31
$\mathrm{T}(\mathrm{n})=2 \mathrm{~T}\left(\frac{\mathrm{n}}{2}\right)+\mathrm{n}^3$ ，求 $\mathrm{T}(\mathrm{n})=\theta($ ？）
解 $\because \mathrm{a}=2, \mathrm{~b}=2, \mathrm{f}(\mathrm{n})=\mathrm{n}^3$
且 $n^{\log _b{ }^a}=n^{\log _2{ }^2}=n$
$$
\therefore \frac{\mathrm{f}(\mathrm{n})}{\mathrm{n}^{\log _{\mathrm{b}}{ }^2}}=\frac{\mathrm{n}^3}{\mathrm{n}}=\mathrm{n}^2
$$
Apply case 3 （of master theorem），$T(n)=\theta\left(n^3\right)$
例題 1－32
$\mathrm{T}(\mathrm{n})=\mathrm{T}\left(\frac{9 \mathrm{n}}{10}\right)+\mathrm{n}$
解 $\because \mathrm{a}=1, \mathrm{~b}=\frac{10}{9}, \mathrm{f}(\mathrm{n})=\mathrm{n}$
而 $\mathrm{n}^{\log _b \mathrm{a}}=\mathrm{n}^{\log _{10}{ }^1}=\mathrm{n}^0=1$
$$
\text { 又 } \frac{f(n)}{n^{\log _b{ }^a}}=\frac{n}{1}=n
$$
則 Apply case 3．of the master theorem， $\mathrm{T}(\mathrm{n})=\theta(\mathrm{n})$

例題 1－33
$\mathrm{T}(\mathrm{n})=16 \mathrm{~T}\left(\frac{\mathrm{n}}{4}\right)+\mathrm{n}^2$
解 $\because a=16, b=4, f(n)=n^2$
而 $n^{\log _b{ }^a}=n^{\log _4{ }^{16}}=n^2$
$$
\text { 又 } \frac{f(n)}{n^{\log _b{ }^a}}=\frac{n^2}{n^2}=1
$$
∴ Apply case 2 of master theorem
$$
f(n)=\theta\left(n^2 \log n\right) \quad\left(\because \theta\left(n^{\log _b{ }^a} \log n\right)\right)
$$