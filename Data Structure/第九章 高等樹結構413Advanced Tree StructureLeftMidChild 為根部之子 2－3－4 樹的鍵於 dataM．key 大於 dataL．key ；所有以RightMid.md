第九章 高等樹結構
413
Advanced Tree Structure

LeftMidChild 為根部之子 2－3－4 樹的鍵於 dataM．key 大於 dataL．key ；所有以RightMidChild 為根部之子 2－3－4 樹的鍵大於 dataM．key 但小於 dataR．key；所有以RightChild 為根部之子 2－3－4 樹的鍵大於 dataR．key。
\begin{itemize}
\item[（五）] 所有外部節點皆位於同一階層。
\item[] 例：
\end{itemize}

一高度為 $h$ ，其元素數目介於 $2^h-1$ 到 $4^h-1$ 之間。而含有 $n$ 個元素的2—3—4樹，其高度介於：
$$
\left[\log _4(\mathrm{n}+1)\right] \text { 和 }\left[\log _2(\mathrm{n}+1)\right] \text { 之間 }
$$

\section*{9 －9 2－3－4 樹的插入}
\begin{itemize}
\item[（一）] 插入 2，3 節點，皆不須 Split，直接插入即可。
\item[（二）] 如果將被插入元素之樹葉節點為 4－節點，那麼此節將被 Split 分割並開始一反向樹葉到根部之過程。這個反向過將在碰到2－或3－節點或者根部 Split 時終止。
\item[1．] 它為 2－3－4 樹的根部
\end{itemize}