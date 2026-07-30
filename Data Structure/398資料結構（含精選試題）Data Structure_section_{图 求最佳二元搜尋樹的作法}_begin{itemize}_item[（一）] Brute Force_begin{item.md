398
資料結構（含精選試題）
Data Structure

\section*{图 求最佳二元搜尋樹的作法}
\begin{itemize}
\item[（一）] Brute Force
\begin{itemize}
\item[1．] 對於 n 個節點，先將各種可能的二元樹列舉出來：
$$
\binom{2 n}{n} \frac{1}{n+1}
$$
\item[2．] 算出各二元樹的搜尋成本。
\item[3．] 找出最小成本的二元搜尋樹。
在有 n 個節點的樹中，每個二元搜尋樹可在 0（n）時間內決定成本。如果，N（n）是所有含有 n 個識別字的不同二元搜尋樹，此演法的複雜度可達 $0(\mathrm{nN}(\mathrm{n}))$ ，而 $\mathrm{N}(\mathrm{n})$為 $\mathrm{O}\left(2^{\mathrm{n}}\right)$ 。
\end{itemize}
\item[（二）] 有效的演算法（動態分配）
\begin{itemize}
\item[1．] 假設 $\mathrm{a}_1<\mathrm{a}_2 \cdots \mathrm{a}_{\mathrm{n}}$ 為代表二元搜尋樹中的 n 個識別字。我們以 $\mathrm{T}_{\mathrm{i}} \mathrm{j}$ 來表示 $\mathrm{a}_{\mathrm{i}+1}, \cdots$ ，$a_j$ ，$i<j$ 的最佳二元樹。假設 $T_{i i}$ 為一空樹，且 $T_{i j}$ 並不為 $i>j$ 而定義，以 $c_{i j}$ 代表 $\mathrm{T}_{\mathrm{ij}}$ 的成本。且定義 $\mathrm{c}_{\mathrm{ii}}$ 為 0 ，而 $\mathrm{r}_{\mathrm{ij}}$ 代表 $\mathrm{t}_{\mathrm{ij}}$ 的根部，而：
$$
\mathrm{w}_{\mathrm{ij}}=\mathrm{q}_{\mathrm{i}}+\sum_{\mathrm{k}=\mathrm{I}+1}^{\mathrm{j}}\left(\mathrm{q}_{\mathrm{k}}+\mathrm{p}_{\mathrm{k}}\right)
$$
將代表 $\mathrm{T}_{\mathrm{ij}}$ 的權值。而藉由定義 $\mathrm{r}_{\mathrm{ii}}=0$ ，同時 $\mathrm{w}_{\mathrm{ii}}=\mathrm{q}_{\mathrm{i}}, 0 \leq \mathrm{i} \leq \mathrm{n} 。$ 則 $\mathrm{a}_1, \cdots, \mathrm{a}_{\mathrm{n}}$ 的最佳二元搜尋樹為 $\mathrm{T}_{\text {on }}$ ，其成本為 $\mathrm{c}_{\text {on }}$ ，權值為 $\mathrm{w}_{\text {on }}$ 而其根為 $\mathrm{r}_{\text {on }}$ 。
\end{itemize}
\item[2．] 如果 $\mathrm{T}_{\mathrm{ij}}$ 是 $\mathrm{a}_{\mathrm{i}+1}, \cdots, \mathrm{a}_{\mathrm{j}}$ 的最佳二元搜尋樹，並且 $\mathrm{r}_{\mathrm{ij}}=\mathrm{k}, \mathrm{i}<\mathrm{k} \leq \mathrm{j}$ 那麼 $\mathrm{T}_{\mathrm{ij}}$ 有二個子樹 L 和 R。L 為左子樹，其中含有識別字 $\mathrm{a}_{\mathrm{i}+1}, \cdots, \mathrm{a}_{\mathrm{k}-1}$ ，而 R 為右子樹，含有識別字 $\mathrm{a}_{\mathrm{k}+1}, \cdots, \mathrm{a}_{\mathrm{j}}$ ， $\mathrm{T}_{\mathrm{ij}}$ 的成本 $\mathrm{c}_{\mathrm{ij}}$ 為：
$$
c_{i j}=p_k+\cos t(L)+\cos t(R)+\operatorname{weight}(L)+\operatorname{weight}(R)
$$
其中， $\operatorname{weight}(\mathrm{L})=\operatorname{weight}\left(\mathrm{T}_{\mathrm{i}, \mathrm{k}-1}\right)=\mathrm{w}_{\mathrm{i}, \mathrm{k}-1}$ 而且 $\operatorname{weight}(\mathrm{R})=\operatorname{weight}\left(\mathrm{T}_{\mathrm{kj}}\right)=\mathrm{w}_{\mathrm{kj}} 。$《圖示》最佳的二元搜尋樹 $\mathrm{T}_{\mathrm{ij}}$
$$
c_{i j}=p_k+c_{i, k-1}+c_{k j}+w_{i, k-1}+w_{k j}=w_{i j}+c_{i, k-1}+c_{k j}
$$
\end{itemize}