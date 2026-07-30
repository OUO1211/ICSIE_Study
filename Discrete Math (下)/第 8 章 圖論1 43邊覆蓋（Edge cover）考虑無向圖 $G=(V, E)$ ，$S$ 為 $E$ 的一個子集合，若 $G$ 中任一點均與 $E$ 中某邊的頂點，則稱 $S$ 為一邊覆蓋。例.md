第 8 章 圖論1 43

邊覆蓋（Edge cover）
考虑無向圖 $G=(V, E)$ ，$S$ 為 $E$ 的一個子集合，若 $G$ 中任一點均與 $E$ 中某邊的頂點，則稱 $S$ 為一邊覆蓋。

例如下圖中，
$\{(a, c),(b, e),(d, f),(g, h)\}$ 即為一邊覆蓋，且亦為極小邊覆蓋。

Note
\begin{itemize}
\item[（1）] 若在一個邊覆蓋 $S$ ，滿足再任拿掉一邊，會變成不是邊覆蓋，則稱 $S$ 為極小邊覆蓋（minimaledge cover）。
\item[（2）] The edge covering number $\beta^{\prime}(G): G$ 中具最少邊的邊覆蓋的邊數。
\item[（3）] 若 $G$ 沒有孤立點，則 $|V(G)|=\alpha^{\prime}(G)+\beta^{\prime}(G)$ 。（此結果之證明較複雜，請讀者參考圖論相關書籍）
\end{itemize}