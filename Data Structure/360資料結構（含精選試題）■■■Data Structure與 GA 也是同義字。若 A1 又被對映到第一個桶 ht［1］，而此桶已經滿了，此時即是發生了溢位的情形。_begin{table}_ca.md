360
資料結構（含精選試題）
■■■

Data Structure

與 GA 也是同義字。
若 A1 又被對映到第一個桶 ht［1］，而此桶已經滿了，此時即是發生了溢位的情形。

\begin{table}
\captionsetup{labelformat=empty}
\caption{SLOT 1 SLOT 2}
\begin{tabular}{|l|l|l|}
\hline 1 & A & A2 \\
\hline 2 & 0 & 0 \\
\hline 3 & 0 & 0 \\
\hline 4 & 0 & 0 \\
\hline 5 & 0 & 0 \\
\hline 6 & 0 & 0 \\
\hline 7 & GA & G \\
\hline ： & ： & ： \\
\hline 26 & 0 & 0 \\
\hline \multicolumn{3}{|c|}{0 代表空槽} \\
\hline
\end{tabular}
\end{table}
\begin{itemize}
\item[（七）] 散置法的優點
\begin{itemize}
\item[1．] 使用 Hashing Search，檔案不須事先排序過。
\item[2．] 在沒有 Collision 及 Overflow 的情形下，只需一次讀取即可，且其搜尋速度與資料量多寡無關。
\item[3．] 保密性高，若不知 Hashing Function，無法擷取資料。
\item[4．] 可做資料壓縮（Data Compression），利用適當的 Hashing Function，可將資料壓縮到較小的範圍內，節省空間。
\end{itemize}
\end{itemize}

總而言之，雜湊（Hashing）法是透過一雜湊函數 f 將識別字做一個轉換得到表中之位址。f 的選擇以計算簡單且碰撞少者為佳。雜湊技術須選擇好的雜湊函數及必要的 overflow 處理。

\section*{8－3 雜湊函數}
\begin{itemize}
\item[（一）] 一個好的 Hashing Function 應具備的性質如下：
\begin{itemize}
\item[1．] 計算簡單。
\item[2．] 碰撞少。
\item[3．] 不要造成雑湊表局部偏重的情形。
\end{itemize}
\end{itemize}