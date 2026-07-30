122
離散數學（下）

\section*{相關定理}

考虑無孤立點的無向圖 $G$ ，
\begin{itemize}
\item[（1）] 有尤拉迴路 ⇔ 每點度数為偶數且 $G$ 為連通。
\end{itemize}

【重要】
\begin{itemize}
\item[（2）] 有尤拉路線 ⇔ 恰只兩個奇度数的點且 $G$ 為連通。
\end{itemize}

【91 清大資應】【104 中興資科】考虑無孤立點的有向圖 $G$ ，
（3）$G$ 有有向尤拉迴路 ⇔ 每點的入度數與出度数相同且 $G$ 為弱連通。
【94 東華資工】【106 成大工科】
解（1）（⇒）假設 $G$ 有 Euler circuit $C$ ，則 $C$ 每次經過 $G$ 中的點 $v$ ，一進一出，必使用了兩個 $v$ 的不同邊。故得，$\forall v \in V, \operatorname{deg} v$ 為偶數。
（⇐）對 $|E(G)|$ 做歸納法：當 $|E(G)|=1$ 時，$G$ 為單點且有一loop，故有 Euler circuit。設所有邊數 $\leq k$ 的連通且所有點均偶度數的圖，均有 Euler circuit。
則對邊數 $k+1$ 的連通圖 $G$ ，因為 $G$ 沒有度數 1 的點，故存在一 cycle，設為 $C$ ，令圖 $G^{\prime}$ 為去掉 $C$ 上的邊所得之 $G$ 的子圖，且分量圖為 $G_1^{\prime}, G_2^{\prime}, \ldots, G_t^{\prime}, t \geq 1$ ，則每個 $G_i^{\prime}$ 均為連通，且邊數 $\leq k$ ，又因為對每個 $C$ 上的點 $v$ 只被減少 $v$ 的兩個邊，故$\forall v \in G_i^{\prime}, 1 \leq i \leq t, \operatorname{deg} v$ 為偶。由歸納假設知，每個 $G_i^{\prime}$ 若不是孤立點就是均有 Eulercircuit $C_i^{\prime}, ~ 1 \leq i \leq t$ 。最後，從 $C$ 出發，若遇到某點 $v$ 上有 $G_i^{\prime}$ 的 $C_i^{\prime}$ ，則走完 $C_i^{\prime}$ 後再走 $C$ 上的邊，如此可得 $G$ 上的一Euler circuit。故由歸納法知此定理成立。
\begin{itemize}
\item[（2）] （⇒）假設 $G$ 有 Euler trail $T$ ，則除了起點與終點外，$T$ 每次經過 $G$ 中的點 $v$ ，一進一出，必使用了兩個 $v$ 的邊。故得，除了起點與終點外，$\forall v \in V$ ， $\operatorname{deg} v$ 為偶數。（⇐）設 $G$ 中奇度數的點為 $x 、 y$ ，則把 $G$ 加上邊 $(x, y)$ 成為圖 $G^{\prime}$ ，則 $G^{\prime}$ 為連通且所有點均為偶度數，故由（1）知 $G^{\prime}$ 必有 Euler circuit，接著把此 Euler circuit 去掉邊$(x, y)$ 即成為圖 $G$ 的 Euler trail。（也因此得 ：$G$ 的 Euler trail 起終點必在奇度數的點）
\item[（3）] （⇒）設 $G$ 有 Euler circuit $C$ ，則 $C$ 每次經過 $G$ 中的點 $v$ ，一進一出，必使用了兩個$v$ 的邊。故得每點都是入度數＝出度數，又因為 $C$ 經過 $G$ 的所有點，所以 $G$ 為弱連通圖。
（⇐）因為 $G$ 為連通且 $\forall v \in V, i d(v)=o d(v)$ ，從任—點出發必可走出一個 directedcircuit $C$ ，再同（1）考慮去掉此 $C$ 後所得的子圖，以逐步探訪的方式可得 $G$ 的 directedEuler circuit •
\end{itemize}