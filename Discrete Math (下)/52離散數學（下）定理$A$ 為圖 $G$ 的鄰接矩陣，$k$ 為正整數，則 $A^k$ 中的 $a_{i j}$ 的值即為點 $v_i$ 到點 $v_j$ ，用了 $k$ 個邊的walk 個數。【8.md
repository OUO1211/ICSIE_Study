52
離散數學（下）

定理
$A$ 為圖 $G$ 的鄰接矩陣，$k$ 為正整數，則 $A^k$ 中的 $a_{i j}$ 的值即為點 $v_i$ 到點 $v_j$ ，用了 $k$ 個邊的walk 個數。

【84、87 中山資工類題】【87 中山電機】【107 成大工科】
【證明】
對 $k$ 做歸納法，$k=1$ 時，明顯成立。設 $k=s \geq 1$ 時，定理成立，
則 $k=s+1$ 時，令 $A^{s+1}=\left[a_{i j}\right]_{n \times n}, A^s=\left[b_{i j}\right]_{n \times n}, A=\left[c_{i j}\right]_{n \times n}, n=|V(G)|$ ，
$\therefore a_{i j}=\sum_{t=1}^n b_{i t} c_{t j}$ ，其中，$b_{i t}$ 為從 $v_i$ 走 $s$ 步到 $v_t$ 的方法數，$c_{t j}$ 為從 $v_t$ 走 1 步到 $v_j$ 的方法數，故 $b_{i t} c_{t j}$ 為從 $v_i$ 走 $s$ 步到 $v_t$ 再一步到 $v_j$ 的方法數，
故知 $a_{i j}=\sum_{t=1}^n b_{i t} c_{t j}$ 為從 $v_i$ 走 $(s+1)$ 步到 $v_j$ 的總方法數，所以由歸納法知此定理成立。

例題（2）
$(10 \%)$ Let $G$ be the graph with vertices $v_1, v_2$ and $v_3$ and with $A$ as its adjacency matrix． Compute the matrix $A^2$ and $A^3$ and find the number of walks of length 2 from $v_1$ to $v_3$ and the number of walks of length 3 from $v_1$ to $v_3 . A=\left[\begin{array}{lll}1 & 1 & 2 \\ 1 & 0 & 1 \\ 2 & 1 & 0\end{array}\right]$ ．

【101 成大電通】

解 $A^2=\left[\begin{array}{lll}1 & 1 & 2 \\ 1 & 0 & 1 \\ 2 & 1 & 0\end{array}\right]\left[\begin{array}{lll}1 & 1 & 2 \\ 1 & 0 & 1 \\ 2 & 1 & 0\end{array}\right]=\left[\begin{array}{lll}6 & 3 & 3 \\ 3 & 2 & 2 \\ 3 & 2 & 5\end{array}\right]$ ，故 $v_1$ 到 $v_3$ 長度 2 的 walks 有 3 種。$A^3=\left[\begin{array}{lll}6 & 3 & 3 \\ 3 & 2 & 2 \\ 3 & 2 & 5\end{array}\right]\left[\begin{array}{lll}1 & 1 & 2 \\ 1 & 0 & 1 \\ 2 & 1 & 0\end{array}\right]=\left[\begin{array}{ccc}15 & 9 & 15 \\ 9 & 5 & 8 \\ 15 & 8 & 8\end{array}\right]$ ，故 $v_1$ 到 $v_3$ 長度 3 的 walks 有 15 種。