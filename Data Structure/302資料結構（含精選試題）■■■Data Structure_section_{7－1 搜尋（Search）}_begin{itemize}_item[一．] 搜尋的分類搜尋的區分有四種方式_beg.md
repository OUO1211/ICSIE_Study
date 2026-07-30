302
資料結構（含精選試題）
■■■

Data Structure

\section*{7－1 搜尋（Search）}
\begin{itemize}
\item[一．] 搜尋的分類
搜尋的區分有四種方式
\begin{itemize}
\item[（一）] 內部或外部搜尋。
\begin{itemize}
\item[1．] Internal Searching（內部搜尋）
若要找尋的表格資料較小時，可直接置於記憶體中，來進行搜尋的工作，稱為Internal Searching。
\item[2．] External Searching（外部搜尋）
若要找的對象是大檔案，無法一次置於記憶體，通常儲存於輔助記憶體中（如Disk），因此稱之。
\end{itemize}
\item[（二）] 靜態（Static）搜尋或動態（Dynamic）搜尋 ：
靜態搜尋：指靜態之表格或檔案，資料是固定的，加入或刪除動作不多，且能事先預知。
動態搜尋：資料是變動的，加入或刪除之動作頻繁且無法事先預知。
\item[（三）] 比較整個鍵值或部份鍵值之搜尋。
\item[（四）] 以 Actual Key 或 Transformation Key 之搜尋。
例：Transformation Key Searching 是指 Hashing。
\end{itemize}
\end{itemize}

\section*{二．四種不同的搜尋方法}
\begin{itemize}
\begin{itemize}
\item[（一）] 循序搜尋（Sequential Search）或線性搜尋（Linear Searching）
\begin{itemize}
\item[1．] 是一種相當簡單的方法。
\item[2．] 被搜尋的檔案，不須事先經過排序。
\item[3．] 找尋的過程是從檔案的第一筆記錄（或最後一筆記錄）開始，依序一個一個地比較每個鍵值，直到找到所要的記錄為止，若搜尋完整個資料檔案仍未找到符合的鍵值時，則表示該筆記錄不存在，為失敗搜尋。
\item[4．] 有兩種方式：
$\left\{\begin{array}{l}\text { Non－Sentinel Sequential Searching } \\ \text { Sentinel Sequential Seaching }\end{array}\right.$
\begin{itemize}
\item[（1）] Non－Sentinel Sequential Searching
假設一個含有 n 個記錄，鍵值為 Key 的檔案 f，i 為輸出參數
Procedure Non＿Sentinel（ $\mathrm{F}: \mathrm{file}, \mathrm{i}, \mathrm{n}, \mathrm{k}:$ integer）
Begin
\end{itemize}
\end{itemize}
\end{itemize}
\end{itemize}