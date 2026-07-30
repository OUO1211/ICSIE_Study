第六章 圖形 245
Graph
```
while not EmptyQueue(q) do
Begin
    DeleteQueue(q, v);
    for all vertices w adjacent to v do
        if not visited[w] then
            Begin
                visited[w] : = true;
                AddQueue(q, w);
            End;
    End;
```

End;
BFS 的追蹤是 Level-by-Level, 使用佇列(Queue)資料結構作為輔助, 而 DFS 的追
蹤可用遞迴進行, 使用堆疊(Stack)作為輔助。
例: 以上例來講, BFS 順序為:
    $\mathrm{V}_1 、 \mathrm{~V}_2 、 \mathrm{~V}_3 、 \mathrm{~V}_4 、 \mathrm{~V}_5 、 \mathrm{~V}_6 、 \mathrm{~V}_7 、 \mathrm{~V}_8$ (不只一種)
\begin{itemize}
\item[（二）] Time 分析 ：
若用相鄰串列，Time Complexity：0（e）
相鄰矩陣，Time Complexity： $0\left(\mathrm{n}^2\right)$
\end{itemize}

\section*{6－3 圖形走訪的應用}
\begin{itemize}
\item[（一）] 判斷圖形否連通（Connected）
以圖形的任一頂點 V 為起始點，利用 DFS 或 BFS 來拜訪所有的相鄰頂點，若圖形的所有頂點都被拜訪過時，則為 Connected。
\item[（二）] 找出圖形的連通單元。
\item[（三）] 找出圖形的雙連通單元。
\item[（四）] 找一個連通圖形的展開樹（Spanning Tree）。
\end{itemize}
若以相鄰串列表示，則上述 algorithm 之 time 為 $\mathrm{O}(\mathrm{n}+\mathrm{e})$ ，以相鄰矩陣表示則為 $\mathrm{O}\left(\mathrm{n}^2\right)$