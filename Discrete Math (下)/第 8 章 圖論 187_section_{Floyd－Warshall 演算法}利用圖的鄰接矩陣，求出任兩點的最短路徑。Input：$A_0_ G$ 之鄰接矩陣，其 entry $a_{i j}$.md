第 8 章 圖論 187

\section*{Floyd－Warshall 演算法}

利用圖的鄰接矩陣，求出任兩點的最短路徑。
Input：$A_0: G$ 之鄰接矩陣，其 entry $a_{i j}$ 表點 $v_i$ 到點 $v_j$ 的邊上的 weight，若無邊，記為 $\infty$ 。 Output：distance matrix of $G$ ．
Step 1 ：$k \leftarrow 1$ ．
Step 2 ：for every $1 \leq i, j \leq n, A_k[i, j] \leftarrow \min \left\{A_{k-1}[i, j], A_{k-1}[i, k]+A_{k-1}[k, j]\right\}$ ．
Step 3 ：if $k=n$ stop
$$
\text { else } k \leftarrow k+1 \text { go to step2. }
$$
【102、105清大資工】
Note
\begin{itemize}
\item[（1）] 若 $A_0$ 中之 entry 均改以 1， 0 表示有邊相連與否，且 Step 2 改成
$$
A_k[i, j] \leftarrow\left[A_{k-1}[i, j] \vee\left(A_{k-1}[i, k] \wedge A_{k-1}[k, j]\right)\right],
$$
則可得 $G$ 之可達性矩陣（reachable matrix），表達 $G$ 中任兩點間是否存在路徑。
\item[（2）] 考題少見，但之後求關係的遞移閉包比較常用到。
\item[（3）] Dijkstra＇s 與 Floyd－Warshall algorithm 之比較 ：
【91 清大通訊】
Dijkstra＇s algorithm ：求一個點到各點的最短路徑；邊上的權值為負時，則可能失效。
Floyd－Warshall algorithm ：可求任兩點的最短路徑的值；允許邊值有負值。
\end{itemize}