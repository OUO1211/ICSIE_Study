第六章 圖形 253
Graph

\begin{table}
\captionsetup{labelformat=empty}
\caption{例：求從頂點5到其他頂點的最短路徑之過程，如下所示}
\begin{tabular}{|l|l|l|l|l|l|l|l|l|l|l|l|}
\hline \multirow[b]{2}{*}{Iteration} & \multicolumn{11}{|c|}{Vertex} \\
\hline & S & Selected & DIST & （1） & （2） & （3） & （4） & （5） & （6） & （7） & （8） \\
\hline Initial & & － & & $\infty$ & $\infty$ & $\infty$ & 1500 & 0 & 250 & $\infty$ & $\infty$ \\
\hline 1 & 5， & 6 & & $\infty$ & $\infty$ & $\infty$ & 1250 & 0 & 250 & 1150 & 1650 \\
\hline 2 & 5，6 & 7 & & $\infty$ & $\infty$ & $\infty$ & 1250 & 0 & 250 & 1150 & 1650 \\
\hline 3 & 5，6，7 & 4 & & $\infty$ & $\infty$ & 2450 & 1250 & 0 & 250 & 1150 & 1650 \\
\hline 4 & 5，6，7，4 & 8 & & $\infty$ & $\infty$ & 2450 & 1250 & 0 & 250 & 1150 & 1650 \\
\hline 5 & 5，6，7，4，8 & 3 & & 3350 & $\infty$ & 2450 & 1250 & 0 & 250 & 1150 & 1650 \\
\hline 6 & 5，6，7，4，8，3 & 2 & & 3350 & 3250 & 2450 & 1250 & 0 & 250 & 1150 & 1650 \\
\hline & 5，6，7，4，8，3，2 & & & 3350 & 3250 & 2450 & 1250 & 0 & 250 & 1150 & 1650 \\
\hline
\end{tabular}
\end{table}

演算法 ：
Procedure ShorTest＿PATH（v，COST，DIST，n）；
／DIST（j）， $1 \leq \mathrm{j} \leq \mathrm{n} \quad$ is set to the length of the shortest path from vertex v to the vertex j in a digraph G with n vertices．DIST（v）is set to zero． G is represented by its cost adjacency matrix， $\operatorname{COST}(\mathrm{n}, \mathrm{n}) / /$
Var S（1 ：n）；
for $\mathrm{i}=1$ to n do
$$
\mathrm{S}(\mathrm{i})=0 ; \quad \operatorname{DIST}(\mathrm{i})=\operatorname{COST}(\mathrm{v}, \mathrm{i}) ;
$$
End；
$$
\mathrm{S}(\mathrm{v})=1 ; \quad \text { DIST }(\mathrm{v}) \leftarrow 0 ; \quad \text { num←2; } \quad / / \text { Put vertex } \mathrm{v} \text { in set } \mathrm{S} / /
$$

While num＜ndo／／Determine $\mathrm{n}-1$ paths from vertex $\mathrm{v} / /$
$$
\begin{aligned}
& \text { choose } u: \operatorname{DIST}(u)=\min \quad\{\operatorname{DIST}(w), \text { 且 } S(w)=\phi\} \\
& \mathrm{S}(\mathrm{u}) \leftarrow 1 ; \quad \text { num } \leftarrow \mathrm{num}+1 ;
\end{aligned}
$$
for all w with $\mathrm{S}(\mathrm{w})=0$ do
$$
\operatorname{DIST}(\mathrm{w}) \leftarrow \min \quad\{\operatorname{DIST}(\mathrm{w}), \operatorname{DIST}(\mathrm{u})+\operatorname{COST}(\mathrm{u}, \mathrm{w})\} ;
$$
End
End
End ShorTest＿PATH