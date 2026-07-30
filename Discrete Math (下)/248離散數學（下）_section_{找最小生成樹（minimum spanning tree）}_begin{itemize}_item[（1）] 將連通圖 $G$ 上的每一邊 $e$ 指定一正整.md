248
離散數學（下）

\section*{找最小生成樹（minimum spanning tree）}
\begin{itemize}
\item[（1）] 將連通圖 $G$ 上的每一邊 $e$ 指定一正整數 $w t(e)$ 稱為 $e$ 的權重（weight），此時稱 $G$ 為一加權圖（weighted graph）。
\item[（2）] 設 $G=(V, E)$ 為一連通加權圖，$T=\left(V, E^{\prime}\right)$ 為 $G$ 的一個生成樹，若 $T$ 的所有邊的權重和 $w t(T)=\sum_{e \in E^{\prime}} w t(e)$ 為 $G$ 的所有生成樹中最小，則稱 $T$ 為 $G$ 的最小生成樹。
【93 交大資工】
\end{itemize}

Note
\begin{itemize}
\item[（1）] 最小生成樹不一定唯一，但邊數都是點數－1。
\end{itemize}

【99 雲科資工】
\begin{itemize}
\item[（2）] 若 $e$ 為簡單圖 $G$ 中唯一權重最小的邊，則 $G$ 的每個最小生成樹都會包含 $e$ 這個邊。
【93 交大應數】【103 台科資工】【111 成大資工】
\end{itemize}

【證明】
設 $T$ 為 $G$ 的 spanning tree 使 weight $w(T)$ 為最小，
設 $e \notin E(T)$ ，則 $T \cup\{e\}$ 必含有一 cycle $C$ 通過 $e$ ，
設 $e=(a, b)$ ，考慮 $C$ 中連到 $a$ 的邊 $f, f \neq e$ ，
則由題意知 $w(e)<w(f)$ ，故 $T \bigcup\{e\}-\{f\}$ 仍為 $G$ 的 spanning tree，
且 $w(T \bigcup\{e\}-\{f\})=w(T)+w(e)-w(f)<w(T)$ ，而得矛盾。
\begin{itemize}
\item[（3）] 若 loop－free 之連通加權圖中每邊的 weight 均不同，則最小生成樹為唯一。
【81 中正資工】【99 台大資工】【108、 111 台聯電機】
\end{itemize}

【證明】
設 $T_1, T_2$ 均為 $G$ 之兩棵不同生成樹，且 $w t\left(T_1\right)=w t\left(T_2\right)=$ 最小，
則因為 $T_1 \neq T_2$ ，故存在 $e \in E\left(T_1\right), e \notin E\left(T_2\right)$ ，
而由換邊定理知存在 $f \in E\left(T_2\right), f \notin E\left(T_1\right)$ ，使得
$T_3=\left(T_1-\{e\}\right) \bigcup\{f\}, T_4=\left(T_2-\{f\}\right) \bigcup\{e\}$ 均為 $G$ 之生成樹。
若 $w t(f)<w t(e)$ ，則 $w t\left(T_3\right)=w t\left(T_1\right)-w t(e)+w t(f)<w t\left(T_1\right)$ ，
若 $w t(f)>w t(e)$ ，則 $w t\left(T_4\right)=w t\left(T_2\right)-w t(f)+w t(e)<w t\left(T_2\right)$ ，
而這兩個結果都與 $w t\left(T_1\right)=w t\left(T_2\right)=$ 最小矛盾。

（4）（3）之逆敘述不成立。
【91 中正資工】