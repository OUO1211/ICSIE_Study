80
離散數學（下）

\section*{8－6 找最短路徑}

本節討論給定加權圖（weighted graph）後，找出圖中某兩點的最短路徑的演算法。

\section*{Dijkstra＇s shortest path algorithm}

Input：每邊為正值之連通加權圖 $G=(V, E)$ 。
Output：$a$ 到各點 $v$ 的距離 distance $D[v]$ 。
Step 1 ：$S \leftarrow a$
Step 2 ：$D[a] \leftarrow 0$
Step 3 ：for each $v \in V-\{a\}$ do $D[v] \leftarrow w t(a, v)$ ：邊 $(a, v)$ 的權重
Step 4 ：while $S \neq V$ do
begin
Step 5：choose a vertex $w$ in $V-S$ such that $D[w]$ is a minimum．
Step 6：add $w$ to $S$
Step 7：for each $v \in V-S$ do $D[v] \leftarrow \min (D[v], D[w]+w t[w, v])$
end
作法：
以例題1圖（2）為例，欲求 $a$ 到 $z$ 的最短路徑，
\begin{itemize}
\item[0．] 第一列標示 $D[b], D[c], \cdots$
\item[1．] 第二列紀錄：$a$ 以一個邊連到其他點的 weight，若沒有邊相連則以 $\infty$ 記之。
\item[2．] 標出第二列的最小數字，若同時有多個，則任取一個，將該點（設為 $x$ ）紀錄在下一列的最左端。
\item[3．] 計算 $a$ 到 $x$ 與 $x$ 到 $b$ 的 weight 的和，比較是否比上一列的 $a$ 到 $b$ 的 weight 少，若是，則更改，否則不變。
\item[4．] 計算 $a$ 到 $x 、 x$ 到 $c$ 的 weight 的和，比較是否比上一列的 $a$ 到 $c$ 的 weight 少，若是，則更改，否則不變。
\item[5．] 直到所有點都考慮過，剛才的 $x$ 就不用再比了。
\item[6．] 完成第三列後，標出其中最小的數字，重複演算法的步驟2到5，直到 $a-z$ 的最短路徑被求出。
\end{itemize}