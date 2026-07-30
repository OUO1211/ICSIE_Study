第九章 高等樹結構
415
Advanced Tree Structure

\section*{9－10 紅黑－樹（Rod－Black Tree）}

一紅－黑樹為表示成 2－3－4 樹的二元樹。紅－黑樹節點的兒子指標有二種型態：紅和黑。如果兒子指標沒有出現在原來 2－3－4 樹中，它即是紅指標（red pointers）。否則為黑指標（black pointers）。

2－3－4 樹，轉換成紅－黑樹的方法如下：
\begin{itemize}
\item[（一）] 2－節點 p 用 Red Black 節點 q 來表示，而雙方的顏色欄位皆為黑。而且 data＝dataL；$\mathrm{q} \uparrow$. LeftChold $=\mathrm{p} \uparrow$. LeftChild． $\mathrm{q} \uparrow$.
RightChild $=\mathrm{p} \uparrow$ ．LeftMidChild。
\item[（二）] 3－節點 p 用二個以下紅指標連接的 RedBlack 節點來表示。有兩種方法來做此轉換。
\item[（三）] 4－節點用三個 Red Black 節點來表示。
\item[（3）] 紅－黑樹有下列特性
\item[（一）] 是一二元搜尋樹。
\item[（二）] 每個根到樹葉路徑有相同的黑鏈結（black links）數目。
\item[（三）] 根部到樹葉路徑上沒有二個以上的（含二個）連續的紅指標。
\end{itemize}