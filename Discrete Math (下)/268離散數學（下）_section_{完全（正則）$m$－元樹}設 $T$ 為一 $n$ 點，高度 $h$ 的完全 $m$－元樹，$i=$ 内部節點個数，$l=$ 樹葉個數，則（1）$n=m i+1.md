268
離散數學（下）

\section*{完全（正則）$m$－元樹}

設 $T$ 為一 $n$ 點，高度 $h$ 的完全 $m$－元樹，$i=$ 内部節點個数，$l=$ 樹葉個數，則
（1）$n=m i+1$ ．
【96清大資應】【98暨南資工】
（2）$l \leq m^h$ ．
（3）$(m-1)(h-1)+m \leq l \leq m^h$ ．
【96、99清大資應】

【證明】
\begin{itemize}
\item[（1）] 因為有 $i$ 個內部節點，每個內部節點恰 $m$ 個兒子，再加上 root，故得總點數為 $m i+1$ ，即 $n=m i+1$ 。
\item[（2）] 因為高度1的點有 $m$ 個，高度2的點頂多 $m^2$ 個，高度3的點頂多 $m^3$ 個，⋯ ，故高度 $h$ 的點（即葉子）頂多 $m^h$ 個，即 $l \leq m^h$ 。
\item[（3）] 因為高度1的點有 $m$ 個，高度2的點頂多 $m^2$ 個，高度3的點頂多 $m^3$ 個，⋯，故高度 $h$ 的樹的葉子頂多 $m^h$ 個。
另一方面，葉子數最少時應是除最末層外，每一層恰只一內部節點，而第 $h$ 層恰 $m$ 點，∴ 葉子數 $=\underbrace{(m-1)+(m-1)+\ldots+(m-1)}_{h-1}+m=m+(h-1)(m-1) 。$
\end{itemize}

Note
\begin{itemize}
\item[（1）] 完全二元樹時，$n=2 i+1$ 。【95 中正資工】【101 成大電通】
\item[（2）] 完全二元樹時，$l=i+1$ 。【93中正資工】
\item[（3）] 完全二元樹時， $1+2 h \leq n \leq 2^{h+1}-1$ 。【98、100交大資訊】
\item[（4）] 當 $T=(V, E)$ 為一高度 $h$ 的完全 $m$－元平衡樹時，$h=\left\lceil\log _m l\right\rceil$ 。【93 成大工科】
\end{itemize}

【證明】
因為 $T$ 為高度 $h$ 的完全 $m$－元樹，∴ 葉子數 $l \leq m^h$ ，
又因為 $T$ 是高度 $h$ 的平衡樹，必有葉子在 level $h \therefore$ 葉子數 $l>m^{h-1}$ ，
故得 $m^{h-1}<l \leq m^h, \therefore \log _m m^{h-1}<\log _m l \leq \log _m m^h$ ，
$\therefore h-1<\log _m l \leq h$ ，得 $h=\left\lceil\log _m l\right\rceil$ 。