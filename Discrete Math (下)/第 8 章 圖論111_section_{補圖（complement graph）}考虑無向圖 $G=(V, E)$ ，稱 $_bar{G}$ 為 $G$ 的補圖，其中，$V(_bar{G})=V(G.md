第 8 章 圖論1
11

\section*{補圖（complement graph）}

考虑無向圖 $G=(V, E)$ ，稱 $\bar{G}$ 為 $G$ 的補圖，其中，
$V(\bar{G})=V(G)$ 且 $E(\bar{G})=\left\{\left(v_i, v_j\right) \mid\left(v_i, v_j\right) \notin E(G), v_i \neq v_j\right\} 。$
例如 ：

Note
\begin{itemize}
\item[（1）] 補圖不放 loop。
\item[（2）] $|V(G)|=|V(\bar{G})|$ ；當 $G$ 是簡單圖時，$|E(G)|+|E(\bar{G})|=\binom{|V|}{2}$ ； $\bar{G}$ 有時也記做 $G^c$ 。
\end{itemize}

\section*{例題（2）}
（5％）If $G$ is a simple graph with 27 edges and $\bar{G}$ has 28 edges，how many vertices does $G$ have？
【93 中興資科】【98 交大資訊類題】【108、110中正資工】
解 若 $G$ 有 $n$ 點，則 $|E(G)|+|E(\bar{G})|=\binom{n}{2}$ ，
解 $27+28=\frac{n(n-1)}{2}$ ，得 $n^2-n-110=(n-11)(n+10)=0$ ，
故 $n=11$ 。