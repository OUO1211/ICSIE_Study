第 3 章 函數
273

常用性質
（1） $1+2+\ldots+n=\frac{1}{2} n(n+1)=\Theta\left(n^2\right)$ ．
（2） $1^2+2^2+\ldots+n^2=\frac{1}{6} n(n+1)(2 n+1)=\Theta\left(n^3\right)$ ．
（3）由 $n!\leq n^n$ ，故 $n!=O\left(n^n\right)$ 。
【91中山資工】【91成大工科】
（4）當 $n>3$ 時， $2^n \leq n!$ ，故 $2^n=O(n!)$ 。
【 91 成大工科】
（5）對任意 $a 、 b>1, \log _a n=\Theta\left(\log _b n\right)$ 。
（6） $\log _2(n!)=\Theta(n \log n)$ ．
【重要且常考】
【證明】（1）～（4）可由歸納法得證，請讀者自行完成。
（5）$\because \log _a n=\frac{\log _b n}{\left|\log _b a\right|}, \therefore \frac{1}{\left|\log _b a\right|} \times\left|\log _b n\right| \leq\left|\log _a n\right| \leq \frac{1}{\left|\log _b a\right|} \times\left|\log _b n\right|$ ，
取 $c_1=c_2=\frac{1}{\left|\log _b a\right|}, n_0=1$ ，由定義得 $\log _a n=\Theta\left(\log _b n\right)$ 。
（6）（1）$\because \log _2 n!=\log _2 1+\log _2 2+\log _2 3+\ldots+\log _2 n \leq n \log _2 n$ ，
∴ 取 $c=1, n_0=1$ ，得 $\log _2(n!)=O\left(n \log _2 n\right)=O(n \log n)$ ．
（亦可由 $n!<n^n, \therefore \log n!<n \log n$ 而得到。）
（2）
$$
\begin{align*}
\because \log _2 n! & =\log _2 1+\log _2 2+\log _2 3+\ldots+\log _2 n \\
& \geq 0+\ldots+0+\log _2 \frac{n}{2}+\ldots+\log _2(n-1)+\log _2 n \\
& \geq \log _2 \frac{n}{2}+\log _2 \frac{n}{2}+\ldots+\log _2 \frac{n}{2} \\
& \geq \frac{n}{2} \log _2 \frac{n}{2} \geq \frac{n \log _2 n}{4}, \text { when } n \geq 4 \ldots \ldots \ldots \ldots \ldots . . \tag{?}
\end{align*}
$$
（pf of（？）：$\frac{n}{2} \log _2 \frac{n}{2} \geq \frac{n \log _2 n}{4} \Leftrightarrow 2 \log _2 \frac{n}{2} \geq \log _2 n \Leftrightarrow\left(\frac{n}{2}\right)^2 \geq n \Leftrightarrow n \geq 4$ ）
∴ 取 $c=\frac{1}{4}, n_0=4$ ，得 $\log _2(n!)=\Omega\left(n \log _2 n\right)=\Omega(n \log n)$ 。
【另證】 $\because n!\approx \sqrt{2 \pi n}\left(\frac{n}{e}\right)^n, \therefore \log _2 n!\geq \log _2\left(\frac{n}{e}\right)^n=n \log _2\left(\frac{n}{e}\right)$ ，
$$
\therefore \log _2(n!)=\Omega\left(n \log _2\left(\frac{n}{e}\right)\right)=\Omega\left(n \log _2 n\right) .
$$