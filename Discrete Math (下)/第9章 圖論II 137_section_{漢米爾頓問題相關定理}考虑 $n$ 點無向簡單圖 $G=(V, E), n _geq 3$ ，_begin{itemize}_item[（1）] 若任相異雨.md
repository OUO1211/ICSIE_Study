第9章 圖論II 137

\section*{漢米爾頓問題相關定理}

考虑 $n$ 點無向簡單圖 $G=(V, E), n \geq 3$ ，
\begin{itemize}
\item[（1）] 若任相異雨點均滿足度數和 $\geq n-1$ ，則 $G$ 有 Hamilton path。
\end{itemize}

【84中正資工】
\begin{itemize}
\item[（2）] 若每點度數均 $\geq(n-1) / 2$ ，則 $G$ 必有 Hamilton path。
\item[（3）] 若任不相鄰雨點均滿足度數和 $\geq n$ ，則 $G$ 有 Hamilton cycle。（此為 Ore 定理）
【99台大資工】
\item[（4）] 若每點度數均 $\geq n / 2$ ，則 $G$ 有 Hamilton cycle。
\end{itemize}

【84中山資工】【103交大應數】
\begin{itemize}
\item[（5）] 若 $|E| \geq\binom{ n-1}{2}+2$ ，則 $G$ 有 Hamilton cycle。
\end{itemize}

【95彰師資工】

【證明】
\begin{itemize}
\item[（1）] 先證此時 $G$ 必為［連通圖］：
若 $G$ 不連通，則存在兩點 $x, y$ 分屬不同分量 $G_1, G_2$ ，
則 $\operatorname{deg} x+\operatorname{deg} y \leq\left(\left|V\left(G_1\right)\right|-1\right)+\left(\left|V\left(G_2\right)\right|-1\right) \leq n-2<n-1$ ，矛盾。
再令 $G$ 中之最長路徑為 $P: v_1-v_2-\ldots v_s$ 。
若 $s=n$ ，即此 $P$ 經過 $G$ 的所有點，$P$ 為一Hamilton path。
若 $s \leq n-1$ ，則 $P$ 上的點經過重新排列後可走成一環路（cycle）．．．．．．（＊證明在下方）
則因為 $G$ 為連通圖，所以那些其他還末被 $P$ 走到的點（例如 $x$ ），亦有路徑能連到 $P$ 上的某些點（例如 $y$ ），則從 $x$ 出發先走到 $y$ ，再由 $y$ 走 $P$ 上的 cycle，於是形成一比 $P$ 更長的路徑，與當初假設 $P$ 是 $G$ 中最長的路徑相矛盾。
證＊：
\begin{itemize}
\item[（1）] 若 $\left(v_1, v_s\right) \in E(G)$ ，則性質成立。
\item[（2）] 若存在 $P$ 上某 $v_i$ 使 $\left(v_1, v_i\right) \in E(G)$ 且 $\left(v_{i-1}, v_s\right) \in E(G), i=3 \sim s-1$ ，
則 $v_1-v_2-\ldots-v_{i-1}-v_s-v_{s-1}-v_{s-2}-\ldots-v_i-v_1$ 也形成 cycle，性質成立。
\item[（3）] 否則，因為 $P$ 是最長路徑，故 $v_s$ 的鄰點最多只能是 $v_1 \sim v_{s-1}$ ，但已經排除①所以剩下最多是 $v_2 \sim v_{s-1}$ ；但又要排除②，所以 $v_1$ 在 P 上的鄰點的前面一個位置也都不能是 $v_s$的鄰點，故 $v_s$ 的鄰點又少了 $\operatorname{deg} v_1-1$（因為是算這些鄰點的前一處，所以 $v_1$ 本來就連到的 $v_2$ 也不能算在內），得 $\operatorname{deg} v_s \leq(s-2)-\left(\operatorname{deg} v_1-1\right)$ ，
即 $\operatorname{deg} v_1+\operatorname{deg} v_s \leq s-1 \leq n-2<n-1, \ldots \ldots$ 矛盾。
\end{itemize}
\end{itemize}
故由上述討論知，$P$ 上的點經過重新排列後可走成一環路（cycle）。