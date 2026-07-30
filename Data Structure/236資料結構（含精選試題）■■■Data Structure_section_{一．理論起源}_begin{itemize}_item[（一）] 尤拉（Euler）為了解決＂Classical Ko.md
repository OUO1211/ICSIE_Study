236
資料結構（含精選試題）
■■■

Data Structure

\section*{一．理論起源}
\begin{itemize}
\item[（一）] 尤拉（Euler）為了解決＂Classical Koenigsberg Bridge＂的問題，把土地部份用頂點（Vertex）表，橋用邊（Edge）表示，圖示如下：
欲解決的問題如下：
＂若由某個地區出發，最後再回原到出發地區，且把每座橋都走過一次，而且僅能走過一次＂，是否可能。
\item[（二）] 兩個重點的理論
\begin{itemize}
\item[1．] Eulerian Cycle
定義：從任何一點開始，經過每個邊一次，再回到原出發點時稱之。充分且必要條件：每個頂點的分支度都必須為偶數。
\item[2．] Eulerian Chain
定義：從任何一個頂點開始，經過每個邊一次，但不一定要回到原出發點。充分且必要條件：只有兩個頂點的分支度是奇數，其餘必須均為偶數。
\end{itemize}
\item[（三）] 圖形的應用
\begin{itemize}
\item[1．] 電路分析。
\item[2．] 工作計畫分析。
\item[3．] 尋找最短路徑。
\item[4．] 城市間的交通路線圖。
\end{itemize}
\end{itemize}

\section*{二．定義與術語}
\begin{itemize}
\item[（一）] 圖形（Graph）是由兩個非空的有限集合所組成 ：
\begin{itemize}
\item[1．] V：代表所有的頂點（Vertices）的集合。
\item[2．] E：代表所有的邊（Edge）所成的集合，且每一個邊由成對的頂點所表示。
\end{itemize}
\item[（二）] 圖形的兩大種類
\begin{itemize}
\item[1．] 無向圖形（Undirected Graph）
定義：在一無向圖形中，$\left(\mathrm{V}_1, \mathrm{~V}_2\right)$ 和 $\left(\mathrm{V}_2, \mathrm{~V}_1\right)$ 所代表的是同一個邊。
\end{itemize}
\end{itemize}