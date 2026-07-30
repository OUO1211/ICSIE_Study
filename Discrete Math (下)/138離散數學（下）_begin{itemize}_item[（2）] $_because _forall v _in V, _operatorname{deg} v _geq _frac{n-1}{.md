138
離散數學（下）
\begin{itemize}
\item[（2）] $\because \forall v \in V, \operatorname{deg} v \geq \frac{n-1}{2} \therefore \forall x, y \in V, \operatorname{deg} x+\operatorname{deg} y \geq(n-1)$ ，則由（1）知 $G$ 有 Hamiltonpath ∘
\item[（3）] 設存在有滿足前提，但卻沒有 Hamilton cycle 的圖，找出所有這種圖中邊數最多的那個，設為 $G$ ，則
\begin{itemize}
\item[（1）] $G$ 不會是 $K_n \ldots \ldots$（ $\because K_n$ 有 Hamilton cycle）。
\item[（2）] 由（i）知 $\exists a, b \in V(G),(a, b) \notin E(G)$ ，且因為 $G$ 是最多邊的反例，所以有一 $a$ 到 $b$ 的 Hamilton path，令為 $P: a=v_1-v_2 \ldots-v_n$ 。
\item[（3）] 此時若有 $\left(v_1, v_i\right) \in E(G)$ ，and $\left(v_{i-1}, v_n\right) \in E(G)$ ，for some $i=3 \sim n-1$ ，則 $v_1-v_2-\ldots-v_{i-1}-v_n-v_{n-1}-v_{n-2}-\ldots-v_i-v_1$ 為一Hamilton cycle。不然就會有 $\operatorname{deg} v_n \leq(n-2)-\left(\operatorname{deg} v_1-1\right)$ ，而得 $\operatorname{deg} v_1+\operatorname{deg} v_n \leq n-1<n, \ldots .$. 矛盾。
\end{itemize}
\item[（4）] $\because \forall v \in V, \operatorname{deg} v \geq \frac{n}{2}, \therefore \forall x, y \in V, \operatorname{deg} x+\operatorname{deg} y \geq n$ ，則由（3）知 $G$ 有 Hamilton cycle。
\item[（5）] 若 $G=K_n$ ，則 $G$ 當然有 Hamilton cycle。
因此，只需考慮 $G$ 中有某些點沒有邊相連的情形，接著，只需證明出 $G$ 中那些沒有邊相連的點 $x, y$ ，其度數和 $\operatorname{deg} x+\operatorname{deg} y \geq$ 總點數 $n$ ，則由定理（3）可知，$G$ 必有 Hamilton cycle。以反證法：設存在 $x, y \in V(G),(x, y) \notin E(G), \operatorname{deg} x+\operatorname{deg} y<n$ ，
則此時 $G$ 最多邊的情形是其餘的 $n-2$ 個點形成完全圖，然後 $x, y$ 再與這其中的某些點相連（頂多 $n-1$ 邊），
即 $|E(G)|<\binom{n-2}{2}+n=\frac{(n-2)(n-3)}{2}+n=\frac{n^2-3 n+2}{2}+2=\binom{n-1}{2}+2 \ldots$ 與已知不合，故 $G$存在有 Hamilton cycle。
\end{itemize}