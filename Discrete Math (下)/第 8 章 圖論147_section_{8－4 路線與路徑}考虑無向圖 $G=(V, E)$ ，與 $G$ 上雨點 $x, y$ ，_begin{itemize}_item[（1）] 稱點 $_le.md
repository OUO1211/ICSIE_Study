第 8 章 圖論1
47

\section*{8－4 路線與路徑}

考虑無向圖 $G=(V, E)$ ，與 $G$ 上雨點 $x, y$ ，
\begin{itemize}
\item[（1）] 稱點 $\left(v_i\right)$ 邊 $\left(e_j\right)$ 的序列 $P: x e_1 v_1 e_2, \ldots, e_{k-1} v_{k-1} e_k y$ 為一 $x$ 到 $y$ 的路（walk）；並以其邊數稱為該路的長度（length）。當 $x=y$ 時，稱 $P$ 為一封閉路（closed walk），否則稱為一開路（open walk）。
\item[（2）] 邊不重覆的路稱為路線（trail）；封閉的路線稱為迴路（circuit）。
\item[（3）] 點不重覆的路稱為路徑（path）；封閉的路徑稱為環路（cycle）。
\end{itemize}

例如右圖中，
$a-b-c-e-b-d-e$ 為長度為 6 的 trail ；
$b-c-e-d-b$ 為長度為 4 的 circuit ；
$a-b-c-e-d$ 為長度為 4 的 path ；
$b-c-e-d-b$ 為長度為 4 的 cycle。

Note
\begin{itemize}
\item[（1）] 這裡的 walk，在 Rosen 的書中被稱為 path；而這裡的 trail，被稱為 simple path。 因此每個題目在討論之前，都需先釐清題目敘述的 path 是否可以重複行走。
\item[（2）] circuit 可以只一邊，即為 loop；但 cycle 通常都至少三邊。
\item[（3）] Cycle graph $C_n$ ，即一 $n$ 點 $n$ 邊的 cycle ；Path graph $P_n$ ，即一 $n$ 點 $n-1$ 邊的 path。
\item[（5）] $G$ 中最小的 cycle 的長度稱為腰圍（girth）。
\end{itemize}

例題 1
\begin{itemize}
\item[] （10％）How many paths of length four are there from $a$ to $d$ in the following graph？List all paths．
【109中正資工】
\item[解] 本題的 path 為任意路徑，不須點不重複。
$$
\begin{aligned}
& a-b-a-b-d, a-b-a-c-d, a-b-d-b-d, a-b-d-c-d, \\
& a-c-c 1-d \| .
\end{aligned}
$$
\end{itemize}