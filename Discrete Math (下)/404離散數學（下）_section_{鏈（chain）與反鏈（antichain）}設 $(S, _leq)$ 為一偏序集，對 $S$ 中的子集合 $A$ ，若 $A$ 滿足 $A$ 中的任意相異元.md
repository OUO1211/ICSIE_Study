404
離散數學（下）

\section*{鏈（chain）與反鏈（antichain）}

設 $(S, \leq)$ 為一偏序集，對 $S$ 中的子集合 $A$ ，若 $A$ 滿足 $A$ 中的任意相異元素 $a, b:$
\begin{itemize}
\item[（1）] $a \leq b$ 與 $b \leq a$ 恰有一者成立，則稱 $A$ 為一個锺。
\item[（2）] $a \leq b$ 與 $b \leq a$ 均不成立，則稱 $A$ 為一個反锺。
\end{itemize}

例如
\begin{itemize}
\item[（1）] $(N, \leq)$ 中，$N$ 即為一鏈。
\item[（2）] $A=\{1,2,3\}, ~(P(A), \subseteq)$ 中，
$\{\varnothing,\{1\},\{1,2\},\{1,2,3\}\}$ 即為一鏈（也是最長的），｛ 1\}, \{2\}, \{3\}\} 即為一反鏈。
\item[（3）] $\left(D_{12}, \mid\right)$ 中，$\{1,2,12\}$ 為一鏈，$\{3,4\}$ 為一反鏈。
\end{itemize}

Note
\begin{itemize}
\item[（1）] 鏈又稱為線性有序集（linearly ordering set）。
\item[（2）] 若 $S$ 本身即為一鏈，則 $S$ 為一全序集。
\item[（3）] $n$ 元集 $A$ 上定義的二元關係中，有 $n!$ 種為全序。
\item[（4）] 鏈中的元素個數定義為此鏈的長度。
\item[（5）] $|A|=n$ ，則偏序集（ $P(A), \subseteq$ ）中最長鏈長度為 $n+1$ 。
【證明】
設 $A=\left\{a_1, a_2, \ldots, a_n\right\}$ ，則 $\varnothing,\left\{a_1\right\},\left\{a_1, a_2\right\}, \ldots,\left\{a_1, a_2, \ldots, a_n\right\}$ ，
這 $n+1$ 個 $A$ 的子集所構成的 path 就是一個 $P(A)$ 中的最長鏈。
\item[（6）] 設 $(S, \leq)$ 為一偏序集，則
\begin{itemize}
\item[（i）] 若 $S$ 中最長鏈的長度為 $n$ ，則 $S$ 可分割成 $n$ 個互斥的反鏈。
【93 成大電機】【96 清大資工】
\item[（ii）] 若 $|S|=m n+1$ ，則 $S$ 中包含一個 $m+1$ 個元素的反鏈，或長 $n+1$ 的鏈。
【證明】
\item[（i）] 對 $n$ 作歸納法：當 $n=1$ ，即 $S$ 中最長鏈長度為1，即任兩個元素都不相關，所以$S$ 本身就是一個反鏈。設 $n=k \geq 1$ 時，命題成立，則 $n=k+1$ 時，令 $M=\{x \mid x$ 為 $S$中之極大元素\}, 則 $M$ 為一反鏈且 $M \neq \varnothing$ 。此時再考慮偏序集（ $S-M, \leq$ ），則$(S-M, \leq)$ 中最長鏈的長度只 $k$ ，再由歸納法假設知 $(S-M, \leq)$ 可分割成 $k$ 個互斥的反鏈，再加上 $M$ ，則找到了 $S$ 的 $k+1$ 個互斥的反鏈。
\item[（ii）] 若 $S$ 中每個反鏈長均 $<m+1$ ，且 $S$ 中最長鏈的長為 $k, k \leq n$ ，則由（i）知 $S$ 可分割成 $k$ 個互斥的反鏈，所以 $|S| \leq k m \leq m n$ ，得一矛盾。
\end{itemize}
\end{itemize}