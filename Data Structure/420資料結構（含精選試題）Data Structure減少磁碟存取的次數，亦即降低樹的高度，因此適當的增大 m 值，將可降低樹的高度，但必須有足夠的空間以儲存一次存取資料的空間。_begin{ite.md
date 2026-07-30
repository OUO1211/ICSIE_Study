420
資料結構（含精選試題）

Data Structure
減少磁碟存取的次數，亦即降低樹的高度，因此適當的增大 m 值，將可降低樹的高度，但必須有足夠的空間以儲存一次存取資料的空間。
\begin{itemize}
\item[2．] 高度為 $h$ 的 m－way search tree，$h \geq 1$ ，則其最多的節點數目是
$$
m^0+m^1+m^2+\cdots m^h-1=\sum_{0 \leq i \leq h-1} m^i=\left(m^h-1\right) /(m-1)
$$
\item[3．] 高度為 $h$ 的 m－way search tree，$h \geq 1$ ，其每個節點的結構是 $n . A_0,\left(K_1, A_1\right), \cdots$ ，$\left(\mathrm{K}_{\mathrm{n}}, \mathrm{A}_{\mathrm{n}}\right)$ 。由於 degree $\leq \mathrm{m}$ ，因此每個節點最多含有 $\mathrm{m}-1$ 個鍵值，所以其最多的鍵值數目是
$$
\left(m^h-1\right) /(m-1)^* m-1=m^h-1
$$
\item[] 例：高度為3的3－way search tree，其最多的節點數目是 $\left(3^3-1\right) /(3-1)=13$ ，且其最多的鍵值數目是 $13^*(3-1)=26$（因每個節點最多祇有兩個鍵值）

＂×＂表示鍵值
\item[（四）] 將 m－way search tree 平衡化，使其所有的終端節點（terminal node）都在同一個階度（level）上，如此則成為最佳化的 m－way search tree，使得樹的高度及每一個節點的鍵值數目都是最佳值。平衡的 m－way search tree 就是 B－tree of order m。
\end{itemize}

\section*{■ B 樹（B tree）}
\begin{itemize}
\item[（一）] B－tree 的定義
一個 B－tree，$T$ of order $m$ ，是一個（m－way search tree，可能是空集合，或是高度 $\leq 1$ 。且 B－tree 是一種外部搜尋法（external searching），其滿足下列三項性質：
\begin{itemize}
\item[1．] 樹根節點至少有 2 個子節點。（亦即子節點數介於 2 與 m 之間）。
\item[2．] 除樹根節點及失敗節點外的所有節點至少含［m／2］個子節點。（亦即子節點介於$\lceil\mathrm{m} / 2\rceil \sim \mathrm{m})$ 。
\item[3．] 所有的失敗節點都在同樣的階度上。
\end{itemize}
\item[（二）] B－tree 中的節點，鍵值數目
\begin{itemize}
\item[1．] 高度為 $h$ 的 B－tree，$h \geq 1$ ，最多的節點數目與 m－way search tree 一樣是
\end{itemize}
\end{itemize}