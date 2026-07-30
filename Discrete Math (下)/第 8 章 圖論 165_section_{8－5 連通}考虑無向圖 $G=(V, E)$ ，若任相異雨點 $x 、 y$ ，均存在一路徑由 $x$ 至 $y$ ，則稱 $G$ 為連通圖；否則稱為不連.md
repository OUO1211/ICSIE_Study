第 8 章 圖論 165

\section*{8－5 連通}

考虑無向圖 $G=(V, E)$ ，若任相異雨點 $x 、 y$ ，均存在一路徑由 $x$ 至 $y$ ，則稱 $G$ 為連通圖；否則稱為不連通圖（disconnected graph）。
考虑有向圖 $G=(V, E)$ ，
\begin{itemize}
\item[（1）] 若任相異雨點 $x 、 y$ ，均存在一有向路徑由 $x$ 至 $y$ ，且有一有向路徑由 $y$ 至 $x$ ，則稱 $G$ 為強連通圖（strong connected graph）。
\item[（2）] 若任相異兩點 $x 、 y$ ，均存在一有向路徑由 $x$ 至 $y$ ，或一有向路徑由 $y$ 至 $x$ ，則稱 $G$ 為單方向連通圖（unilaterally connected graph）。
\item[（3）] 若不計方向時，$G$ 為一連通圖，
則稱 $G$ 為弱連通圖（weakly connected graph）。
【 93 海洋電機】【 94 台大工工】【 109 台大工科】
\end{itemize}

例如，下列各圖中，
又如下列無向圖為不連通圖，且有 7 個分量圖（components、同一個分量圖中的任兩點均存在路徑。）