252
資料結構（含精選試題）
■■

Data Structure
\begin{itemize}
\item[（二）] 假設條件及所需的資料結構
\begin{itemize}
\item[1．] 成本矩陣：將 $\mathrm{G}=(\mathrm{V}, \mathrm{E})$ 以相鄰矩陣的方式，將各邊的 Weight（或 Cost）存於一個二維陣列 $\operatorname{Cost}(1: n, 1: n)$ 之中，定義如下：
\item[] → $\quad \operatorname{Cost}(\mathrm{i}, \mathrm{j})=$ Weight 值 ，if＜i，j＞存在
$\operatorname{Cost}(\mathrm{i}, \mathrm{j})=\infty \quad$, if $\langle\mathrm{i}, \mathrm{j}\rangle$ 不存在
$\operatorname{Cost}(\mathrm{i}, \mathrm{j})=0 \quad$, if $\mathrm{i}=\mathrm{j}$
\item[2．] $\mathrm{S}(1 . . \mathrm{n})$ 為一個一維陣列，代表頂點的集合；若 $\mathrm{S}(\mathrm{i})=1$ 表示從 $\mathrm{V}_0$ 到此頂點 $\mathrm{V}_{\mathrm{i}}$ 的最短路徑已被找出。
\item[3．] DIST（1．．n）為一個一維陣列，DIST $(\mathrm{j})$ 表示頂點 $\mathrm{V}_0$ 到達 $\mathrm{V}_{\mathrm{j}}$ 的最短路徑長度。
\end{itemize}
\item[] 例：下圖（a）是一個含有 8 個頂點的有向圖，其成本矩陣如下圖（b）所示。

圖（a）

\begin{table}
\begin{tabular}{|l|l|l|l|l|l|l|l|l|}
\hline & 1 & 2 & 3 & 4 & 5 & 6 & 7 & 8 \\
\hline 1 & 0 & & & & & & & \\
\hline 2 & 300 & 0 & & & & & & \\
\hline 3 & 1000 & 800 & 0 & & & & & \\
\hline 4 & & & 1200 & 0 & & & & \\
\hline 5 & & & & 1500 & 0 & 250 & & \\
\hline 6 & & & & 1000 & & 0 & 900 & 1400 \\
\hline 7 & & & & & & & 0 & 1000 \\
\hline 8 & 1700 & & & & & & & 0 \\
\hline
\end{tabular}
\captionsetup{labelformat=empty}
\caption{圖（b）：圖（a）的花費相鄰矩陣，未表示的值為 $\infty$}
\end{table}
\end{itemize}