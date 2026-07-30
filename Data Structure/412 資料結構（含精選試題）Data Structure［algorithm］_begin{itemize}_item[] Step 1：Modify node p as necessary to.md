412 資料結構（含精選試題）
Data Structure

［algorithm］
\begin{itemize}
\item[] Step 1：Modify node p as necessary to reflect its status the desired element has been deleted．
\item[] Step 2：While p has zero elements and p is not the root Do
Begin
let $r$ be the parent of $p$ and
let q be the left or right sibling of p（as appropriate）；
if q is a 3－node then perform a rotation
else perform a combine；
$\mathrm{p}:=\mathrm{r} ;$
End；
\item[] Step 3：If has zero elements，than $p$ must be the root．The left child of $p$ becomes the new root and the node p is deleted．
\end{itemize}

\section*{9 －8 2－3－4 樹}

B－tree of order 4 。
定義：2－3－4 樹為一空的或滿足下列特性的搜尋樹：
\begin{itemize}
\item[（一）] 每個內部節點為：2－、3－或4－節點，2－節含1個元素，3－節點含 2 個元素，4－節點則含有 3 個元素。
\item[（二）] 假設 LeftChild 和 LeftMiddCild 代表 2－節點的兒子。又設 dataL 為此節點的元素而dataL．key 為其鍵。所有以 LeftChild 為根部之子 2－3－4 樹（Sub 2－3－4 樹）的元素其鍵小於 dataL．key，而所有以 LeftMidChild 為根部之子 2－3－4 樹的元素其鍵大於dataL．key 。
\item[（三）] 假設 LeftChild，LeftMidChild 和 RightMidChild 代表 3－節點的兒子。又設 dataL 和dataM 為此節點的二個元素，那麼 dataL．key 小於 dataM．key。所以以 LeftChild 為根部之子 2－3－4 樹的鍵小於 dataL．key，所有以 LeftMidChild 為根部之子 2－3－4 樹的鍵小於 dataL．key，所有以 LeftMidChild 為根部之子 2－3－4 樹的鍵小於 dataM．key而所有以 RightMidChild 為根部之子 2－3－4 樹的鍵大於 dataM．key。
\item[（四）] 假設 LeftChild、LeftMidChile、RightMidChild 和 RightChild 代表 4－節點的兒子。又假設 dataL、dataM、dataR 為此節點的三個元素，那麼 dataL．key＜dataM．key＜dataR．key，所有以 LeftChild 為根部之子 2－3－4 樹的鍵小於 dataL．key；所有以
\end{itemize}