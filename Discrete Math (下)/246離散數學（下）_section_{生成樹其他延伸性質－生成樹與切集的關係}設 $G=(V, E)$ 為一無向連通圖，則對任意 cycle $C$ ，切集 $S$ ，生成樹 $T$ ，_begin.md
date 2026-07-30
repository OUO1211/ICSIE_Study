246
離散數學（下）

\section*{生成樹其他延伸性質－生成樹與切集的關係}

設 $G=(V, E)$ 為一無向連通圖，則對任意 cycle $C$ ，切集 $S$ ，生成樹 $T$ ，
\begin{itemize}
\item[（1）] $E(C) \cap E(\bar{T}) \neq \varnothing$ ．
\item[（2）] $E(S) \cap E(T) \neq \varnothing$ ．
\item[（3）] $|E(C) \cap E(S)|=$ 偶數。
\item[（4）] The complement of a spanning tree does not contain a cut set．
\end{itemize}

【90台科資工】
【96、98 清大資應】
【90交大資工】
【90清大資應】
\begin{itemize}
\item[（5）] The complement of a cut set does not contain a spanning tree．
\end{itemize}

【證明】
\begin{itemize}
\item[（1）] 若存在有一 cycle $C$ ，一 spanning tree $T$ ，使得 $E(C) \cap E(\bar{T})=\varnothing$ ，則表示此 $C$ 完全不與 $T$ 的補圖相交，表示此 $C$ 完全落在 $T$ 中，但 $T$ 為 tree，不含 cycle，故得矛盾。
\item[（2）] 任找一 cut set $S$ ，設 $G-E(S)=G_1 \bigcup G_2$ ，且 $G_1 \cap G_2=\varnothing$ ，設 $T$ 為 $G$ 之任一 spanning tree，則 $T$ 必須經過 $S$ 上的邊才能聯通 $G_1$ 與 $G_2$ ，故 $E(S) \cap E(T) \neq \varnothing$ 。
\item[（3）] 任找一 cut set $S$ ，設 $G-E(S)=G_1 \bigcup G_2$ ，且 $G_1 \cap G_2=\varnothing$ ，設 $C$ 為 $G$ 之任一 cycle，若 $C$ 只屬於 $G_1$ 或 $G_2$ ，表示 $C$ 與 $S$ 都沒有接觸到，則 $|E(C) \cap E(S)|=0$ ：偶數。若 $C$ 連接 $G_1$ 與 $G_2$ ，設從 $G_1$ 出發，則經 $S$ 上的某邊走到 $G_2$ 後，必再走 $S$ 上的別的邊回到 $G_1$ ；每次走向 $G_2$ ，亦必須走回 $G_1$ ，故 $|E(C) \cap E(S)|=$ 偶數。
\item[（4）] 若存在有一 $\operatorname{cut} \operatorname{set} S$ ，一 spanning tree $T$ ，使得 $E(S) \subseteq E(\bar{T})$ ，則表示此 $S$ 完全不與 $T$ 相交即存在 cut set $S$ ，存在 spanning tree $T, E(S) \cap E(T)=\varnothing$ ，與（2）矛盾。
\item[（5）] 若存在有一 $\operatorname{cut} \operatorname{set} S$ ，一spanning tree $T$ ，使得 $E(T) \subseteq E(\bar{S})$ ，則表示此 $T$ 完全不與 $S$ 相交即存在 cut set $S$ ，存在 spanning tree $T, E(S) \cap E(T)=\varnothing$ ，與（2）矛盾。
\end{itemize}