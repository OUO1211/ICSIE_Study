58
離散數學（下）

\section*{兩點的距離（distance）}
\begin{itemize}
\item[（1）] 兩點 $x, y$ 間之最短路徑的邊數稱為 $x, y$ 間的距離，記作 $d(x, y)$ 或 $\operatorname{dist}(x, y)$ 。
\item[（2）] 無向圖 $G$ 的直徑（diameter）， $\boldsymbol{\operatorname { d i a m }}(G)$ ，定義成 $\max \{d(x, y) \mid x, y \in V(G)\} 。$（即 $G$ 中最遠的兩點距離）。
\item[（3）] 無向圆 $G$ 的半徑（radius）定義成 $\min \{e c c(v) \mid v \in V(G)\}$ ，其中，$e c c(v)=\max \{d(v, y) \mid y \in V(G)\}$ 。
\end{itemize}

Note
$1+\Delta+\Delta(\Delta-1)+\Delta(\Delta-1)^2+\ldots+\Delta(\Delta-1)^{d-1} \geq n$,
其中，$\Delta=G$ 的最大度數，$d=\operatorname{diam}(G), n=|V(G)|$ 。【83中山資工】【96清大資應】
【證明】
可視 $G$ 為連通圖，（不然 $\operatorname{diam}(G)=\infty$ ，本式亦成立。）
任取一點 $x$ ，則 $G$ 中得其餘點可依與 $x$ 之遠近分類如下：
$$
\begin{aligned}
& |\{y \mid \operatorname{dist}(x, y)=1\}| \leq \Delta \\
& |\{y \mid \operatorname{dist}(x, y)=2\}| \leq \Delta(\Delta-1) \\
& |\{y \mid \operatorname{dist}(x, y)=3\}| \leq \Delta(\Delta-1)(\Delta-1) \\
& \quad \vdots
\end{aligned}
$$
$|\{y \mid \operatorname{dist}(x, y)=\operatorname{diam}(G)=d\}| \leq \Delta(\Delta-1)^{d-1}$,
故得 $|V(G)| \leq 1+\Delta+\Delta(\Delta-1)+\ldots+\Delta(\Delta-1)^{d-1}$ 。