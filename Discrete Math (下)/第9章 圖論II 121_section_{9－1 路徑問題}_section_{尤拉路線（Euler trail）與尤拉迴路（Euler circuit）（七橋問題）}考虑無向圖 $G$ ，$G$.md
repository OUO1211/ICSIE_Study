第9章 圖論II 121

\section*{9－1 路徑問題}

\section*{尤拉路線（Euler trail）與尤拉迴路（Euler circuit）（七橋問題）}

考虑無向圖 $G$ ，
$G$ 上的一個尤拉路線，是指經過 $G$ 的每一邊恰一次的走法；
$G$ 上的一個尤拉迴路，是指經過 $G$ 的每一邊恰一次且回起點的走法。
若 $G$ 有尤拉迴路，則可稱 $G$ 為一尤拉圖（Eulerian graph）。

圖（1）
【105 交大應數】

圖（2）
【101 専利商標】

圖（3）
【105 交大應数】

圖（1）有 Euler circuit：1－2－6－5－2－3－5－4－3－1－4－6－1 。
圖（2）有 Euler trail： $3-2-1-3-4-1-6-4-5-6$ 。
圖（3）沒有 Euler circuit，也沒有 Euler trail。

Note
\begin{itemize}
\item[（1）] 上述定義也可對有向圖做討論。
\item[（2）] 尤拉路線也被稱作 Euler path。
\item[（3）] 尤拉迴路也被稱作 Euler cycle 或 Euler tour。
\item[（4）] 討論這個進度時，一般不會有孤立點。
\item[（5）] 有些書上把 Euler circuit 也算成 Euler trail，但這裡不把 Euler circuit 看做 Euler trail。
\end{itemize}