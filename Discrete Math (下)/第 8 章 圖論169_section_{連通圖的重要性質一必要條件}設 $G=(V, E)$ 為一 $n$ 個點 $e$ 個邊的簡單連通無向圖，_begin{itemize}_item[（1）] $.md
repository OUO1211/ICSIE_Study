第 8 章 圖論1
69

\section*{連通圖的重要性質一必要條件}

設 $G=(V, E)$ 為一 $n$ 個點 $e$ 個邊的簡單連通無向圖，
\begin{itemize}
\item[（1）] $n \geq 2$ 時，$G$ 有一點度數為1，或 $G$ 含一環路（cycle）。
【90中央資工】
\item[（2）] $e \geq n-1 。$
【91北科資工】
92中正資エ】
【99雲科資工】
\end{itemize}

解（1）若 $G$ 有度數為 1 的點，則證明完畢。
否則，令 $P: v_1-v_2-v_3-\ldots-v_s$ 為 $G$ 之最長路徑，$s \leq n$ ，
則因為 $\operatorname{deg} v_1 \geq 2$ ，所以 $v_1$ 還有 $v_2$ 之外的鄰點 $x$ ，
\begin{itemize}
\begin{itemize}
\item[（1）] 若 $x$ 不在 $P$ 上，則 $x-v_1-v_2-v_3 \ldots-v_s$ 為比 $P$ 長的路徑，矛盾。
\item[（2）] 故 $x$ 在 $P$ 上，令 $x=v_i, 3 \leq i \leq s$ ，即存在一 cycle，$v_1-v_2 \ldots-v_i-v_1$ 。
\end{itemize}
\item[（2）] Note：此時 $G$ 只需連通即有此特性，且可由第十章：當 $G$ 為樹時，邊數最少（即$n-1$ 邊）而得知。
也可如下用強數學歸納法證明，
$n=1$ ，則只有 1 個點， 0 個邊，原式成立。
設對所有 $\leq k$ 個點的連通圖，原式均成立，
則考虑 $k+1$ 個點的連通圖 $G$ ，去掉此圖中的任一點 $x$ ，得圖 $G^{\prime}$ ，
設 $G^{\prime}=G_1 \cup G_2 \cup \ldots \cup G_t, G_i$ 為 $G^{\prime}$ 的分量圖，且 $t \leq \operatorname{deg} x$ ，
則每個 $G_i$ 當然是連通且點數 $\leq k$ ，故由歸納法假設得知，
$\left|E_i\right| \geq\left|V_i\right|-1, \forall i=1 \sim t$ ，其中，$\left|E_i\right| 、\left|V_i\right|$ ，分別為 $G_i$ 之邊數與點數，
$$
\therefore \sum_i\left|E_i\right| \geq \sum_i\left|V_i\right|-t \text {, }
$$
而 $|E|=\left(\sum_{i=1}^t\left|E_i\right|\right)+\operatorname{deg} x,|V|=\left(\sum_{i=1}^t\left|V_i\right|\right)+1$ ，且 $t \leq \operatorname{deg} x$ ，
$$
\therefore|E|-\operatorname{deg} x \geq|V|-1-t,
$$
$\therefore|E| \geq|V|-1+(\operatorname{deg} x-t) \geq|V|-1$ ，故由歸納法知原式成立。
\end{itemize}

Note
\begin{itemize}
\item[（1）] 若 $G$ 為 $m$ 邊，$n$ 點 $k$ 個分量的無向圖，則 $m \geq n-k$ 。
【證明】
設 $G$ 之分量圖為：$G_1=\left(V_1, E_1\right), \ldots, G_k=\left(V_k, E_k\right)$ ，則因為每個 $G_i$ 為連通，所以 $\left|E_i\right| \geq\left|V_i\right|-1$ ，
$$
\forall i=1 \sim k, \therefore \sum_{i=1}^k\left|E_i\right| \geq \sum_{i=1}^k\left(\left|V_i\right|-1\right), \therefore m \geq n-k .
$$
\end{itemize}