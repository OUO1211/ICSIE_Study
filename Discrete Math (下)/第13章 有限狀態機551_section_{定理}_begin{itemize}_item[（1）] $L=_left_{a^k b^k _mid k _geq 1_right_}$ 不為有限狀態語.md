第13章 有限狀態機
551

\section*{定理}
\begin{itemize}
\item[（1）] $L=\left\{a^k b^k \mid k \geq 1\right\}$ 不為有限狀態語言
【92北科資工】【88、92、95政大資科】【93中央绸科】【98清大資應】
\item[（2）] $L=\left\{a^k \mid k=i^2, i>0\right\}$ 不為有限狀態語言。
【94 北科資工】【98 清大資應】
\item[（3）] $L=\left\{1^i 0^j \mid i \geq j\right\}$ 不為有限狀態語言。
【90 清大資應】【94 雲科資工】
\item[（4）] $L=\left\{x x \mid x \in\{0,1\}^*\right\}$ 不為有限狀態語言。
【90政大資科】【96清大資工】
\end{itemize}

\section*{【證明】}
\begin{itemize}
\item[（1）] 若 $L=\left\{a^k b^k \mid k \geq 1\right\}$ 為有限態語言，則有一有限狀態機 $M$ 能認知 $L$ ，
若 $M$ 有 $n$ 個狀態，則考慮字串 $\alpha=a^n b^n$ ，由 $L$ 的定義知 $\alpha \in L$ ，
設此字串從輸入到被接受的狀態變化為：$S_{t_0} \rightarrow S_{t_1} \rightarrow \cdots \rightarrow S_{t_{2 n}}$ ，
考慮 $S_{t_0}, S_{t_1}, \cdots, S_{t_n}$ 這 $n+1$ 個狀態，因為 $M$ 只有 $n$ 個狀態，
故其中必有某兩個為同一個狀態，設為 $S_{t_i}=S_{t_j}, 0 \leq i<j \leq n$ ，
即原流程為 ：
$$
\begin{aligned}
S_{t_0} & \xrightarrow{a} S_{t_1} \xrightarrow{a} \cdots \xrightarrow{a} S_{t_{i-1}} \xrightarrow{a} S_{t_i} \xrightarrow{a} S_{t_{i+1}} \xrightarrow{a} \cdots \\
& \xrightarrow{a} S_{t_{j-1}} \xrightarrow{a} S_{t_j} \xrightarrow{a} S_{t_{j+1}} \xrightarrow{a} \cdots \xrightarrow{a} S_n \xrightarrow{b} S_{n+1} \rightarrow \cdots \xrightarrow{b} S_{2 n},
\end{aligned}
$$
則考慮另一字串 $\beta=a^{n-(j-i)} b^n$ ，可依下列流程而被接受：
$$
\begin{aligned}
S_{t_0} & \xrightarrow{a} S_{t_1} \xrightarrow{a} \cdots \xrightarrow{a} S_{t_{i-1}} \xrightarrow{a} S_{t_i} \xrightarrow{a} S_{t_{j+1}} \xrightarrow{a} \cdots \\
& \xrightarrow{a} S_n \xrightarrow{b} S_{n+1} \rightarrow \cdots \xrightarrow{b} S_{2 n}
\end{aligned}
$$
但很明顯 $\beta \notin L$ ，得一矛盾。
\item[（2）] 反之，設有一有限狀態機 $M$ 能認知 $L$ ，且設 $M$ 有 $N$ 個狀態，
定義 $i$ ，為使 $(i+1)^2-i^2>N$ 成立之整數，考虑字串 $\alpha=a^{(i+1)^2}$ ，則由 $L$ 的定義知 $\alpha \in L$ ，設此字串從輸入到被接受的狀態變化為：$S_{t_0} \rightarrow S_{t_1} \rightarrow \cdots \rightarrow S_{(i+1)^2}$ ，
考虑 $S_{t^2+1}, S_{t^2+2}, \cdots, S_{t_{(i+1)}}$ 這 $(i+1)^2-i^2$ 個狀態，因為 $M$ 只有 $N$ 個狀態，而 $(i+1)^2-i^2>N$ ，故其中必有某兩個為同一個狀態，設為 $S_{t^{\prime}+1+p}=S_{t^{\prime}+1+q}, 0 \leq p<q \leq(i+1)^2-i^2+1$ ，
即原流程為：
$$
\begin{aligned}
S_{t_0} \rightarrow S_{t_1} \rightarrow \cdots \rightarrow & S_{t_{t^2+1+p-1}} \rightarrow S_{t_{t^2+1+p}} \rightarrow S_{t_{t^2+1+p+1}} \rightarrow \cdots \\
& \rightarrow S_{t_{t^2+1+q-1}} \rightarrow S_{t_{t^2+1+q}} \rightarrow S_{t_{t^2+1+q+1}} \rightarrow \cdots \rightarrow S_{t_{(i+1)^2-1}} \rightarrow S_{t_{(i+1)^2}}
\end{aligned}
$$
\end{itemize}