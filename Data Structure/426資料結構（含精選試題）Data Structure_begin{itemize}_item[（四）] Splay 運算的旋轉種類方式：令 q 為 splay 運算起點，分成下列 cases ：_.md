426
資料結構（含精選試題）
Data Structure
\begin{itemize}
\item[（四）] Splay 運算的旋轉種類方式：
令 q 為 splay 運算起點，分成下列 cases ：
\begin{itemize}
\item[1．] 若 q 為 NULL 或 root，則 splay 運算結束。
\item[2．] 若 q 有父節點 P 但沒有祖父節點，則執行下圖的旋轉並結束 splay 運算。

a，b，c 為子樹
\end{itemize}
\item[3．] 若 q 有父親節點 P 與祖父節點 gp，則旋轉分為 LL，LR，RL，RR 。如下圖所示。

（a）RR 類型

（b）RL 類型
注意：所有的旋轉都是將 q 向 tree 的上方移動，且在 splay 後以 q 為 search tree的新 root 節點。
\end{itemize}