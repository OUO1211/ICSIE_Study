424
資料結構（含精選試題）
■■■

Data Structure
步驟二：若節點 P 是終端節點，則分成兩種情況：
\begin{itemize}
\item[1．] 將鍵值 X 刪除後，若節點 P 的剩餘鍵值 $\geq\lceil\mathrm{m} / 2\rceil-1$ ，則符合 B－tree 的定義，不需再做調整，這是最簡單的情況。
\item[2．] 將鍵值 X 刪除後，節點 P 的剩餘鍵值已少於［m／2］－1，則不符合 B－tree定義，必須予以調整，茲依情況可再區分成下列三種情形來調整：
\begin{itemize}
\item[（1）] 首先找到右邊最靠近的兄弟（sibling）節點 $\mathrm{P}^{\prime}$ ，右 $\mathrm{P}^{\prime}$ 內含鍵值數尚大於$\lceil\mathrm{m} / 2\rceil-1$ ，則取出 $\mathrm{P}^{\prime}$ ，中最小鍵值，並置於其 parent 節點，且將 parent節點中，第一個大於等於鍵值 X 的鍵值移到 P 中。如此，P 與 parent節點的鍵值數均不變，而右邊的 sibling 節點 $\mathrm{P}^{\prime}$ 則少一個鍵值。
\item[（2）] 若右邊找不到，若找尋左邊最靠近的兄弟（sibling）節點 $\mathrm{P}^{\prime}$ ，若 $\mathrm{P}^{\prime}$ 內含鍵值數尚大於 $\lceil\mathrm{m} / 2\rceil-1$ ，則取出 $\mathrm{P}^{\prime}$ ，中最大鍵值，並置於 parent 節點，且將 parent節點中第一個小於等於 X 的鍵值移到 P 中。如上，P 與 parent節點的鍵值數均不變，而 $\mathrm{P}^{\prime}$ 則少一。
\item[（3）] 若左右兄弟節點均找不到，則找尋 parent 節點，找到 $K_i \leq X \leq K_i+1$ ，然後搜尋指標 $\mathrm{A}_{\mathrm{i}}+1$ 的節點 $\mathrm{P}^{\prime}$ ，並且將原來節點 P 中剩餘的鍵值，以及 parent 節點第一個大於 $X$ 的鍵值加到節點 $P^{\prime}$ 中。
\end{itemize}
\end{itemize}

步驟三：若節點 $P$ 不是終端節點，則令 $K_i=X$ ，接著搜尋指標 $A_i$ 到一節點 $P^{\prime}$ ，$P^{\prime}$ 中包含一鍵值 Y，且 Y 是所有大於X的鍵值中最小的，將Y 移至原來 P 節點 $K_i$的位置上，若 $\mathrm{P}^{\prime}$ 中的鍵值數因而小於 $\lceil\mathrm{m} / 2\rceil-1$ 則進行步驟二的終端節點調整。

例題 9－1
下圖是一個 B－tree of order 3 ，請畫出（一）删除 58 （二）删除 65 動作後的圖形。

解
由於 $\mathrm{m}=3$ ，因此各節點的鍵值 $\lceil\mathrm{m} / 2\rceil-1 \sim \mathrm{~m}-1$ 之間，亦即 $1 \leq$ 鍵值數 $\leq 2$ 。