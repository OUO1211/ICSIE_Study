26
離散數學（下）

\section*{度數序列（degree sequence）}

將 $G$ 中所有點的度數，由大到小順序排列，稱為 $G$ 的度數序列。
Note
\begin{itemize}
\item[（1）] 有時沒排序；有時用由小到大的順序排列。
\item[（2）] 數列 $d_1, \ldots, d_n$ 為一多重圖（multi－graph）之度數序列 ⇔ $\sum d_i$ 為偶數。【99交大應數】【證明】
$(\Rightarrow)$ 由 $\sum_{v \in V} \operatorname{deg}(v)=2|E|$ 可知。
$(\Leftarrow) \because \sum d_i$ 為偶數，故數列 $\left\{d_i\right\}_{i=1}^n$ 中奇數的必有偶個，將這些奇數的兩兩連以一邊，剩下的偶數（設為 $2 m$ ），均以 loop（ $m$ 個）附在點上，則可得一有 loop 的圖，其度數序列為 $\left\{d_i\right\}_{i=1}^n$ 。
\item[（3）] 如果存在一 $n$ 點之簡單圖，其度數數列為 $d_1, \ldots, d_n$ ，則稱此數列為 graphical。
\item[（4）] 判斷數列 $d_1, \ldots, d_n$ 是否為 graphical 的常用必要條件：
\begin{itemize}
\item[（1）] $\sum d_i$ 為偶數。
\end{itemize}
\end{itemize}

【證明】
由 $\sum_{v \in V} \operatorname{deg}(v)=2|E|$ 可知。
\begin{itemize}
\item[（2）] $d_1, \ldots, d_n$ 必有兩數相同。（等同於任一群人中必有兩個人朋友數相同）
【98 清大資工】【100中山電機】【102 台大資工】【105 台北資工】
\end{itemize}

【證明】
因為是 $n$ 點簡單圖的度數，故度數都介於 $0 \sim n-1$ ；但數字 0 與數字 $n-1$ 不會同時出現（因為 $G$ 中若有弧立點，就不會有某點連到其它所有點），
故此 $n$ 個數字：$d_1, \ldots, d_n$ 最多只有 $n-1$ 種可能值： $1,2, \ldots, n-2, n-1$（或 0 ），由鴿籠原理知，必有某兩數 $d_i=d_j$ ，for some $i \neq j$ 。
\begin{itemize}
\item[（3）] 令 $\left\{d_i\right\}_{i=1}^n$ 為為一遞減數列，則
$\left\{d_1, d_2, \ldots, d_n\right\} \quad$ is graphical $\Leftrightarrow\left\{d_2-1, d_3-1, \cdots, d_{d_1+1}-1, d_{d_1+2}, \ldots, d_n\right\} \quad$ is graphical.
【88 清大資工】
\end{itemize}