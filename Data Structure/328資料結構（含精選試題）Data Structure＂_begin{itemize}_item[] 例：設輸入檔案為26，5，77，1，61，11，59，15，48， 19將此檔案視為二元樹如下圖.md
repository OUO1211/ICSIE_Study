328
資料結構（含精選試題）

Data Structure

＂
\begin{itemize}
\item[] 例：設輸入檔案為
26，5，77，1，61，11，59，15，48， 19
將此檔案視為二元樹如下圖所示：
\begin{itemize}
\item[] Sorted ： 77
\end{itemize}
\end{itemize}

Sorted ：61， 77
Heap Size ： $\mathrm{i}=8$

Sorted ：59，61， 77
Heap Size ： $\mathrm{i}=7$
\begin{itemize}
\item[（四）] 處理程序之步驟
\begin{itemize}
\item[1．] 將輸入的 Records 建立成一個 Complete Binary Tree。
\item[2．] 轉換成 Heap Tree（Max Heap）。
\item[3．] 樹根是最大值，輸出樹根，並將二元樹中最後一個節點位置樹根中，再回到步驟二。如此步驟二、三反覆進行，可由大到小排序。
\item[] 例：35，21，37，15，52，15＋，5， 40 ，則 Heap Sort 過程如下：
\end{itemize}
\end{itemize}