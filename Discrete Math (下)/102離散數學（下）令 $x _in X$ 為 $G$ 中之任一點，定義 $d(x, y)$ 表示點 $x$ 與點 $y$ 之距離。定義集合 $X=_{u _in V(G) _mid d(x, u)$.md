102
離散數學（下）

令 $x \in X$ 為 $G$ 中之任一點，定義 $d(x, y)$ 表示點 $x$ 與點 $y$ 之距離。
定義集合 $X=\{u \in V(G) \mid d(x, u)$ is even $\}, Y=\{u \in V(G) \mid d(x, u)$ is odd $\}$ ，
則可得 $X \cap Y=\varnothing$ ；又因為 $G$ 為連通圖，故 $X \bigcup Y=V(G)$ ，
再由（＊）知集合 $X$ 中的點彼此均沒有邊相連，（ $Y$ 中之點亦然），故得 $G$ 為雙分圖。 $\operatorname{show}\left({ }^*\right)$ 若 $\exists u, ~ v \in X, ~(u, ~ v) \in E(G)$ ，
令 $P_1$ ：從 $x$ 到 $u$ 之最短路徑，$P_2$ ：從 $x$ 到 $v$ 之最短路徑，
則 $P_1-(u, v)-P_2$ 為一從 $x$ 到 $x$ 的 closed odd walk，
而因為一 closed odd walk 中必含有一 odd cycle，故得矛盾。
\begin{itemize}
\item[（2）] $n$ 個點的簡單雙分圖其邊數 $e \leq\left\lfloor\frac{n}{2}\right\rfloor\left\lceil\frac{n}{2}\right\rceil$ 。
【93 交大資工】【台科資工】
\end{itemize}

【證明】
設 $|A|=x,|B|=n-x, 1 \leq x \leq n-1$ ，則邊數 $e \leq x(n-x)=-\left(x-\frac{n}{2}\right)^2+\left(\frac{n}{2}\right)^2$ ，
若 $n=2 k, k \in Z^{+}$，取 $x=k$ ，得邊數最大為 $k^2=\left\lfloor\frac{n}{2}\right\rfloor\left\lceil\frac{n}{2}\right\rceil$ 。
若 $n=2 k+1, k \in Z^{+}$，取 $x=k$ ，得邊數最大為 $k(k+1)=\left\lfloor\frac{n}{2}\right\rfloor\left\lceil\frac{n}{2}\right\rceil$ 。
∴ 最大值為 $\left\lfloor\frac{n}{2}\right\rfloor\left\lceil\frac{n}{2}\right\rceil$ 。
\begin{itemize}
\item[（3）] $\left|V\left(K_{m, n}\right)\right|=m+n,\left|E\left(K_{m, n}\right)\right|=m \cdot n$ 。
【 96 台大電機】【 98 政大資科】【 102 中央資工】【 109 中山資工】
\end{itemize}