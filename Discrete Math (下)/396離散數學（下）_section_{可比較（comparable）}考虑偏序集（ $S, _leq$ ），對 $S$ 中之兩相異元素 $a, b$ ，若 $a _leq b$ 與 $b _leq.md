396
離散數學（下）

\section*{可比較（comparable）}

考虑偏序集（ $S, \leq$ ），對 $S$ 中之兩相異元素 $a, b$ ，若 $a \leq b$ 與 $b \leq a$ 恰一成立，即稱 $a, b$ 可比較，否則稱 $a, b$ 不可比較。

例如，
$(P(\{1,2,3\}), \subseteq)$ 中，$\{1\} \subseteq\{1,2\}$ ，故兩者可比較，但｛2，3\}與\{1,3\}兩者不可比較。
$\left(D_{12}, \mid\right)$ 中， $2 \mid 12$ ，故兩者可比較，但 2 與 3 兩者不可比較。

\section*{全序關係（Totally ordering relation）}

考虑偏序集 $(S, \leq)$ ，若 $S$ 中之任相異元素均可比較，則稱 $\leq$ 為一全序關係，
且稱 $(S, \leq)$ 為一全序集（TOS）。

\section*{Note}
\begin{itemize}
\item[（1）] $(N, \leq),(Z, \geq)$ 為全序集。
\end{itemize}

【99 中興資科】
\begin{itemize}
\item[（2）] 考慮質數 $p$ ，則 $\left(\left\{1, p, p^2, \ldots, p^k\right\}, \mid\right)$ 為全序集。
\end{itemize}

【91 交大資科】
\begin{itemize}
\item[（3）] 拓樸排序演算法（Topological sorting algorithm）：每次取出 Hasse 圖的任一個 minimal並重複到最後沒有點剩下。所得又稱為一致列舉數列（consistent enumeration），是一種不違反原來先後的一種順序，也被稱做把偏序化成全序。
【105高雄資工】
\item[（4）] 若 $(S, \leq)$ 為一全序集，且滿足 $S$ 的任意非空子集均有最小元素，則稱 $(S, \leq)$ 為一良序集（well ordered set）。例如 $\left(Z^{+}, \leq\right)$。
【 99 中興資科】【 99 台大電機】
\end{itemize}