370
離散數學（下）

\section*{等價關係的計算－集合的分割法計算}

定義在集合 $\{1,2, \ldots, m\}$ 上的不同的等價關係的個數
= 分割集合 $\{1,2, \ldots, m\}$ 的方法數
$=m$ 個相異物入 $m$ 個相同箱可空之方法數
$=\sum_{i=1}^m S(m, i)$ 。
【96 交大資訊】

Note
\begin{itemize}
\item[（1）] $S(m, n)$ Stirling number，代表 $m$ 元集合分割成 $n$ 個非空子集的方法數。
$S(m, n)=\frac{\operatorname{Onto}(m, n)}{n!}=\frac{\sum_{i=0}^n(-1)^i\binom{n}{i}(n-i)^m}{n!} ;$
$S(m, 1)=1$ ；
$S(m, 2)=2^{m-1}-1$ ；
$S(m, n)=S(m-1, n-1)+n S(m-1, n)$ ；
$S(m, m-1)=\binom{m}{2} ;$
$S(m, m)=1$ 。
\item[（2）] 也可以遞迴方式討論：
令分割 $m$ 元集合 $A$ 的方法為 $P_m$ ，則考慮 $A$ 中任一元素 $x$ 所在子集 $A_1$ ，若 $A_1$ 中月 $k+N$元素， $0 \leq k \leq m-1$ ，則有 $\binom{m-1}{k}$ 種從 $A$ 中選取 $k$ 個元素與 $x$ 形成 $A_1$ 的方式，而剩下的 $m-k-1$ 個元素分割成非空子集的方法有 $P_{m-1-k}$ ，
故得 $P_m=\sum_{k=0}^{m-1} P_{m-1-k}\binom{m-1}{k}=\sum_{k=0}^{m-1} P_{m-1-k}\binom{m-1}{m-1-k}=\sum_{i=0}^{m-1} P_i\binom{m-1}{i}$ ，其中 $P_0=1$ 。$P_m$ 又被稱為 Bell number。
\end{itemize}