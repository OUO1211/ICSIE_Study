102
資料結構（含精選試題）
Data Structure

\section*{3－3 算術式的計算}

【重點】（1）中序式（infix）如何轉成前序式（prefix）及後序式（Postfix）。
\begin{itemize}
\begin{itemize}
\item[（2）] 後序式的計算過程。
\end{itemize}
\item[一．] 中序式（infix），前序式（prefix）及後序式（postfix）。
【定義】
\begin{itemize}
\item[1．] 中序式
\begin{itemize}
\item[（1）] 一般常用的算術式表示方法。
\item[（2）] ＜運算元1＞運算子＞＜運算元2＞例 ：a＋b
\item[（3）] 困難：算術運算須考慮括號，優先權及結合性，Compiler 處理時會很麻煩，須來回 SCAN 多次才能得出計算結果。
\item[（4）] 解決之道：將中序轉成後序表示法，以後序式處理。
\end{itemize}
\item[2．] 後序式（postfix 或 reverse polish notation）。
\begin{itemize}
\item[（1）] ＜運算元1＞＜運算元2＞＜運算子＞
\item[（2）] 使算術運算容易※因為：（1）postfix 中不再有括號存在。
\begin{itemize}
\item[（2）] postfix 的運算子的優先序及結合性已被預先處理。例 ： $\mathrm{ab}+$
\end{itemize}
\item[（3）] 中序轉後序之快速作法
\begin{itemize}
\item[（1）] 將中序式加上完整的括號。
\item[（2）] 移動運算子來取代最近的右括號。
\item[（3）] 刪去所有的左括號，並輸出剩下的項目。
\end{itemize}
\end{itemize}
\item[3．] 前序式（Prefix 或 Polish notation）。
\begin{itemize}
\item[（1）] 定義：＜運算子＞＜運算元1＞＜運算元2＞
\item[（2）] 例 ：＋ab
\item[（3）] 中序轉前序之快速法。
\begin{itemize}
\item[（1）] 將中序式加上完整的括號。
\end{itemize}
\end{itemize}
\end{itemize}
\end{itemize}