30
資料結構（含精選試題）
Data Structure

\section*{例題 1－40}

比較下列 Time Complexity（Rank from high to low）
$$
\begin{aligned}
& \left(\frac{3}{2}\right)^n,(\sqrt{2})^{\log n}, n^2,(\log n)!, n^3, \log ^2 n, \log (n!), 2^{2^n}, n^{1 / \log n}, \log \log n \\
& n \cdot 2^n, 2^n, 2^{\log n},(\log n)^{\log n}, 4^{\log n},(n+1)!, \sqrt{\log n}, n!, 2^{\sqrt{2 \log n}}, n, n \log n, 1
\end{aligned}
$$

解 下列 identities are useful
\begin{itemize}
\item[（1）] $(\log n)^{\log n}=n^{\log \log n}$
\item[（2）] $4^{\log \mathrm{n}}=\mathrm{n}^2$
\item[（3）] $2^{\log n}=n$
\item[（4）] $2=\mathrm{n}^{1 / \log \mathrm{n}}$ $\_\_\_\_$ （使用（3）to power $1 / \log n$ ） $\left(\right.$ 即 $\left.\left(2^{\log n}\right) \frac{1}{\log n}=n^{\frac{1}{\log n}}\right)$
\item[（5）] $2 \sqrt{2 \log \mathrm{n}}=\mathrm{n}^{\sqrt{2 / \log \mathrm{n}}}$ $\_\_\_\_$用（4）to power $\sqrt{2 \log n})$ $\left(\right.$ 即 $\left.2^{\sqrt{2 \log n}}=\left(n^{\frac{1}{\log n}}\right)^{\sqrt{2 \log n}}=n^{\frac{1}{\log n} \sqrt{2 \log n}}=n^{\sqrt{2 / \log n}}\right)$
\item[（6）] $(\sqrt{2})^{\log \mathrm{n}}=\sqrt{\mathrm{n}}$
$$
\left(\text { 即 }(\sqrt{2})^{\log n}=2^{\frac{1}{2} \cdot \log n}=2^{\log \frac{1}{2}}=2^{\log \sqrt{n}}=\sqrt{n}\right)
$$
Stirling＇s formula $\Rightarrow \mathrm{n}!=\theta\left(\mathrm{n}^{\mathrm{n}+1 / 2} \mathrm{e}^{-\mathrm{n}}\right)$
\item[（7）] $\log (\mathrm{n}!)=\theta(n \log n)$
\item[（8）] $(\log n)!=\theta\left((\log n)^{\log n+1 / 2} e^{-\log n}\right)=\theta\left((\log n)^{\log n+1 / 2} n^{-\log e}\right)$
\end{itemize}