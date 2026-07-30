第 8 章 圖論। 113

\section*{其他主題：}

完全配對（complete matching ）
设 $G=(A \cup B, E)$ 為一雙分圖，若 $A$ 中的點均能被 $M$ 中的遣所速，则稱 $M$ 为從 $A$ 到 $B$ 的一完全配對。

Note
關於雙分圖 $G=(A \cup B, E)$ 中，完全配對的存在性：
\begin{itemize}
\item[（1）] P．Hall 定理 ：$G$ 有從 $A$ 到 $B$ 的一完全配對 $\Leftrightarrow \forall S \subseteq A,|S| \leq|N(S)|$ 【87 成大工科】（ $N(S)$ 表 $S$ 中的點所連到的所有點。此定理之證明較繁瑣，請讀者參考圖論相關書籍）
\item[（2）] 若存在正整數 $k$ ，使對任意 $A 、 B$ 中的點 $x 、 y$ 均滿足 $\operatorname{deg} y \leq k \leq \operatorname{deg} x$ ，則 $G$ 有從 $A$ 到 $B$的一完全配對。
\item[] 解取 $S \subseteq A$ ，則 $k \cdot|S| \leq \sum_{v \in S} \operatorname{deg} v=|E(G[S \bigcup N(S)])| \leq \sum_{u \in N(S)} \operatorname{deg} u \leq k \cdot|N(S)|$ ，$\therefore|S| \leq|N(S)|$ ，故由 P．HALL 定理得，存在 $A$ 到 $B$ 的一組完全配對。
\item[（3）] Marriage 定理 ：A regular bipartite graph has a perfect matching．
【85中央数學】【91 中正資工】
\item[解] Assume $G$ is $k$－regular，take $S \subseteq A$ ，
then $k \cdot|S|=\sum_{v \in S} \operatorname{deg} v=|E(G[S \bigcup N(S)])| \leq \sum_{u \in N(S)} \operatorname{deg} u=k \cdot|N(S)|$ ，
$\therefore|S| \leq|N(S)|$ ，by P．HALL＇s theorem，we get a complete matching from $A$ to $B$ ．
\end{itemize}