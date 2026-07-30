326
資料結構（含精選試題）

Data Structure

的 •
\begin{itemize}
\item[3．] 樹根（Root）的值是 Heap Tree 最大的。
\item[（三）] 同理 Min Heap 的定義類似上面所述，即：
\begin{itemize}
\item[1．] 是一個完整二元樹（Complete Binary Tree）。
\item[2．] 每個節點的值小於等於其子點的值。
\item[3．] 樹根（Root）的值是 Heap Tree 中最小的。
\item[] 例：Max Heap
\end{itemize}
\end{itemize}

例：Min Heap

【程式】調整最大堆積
Procedure Adjust（Var tree ：afile；i，n ：Integer）；
｛Adjust the binary tree with root i to satisfy the heap property．The left and right subtrees of i，i ．c．，whith root 2i and 2i＋1，already satisfy the heap property．No node has index greater than n ．\}
Var j，k ：Integer；
r ：records；
done ：Boolean；
Begin
done ：＝false；
r ：＝tree［i］；
$\mathrm{k}:=$ tree［i］．key；
j ：＝2＊i；
While（ $(\mathrm{j}<=\mathrm{n})$ and not done）Do