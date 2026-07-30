240
資料結構（含精選試題）
■■

Data Structure

\section*{6－1 圖形的表示方式（重要1}

有四種方式：
\begin{itemize}
\item[1．] 相顒矩陣（Adjacency Matrix）
\item[2．] 相憭串列（Adjacency List）
\item[3．] 相鄭多元串列（Adjacency Multilist）
\item[4．] 索引表（Index Table）
\end{itemize}

\section*{一．相数矩陣（Adjacency Matrix）}
\begin{itemize}
\item[（一）] 令 $\mathrm{G}=(\mathrm{V}, \mathrm{E})$ 為一具有 n 個頂點的圖形，其中 $\mathrm{n} \geq 1$ ，則 G 的相鄰矩陣為一個二維$n \times n$ 的陣列 $A$ ，若且唯若 $\left(V_i, V_j\right)$ 為 $E(G)$ 上的一個邊，則 $A[i, j]=1$ ，否則為 $\phi$ 。
\item[（二）] 例 ：
\item[] G2 ：
\item[（三）] 一個無向圖形的相鄰矩陣是對稱的；而一個有向圖形的相鄰矩陣則不一定是對稱的（如 G2）。
\item[（四）] 若使用相鄰矩陣來表示一個圖形，共需要 $\mathrm{n}^2$ 個空間；而在無向圖形的情況中可以只保存矩陣的上三角或下三角，因此大約可省下一半的空間。
\item[（五）] 易判斷是否有一個邊（ $\mathrm{V}_{\mathrm{i}}, \mathrm{V}_{\mathrm{j}}$ ）存在，time 為0（1）。
\item[（六）] 分支度計算
對一個無向圖形而言，任何一個頂點 i 的分支度是相對於該頂點之列中的所有元素和，$\sum_{\mathrm{j}=1}^{\mathrm{n}} \mathrm{A}[\mathrm{i}, \mathrm{j}]$ ；對有向圖形而言，列元素和是頂點的出支度，而行元素和則是入支度。
\item[（七）] 困難
\end{itemize}