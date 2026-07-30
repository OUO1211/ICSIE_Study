第六章 圖形 255
Graph

（三）演算法
Procedure allcosts（cost，var a ：adjacencymatrix；n ：integer）；
｛cost［1．．n，1．．n］is the cost adjacency matrix of a graph with n vertices；a［i，j］is the cost of the shortest path between vetitces $\left.\mathrm{v}_{\mathrm{i}}, \mathrm{v}_{\mathrm{j}} \operatorname{cost}[\mathrm{i}, \mathrm{j}]=0,1 \leq \mathrm{i} \leq \mathrm{n}.\right\}$
var i，j，k ：integer；
Begin
```
for i=1 to n do
    for j=1 to n do
        a[i, j] : = cost[i, j]; {Copy cost into a }
for k=1 to n do {For a path with highest vertex index k}
    for i=1 to n do {For all possible pairs of vertices}
        for j=1 to n do
            if (a[i, k]+a[k, j]) < a[i, j]
                then a[i, j] : = a[i, k]+a[k, j];
```

End; \{end of allcosts\}

例：圖（a）有向圖 G

圖（b）G 的花費矩陣

\begin{tabular}{|l|l|l|l|}
\hline & 1 & 2 & 3 \\
\hline 1 & 0 & 4 & 11 \\
\hline 2 & 6 & 0 & 2 \\
\hline 3 & 3 & $\infty$ & 0 \\
\hline
\end{tabular}

圖（c）四個矩陣 $\mathrm{A}^0, \mathrm{~A}^1, \mathrm{~A}^2, \mathrm{~A}^3$

\begin{tabular}{|l|l|l|l|}
\hline A ${ }^0$ & 1 & 2 & 3 \\
\hline 1 & 0 & 4 & 11 \\
\hline 2 & 6 & 0 & 2 \\
\hline 3 & 3 & $\infty$ & 0 \\
\hline
\end{tabular}

\begin{tabular}{|l|l|l|l|}
\hline A ${ }^1$ & 1 & 2 & 3 \\
\hline 1 & 0 & 4 & 11 \\
\hline 2 & 6 & 0 & 2 \\
\hline 3 & 3 & 7 & 0 \\
\hline
\end{tabular}