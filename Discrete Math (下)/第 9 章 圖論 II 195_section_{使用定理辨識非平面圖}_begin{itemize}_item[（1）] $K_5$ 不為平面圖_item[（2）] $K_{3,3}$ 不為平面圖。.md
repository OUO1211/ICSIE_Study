第 9 章 圖論 II 195

\section*{使用定理辨識非平面圖}
\begin{itemize}
\item[（1）] $K_5$ 不為平面圖
\item[（2）] $K_{3,3}$ 不為平面圖。
\end{itemize}
（3）Petersen graph 不為平面圖。
（4）$K_n$ 不為平面圖 $\Leftrightarrow n>4$ 。
【89北科資工】【94台大工工】
（5）$K_{m, n}$ 為平面圖 $\Leftrightarrow m \leq 2$ 或 $n \leq 2$ 。

【重要】
【重要】
【86中山資工】

【88台大資工】

【證明】
\begin{itemize}
\item[（1）] $K_5$ 的點數 $=5$ ，邊數 $=10$ ，
若 $K_5$ 為平面圖，則 $e \leq 3 v-6$ ，即 $10 \leq 15-6$ ，矛盾。
\item[（2）] $K_{3,3}$ 的點數 $=6$ ，邊數 $=9$ ，而 $K_{3,3}$ 中每個 cycle 長均 $\geq 4$ 。
若 $K_{3,3}$ 為平面圖，則 $e \leq \frac{4}{4-2}(v-2)$ ，即 $9 \leq 2 \cdot(6-2)$ ，矛盾。
\item[（3）] Petersen graph 的點數 $=10$ ，邊數 $=15$ ，而其中每個 cycle 長均 $\geq 5$ 。
因此若為平面圖，則 $e \leq \frac{5}{5-2}(v-2)$ ，即 $15 \leq \frac{5}{3} \cdot(10-2)$ ，矛盾。
\item[（4）] （⇒）很明顯可畫出 $n<5$ 時，即 $K_1, K_2, K_3, K_4$ 均為平面圖。
（⇐）當 $n \geq 5$ 時，$K_n$ 中必含有 $K_5$ 為子圖，故知必不為平面圖。
\item[（5）] （⇐）很明顯可畫出 $m \leq 2$ 或 $n \leq 2$ 時為平面圖。
（⇒）當 $m \geq 3$ 且 $n \geq 3$ 時，$K_{m, n}$ 中必含有 $K_{3,3}$ 為子圖，故知必不為平面圖。
\end{itemize}