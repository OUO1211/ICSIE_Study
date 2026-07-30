第九章 高等樹結構
409
Advanced Tree Structure

為此節點的二個元素。那麼，dataL．key 小於 dataR．key，以 LeftChild 為根部的2－3 子樹的鍵小於 dataL．key 而所有以 MiddleChild 為根部的 2－3 子樹的鍵小於dataR．key 而大於 dataL．key。而以 RinghtChild 為根部的所有鍵大於 dataR．key。
\begin{itemize}
\item[4．] 所有外部節點皆位於同一階層。
\item[（四）] 高度 $h$（亦即：外部節點位於階層 $h+1$ ）的2－3樹的元素數目介於 $2^h-1$ 和 $3^h-1$ 之間。含有 n 個元素的 2－3 樹，其高度介於 $\left[\log _3(\mathrm{n}+1)\right]$ 和 $\left[\log _2(\mathrm{n}+1)\right]$ 之間。
\item[] 2－3 樹可使用型態 TwoThreePtr 的節點來表示，其定義為：
\begin{itemize}
\item[] type TwoThreePtr = ↑ TwoThree；
TwoThree＝record
dataL：element；
dataR：element；
LettChild：TwoThreePtr；
MiddleChild：TwoThreePtr；
RightChild：TwoThreePtr；
end；
\end{itemize}
\end{itemize}

《圖示》2－3樹的例子
\begin{itemize}
\item[（五）] 2－3 樹的搜尋
Procedure Search23（t：TwoThreePtr；x：integer；
var p：TwoThreePtr）；
｛Search the 2－3 tree t for an element with key x．If this key is not in the tree，then return nil in p．Otherwise，return a point to the node that contains key．\}
Var NotDone ：Boolean；
Begin
NotDone ：＝true；p ：＝t；
while（ $p<>$ nil ）and NotDond do
\end{itemize}