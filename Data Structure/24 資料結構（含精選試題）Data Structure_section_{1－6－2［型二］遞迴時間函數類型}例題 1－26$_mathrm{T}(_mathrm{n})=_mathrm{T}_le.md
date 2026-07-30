24 資料結構（含精選試題）
Data Structure

\section*{1－6－2［型二］遞迴時間函數類型}

例題 1－26
$\mathrm{T}(\mathrm{n})=\mathrm{T}\left(\frac{\mathrm{n}}{2}\right)+1, \mathrm{~T}(1)=1$
求 $\mathrm{T}(\mathrm{n})=$ ？$=\mathrm{O}(?)$
解 $\mathrm{T}(\mathrm{n})=\mathrm{T}\left(\frac{\mathrm{n}}{2}\right)+1$
$$
\begin{aligned}
& =T\left(\frac{n}{4}\right)+2=T\left(\frac{n}{8}\right)+3=\ldots .=T\left(\frac{n}{n}\right)+\log _2 n \\
& =T(1)+\log _2 n=1+\log _2 n \\
\therefore \quad & T(n)=O(\log n)
\end{aligned}
$$

例題1－27
$\mathrm{T}(\mathrm{n})=2 \mathrm{~T}\left(\frac{\mathrm{n}}{2}\right)+\mathrm{n}, \quad \mathrm{T}(1)=1$
求 $\mathrm{T}(\mathrm{n})=\mathrm{O}(?)$
解 $\mathrm{T}(\mathrm{n})=\mathrm{O}(\mathrm{n} \log \mathrm{n})$

例題 1－28
$\mathrm{T}(\mathrm{n})=\mathrm{T}(\mathrm{n}-1)+\mathrm{n}, \mathrm{T}(0)=0$
求 $\mathrm{T}(\mathrm{n})=\mathrm{O}(?)$
解 $\mathrm{T}(\mathrm{n})=\mathrm{O}\left(\mathrm{n}^2\right)$

例題 1－29
$\mathrm{T}(\mathrm{n})=2 \mathrm{~T}(\mathrm{n}-1)+1, \mathrm{~T}(1)=1$
求 $\mathrm{T}(\mathrm{n})=?=\mathrm{O}(?)$
解 $\mathrm{T}(\mathrm{n})=2^{\mathrm{n}}-1=\mathrm{O}\left(2^{\mathrm{n}}\right)$