326
離散數學（下）

\section*{特殊二元關係的運算－交集、聯集、合成}

設 $R, S$ 為兩個 $A$ 上之二元關係，
\begin{itemize}
\item[（1）] 若 $R, S$ 具反身性，則 $R \cap S 、 R \cup S 、 R \circ S 、 R^2$ 都具反身性。
\item[（2）] 若 $R, S$ 具對稱性，則 $R \cap S 、 R \cup S 、 R^2$ 都具對稱性。
\item[（3）] 若 $R, S$ 具遞移性，則 $R \cap S 、 R^2$ 都具遞移性。
\end{itemize}

【重要】
【證明】
\begin{itemize}
\item[（1）] $\because R$ 與 $S$ 具反身性，$\therefore \forall x \in A,(x, x) \in R,(x, x) \in S$ ，
$\therefore(x, x) \in(R \cap S),(x, x) \in(R \cup S),(x, x) \in R \circ S,(x, x) \in R \circ R$,
所以 $R \cap S 、 R \cup S 、 R \circ S 、 R^2$ 均具反身性。
\item[（2）] 對 $A$ 中元素 $a, b$ ，若 $a(R \cap S) b$ ，即 $a R b$ 且 $a S b$ ，
則因為 $R$ 與 $S$ 具對稱性，$\therefore b R a$ 且 $b S a$ ，即 $b(R \cap S) a$ ，$\therefore R \cap S$ 有對稱性。
若 $a(R \bigcup S) b$ ，即 $a R b$ 或 $a S b$ ，
但 $R$ 與 $S$ 具對稱性，$\therefore b R a$ 或 $b S a$ ，即 $b(R \bigcup S) a$ ，$\therefore R \bigcup S$ 有對稱性。
若 $(a, b) \in R^2$ ，即存在 $c$ ，使得 $(a, c) \in R$ 且 $(c, b) \in R$ ，
但 $R$ 具對稱性，$\therefore(c, a) \in R$ 且 $(b, c) \in R, \therefore(b, a) \in R^2, ~ \therefore R^2$ 有對稱性。
\item[（3）] 對 $A$ 中元素 $a, b, c$ ，若 $a(R \bigcap S) b$ ，且 $b(R \bigcap S) c$ ，
即 $a R b$ ，$a S b$ 且 $b R c, ~ b S c$ ，
則因為 $R$ 與 $S$ 具遞移性，$\therefore a R c, a S c$ ，即 $a(R \cap S) c, \therefore R \cap S$ 有遞移性。
若 $(a, b) \in R^2,(b, c) \in R^2$ ，
即存在 $x, y \in A$ ，使 $(a, x) \in R$ 且 $(x, b) \in R$ ；且使 $(b, y) \in R,(y, c) \in R$ ，
則因為 $R$ 具遞移性，$\therefore(a, b) \in R$ 且 $(b, c) \in R$ ，合成後得 $(a, c) \in R^2, \therefore R^2$ 有遞移性。
\end{itemize}

Note
\begin{itemize}
\item[（1）] 取 $A=\{1,2,3\}, R=\{(1,2)\}, S=\{(2,3)\}$ ，則 $R$ 、 $S$ 均有遞移性，但 $R \cup S=\{(1,2),(2,3)\}$沒有遞移性。
【93 成大工科】
\item[（2）] 取 $A=\{1,2,3\}, R=\{(1,2),(2,1)\}, S=\{(2,3),(3,2)\}$ ，則 $R$ 、 $S$ 具對稱性，但 $R \circ S=\{(1,3)\}$不具對稱性。
【97、99北科資工】
\item[（3）] 取 $A=\{1,2,3,4\}, ~ R=\{(1,2),(3,4)\}, ~ S=\{(2,3),(4,2),(4,3)\}$ ，則 $R$ 、 $S$ 具遞移性，但$R \circ S=\{(1,3),(3,2),(3,3)\}$ 不具遞移性。
\end{itemize}