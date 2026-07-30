128
資料結構（含精選試題）
■■■
Data Structure

\section*{4－1 為何要 Linked List？}
\begin{itemize}
\item[一．] 線性串列（Linear List，Ordered List，Dense List）
有二種方法來儲存：
\begin{itemize}
\item[（一）] 利用陣列來循序對映（Sequential Mapping），以連續空間來儲存。
\item[（二）] 使用指標形成鏈結串列（Linked List），不必以連續空間來儲存。
\end{itemize}
\item[二．] 比較 Sequential List 與 Linked List 的優缺點【典型考題】
\begin{itemize}
\item[（一）] Linked List 在插入／刪除一個節點很容易，只需要改變指標即可；而 SequentialList 需要移動其他節點的位置，［平均 $=\frac{\mathrm{n}+1}{2}$ 次］。
\item[（二）] Linked List 的共用比較容易，兩個不同的串列若有共同的子串列時，則可共用此串列以節省空間，但 Sequential List 則不可以共用。
\item[（三）] Linked List 合併（Merge）兩個串列成為一個串列或分裂成二個小串列，是很容易的。
\item[（四）] Linked List 不用事先預留一塊大的連續空間，但 Sequential List 則需要。
\item[（五）] Linked List 需要額外的空間來儲存指標，比起 Sequential List 較費一些空間。
\item[（六）] Sequential List 執行循序取出比 Linked List 快，因為 Linked List 中每次讀取一個Node 時，必須花時間去取出鏈結指標，以便讀取下一個節點。
\item[（七）] Sequential List 可以隨意讀取第 i 個 Node，由基底位址加上 C • i 長度即可（c 為元素大小），但 Linked List 卻要從頭循序讀下來。
\end{itemize}
\end{itemize}

\section*{4－2 Linked List 的 Data Structure}
\begin{itemize}
\item[] －．Node
DATA LINK
Data：儲存資料
Link ：pointer to Next Node
\end{itemize}