第10章 樹 219

Note
\begin{itemize}
\item[（1）] 由上列定理知：若｛connect，acyclic，$|E|=|V|-1\}$ 三件中有任兩件成立，則均可得為樹。
\item[（2）] 推廣到 Forest：$G=(V, E)$ 為含 $k$ 個樹的樹林（forest），則 $|E(G)|=|V(G)|-k$ 。【90、105中山電機】【88、92 暨南資工】【97 政大資科】【中正通訊】【104 台聯電機】【證明】
設 $G$ 之分量圖為：$T_1=\left(V_1, E_1\right), \ldots, T_k=\left(V_k, E_k\right)$ ，
因為每個 $T_i$ 為 tree，所以 $\left|E_i\right|=\left|V_i\right|-1, \forall i=1 \sim k$ ，
$$
\therefore \sum_{i=1}^k\left|E_i\right|=\sum_{i=1}^k\left(\left|V_i\right|-1\right), \therefore|E(G)|=|V(G)|-k
$$
\end{itemize}