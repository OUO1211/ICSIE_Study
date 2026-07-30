第七章 搜尋與排序 309
Search＆Sort

\section*{7－2 排序（Sort）}
\begin{itemize}
\item[（一）] 排序是指將某一群資料按照某一種排列的規則，重新安排此群資料的次序（Order）使其形成種遞增（或遞減）的線性次序關係（Linear Order）。
P．S！Linear Order：是一種 Partial Order 關係。
Partial Order：指一集合 S 的 Partial Order是一種關係R，若 S中的任何之元素a，b，c，則滿足下列三個條件：
\begin{itemize}
\item[1．] aRa 為 true（R 是反身性，Reflexive）
\item[2．] aRb 與 bRc，則 aRc（R 是遞移性，Transifive）
\item[3．] aRb 與 bRa，則 a＝b（R 是反對稱性，Antisymmetric）
\end{itemize}
\item[（二）] 穩定排序（Stable Sorting）
若檔中有數個鍵之值相同時，那排列 $\sigma$ 並非唯一。
設 $\sigma_{\mathrm{s}}$ 具有以下之性質 ：
\begin{itemize}
\item[1．] $\mathrm{K}_{\sigma s(\mathrm{i})} \leq \mathrm{K}_{\sigma s(\mathrm{i}+1)}, 1 \leq \mathrm{i} \leq \mathrm{n}-1$
\item[2．] 在輸入檔案中，若 $i<j$ 且 $K_i=K_j$ ，那在排序之檔案中 $R_i$ 排列在 $R_j$ 之前。一個排序方法能產生如 $\sigma_{\mathrm{s}}$ 之排列者稱為穩定的排序法。
\end{itemize}
\item[（三）] 排序的分類
$\left\{\begin{array}{l}\text { Internal Sorting } \\ \text { External Sorting }\end{array}\right.$
\begin{itemize}
\item[1．] 內部排序法
即檔案容量小得足以整個搬到主記憶體中進行排序的方法。
\item[2．] 外部排序法
即資料量大，無法以全部置於主記憶體中進行排序，所以須藉助輔助記憶體的排序方法。
\end{itemize}
\item[（四）] 各種內部排序法：
\begin{itemize}
\item[1．] 插入排序法（Insertion Sort）
\item[2．] 快速排序法（Quick Sort）
\item[3．] 合併排序法（Merge Sort）
\item[4．] 堆積排序法（Heap Sort）
\item[5．] 基數排序法（Radix Sort）
\item[6．] 選擇排序法（Selection Sort）
\item[7．] 氣，泡排序法（Bubble Sort）
\end{itemize}
\end{itemize}