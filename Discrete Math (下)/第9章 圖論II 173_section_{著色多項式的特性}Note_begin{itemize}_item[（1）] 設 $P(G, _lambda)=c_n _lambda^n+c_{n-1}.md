第9章 圖論II 173

\section*{著色多項式的特性}

Note
\begin{itemize}
\item[（1）] 設 $P(G, \lambda)=c_n \lambda^n+c_{n-1} \lambda^{n-1}+\ldots+c_1 \lambda+c_0, c_i$ ：常數，則
（1）次數 $n=|V(G)|$ ；
（2）領導係數 $c_n=1$ ；
（3）第二項係數 $c_{n-1}=-|E(G)|$ ；
（4）常數項 $c_0=0$ ；
（5）係數正負號交錯；
（6）$|E(G)|>0$ 時，係數和 $\sum_{i=0}^n c_i=0$ ．
（7）$\chi(G)=\min \{\lambda \mid P(G, \lambda)>0\}$ ．
\item[（2）] $P\left(K_n, \lambda\right)=\lambda(\lambda-1)(\lambda-2) \ldots(\lambda-n+1)$ ，有時記做 $\lambda^{(n)}$ 。
\item[（3）] $P\left(C_n, \lambda\right)=(\lambda-1)^n+(-1)^n(\lambda-1), n \geq 3$ 。後面有例題可證得此結果。
\item[（4）] $P\left(T_n, \lambda\right)=\lambda(\lambda-1)^{n-1}$ ．
\end{itemize}

【92 交大資科】
\begin{itemize}
\item[（5）] 著色多項式分解定理：令 $G(V, E)$ 為一簡單連通圖，$e=(a, b) \in E$ ，令 $G_e$ 表 $G$ 中去掉 $e$後的子圖；令 $G_e^{\prime}$ 表 $G_e$ 中將 $a, b$ 黏成一點後的圖，則 $P(G, \lambda)=P\left(G_e, \lambda\right)-P\left(G_e^{\prime}, \lambda\right)$ 。
\end{itemize}

【證明】
在對 $G_e$ 著色時，對在 $G_e$ 中沒有相連的 $a, b$ 兩點，可以著同色或著異色，
若著同色，則所影響的只是 $a, b$ 的鄰點不能再著此色，故可將此兩點視成一點，即 $G_c^{\prime}$ ；若著異色，則其多項式就相當於考慮把 $a, b$ 連起來的圖的多項式，即 $G$ ，
故得 $P\left(G_e, \lambda\right)=P\left(G_e^{\prime}, \lambda\right)+P(G, \lambda)$ 。
\begin{itemize}
\item[（6）] 設 $G_1=\left(V_1, E_1\right), G_2=\left(V_2, E_2\right)$ 為無向圖 $G=(V, E)$ 的子圖，
若 $G=G_1 \bigcup G_2=\left(V_1 \bigcup V_2, E_1 \bigcup E_2\right)$ ，且 $G_1 \cap G_2=K_n$ ，則 $P(G, \lambda)=\frac{P\left(G_1, \lambda\right) P\left(G_2, \lambda\right)}{\lambda^{(n)}}$ 。
\end{itemize}

【證明】
【110 中興資科】
單獨對 $G_1$ 列著色多項式時，先對 $K_n$ 的部分討論，則為 $\lambda(\lambda-1)(\lambda-2) \cdots(\lambda-n+1)$ ，
令剩下部分的多項式為 $f(n)$ ；
單獨對 $G_2$ 列著色多項式時，也先討論 $K_n$ 的部分，則為 $\lambda(\lambda-1)(\lambda-2) \cdots(\lambda-n+1)$ ，
令剩下部分的多項式為 $g(n)$ ；
$\therefore P\left(G_1, \lambda\right) P\left(G_2, \lambda\right)=\lambda(\lambda-1)(\lambda-2) \cdots(\lambda-n+1) f(n) \times \lambda(\lambda-1)(\lambda-2) \cdots(\lambda-n+1) g(n)$ ，
對 $G$ 列著色多項式時，也先對 $K_n$ 的部分討論，然後延伸到 $G_1-K_n$ ，再延伸到 $G_2-K_n$ ，則因為 $G_1$ 與 $G_2$ 僅交集在 $K_n$ ，故 $G_1-K_n$ 與 $G_2-K_n$ 互不影響而各為 $f(n) 、 g(n)$ ，所以得$G$ 的著色多項式
$P(G, \lambda)=\lambda(\lambda-1)(\lambda-2) \cdots(\lambda-n+1) \times f(n) \times g(n)=\frac{P\left(G_1, \lambda\right) P\left(G_2, \lambda\right)}{\lambda(\lambda-1)(\lambda-2) \cdots(\lambda-n+1)} 。$