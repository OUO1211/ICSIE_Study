第九章 高等樹結構
421
Advanced Tree Structure
$$
m^0+m^1+m^2+\cdots m^h-1=\sum_{0 \leq i \leq h-1} m^i=\frac{\left(m^h-1\right)}{(m-1)}
$$
\begin{itemize}
\item[2．] 高度為 $h$ 的 B－tree，$h \geq 1$ ，其最少的節點數目是
$$
\begin{aligned}
& 1+2+2\lceil\mathrm{~m} / 2\rceil 2\lceil\mathrm{~m} / 2\rceil+\cdots+2\lceil\mathrm{~m} / 2\rceil^{\mathrm{h}-2} \\
= & 1+\frac{2 *\lceil\mathrm{~m} / 2\rceil^{\mathrm{h}-1}-2}{\lceil\mathrm{~m} / 2\rceil-1}
\end{aligned}
$$
\item[3．] 高度為 $h$ 的 B－tree，$h \geq 1$ ，其最多的鍵值數目是
$$
(m-1) \cdot \sum_{i=0}^{h-1} m^i=(m-1)^* m^{h-1} /(m-1)=m^h-1
$$
\item[4．] 高度為 $h$ 的 B－tree，$h \geq 1$ ，其最少的鍵值數目是
$$
\begin{aligned}
& 1+2^*([\mathrm{~m} / 2]-1)+2\lceil\mathrm{~m} / 2\rceil(\lceil\mathrm{m} / 2\rceil-1)+\cdots+2\lceil\mathrm{~m} / 2\rceil \_\mathrm{h}-2(\lceil\mathrm{~m} / 2\rceil-1) \\
= & 1+2(\lceil\mathrm{~m} / 2\rceil-1)\left[1+\lceil\mathrm{m} / 2\rceil+\cdots+\lceil\mathrm{m} / 2\rceil^{\mathrm{h}-2}\right] \\
= & 1+2\left[\lceil\mathrm{~m} / 2\rceil^{\mathrm{h}-1}-1\right] \\
= & 2\lceil\mathrm{~m} / 2\rceil^{\mathrm{h}-1}-1
\end{aligned}
$$
\end{itemize}

\section*{B tree 的搜尋}

B tree 的每一個節點結構如下圖所示，令其含有 $m-1$ 個鍵值，則由定義可知其含 $m$個指標分別指向不同子樹，亦即 m 是 B－tree 的 degree。
其中 $\mathrm{K}_1<\mathrm{K}_2<\cdots<\mathrm{K}_{\mathrm{n}-1}$ 。當 m 值較小時，可利用線性搜尋法來找尋資料，否則當 m值較大時，可採用二元搜尋法來找尋，令 $x$ 是欲搜尋的鍵值，且假設找到一個 $i$ 值滿足 $\mathrm{K}_{\mathrm{i}} \leq \mathrm{X} \leq \mathrm{K}_{\mathrm{i}+1}$ ，則分成三種情況如下：
\begin{itemize}
\item[（一）] 若 $X>K_i$ ，則繼續搜尋 $A_i$ 指標所指向的節點。
\item[（二）] 若 $\mathrm{X}>\mathrm{K}_{\mathrm{i}}$ ，則表示搜尋成功。
\item[（三）] 若 $\mathrm{A}_{\mathrm{i}}=0$ ，則表示搜尋失敗，鍵值 X 並不存在於 B－tree 內，此時若欲插入資料，可以加於此處。
\item[B] tree 的插入
\item[（一）] 在一次序為 m 的 B－tree（B－tree of order m）中，欲插入一新鍵值 X，則以下述步驟達成。
\end{itemize}