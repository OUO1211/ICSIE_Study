第五章 樹與二元樹
183
Tree＆Binary Tree

\section*{二．從二元樹變成中序引線二元樹的作法}

步驟：（考慮一節點 $\mathrm{P}, \mathrm{P}$ is the any node of binary tree）
\begin{itemize}
\item[1．] 若 P ↑ ．RightChild 原來為 nil，則將此指標改為 Thread 指標，指向中序（LDR）追蹤順序中， P 的下一個節點。
\item[2．] 若 P ↑ ．LeftChild 原來等於 nil，則以引線（Thread）指標來取代，並指向中序追蹤順序中 P 的前一個節點。
\end{itemize}

例：若一二元樹如下：

→則引線二元樹如下：（【註】虛線代表引線）
\begin{itemize}
\item[三．] 在記憶體表示方式中，我們必須能區分引線指標與正常指標。故在每一節點增加兩個布林欄 LeftThread 及 RightThread。
\end{itemize}

如果 Tree ↑ ．Left Thread＝true，則 tree ↑ ．LeftChild 為一條引線：否則的話，它是一個指向 LeftChild 的指標。同樣地，假如 Tree ↑ ．Right－Thread＝true，則 Tree ↑ ．RightChild會是一條引線；否則，它是一個指向 RightChild 的指標。