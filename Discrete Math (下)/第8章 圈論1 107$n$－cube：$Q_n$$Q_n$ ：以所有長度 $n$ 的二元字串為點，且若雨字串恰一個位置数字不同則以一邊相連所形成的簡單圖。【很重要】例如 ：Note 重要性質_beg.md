第8章 圈論1 107

$n$－cube：$Q_n$
$Q_n$ ：以所有長度 $n$ 的二元字串為點，且若雨字串恰一個位置数字不同則以一邊相連所形成的簡單圖。

【很重要】
例如 ：

Note 重要性質
\begin{itemize}
\item[（1）] $Q_n$ is bipartite．
【90、106中山資工】【93、96成大工科】【111台科資工】解 定義集合 $A=\left\{x \in V\left(Q_n\right) \mid x\right.$ 的編號中含有奇數個 0$\}$ ，$B=\left\{x \in V\left(Q_n\right) \mid x\right.$ 的編號中含有偶數個 0$\}$ ，則可得 $A \cup B=V\left(Q_n\right)$ ，且 $A \cap B=\varnothing$ ，又由 $Q_n$ 的定義方式知兩點相連必是因為編號恰相差一個位置，故知 $A$ 中之點必彼此不相連，$B$ 中之點亦彼此不相連，$\therefore Q_n$ 為雙分圖。
\item[（2）] $Q_n$ is $n$－regular．
【97 中興資科】【110 交大資工】【證明】
$\forall v \in Q_n, v$ 的編號為長度 $n$ 的二元字串，而其鄰點有恰1個位置與其不同，這個不同的位置有 $n$ 種可能，即每點均可連到恰 $n$ 個點，所以 $Q_n$ 為 $n$－regular。
\item[（3）] $\left|V\left(Q_n\right)\right|=2^n ;\left|E\left(Q_n\right)\right|=n \cdot 2^{n-1}$ ．
【101、104海洋資工】【證明】【94、97中正資工】【99台大電機】【102、103中央資工】【102中興資科】因為長度 $n$ 的二元字串有 $2^n$ 種，$\therefore|V|=2^n$ ，$\because \sum \operatorname{deg}(v)=2|E|$ ，且每點度數均 $=n, \therefore n \cdot 2^n=2|E|, \therefore|E|=n \cdot 2^{n-1}$ 。另外，
【103中央資工】【110 交大資工】由 $Q_n$ 的遞迴構造方式，也可得邊數的遞迴式 ：$\left|E\left(Q_n\right)\right|=2\left|E\left(Q_{n-1}\right)\right|+2^{n-1}$ 。
\end{itemize}