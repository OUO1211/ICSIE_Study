430
資料結構（含精選試題）
■■

Data Structure
\begin{itemize}
\item[（五）] Leftist Tree 之相關運算的 Time Complexity
Insert，Delete $\min (\max )$ ，Combine（Union）operations are all $\mathrm{O}(\log N)$ 。
\item[（六）] Min Leftist Tree 的 Insert X 動作介紹
Steps：若樹為 A
\begin{itemize}
\item[1．] 建立一個只包含 X 的 min leftist tree B
\item[2．] 結合（Union）兩個 min leftist tree A and B
\end{itemize}
\item[（七）] Min Leftist Tree 的 Delete Min．element 動作介紹 Root 為最小值之所在。令 tree 為 ASteps：
\begin{itemize}
\item[1．] 結合 A．Lchild 和 A．Rchild
\item[2．] 刪除 Root of A
\end{itemize}
\item[（八）] Union of two min leftist Tree 運算
例子：
例 ：Combine two Min－Leftist Tree

（a）

（b）
\item[] 解：$-\because 2<5$ ，2 會是 root of New tree，且 a 的左子樹不變
- 結合 a 的右子樹與 b 樹，為新樹之右子樹
- ∵ 50＞5，5 為 root，5之左子樹不變
- 結合（50）與（5）的右子樹
－∵ 8＜50 ∴ 結合如下：
\end{itemize}