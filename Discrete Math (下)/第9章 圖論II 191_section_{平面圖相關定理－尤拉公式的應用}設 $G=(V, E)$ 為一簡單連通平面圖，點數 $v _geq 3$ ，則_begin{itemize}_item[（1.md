第9章 圖論II 191

\section*{平面圖相關定理－尤拉公式的應用}

設 $G=(V, E)$ 為一簡單連通平面圖，點數 $v \geq 3$ ，則
\begin{itemize}
\item[（1）] $e \leq 3 v-6$ 。
\item[（2）] $e \leq \frac{k}{k-2}(v-2)$ ，若每個環路至少由 $k$ 個邊所圍成。
\end{itemize}

【很重要】
【很重要】

【證明】
\begin{itemize}
\item[（1）] 令 $s=$ 將每個區域繞行一周的邊數之總和，則
∵ 每個邊被數了2次，$\quad \therefore s=2 e$ ，
又 ∵ 每個區域至少 3 個邊，$\therefore s \geq 3 r$ ，∴ 得 $3 r \leq 2 e$ ，
又由尤拉公式，
$\therefore 3(2-v+e) \leq 2 e$ ，∴ 得 $e \leq 3 v-6$ 。
\item[（2）] 令 $s=$ 將每個區域繞行一周的邊數之總和，則
∵ 每個 cycle 至少 $k$ 個邊，∴ 每個區域至少 $k$ 個邊，$\therefore s \geq k r$ ，
∵ 每個邊被數了 2 次，$\therefore s=2 e, \therefore$ 得 $k r \leq 2 e$ ，
又由尤拉公式 $r=2-v+e$ ，
$\therefore k r=k(2-v+e) \leq 2 e$ ，
∴ 得 $e \leq \frac{k}{k-2}(v-2)$ 。
\end{itemize}

Note
\begin{itemize}
\item[（1）] 定理（1）等式成立於每區恰三邊。
\item[（2）] 上述的定理結果，可視為給出 $v$ 點簡單平面圖的邊數的上界。
\item[（3）] 上述定理在不連通圖時，結果仍成立。
\end{itemize}