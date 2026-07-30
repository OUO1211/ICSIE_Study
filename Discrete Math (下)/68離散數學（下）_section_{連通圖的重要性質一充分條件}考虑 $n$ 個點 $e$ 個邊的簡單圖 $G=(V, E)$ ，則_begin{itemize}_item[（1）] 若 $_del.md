68
離散數學（下）

\section*{連通圖的重要性質一充分條件}

考虑 $n$ 個點 $e$ 個邊的簡單圖 $G=(V, E)$ ，則
\begin{itemize}
\item[（1）] 若 $\delta \geq \frac{n-1}{2}$ ，則 $G$ 為連通圖。（ $\delta$ 為 $G$ 的最小度数）【97台大資工】【104中山資工】
\item[（2）] 若 $e>\binom{n-1}{2}$ ，則 $G$ 為連通圖。
\item[] 【95 暨南資工】【96 政大資科】【98 清大資應】【99 宜蘭資工】【92、103交大應数】
\item[] 解（1）反之，若 $G$ 不連通，設 $G$ 有分量圖：$G_1, G_2, \ldots, G_k, k \geq 2$ ，
任取 $x \in V\left(G_1\right) 、 y \in V\left(G_2\right)$ ，
則 $\operatorname{deg}(x)+\operatorname{deg}(y) \leq\left|V\left(G_1\right)\right|-1+\left|V\left(G_2\right)\right|-1 \leq n-2$ ，
但 $\delta \geq \frac{n-1}{2}, \therefore \operatorname{deg}(x)+\operatorname{deg}(y) \geq \frac{n-1}{2}+\frac{n-1}{2}=n-1$ ，得矛盾，故 $G$ 為連通圖。
\begin{itemize}
\item[（2）] 反之，設 $G$ 不連通，有 $k$ 個分量 $G_1, G_2, \ldots, G_k, k>1$ ，
因為邊最多時，是在 $G$ 只含兩個分量且均是完全圖時，設 $G_1=K_s, G_2=K_{n-s}$ ， $1 \leq s \leq n-1$ ，故得邊最多為
$\binom{s}{2}+\binom{n-s}{2}=\frac{1}{2}(s(s-1)+(n-s)(n-s-1))=\left(s-\frac{n}{2}\right)^2+\frac{n^2-2 n}{4}$ ，
得其極大值發生在端點 $s=1$ 或 $n-1$ 時，值為 $\frac{n^2-3 n+2}{2}=\frac{(n-1)(n-2)}{2}=\binom{n-1}{2}$ ，興題意不符，∴ 此圖為連通。
\end{itemize}
\end{itemize}