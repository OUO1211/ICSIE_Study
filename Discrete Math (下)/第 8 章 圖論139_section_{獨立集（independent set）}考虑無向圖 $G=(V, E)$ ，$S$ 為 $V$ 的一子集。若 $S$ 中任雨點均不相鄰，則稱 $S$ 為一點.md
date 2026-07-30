第 8 章 圖論1
39

\section*{獨立集（independent set）}

考虑無向圖 $G=(V, E)$ ，$S$ 為 $V$ 的一子集。
若 $S$ 中任雨點均不相鄰，則稱 $S$ 為一點獨立集。
Note
\begin{itemize}
\item[（1）] The vertex independence number $\alpha(G): G$ 中具最多點的點獨立集的點數。
\item[（2）] 若一個獨立集 $S$ ，滿足再任加入一點後，均會成為相依集，則稱 $S$ 為極大獨立集（maximalindependent set）。
例如右圖中，$\{a, g\},\{a, c, f, h\}$ 均為 $G_1$
的點獨立集合，且 $\alpha\left(G_1\right)=4$ ，
$\{t\},\{u, y, w\}$ 均為 $G_2$ 的點
獨立集合，且 $\alpha\left(G_2\right)=3$ 。
\item[（3）] $S$ 為 $G$ 中的 clique $\Leftrightarrow S$ 為 $\bar{G}$ 中的獨立集。【證明】
$S$ 為 $G$ 之 clique
$\Leftrightarrow \forall u, v \in S,(u, v) \in E(G) \Leftrightarrow \forall u, v \in S,(u, v) \notin E(\bar{G}) \Leftrightarrow S$ 為 $\bar{G}$ 中的獨立集。
\item[（4）] 考慮邊子集 $T$ ，若 $T$ 中的邊都沒共同端點，則稱 $T$ 為 $G$ 的一個邊獨立集（又稱為配對，matching）。且邊獨立數（edge independence number）$\alpha^{\prime}(G):$ 為 $G$ 中最多邊的邊獨立集的邊數。本章最末單元另有討論雙分圖的邊獨立集問題供同學參考。
\item[（5）] 任意大於等於 6 個點簡單圖 $G, G$ 或 $\bar{G}$ 必有 $K_3$ 為子圖。【84台大資工】
【證明】
任取 $G$ 中六點：$a, b, c, d, e, f$ ，依是否在 $G$ 中與 $a$ 相鄰，定義兩集合：
$A=\{x \mid(a, x) \in E(G)\}, B=\{x \mid(a, x) \in E(\bar{G})\}$ ，則由鴿籠原理知：$|A| \geq 3$ 或 $|B| \geq 3$ ，
\begin{itemize}
\item[（1）] $|A| \geq 3$ ，不失一般性，設 $b, c, d \in A$ ，考慮 $a, b, c, d$ 四點：
若 $b, c, d$ 在 $G$ 中彼此不相鄰，則 $b, c, d$ 為 $\bar{G}$ 之一 $K_3$ 。
若 $b, c, d$ 在 $G$ 中非彼此不相連，即至少有兩點（設為 $b, c$ ）相鄰，則 $b, c, a$ 為 $G$ 之一 $K_3$ 。
\item[（2）] $|B| \geq 3$ ，不失一般性，設 $b, c, d \in B$ ，考慮 $a, b, c, d$ 四點：
若 $b, c, d$ 在 $G$ 中彼此相鄰，則 $b, c, d$ 為 $G$ 之一 $K_3$ 。
若 $b, c, d$ 在 $G$ 中非彼此相連，即至少有兩點（設為 $b, c$ ）不相鄰，則 $b, c, a$ 為 $\bar{G}$ 之一 $K_3$ 。
\end{itemize}
\item[（6）] 上述等同於任意大於等於 6 個點的簡單圖中，必存在有 3 點的 clique 或 3 點的獨立集；也等同於任六人中必有 3 人互相認識或互相不認識。
\end{itemize}