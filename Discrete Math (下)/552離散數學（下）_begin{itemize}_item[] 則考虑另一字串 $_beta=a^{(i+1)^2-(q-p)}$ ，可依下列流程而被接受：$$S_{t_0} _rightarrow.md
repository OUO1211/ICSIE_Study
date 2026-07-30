552
離散數學（下）
\begin{itemize}
\item[] 則考虑另一字串 $\beta=a^{(i+1)^2-(q-p)}$ ，可依下列流程而被接受：
$$
S_{t_0} \rightarrow S_{t_1} \rightarrow \cdots \rightarrow S_{t_{i^2+1+p-1}} \rightarrow S_{t_{i^2+1+p}}\left(=S_{t_{i^2+1+q}}\right) \rightarrow S_{t_{i^2+1+q+1}} \rightarrow \cdots \rightarrow S_{t_{(i+1)^2-1}} \rightarrow S_{t_{(i+1)^2}}
$$
但很明顯 $\beta \notin L$ ，得一矛盾。
\item[（3）] 設有一有限狀態機 $M$ 能認知 $L$ ，且設 $M$ 有 $N$ 個狀態，
考慮字串 $\alpha=1^N 0^N$ ，則由 $L$ 的定義知 $\alpha \in L$ ，
設此字串從輸入到被接受的狀態變化為：$S_{t_0} \xrightarrow{1} S_{t_1} \xrightarrow{1} \cdots \xrightarrow{0} S_{t_{2 N}}$ ，
考慮 $S_{t_0}, S_{t_1}, \cdots, S_{t_N}$ 這 $N+1$ 個狀態，因為 $M$ 只有 $N$ 個狀態，
故其中必有某兩個為同一個狀態，設為 $S_{t_p}=S_{t_q}, 0 \leq p<q \leq N+1$ ，
即原流程為 ：
$$
\begin{aligned}
S_{t_0} \xrightarrow{1} S_{t_1} \xrightarrow{1} \cdots & \xrightarrow{1} S_{t_{p-1}} \xrightarrow{1} S_{t_p} \xrightarrow{1} S_{t_{y+1}} \xrightarrow{1} \cdots \\
& \xrightarrow{1} S_{t_{q-1}} \xrightarrow{1} S_{t_q} \xrightarrow{1} S_{t_{q+1}} \xrightarrow{1} \cdots \xrightarrow{0} S_{t_{2 N}} \xrightarrow{0} S_{t_{2 N}},
\end{aligned}
$$
則考慮另一字串 $\beta=1^{N-(q-p)} 0^N$ ，可依下列流程而被接受：
$$
S_{t_0} \xrightarrow{1} S_{t_1} \xrightarrow{1} \cdots \xrightarrow{1} S_{t_{p-1}} \xrightarrow{1} S_{t_q} \xrightarrow{1} S_{t_{q+1}} \xrightarrow{1} \cdots \xrightarrow{0} S_{t_{2 N}} \xrightarrow{0} S_{t_{2 N}} \text {, }
$$
但很明顯 $\beta \notin L$ ，得一矛盾。
\item[（4）] 若 $L=\left\{x x \mid x \in\{0,1\}^*\right\}$ 為正規語言，則一有限狀態機 $M$ 能認知 $L$ ，
設 $M$ 有 $N$ 個狀態，考慮字串 $\alpha=1^N 1^N$ ，則由 $L$ 的定義知 $\alpha \in L$ ，
設此字串從輸入到被接受的狀態變化為：$S_{t_0} \xrightarrow{1} S_{t_1} \xrightarrow{1} \cdots \xrightarrow{1} S_{t_{2 N}}$ ，
考慮 $S_{t_0}, S_{t_1}, \cdots, S_{t_N}$ 這 $N+1$ 個狀態，因為 $M$ 只有 $N$ 個狀態，
故其中必有某兩個為同一個狀態，設為 $S_{t_p}=S_{t_q}, 0 \leq p<q \leq N+1$ ，
即原流程為：
$$
\begin{aligned}
S_{t_0} \xrightarrow{1} S_{t_1} \xrightarrow{1} \cdots & \xrightarrow{1} S_{t_{p-1}} \xrightarrow{1} S_{t_p} \xrightarrow{1} S_{t_{y+1}} \xrightarrow{1} \cdots \\
& \xrightarrow{1} S_{t_{q-1}} \xrightarrow{1} S_{t_q} \xrightarrow{1} S_{t_{q+1}} \xrightarrow{1} \cdots \xrightarrow{1} S_{t_{2 N}} \xrightarrow{1} S_{t_{2 N}},
\end{aligned}
$$
則考慮另一字串 $\beta=1^{N-(q-p)} 1^N$ 可依下列流程而被接受：
$$
S_{t_0} \xrightarrow{1} S_{t_1} \xrightarrow{1} \cdots \xrightarrow{1} S_{t_{p-1}} \xrightarrow{1} S_{t_q} \xrightarrow{1} S_{t_{q+1}} \xrightarrow{1} \cdots \xrightarrow{1} S_{t_{2 N}} \xrightarrow{1} S_{t_{2 N}} \text {, }
$$
但很明顯 $\beta \notin L$ ，得一矛盾。
\end{itemize}