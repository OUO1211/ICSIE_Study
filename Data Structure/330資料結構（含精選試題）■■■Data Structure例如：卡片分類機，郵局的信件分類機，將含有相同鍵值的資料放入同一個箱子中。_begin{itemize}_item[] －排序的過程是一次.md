330
資料結構（含精選試題）
■■■

Data Structure
例如：卡片分類機，郵局的信件分類機，將含有相同鍵值的資料放入同一個箱子中。
\begin{itemize}
\item[] －排序的過程是一次使用一個位數來做比較，通常依其比較方向又分為兩種：
\begin{itemize}
\item[（一）] MSD（Most Significant Digit First）
\item[（二）] LSD（Least Significant Digit First）
\end{itemize}
\item[] －整個處理步驟均是在作 Distribution 與 Merge 的動作。
\item[（一）] LSD 法
\begin{itemize}
\item[1．] 假設以數字的基底 r，作為 LSD 排序數字的根據。若有 m 位數字（不是 m 個）則 LSD 須要 m 次的 Pass，每一次要執行分配與合併的工作。
\item[2．] 需要準備 r 個 buckets（編號：$\phi \sim \mathrm{r}-1$ ）
\end{itemize}
\end{itemize}

例子

$\mathrm{i}=3$
第一趟後之鏈結