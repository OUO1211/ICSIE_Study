184
資料結構（含精選試題）
Data Structure
\begin{itemize}
\item[四．] 為了使每一個 Thread 都有節點可指，亦加入一個 Head Node $t$ ，所以上圖將以如下之形式出現：
\item[] 而一個空的二元樹，則如下所示：

\begin{tabular}{|l|l|l|l|l|}
\hline LeftThread & LeftChild & data & RighChild & RightThread \\
\hline true & & & & false \\
\hline A & & & & \\
\hline
\end{tabular}
\end{itemize}

\section*{五．使用引線二元樹的效果}
\begin{itemize}
\begin{itemize}
\item[（一）] 簡化中序演算法
\item[（二）] 中序追蹤時，沒有利用任何有關中序先行者的資料，而且無須額外堆疊支援，因為不用遞迴。
\item[（三）] Insuc 演算法
目的：找引線二元樹中的任一節點 x 的中序後繼者。
觀念：如果 x ↑ ．RightThread＝true 那麼 x 的中序後繼者就是 x ↑ ．RightChild；否則的話 x 的中序後繼者就是從 x 的右兒子之左兒子鏈結（含右兒子），直到找到 LeftThread＝true 之節點。
程式 ：function insuc（tree：ThreadedPointer）：ThreadedPointer；
｛Find the inorder successor of tree in a threaded binary tree．\}
var temp ：ThreadedPonter；
begin
temp ：＝tree ↑ ．RightChild；
if not tree ↑ ．RightThread then
\end{itemize}
\end{itemize}