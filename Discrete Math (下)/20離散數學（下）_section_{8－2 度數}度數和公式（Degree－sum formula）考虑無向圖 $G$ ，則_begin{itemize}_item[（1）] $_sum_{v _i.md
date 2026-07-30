20
離散數學（下）

\section*{8－2 度數}

度數和公式（Degree－sum formula）
考虑無向圖 $G$ ，則
\begin{itemize}
\item[（1）] $\sum_{v \in V} \operatorname{deg}(v)=2|E|$ ．
\item[（2）] 度數為奇數的頂點必有偶數個。
\end{itemize}

【超重要】
【重要】

考虑有向圖 $G$ ，則
\begin{itemize}
\item[（3）] $\sum_{v \in V} i d(v)=\sum_{v \in V} o d(v)=|E|$ ．
\end{itemize}

【證明】
\begin{itemize}
\item[（1）] 考慮 $G$ 中任一邊 $e=(a, b)$ ，加總度數和時，算 $\operatorname{deg}(a)$ 時 $e$ 被算了一次，算 $\operatorname{deg}(b)$ 時 $e$ 又被算了一次，故知，$G$ 中的每邊在 $\sum \operatorname{deg}(v)$ 時都被算了兩次，故得 $\sum_{v \in V} \operatorname{deg}(v)=2|E| 。$另外，也可看 $G$ 的 incidency matrix，
每個橫列的和為該點的度數，加總所有點的度數，即為矩陣之各元素總和，
但計算矩陣之各元素總和時，亦可先計算各直行的總和（均為2），
而因為有 $|E|$ 個邊，故總和為 $2|E|$ ，得證。
\item[（2）] $\because \sum_{v \in V} \operatorname{deg}(v)=\sum_{\text {偶度點 }} \operatorname{deg}(v)+\sum_{\text {奇度點 }} \operatorname{deg}(v)$ ，
而左式 $=2|E|$ 為偶數，右式第一項亦偶數，
$\therefore \sum_{\text {奇度點 }} \operatorname{deg}(v)$ 亦必為偶數，
∴奇度數的點不可能是奇個。
\item[（3）] $\forall e=(a, b) \in E(G)$ ，算outdeg（a）時 $e$ 被算了一次，算 $\operatorname{indeg}(b)$ 時 $e$ 又被算了一次，故知，$G$ 中的任一邊在等式的兩邊均貢獻 1 次，
$\therefore \sum_{v \in V} \operatorname{indeg}(v)=\sum_{v \in V} \operatorname{outdeg}(v)$ ．
\end{itemize}

Note
\begin{itemize}
\item[（1）] 定理（1）又稱為握手定理。
\end{itemize}

【101 中興資科】
\begin{itemize}
\item[（2）] 若圓 $G$ 為 $k$－regular，且 $k$ 為奇數，則 $G$ 的點數不可能是奇數。
\end{itemize}