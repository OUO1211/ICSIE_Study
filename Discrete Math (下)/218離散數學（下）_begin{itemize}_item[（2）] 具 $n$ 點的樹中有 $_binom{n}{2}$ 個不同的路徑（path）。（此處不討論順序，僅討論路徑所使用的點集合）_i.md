218
離散數學（下）
\begin{itemize}
\item[（2）] 具 $n$ 點的樹中有 $\binom{n}{2}$ 個不同的路徑（path）。（此處不討論順序，僅討論路徑所使用的點集合）
\item[（3）] $T$ 為非退化樹 ⇔ $T$ 為連通圖且每一邊均為切邊（cut edge、bridge）。
\item[（4）] $T$ 為非退化樹 ⇔ $T$ 不含環路且將 $T$ 中不相連的兩點間加上一邊後必含有唯一 cycle。
\item[（5）] 樹是一種雙分圖；樹是一種平面圖。
\end{itemize}

【 91、100 成大工科】

重要定理
設 $G=(V, E)$ 為一無迴圈的無向圖，則下列敘述互為等價：
\begin{itemize}
\item[（1）] $G$ 為樹。
\item[（2）] $G$ 中不含環路且 $|E|=|V|-1$ ．
\end{itemize}

【重要】
\begin{itemize}
\item[（3）] $G$ 為連通圖且 $|E|=|V|-1$ 。
\end{itemize}

【證明】
（1）⇒（2）
因為 $G$ 為樹，所以連通且不含 cycle，故只需證明：$|E|=|V|-1$ ，
對 $|E|$ 作歸納法：
$|E|=0$ 時即為一退化樹，$|V|=1$ ，等式成立。設對所有 $|E| \leq k$ 的圖，等式均成立。
則對邊數為 $k+1$ 的圖 $G$ ，去掉 $G$ 上的任一邊得兩樹，$T_1 、 T_2$ ，
則由歸納假設知：$\left|E\left(T_1\right)\right|=\left|V\left(T_1\right)\right|-1$ ，$\left|E\left(T_2\right)\right|=\left|V\left(T_2\right)\right|-1$ ，
得 $|E(G)|=\left|E\left(T_1\right)\right|+\left|E\left(T_2\right)\right|+1=\left(\left|V\left(T_1\right)\right|-1\right)+\left(\left|V\left(T_2\right)\right|-1\right)+1=|V(G)|-1$ ，
故由歸納法知，對所有的樹，$|E|=|V|-1$ 均成立。
（2）⇒（3）
設 $G$ 為不連通圖，具有分量圖 ：$G_1, G_2, \ldots, G_k, k>1$ ，
則每個 $G_i$ 均為連通，又因 $G$ 不具有 cycle，故每個 $G_i$ 為樹，
$\therefore\left|E\left(G_i\right)\right|=\left|V\left(G_i\right)\right|-1, \quad \therefore \sum_{i=1}^k\left|E\left(G_i\right)\right|=\sum_{i=1}^k\left(\left|V\left(G_i\right)\right|-1\right)$ ，
$\therefore|E(G)|=|V(G)|-k$ ，與已知 $|E(G)|=|V(G)|-1$ 矛盾，故知 $G$ 必為連通圖。
（3）⇒（1）
設 $G$ 中含有 cycle，令 $G^{\prime}$ 為自 $G$ 一直刪去邊直到不含 cycle 且仍維持連通的子圖，
設刪去了 $k$ 個邊，$k \geq 1$ ，即 $\left|E\left(G^{\prime}\right)\right|=|E(G)|-k,\left|V\left(G^{\prime}\right)\right|=|V(G)|$ ，
而因為 $G^{\prime}$ 連通且不含 cycle，故知 $G^{\prime}$ 為樹，$\therefore\left|E\left(G^{\prime}\right)\right|=\left|V\left(G^{\prime}\right)\right|-1$ ，
所以得 $|E(G)|-k=|V(G)|-1$ ，與已知 $|E(G)|=|V(G)|-1$ 矛盾，故知 $G$ 中不含有 cycle。