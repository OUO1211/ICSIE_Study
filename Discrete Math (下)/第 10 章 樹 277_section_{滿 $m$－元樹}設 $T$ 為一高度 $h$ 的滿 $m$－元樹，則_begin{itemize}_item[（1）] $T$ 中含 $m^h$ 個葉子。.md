第 10 章 樹 277

\section*{滿 $m$－元樹}

設 $T$ 為一高度 $h$ 的滿 $m$－元樹，則
\begin{itemize}
\item[（1）] $T$ 中含 $m^h$ 個葉子。
\item[（2）] $T$ 中含 $\frac{m^h-1}{m-1}$ 個內部節點。
\item[（3）] $T$ 中含 $m^h+\frac{m^h-1}{m-1}$ 個點。
\item[（4）] $T$ 中含 $\frac{m\left(m^h-1\right)}{m-1}$ 個邊。
\end{itemize}

解（1）因為葉子高度都為 $h$ ，且高度 $k$ 的點有 $m^k$ 個，故高度 $h$ 的點（即葉子）有 $m^h$ 個，即 $l=m^h$ 。
\begin{itemize}
\item[（2）] 因為高度 $k$ 的點有 $m^k$ 個，故內部節點共有 $m^0+m^1+m^2+\ldots+m^{h-1}=\frac{m^h-1}{m-1}$ 。
\item[（3）] 總點數 $=l+i=m^h+\frac{m^h-1}{m-1}$ 。
\item[（4）] 邊數 = 點數 $-1=m^h+\frac{m^h-1}{m-1}-1=\frac{m\left(m^h-1\right)}{m-1}$ 。
\end{itemize}

Note
\begin{itemize}
\item[（1）] 設 $T=(V, E)$ 為一高度 $h$ 的滿二元樹，則
（1）$T$ 中含 $2^h$ 個葉子，
（2）$T$ 中含 $2^h-1$ 個內部節點，
（3）$T$ 中含 $2^{h+1}-1$ 個點，
（4）$T$ 中含 $2^{h+1}-2$ 個邊。
【82 中山電機】
\item[（2）] A full binary tree with $2 n-1$ vertices has $n$ leaves．
\end{itemize}