第六章 圖形 239
Graph

但 G4 不是 Connected
\begin{itemize}
\item[8．] Connected Components
定義：圖形中相連通的子圖。
例：G4 有兩個 Connected Components，H1 和 H2。
\item[9．] Strongly Connected（有向圖）
定義：在有向圖中，如果每個相異的成對頂點，$\left(\mathrm{V}_{\mathrm{i}}, \mathrm{V}_{\mathrm{j}}\right)$ 都有條路徑從 $\mathrm{V}_{\mathrm{i}}$ 到$V_j$ ，同時也有路徑從 $V_j$ 到 $V_i$ ，則稱之。
\item[10．] Strongly Connected Component
\item[11．] In－Degree 與 Out－Degree
定義：頂點 V 的入支度（In－Degree）是指向 V 的邊數目。Out－Degree 則是從 V出去的邊的數目。
例：參看上圖。
$$
\begin{array}{ll}
\mathrm{V}_2 \text { 的 } & \text { In-Degree 為 } 1 \\
& \text { Out-Degree 為 } 2
\end{array}
$$
\item[12．] In undirected Graph ，頂點 i 的分支度為 di ，若該圖有 n 個頂點及 e 個邊則：
$$
\mathrm{e}=\frac{1}{2} \sum_{\mathrm{i}=1}^{\mathrm{n}} \mathrm{~d}_{\mathrm{i}}
$$
\end{itemize}