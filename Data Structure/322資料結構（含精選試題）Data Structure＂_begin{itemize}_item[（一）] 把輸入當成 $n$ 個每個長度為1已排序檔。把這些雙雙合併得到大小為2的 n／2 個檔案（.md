322
資料結構（含精選試題）

Data Structure

＂
\begin{itemize}
\item[（一）] 把輸入當成 $n$ 個每個長度為1已排序檔。把這些雙雙合併得到大小為2的 n／2 個檔案（如果 n 為奇數，那麼有一個檔案大小為 1）。在把這些 n／2 個檔案雙雙合併直到只剩下一個檔案為止。下面的範例圖解此過程。
例：設輸入檔案為
$$
26,5,77,1,61,11,59,15,48,19
$$
下圖所示，即為在每次合併時所產生的結果：（合併樹）
從上列中，很明顯地可以看出合併排序時，需要對記錄處理好幾趟。每一次，被合併之檔案的長度為1，第二次時為2，第 i 次時被合併之檔案的長度就變為 $2^{i-1}$ 。因此，對於 n 個記錄，共需對其做 $\log _2$ n 次合併。因為每次合併兩個檔案，所需要的時間與記錄個數成線性關係。因此，每趟之費時為0（n）。因為共需 $\log _2 n$ 趟，故總時間為 $0\left(\mathrm{n} \log _2 \mathrm{n}\right)$ 。
\item[（二）] 為了方便於雙方合併排序演算法的設計，我們首先寫一個執行一趟合併工作的演算法 Mpass，如下：
Procedure Mpass（Var x，y：afile；n， 1 ：lnteger）；
｛This algorithm performs one pass of the merge sort．It merges adjacent pairs of subfiles of length 1 form the list x to list y．n is the number of record in x．\}
Var i，t ：Interger；
Begin
$$
\begin{aligned}
& \mathrm{i}:=1 ; \\
& \text { While } \mathrm{i}<=\left(\mathrm{n}-2^* 1+1\right) \text { Do Begin } \\
& \qquad \begin{array}{l}
\text { Merge }\left(\mathrm{x}, \mathrm{y}, \mathrm{j}, \mathrm{i}+1-1, \mathrm{i}+2^* 1-1\right) \\
\mathrm{i}:=\mathrm{i}+2^* 1 ;
\end{array}
\end{aligned}
$$
\end{itemize}