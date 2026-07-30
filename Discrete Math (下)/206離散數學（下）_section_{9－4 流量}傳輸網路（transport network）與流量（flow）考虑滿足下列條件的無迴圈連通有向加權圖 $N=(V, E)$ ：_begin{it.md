206
離散數學（下）

\section*{9－4 流量}

傳輸網路（transport network）與流量（flow）
考虑滿足下列條件的無迴圈連通有向加權圖 $N=(V, E)$ ：
\begin{itemize}
\item[（1）] 唯一存在一起點（source）$a, \operatorname{indeg}(a)=0$ ，
\item[（2）] 唯一存在一终點（sink）$z, \operatorname{outdeg}(z)=0$ ，
\item[（3）] 每個邊上㒃予權值（weight）稱為其容量（capacity）：$c(e)$ ，
\end{itemize}

則稱 $N$ 為一傳輸網路。
若函数 $f: E \rightarrow Z^{+}$滿足下列條件：
\begin{itemize}
\item[（1）] $f(e) \leq c(e), \quad \forall e \in E$ ，（2）$\forall v \in V, \quad v \neq\{a, z\}, \sum_{u \in V} f(u, v)=\sum_{u \in V} f(v, w)$ ，
\end{itemize}

則稱 $f$ 為 $N$ 的一個流量，且流量值（value）定義為 $\operatorname{val}(f)=\sum_{v \in V} f(a, v)=\sum_{v \in V} f(v, z)$ 。
a－z 切集（a－z cut）
若 $C$ 為傳輸網路 $N=(V, E)$ 上的一個切集（cut－set），且使得 $N$ 去掉 $C$ 之後，$a$ 與 $z$ 會位於兩個不同的分量圖 $P$ 與 $\bar{P}$ 中，則稱 $C$ 為一 $\boldsymbol{a} \boldsymbol{-} \mathbf{z}$ 切集或簡稱切集，記為 $\operatorname{cut}(P, \bar{P})$ ，且 $C$ 的容量定義為 $P$ 往 $\bar{P}$ 的邊的容量和。

Note
\begin{itemize}
\item[（i）] 任一切集的容量值都大於等於任一流量值（證明在後方進階類題）。
\item[（ii）] Max－flow＆min－cut 定理（Ford＆Fulkerson）
【90中正資工】設 $N=(V, E)$ 為傳輸網路，則 $N$ 上最大流量的流量值等於 $N$ 上的最小切集的容量。
\end{itemize}

例如，右圖傳輸網路上的流量，流量值 $=4+2=6$ ；$\operatorname{Cut}(\{\mathrm{a}, \mathrm{b}, \mathrm{d}\},\{\mathrm{c}, \mathrm{e}, \mathrm{z}\})$ 的容量為 $2+2+2=6$ ；
而由定理知，此流量為最大，此切集為最小。

【91師大資工】