第8意 富訪1 101

\section*{8－8 雙分闘}

雙分團（二分圖、二部團、bipartite graph）
考虑無向圆 $G=(V, E)$ ，
\begin{itemize}
\item[（1）] 若 $V$ 可分割成 $A$ 、 $B$ ，使 $A$ 、 $B$ 各自都是嶧立集，财稱 $G$ 為一慧分圈。【88中山資工】【90 北科資工】【104 羔美資工】【105 責就技師】
\item[（2）] 若 $G$ 为隻分圖且 $A$ 之每一频與 $B$ 之每一频均相䣋 • 财稱 $G$ 為一完全慧分圈 • 若 $|A|=m$ ，$|B|=n$ ，則 $G$ 也記成 $K_{m, n}$ 。
【98 高倠資工】
\end{itemize}

例如，下列都是雙分圖。

下列都不是雙分圖。

Note
\begin{itemize}
\item[（1）] 雙分圖必不含奇圈（odd cycle）；反之，不含奇圈的圖必為雙分圖。【105 清大資工】【106 台大資工】【106 中山資工】【證明】
⇒ 設 $C: v_1-v_2-\ldots v_k-v_1$ ，為 $G$ 中之一 cycle，則 $C$ 必來回於 $A, B$ 間。
不失一般性，設 $v_1 \in A$ ，則 $v_1, v_3, v_5, \ldots \in A, v_2, v_4, \ldots \in B$ ，
若 $k$ ：odd，則 $v_k \in A$ ，但 $v_k, v_1$ 同為 $A$ 的點，故不相連…矛盾$\therefore k$ ：even，故知 $C$ 之長度為偶。
⇐ 設 $G$ 中之 cycle 長度均為偶，
\end{itemize}