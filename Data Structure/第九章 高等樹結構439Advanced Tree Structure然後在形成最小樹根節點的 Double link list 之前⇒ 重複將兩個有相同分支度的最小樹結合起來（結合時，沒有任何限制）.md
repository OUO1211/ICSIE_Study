第九章 高等樹結構
439
Advanced Tree Structure

然後
在形成最小樹根節點的 Double link list 之前
⇒ 重複將兩個有相同分支度的最小樹結合起來（結合時，沒有任何限制）
例：承上，結合 8 和 7 或 3 和 12

⇒ 重設指標為（3）

\section*{† 三．Fibonacci Heap}
\begin{itemize}
\item[（一）] 支援三種 Binomial Heap 之 Insert，Delete min or max 及 Combine 運算 • 外帶下列兩種 operations
\begin{itemize}
\item[1．] 刪除指定 Node 之元素
\item[2．] 減少某個 Node 之鍵值
\begin{itemize}
\item[（1）] 可在 $O(1)$ 分攤時間內完成
\item[（2）] 可在 $O(\log n)$ 分攤時間內完成
\end{itemize}
\end{itemize}
\item[（二）] 分為二種：min－Fibonacci Heap 及 max－Fibonacci Heap前者為最小樹的集合，後者為最大樹的集合
\begin{itemize}
\item[] B－Heap 可以視為 F－Heap 之特例
\end{itemize}
\item[（三）] 從 F—累堆刪除一個元素要從 F－累堆 a 刪除任一節點 b，以下列方式完成：
\begin{itemize}
\item[1．] $a=b$ ，則執行一個刪除最小元素；否則執行下列步驟 2， 3 和 4 。
\item[2．] 從所屬的雙向鏈結串列中刪除 b 。
\end{itemize}
\end{itemize}