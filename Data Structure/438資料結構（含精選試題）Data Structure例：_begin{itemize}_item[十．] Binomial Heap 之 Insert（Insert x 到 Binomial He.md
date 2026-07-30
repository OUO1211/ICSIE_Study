438
資料結構（含精選試題）
Data Structure

例：
\begin{itemize}
\item[十．] Binomial Heap 之 Insert
（Insert x 到 Binomial Heap a 中）
\begin{itemize}
\item[（一）] 將 x 放入一個 New Node
\item[（二）] 將 de Node 加入由 a 所指的 Double link Corular list 中
\item[（三）] 若 a 為 NULL，或 x 的鍵值小於由 a 所指 Node 之鍵值，重設 a pointer to this Node。
\item[] →O（1）：time complexity
\end{itemize}
\item[] 十一．Combine two Binomial Heap（a 與 b）
\begin{itemize}
\item[1．] 將 a 和 b 最 b 面的雙向鍵結結合成一個雙向 link list
\item[2．] 新的 B－Heap 指向 a 或 b，視何者有較小 key value 而定
\item[] → time complexity ：O（1）
\end{itemize}
\item[] 十二．Delete min element of Binomial Heap a
若 $\mathrm{a} \neq$ NULL，$\because \mathrm{a}$ 指向 min element，
∴ 刪除 a 所指 Node in Double link list，得到分開子樹
例：承上例，刪最小元素
\end{itemize}

（16）