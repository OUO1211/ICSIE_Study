第九章 高等樹結構 401
Advanced Tree Structure

若要搜尋上圖的任一識別字之平均比較次數為：（I for Jan＋2 for Feb＋⋯＋6 for Nov ）$\div 12=3.5$ 。
如果，輸入的次序為 July，Feb，May，Aug，Dec，Mar，Oct，Apr，Jan，June，Sept 和Nov，那麼將得到下圖：
其平均次數為 $37 / 12 \fallingdotseq 3.1$ 。如果月份以字母次序輸入來代替，樹將退化成為下圖：

Skewed Tree
其平均次數為 6.5 。如此在最壞情況下，在二元搜尋相當於 linear searching。
Why AVL？
\begin{itemize}
\item[（一）] 如果二元搜尋樹能維持完整二元樹，那麼其平均和最大搜尋時間將達到最小。然而，因為面對的是動態的情況，當表格正在建立時，也許正要搜尋識別字，因而若沒有讓加入新項目所需時間變得很長，是很難達到此理想的。這些均衡樹將滿足搜尋和插入的時間為 O（logn）特性。
\end{itemize}