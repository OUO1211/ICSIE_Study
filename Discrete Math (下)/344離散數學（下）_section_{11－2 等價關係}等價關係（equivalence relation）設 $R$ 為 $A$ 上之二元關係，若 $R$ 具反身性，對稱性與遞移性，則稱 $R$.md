344
離散數學（下）

\section*{11－2 等價關係}

等價關係（equivalence relation）
設 $R$ 為 $A$ 上之二元關係，若 $R$ 具反身性，對稱性與遞移性，則稱 $R$ 為一等價關係。
Note
\begin{itemize}
\item[（1）] 考慮 $A$ 中元素 $a$ ，定義 $[a]=\{x \in A \mid a R x\}$ ，表示與 $a$ 有等價關係 $R$ 的元素所成集合，稱 $a$的等價類（equivalence class、又稱為 cell）。每一等價類必不為空集合。
\item[（2）] 定義 $A / R=\{[a] \mid a \in A\}$ 表示 $A$ 的相異等價類所成之集合，稱商集合（quotient set）。
\end{itemize}

例如：
考慮定義在 $\{1,2,3,4,5\}$ 的二元關係 $R=\{(1,1),(2,2),(3,3),(4,4),(5,5),(1,3),(3,1),(1,4)$ ，$(4,1),(3,4),(4,3)\}$ 為一等價關係。其關係圖型與關係矩陣如下，而且有三個相異等價類：
\begin{itemize}
\item[] $[1]=\{1,3,4\},[2]=\{2\},[5]=\{5\}$ ．
$$
\left.\begin{array}{c} 
\\
1 \\
3 \\
4 \\
2 \\
5
\end{array} \begin{array}{ccccc}
1 & 3 & 4 & 2 & 5 \\
{\left[\begin{array}{l}
1 \\
1 \\
1 \\
0 \\
0
\end{array}\right.} & 1 & 1 & 0 & 0 \\
1 & 1 & 0 & 0 & 0 \\
0 & 0 & 0 & 1
\end{array}\right]
$$
\end{itemize}