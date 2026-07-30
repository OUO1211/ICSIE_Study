第五章 樹與二元樹
171
Tree＆Binary Tree
\begin{itemize}
\item[B] 的子點為 E，F
又 G 的父點為 C
D 的父點為 A
\item[（五）] 兄弟（Sibling）
定義：同一個父點的所有子點互稱為 Sibling。
例：B，C，D 各為彼此的兄弟。
\item[（六）] 祖先（Ancestors）
定義：同一個節點的祖先—乃是從樹根到該節點路徑中，所包含的所有節點。例：M 的祖先是 A，D，H
\item[（七）] 階段（Level）
定義：樹根的階度為1，若某節點的階度為 I，則子點的階度就為 I＋1。
例：A 的 Level 為 1
B，C，D 的 Level 為 2
M 的 Level 為 4
\item[（八）] 樹的分支度（Degree of Tree）＜對樹而言＞
定義：樹中的節點，具有最大的 Degree 數目，稱為該樹的分支度。
例：此樹的 Degree 為 3
\item[（九）] 高度（Height）或深度（Depth）＜對樹而言＞
定義：一棵樹之節點所具有的最大階度，稱為該樹的高度或深度。
例：此樹的高度為 4
\item[（十）] 森林（Forest）
定義：森林乃是 $\mathrm{n}(\mathrm{n} \geq 0)$ 個互斥樹之集合。［森林可以為空］
例：把 A 去掉，就可得到一個由三棵樹構成的森林。
\end{itemize}

\section*{三．樹的資料結構表現方法}
\begin{itemize}
\item[（一）] 利用 Linked List
假設有 n 個 nodes ，tree degree 為 k ，則 Node structure 設計如下：

\begin{tabular}{|l|l|l|l|l|}
\hline DATA & Link 1 & Link 2 & ⋯ & Link k \\
\hline
\end{tabular}
但其缺點為：
\begin{itemize}
\item[（1）] 浪费記憶體空間，有約 $\frac{k-1}{k}$ 比例的 Link 欄是空的。
\end{itemize}
\end{itemize}