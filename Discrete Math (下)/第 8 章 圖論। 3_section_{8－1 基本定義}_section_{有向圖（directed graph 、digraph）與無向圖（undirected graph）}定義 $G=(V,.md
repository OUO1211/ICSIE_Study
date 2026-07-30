第 8 章 圖論। 3

\section*{8－1 基本定義}

\section*{有向圖（directed graph 、digraph）與無向圖（undirected graph）}

定義 $G=(V, E)$ 為一有向圖，
其中，非空集 $V$ 稱為點集（vertex set、node set），$E$ 稱為邊集（edge set），$E \subseteq V \times V$ 。若不考虑邊的方向性，則稱 $G=(V, E)$ 為一無向圖。

Note
\begin{itemize}
\item[（1）] 有些模型需要同時出現有向邊與無向邊，這種圖被稱做混合圖（mixed graph）。
\item[（2）] 若存在相異兩點間至少二個邊，則稱 $G$ 為一多重圖（multi－graph）。
\item[（3）] 若一個邊的兩端點相同，則稱此邊為迴圈（loop），同一點可以有多個 loop ；Rosen 的書上把允許 loop 與重邊的圖稱為虛擬圖（pseudo－graph）。
【107 中央資工】
\item[（4）] 沒有重邊且沒有迴圈（loop－free）的稱為簡單圖（simple graph）。
\item[（5）] $n$ 點無向簡單圖的邊數 $\leq\binom{ n}{2} ; n$ 點無向簡單圖共 $2^{\binom{n}{2}}$ 種。
【重要】證明：$n$ 相異點，任兩點恰一邊，邊數最多，為 $\binom{n}{2}$ ；另外，這些邊出現與否都決定了不同的圖，故有 $2 \times 2 \times \cdots \times 2=2^{\binom{n}{2}}$ 個不同的圖。
\item[（6）] 一個沒有任何邊的點稱為孤立點（isolated vertex）。
\item[（7）] 考慮有向圖 $G$ ，邊 $(a, b)$ 的 $a$ 稱為起點，$b$ 稱為終點且 $(a, b) \neq(b, a)$ 。
\item[（8）] $n$ 點有向簡單圖的邊數 $\leq 2\binom{n}{2} ; n$ 點有向簡單圖共 $2^{2\binom{n}{2}}$ 種。【82 交大資科】【94 中央資工】【107台大資工】
\item[（9）] 允許每點有一個迴圈的 $n$ 點無向簡單圖共 $2^n \times 2^{\binom{n}{2}}$ 種。
【85 成大工科】【89 政大資科】【107 台大資工】
\end{itemize}