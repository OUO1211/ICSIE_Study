416
資料結構（含精選試題）
Data Structure

例：

以紅－黑樹表示的 2－3－4 樹

2－3－4 tree 插入 Node 到4－節點時 Split 轉換。換成紅－黑樹，他們有著下列四圖的形式。
\begin{itemize}
\item[（一）] 改變 q 的二兒子指標成黑色。
\item[（二）] 將 q 與父點之間的 link 改成紅色。
\item[（三）] 如果有兩個連續的紅指標存在，那麼其中之一從 q 的祖父 gp 到 q 的父親 p。而另一個從 p 到 q。此時需要一個類似在 AVL 所執行的旋轉。
\end{itemize}

圖 根部為4－節點的轉換