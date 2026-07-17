286
離散數學（上）

調和數（Harmonic number）$H(n)=1+\frac{1}{2}+\frac{1}{3}+\ldots+\frac{1}{n}$
（1）Show that for all integer $n \geq 0, \frac{n+2}{2} \leq H\left(2^n\right) \leq n+2$ ．

【90政大資科】

（2）Using the above result to show that $H(n)=\Theta(\log n)$ ．
【90政大資科】【94北師資科】【95東華資工】【95海洋資工】
【證明】
（1）由歸納法可得，$\frac{n+2}{2} \leq H\left(2^n\right) \leq n+2, \forall n \in N$ 。
（2）令 $k=2^n$ 代入（1），則
$$
\begin{aligned}
& \frac{1}{2}\left(2+\log _2 k\right) \leq H(k) \leq 2+\log _2 k \\
& \therefore H(k)=\Theta\left(2+\log _2 k\right)=\Theta\left(\log _2 k\right)
\end{aligned}
$$

Note
上述關於調和數的發散等級，也可用積分的方法完成：
考慮函數 $f(x)=\frac{1}{x}$ 與 $x=1, x=n, y=0$ ，
所圍成面積 ： $\int_1^n \frac{1}{x} d x$ ，
而上圖斜線面積 ：$\frac{1}{2}+\frac{1}{3}+\ldots+\frac{1}{n}=H(n)-1$ ，
$$
\begin{aligned}
& \therefore H(n)-1 \leq \int_1^n \frac{1}{x} d x=\left.\ln x\right|_1 ^n=\ln n, \therefore H(n) \leq 1+\ln n, \\
& \therefore H(n)=O(1+\ln n)=O(\ln n)=O(\log n) .
\end{aligned}
$$

另外，
下圖斜線面積 ： $1+\frac{1}{2}+\frac{1}{3}+\ldots+\frac{1}{n-1}=H(n)-\frac{1}{n}$ ，
$$
\begin{aligned}
& \therefore H(n)-\frac{1}{n} \geq \int_1^n \frac{1}{x} d x=\left.\ln x\right|_1 ^n=\ln n \\
& \therefore H(n) \geq \ln n, \therefore H(n)=\Omega(\ln n)=\Omega(\log n)
\end{aligned}
$$

故得 $H(n)=\Theta(\log n)$ 。