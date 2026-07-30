第9章 園論II 197

\section*{平面圖性質討論}

以下（1）～（3）：$G$ 為簡單平面圖；（4）：$G$ 為簡單圖。
令 $G=(V, E)$ 為一簡單平面圖，則
\begin{itemize}
\item[（1）] $G$ has a vertex of degree 5 or less．（i．e．$\delta(G) \leq 5$ ）
\end{itemize}

【重要】
\begin{itemize}
\item[（2）] If $|V|<12$ ，then $G$ has a vertex of degree 4 or less．（i．e．，$\delta(G) \leq 4$ ）
\item[（3）] If $|E|<30$ ，then $G$ has a vertex of degree 4 or less．（i．e．，$\delta(G) \leq 4)$
【82 交大資科】
【90高考専技】
\item[（4）] If $|V| \geq 11$ ，then either $G$ or $\bar{G}$ is not planar．
【90 高科電資】【91 中正資工】
【100中山資工】
101 台大電機】
【109成大資工】
\end{itemize}

【證明】
\begin{itemize}
\item[（1）] 若 $G$ 中的點度數均 $\geq 6$ ，則 $2 e=\sum \operatorname{deg}(x) \geq 6 v$ ，
但 $G$ 為簡單平面圖，$\therefore e \leq 3 v-6$ ，即 $6 v \leq 2 e \leq 2 \cdot(3 v-6)$ ，矛盾。
\item[（2）] 設 $G$ 的點數 $|V|=v<12$ ，且 $\forall x \in V(G), ~ \operatorname{deg} x \geq 5$ ，則 $2 e=\sum \operatorname{deg}(x) \geq 5 v$ ，
但 $G$ 為簡單平面圖，$\therefore e \leq 3 v-6$ ，即 $6 v \leq 2 e \leq 2 \cdot(3 v-6)$ ，
得 $5 v \leq 6 v-12$ ，即 $v \geq 12$ ，矛盾。
\item[（3）] 設 $G$ 的邊數 $|E|=e<30$ ，且 $\forall x \in V(G), ~ \operatorname{deg} x \geq 5$ ，
則 $2 e=\sum \operatorname{deg}(x) \geq 5 v$ ，即 $v \leq \frac{2}{5} e$ ，
但 $G$ 為簡單平面圖，$\therefore e \leq 3 v-6 \leq \frac{6}{5} e-6$ ，
得 $5 e \leq 6 e-30$ ，即 $e \geq 30$ ，矛盾。
\item[（4）] 設 $G$ 的點數 $|V|=v \geq 11$ ，且 $G$ 與 $\bar{G}$ 均為平面圖，設 $\bar{G}$ 有 $\bar{e}$ 邊 $\bar{v}$ 點，
則得 $e \leq 3 v-6$ ，且 $\bar{e} \leq 3 \bar{v}-6$ ，
但 $\because v=\bar{v}, e+\bar{e}=\binom{v}{2}$ ，故得 $\frac{v(v-1)}{2} \leq 6 v-12$ ，
$\therefore v^2-13 v+24 \leq 0$ ，解得 $\frac{13-\sqrt{73}}{2} \leq v \leq \frac{13+\sqrt{73}}{2} \approx 10.5$ ，
與 $v \geq 11$ 矛盾。
\end{itemize}