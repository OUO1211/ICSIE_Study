第九章 高等樹結構
419
Advanced Tree Structure

m－way search tree
\begin{itemize}
\item[（一）] 定義
m 路搜尋樹 T 是一個所有的節點分支度 $\leq \mathrm{m}$ 的樹。若 T 是空樹（即 $\mathrm{T}=0$ ），那麼 T仍然是一個 m 路搜尋樹。若 T 不是空樹時，則它具有下列性質：
\begin{itemize}
\item[1．] 節點的結構是
其中
$$
\begin{aligned}
& n, A_0,\left(k_1, A_1\right),\left(k_2, A_2\right), \cdots,\left(k_n, A_n\right) \\
& A_i, 0 \leq i \leq n \text { 是指向 } T \text { 子樹的指標, 且 } \\
& k_i, 1 \leq i \leq n \text { 為 } T \text { 中的鍵值。 }
\end{aligned}
$$
\item[2．] 節點中的鍵值是由小而大排列的，因此 $\mathrm{k}_{\mathrm{i}}<\mathrm{k}_{\mathrm{i}}+1,1 \leq \mathrm{i} \leq \mathrm{n} 。$
\item[3．] 子樹 $\mathrm{A}_{\mathrm{i}}$ 的所有鍵值均小於鍵值 $\mathrm{K}_{\mathrm{i}}+1,0 \leq \mathrm{i} \leq \mathrm{n}$
\item[4．] 子樹 $A_n$ 的所有鍵值均大於鍵值 $K_n$ 。
\item[5．] 子樹 $A_i, 0 \leq i \leq n$ 同樣是 m 路搜尋樹。
\end{itemize}
\end{itemize}
若要搜尋某一記錄 R ，其鍵值為 Y 。首先搜尋樹根，比較樹根中的每一個鍵值 $\mathrm{k}_{\mathrm{i}}$ ，$1 \leq k \leq n$ ；若 $Y=k_i$ ，則搜尋成功，否則必定存在 $k_i \leq Y<k_i+1, Y$ 必存在子樹 $\mathrm{A}_{\mathrm{i}}$ 中，因此繼續搜尋子樹 $\mathrm{A}_{\mathrm{i}}$ 。
\begin{itemize}
\item[（二）] 演算法
Procedure $\operatorname{MSEARCH}(\mathrm{T}, \mathrm{Y})$
$\mathrm{P} \leftarrow \mathrm{T} ; \mathrm{K}_0 \leftarrow[-\infty] ; \mathrm{Q} \leftarrow 0 / / \mathrm{Q}$ is the parent of $\mathrm{P} / /$
while $\mathrm{P} \neq 0$ do
input node P form disk
Let P define n， $\mathrm{A}_0\left(\mathrm{~K}_1, \mathrm{~A}_1\right), \cdots,\left(\mathrm{K}_{\mathrm{n}}, \mathrm{A}_{\mathrm{n}}\right)$
$\mathrm{K}_{\mathrm{n}}+1 \leftarrow[+\infty]$
Let i be such that $\mathrm{K}_{\mathrm{i}} \leq \mathrm{Y}<\mathrm{K}_{\mathrm{i}}+1$
if $\mathrm{Y}=\mathrm{K}_{\mathrm{i}}$ then［／／Y has been found／／return（ $\mathrm{p}, \mathrm{i}, 1$ ）］
$\mathrm{Q} \leftarrow \mathrm{P} ; \mathrm{P} \leftarrow \mathrm{A}_{\mathrm{i}}$
end
／／Y not in T；return node into which insertion can
take place／／
return（Q，i，0）
end MSEARCH
\item[（三）] m－路搜尋樹的評估
\begin{itemize}
\item[1．] 磁碟存取動作的最高數目與樹的高度相等；因此欲增快資料的搜尋速度，則須
\end{itemize}
\end{itemize}