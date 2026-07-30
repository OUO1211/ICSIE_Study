第六章 圖形 247
Graph

DFS展開樹

BFS展開樹

\section*{二．最小成本展開樹（Minimum Cost Spanning Tree）}
\begin{itemize}
\item[（一）] 應用由來
如果 G 中的點代表城市，邊代表二個城市間的交通連線，則把 n 個城市連在一起至少需要 n－1 個連線；而所有的展開樹可代表所有可能的選擇。由於每個邊上將會有加權值，代表架設成本、連線的長度等等。給定如此的一個加權圖形，若希望找到一組交通連線把所有的城市連接起來，而其成本和或長度和為最小。即為此應用。
\end{itemize}

\section*{三．展生 Minimum Cost Spanning Tree 之方法}

應用 Greedy 方法，求一連通無向圖形的最小成本展開樹之演算法有三種：① Kruskal演算法，② Prim 演算法和③ Sollin 演算法。
\begin{itemize}
\item[（一）] Kruskal 演算法
\begin{itemize}
\item[1．] 在 Kruskal 演算法中，一個最小成本展開樹 T 是依照它們的成本，由小到大逐一挑選。
如果一個邊不會和已在 T 中的邊構成一個循環（Cycle），就把這個邊加入 T 中，否則放棄。G 是連通的才有可能產生 spanning tree，否則無法產生。
\end{itemize}
\item[2．] 演算法
$$
\begin{aligned}
& T:=0 \\
& \text { while } T \text { contains less }(n-1) \text { edges and ( } E \text { is not empty) do } \\
& \text { begin } \\
& \text { choose an edge }(v, w) \text { from } E \text { of lowest cost; } \\
& \text { delete }(v, w) \text { from } E \text {; }
\end{aligned}
$$
\end{itemize}