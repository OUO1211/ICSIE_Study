第9章 圖論II 145

\section*{完全雙分圖與漢米爾頓問題}
\begin{itemize}
\item[（1）] $K_{m, n}$ 有 Hamilton cycle $\Leftrightarrow m=n$ 。
\end{itemize}
（2）$K_{m, n}$ 有 Hamilton path $\Leftrightarrow|m-n| \leq 1$ 。
（3）$K_{n, n}$ 中有 $\frac{(n-1)!n!}{2}$ 個相異的 Hamilton cycle。
\begin{itemize}
\item[（4）] $K_{m, n}$ 中有 $m!n!$ 個相異的 Hamilton path $\circ(|m-n|=0$ 或 1$)$
\end{itemize}

【81 交大】【89 台大資工】【105 中正資工】
【81 交大資工】

【證明】
設 $K_{m, n}=(A \cup B, E), A=\left\{v_1, v_2, \ldots, v_m\right\}, B=\left\{u_1, u_2, \ldots, u_n\right\}$ ，
\begin{itemize}
\item[（1）] ⇐ 若 $m=n$ ，則取 $v_1-u_1-v_2-u_2-\ldots-v_m-u_m-v_1$ 即為一Hamilton cycle。
⇒ 因為是雙分圖，故其環路上的點必是 $A, B$ 交錯，一去一回，故 $m=n$ 。
\item[（2）] $\Leftarrow m=n$ 時，取 $v_1-u_1-v_2-u_2-\ldots-v_m-u_m$ 即為一Hamilton path。
$m=n+1$ 時，$v_1-u_1-v_2-u_2-\ldots-v_n-u_n-v_{n+1}$ 即為一Hamilton path。
（ $n=m+1$ 時亦同上）
⇒ 因為是雙分圖，故其路徑的點必 $A, B$ 交錯，則此路徑之點數若為偶數，必是 $|A|=|B|$ ，
若為奇數，則起終點同為 $A$（或 $B$ ）的點，故 $|A|-|B|=1$（或 $|B|-|A|=1$ ）。
\item[（3）] 即考慮 $n$ 男 $n$ 女圍坐在圓桌使男女交錯的坐法：
不失一般性，先讓男生入座，則因環狀排列，故有 $(n-1)!$ 種坐法，此時女生再入座就沒有環狀的顧慮了，而有 $n!$ 種坐法；但對環路而言，同一種走法有順時與逆時兩種表達方式，故需再除以 2 ，所以共 $\frac{(n-1)!n!}{2}$ 種。
\item[（4）] 設 $|A|=m,|B|=n$ ，
從 $A$ 中選出第一點有 $m$ 種選法；從 $B$ 中選出第一點有 $n$ 種選法；
從 $A$ 中選出第二點有 $(m-1)$ 種選法；從 $B$ 中選出第二點有 $(n-1)$ 種選法；
從 $A$ 中選出第三點有 $(m-2)$ 種選法；從 $B$ 中選出第一點有 $(n-2)$ 種選法；
$\cdots$ ，故由乘法原理共 $m \cdot n \cdot(m-1) \cdot(n-1) \cdot(m-2) \cdot(n-2) \cdot \ldots \cdot 1 \cdot 1=m!n!$ 。
（若考慮 $a-b-c-d$ 與 $d-c-b-a$ 視為相同，則需再除以 2 。）
\end{itemize}