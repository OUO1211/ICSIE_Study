第六章 圖形
243

\section*{Graph}

\section*{6－2 圖形追蹤（Graph Traversal）}

給定一個無向圖形 $\mathrm{G}=(\mathrm{V}, \mathrm{E})$ 及 $\mathrm{V}(\mathrm{G})$ 中的一個頂點 V，拜訪 G 中所有可能從 V 到達的頂點（即所有和 V 連通的頂點）；有下列二種方法：
\begin{itemize}
\item[] －縱向（深度）優先搜尋（Depth First Search）
\item[] －橫向（廣度）優先搜尋（Breadth First Search）
\end{itemize}
- ．縱向優先搜尋（Depth First Search，DFS）
- 個無向圖形之縱向優先搜尋過程如下：走訪起始頂點 V 上，然後選擇一個相鄰至 V而尚未被走過的頂點 W，以 W 為起始點再做縱向優先搜尋。如果從任何已走過的頂點，都無法再走到一個尚未被走過的頂點時，則結束搜尋。
（一）演算法如下 ：
```
Procedure DFS(v : integer);
    {Given an undirected graph G=(V, E) with n vertices and an array visited[n]
    initially set to false, this algorithm visits all vertices reachable from v. Visited is
    global.}
var w : integer;
Begin
    visited[v] : = true;
    for each vertex w adjacent to v do
        if not visited[w] then DFS(w);
    End; {of DFS}
```

\begin{itemize}
\item[（二）] Time 分析 ：
如果 G 是相鄰串列來表示，則所有相鄰至 V 的頂點 W 均可由沿著鏈結所組成鏈而得到；因為演算法 DFS 會檢查相鄰串列裡每個節點最多一次，而總共有2e 個串列節點，因此完成搜尋所需要的時間為0（e）。如果G是用相鄰矩陣來表示，則要決定所有相鄰至 V 之頂點所需的時間是 0（n）；而因為至多要走訪 n 個頂點，所以總共所需的時間為 $0\left(n^2\right)$ 。
\end{itemize}