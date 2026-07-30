264
離散數學（下）

\section*{$\boldsymbol{m}$－元樹}

設 $T$ 為一 $n$ 點，高度 $h$ 的 $m$－元樹，$i=$ 内部節點個數，$l=$ 樹葉個數，則
（1）$n \leq m i+1 。$（即 $i \geq \frac{n-1}{m}$ ）
（2）$l \leq(m-1) i+1 。$（即 $i \geq \frac{l-1}{m-1}$ ）

【105台大資工】
\begin{itemize}
\item[（3）] $l \leq m^h$ 。
\item[（4）] $h+1 \leq n \leq \frac{m^{h+1}-1}{m-1} 。$
\end{itemize}

【很重要】

【證明】
\begin{itemize}
\item[（1）] 因為有 $i$ 個內部節點，每個內部節點頂多 $m$ 個兒子，再加上 root，故得總點數最多為 $m i+1$ ，即 $n \leq m i+1$ 。
\item[（2）] 因為 $n=l+i$ ，故由（1）得 $l+i \leq m i+1$ ，即 $l \leq(m-1) i+1 。$
\item[（3）] 點數最多時，第 $i$ 層有 $m^i$ 點，而點數最多時葉子都在第 $h$ 層，此時葉子數 $m^h$ 。
\item[（4）] 點數最少在於此樹恰成一path，而因高度為 $h$ ，故總點數為 $h+1$ ；
點數最多在於成為完全 $m$ 元樹時，而因高度為 $h$ ，
故點數為 $1+m+m^2+\ldots+m^h=\frac{1 \cdot\left(m^{h+1}-1\right)}{m-1}$ ，故 $h+1 \leq n \leq \frac{m^{h+1}-1}{m-1}$ 。
\end{itemize}