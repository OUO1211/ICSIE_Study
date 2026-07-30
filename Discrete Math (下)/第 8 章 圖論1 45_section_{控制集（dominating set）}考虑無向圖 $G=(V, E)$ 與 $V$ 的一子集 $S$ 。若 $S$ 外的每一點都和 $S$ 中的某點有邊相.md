第 8 章 圖論1 45

\section*{控制集（dominating set）}

考虑無向圖 $G=(V, E)$ 與 $V$ 的一子集 $S$ 。若 $S$ 外的每一點都和 $S$ 中的某點有邊相連，則稱$S$ 為控制集。（即 $\forall v \in V(G) \Rightarrow v \in S$ or $(v, u) \in E(G)$ for some $u \in S$ ）

例如右圖中，$\{b, c, d, f\}$ 即為一控制集，
而 $\{c, f\},\{a, d, f\}$ 均為 minimal dominating set。

Note
\begin{itemize}
\item[（1）] 控制集是一種點的子集合，其特色是，每個沒有被選到的點都會與某個被選到的點相連。類似於從許多城市中選定部隊駐紮的地方，那當然是每個城市都選最好了，但人力有限，故退而求其次，那些沒有部隊駐紮的地方只要能很快有部隊趕到就好了（即有一邊相連），故所求的控制集常希望是最小的（minimum）。
\item[（2）] The dominating number $\gamma(G)$ ：為具最少點的控制集的點數。
\item[（3）] 若在一個控制集中再任拿掉一點，均會令其不為控制集，則稱其為極小控制集（minimal dominating set）。
\end{itemize}