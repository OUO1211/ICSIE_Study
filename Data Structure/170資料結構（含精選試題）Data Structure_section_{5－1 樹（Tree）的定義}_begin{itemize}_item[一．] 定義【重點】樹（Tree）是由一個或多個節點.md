170
資料結構（含精選試題）
Data Structure

\section*{5－1 樹（Tree）的定義}
\begin{itemize}
\item[一．] 定義【重點】
樹（Tree）是由一個或多個節點（Node）構成的有限集合，並具有以下兩個特性：
\begin{itemize}
\item[（一）] 有一特定節點稱為樹根（Root）。［樹不可以為空］
\item[（二）] 其餘的節點分成 $\mathrm{n}(\mathrm{n} \geq 0)$ 個互斥之集合 $\mathrm{T}_1, \mathrm{~T}_2, \cdots, \mathrm{~T}_{\mathrm{n}}$ 。而這些互斥之集合又都是一棵樹， $\mathrm{T}_1, \cdots, \mathrm{~T}_{\mathrm{n}}$ 稱為樹根節點的子樹（Subtree）。
\end{itemize}
\end{itemize}

\section*{二．樹的基本術語【重點】}
\begin{itemize}
\begin{itemize}
\item[（一）] 分支度（Degree）＜對節點而言＞
定義：每個節點的子樹個數。
例：A 的 Degree 為 3
E 的 Degree 為 2
C 的 Degree 為 1
K 的 Degree 為 0
\item[（二）] 樹葉（Leaf）或終端節點（Terminal Node）
定義：分支度（Degree）為零的節點。
例：K，L，F，G，M，I，J 皆為 Leaf。
\item[（三）] 非終端節點（Nonterminal Node）或 Non－Leaf Node
定義：在一樹中，所有的非樹葉節點，稱之。亦即 Degree $\geq 1$ 的節點。例 ：A，B，C，D，E，H
\end{itemize}
\item[（四）] 子點（Child）與父點（Parent）
定義：某節點 x 的所有子樹的樹根，稱為 x 節點的子點，而 x 為它們的父點（Parent）＊例：A 的子點為 B，C，D
\end{itemize}