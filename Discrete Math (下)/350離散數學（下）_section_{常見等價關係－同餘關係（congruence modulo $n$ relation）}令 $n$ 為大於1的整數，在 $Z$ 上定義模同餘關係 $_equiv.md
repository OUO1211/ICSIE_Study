350
離散數學（下）

\section*{常見等價關係－同餘關係（congruence modulo $n$ relation）}

令 $n$ 為大於1的整數，在 $Z$ 上定義模同餘關係 $\equiv_n$ 為，$a \equiv_n b \Leftrightarrow n \mid a-b$ ，則 $\equiv_n$ 為 Z 上的一等價關係。

【很重要】
【證明】
$\forall a, b, c \in Z$,
\begin{itemize}
\item[（1）] $\because n \mid a-a, \therefore a \equiv_n a, \therefore \equiv_n$ 具有反身性。
\item[（2）] 設 $a \equiv_n b$ ，即 $n \mid a-b$ ，所以 $n \mid b-a, \therefore b \equiv_n a, \therefore$ 有對稱性。
\item[（3）] 設 $a \equiv_n b$ 且 $b \equiv_n c$ ，則 $n \mid a-b$ 且 $n|b-c, \therefore n|(a-b)+(b-c)$ ，即 $n \mid a-c$ ，$\therefore a \equiv_n c$ ，所以有遞移性。
\end{itemize}

Note
（1）商集合為 $Z / \equiv_n=\{[0],[1], \cdots,[n-1]\}$ ，其中 $[r]=\{r+t n \mid t \in Z\}, r=0,1, \ldots, n-1$ 。
（2）$\left(\equiv_m \cap \equiv_n\right)=\equiv_k \Leftrightarrow k=\operatorname{lcm}(m, n)$ ．
【92 交大資科】
解即 $k$ 為 $m, n$ 之最小公倍數。
$\left(\equiv_m \cap \equiv_n\right) \subseteq \equiv_k:$
任取 $(a, b) \in\left(\equiv_m \cap \equiv_n\right)$ ，所以 $(a, b) \in \equiv_m$ 且 $(a, b) \in \equiv_n$ ，
即 $m \mid a-b$ ，且 $n \mid a-b$ ，得 $(a-b)$ 為 $m, n$ 之公倍數，
而 $k$ 為 $m, n$ 之最小公倍數，$\therefore k \mid a-b, \therefore(a, b) \in \equiv_k, \therefore\left(\equiv_m \cap \equiv_n\right) \subseteq \equiv_k$ 。
$\equiv_k \subseteq\left(\equiv_m \bigcap \equiv_n\right):$
任取 $(a, b) \in \equiv_k$ ，即 $k \mid a-b$ ，
而因為 $k$ 為 $m, n$ 之最小公倍數，$\therefore m \mid a-b$ ，且 $n \mid a-b$ ，
$\therefore(a, b) \in \equiv_m$ 且 $(a, b) \in \equiv_n, \therefore(a, b) \in\left(\equiv_m \bigcap \equiv_n\right), \therefore \equiv_k \subseteq\left(\equiv_m \bigcap \equiv_n\right)$ 。