308
離散數學（下）

\section*{關係的運算－補關係（complement）}

令 $R: A \rightarrow B$ 為一關係，則 $R$ 之補關係 $\bar{R}: A \rightarrow B$ 定義為$\bar{R}=\{(a, b) \mid a \in A, b \in B,(a, b) \notin R\} 。$

例如：
令 $A=\{1,2,3,4\}, B=\{a, b, c\}$ ，
取 $R=\{(1, a),(1, b),(2, a),(3, a)\}$ ，
則 $R$ 之補關係 $\bar{R}=\{(1, c),(2, b),(2, c),(3, b),(3, c),(4, a),(4, b),(4, c)\}$ ，
其關係矩陣 ：$M_{\bar{R}}=\begin{gathered}a \\ 1 \\ 2 \\ 3 \\ 4\end{gathered}\left[\begin{array}{ccc}0 & 0 & 1 \\ 0 & 1 & 1 \\ 0 & 1 & 1 \\ 1 & 1 & 1\end{array}\right]$ ，其關係圖形：