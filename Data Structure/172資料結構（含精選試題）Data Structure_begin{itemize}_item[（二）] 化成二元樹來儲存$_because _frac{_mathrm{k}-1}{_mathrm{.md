172
資料結構（含精選試題）
Data Structure
\begin{itemize}
\item[（二）] 化成二元樹來儲存
$\because \frac{\mathrm{k}-1}{\mathrm{k}}$ 要最低， $\mathrm{k}=2$ ，其 Degree $\leq 2$ ，故節點結構可以如下：

\begin{tabular}{|l|l|l|}
\hline LLINK & DATA & RLINK \\
\hline
\end{tabular}
\end{itemize}

\section*{5－2 二元樹（Binary Tree）}
\begin{itemize}
\item[一．] 二元樹的定義【重點】
二樹（Binary Tree）乃是一個由節點構成的有限集合，可以是空集合，若不為空，則由樹根及左子樹（Left Subtree）與右子樹（Right Subtree）所構成，而左、右子樹亦是二元樹。【註】二元樹又稱為Knuth樹或Ordered Tree（有序樹），它的每一個節點之 Degree $\leq 2$ ，左、右子樹有次序之分。
\item[二．] 二元樹與樹的不同點之比較【重點】
主要的不同有三點，茲分述如下：
\begin{itemize}
\item[（一）] 樹不可以為空（即至少存在有一個樹根），但二元樹可以為空。
\item[（二）] 樹中每一節點的 Degree $\geq \phi$ ，但二元樹中的每一節點之分支度介於 $\phi$ 與2之間。
\item[（三）] 樹的子樹之間沒有次序之分，但二元樹的子樹之間則有次序之分。例：
在樹中視為相同，但二元樹視為不同。
\end{itemize}
\item[三．] 二元樹的二個基本定理【重點】
定理5－1：1．二元樹之第 i 階度的節點個數最多為 $2^{\mathrm{i}-1}$ ， $\mathrm{i} \geq 1$
2．深度為 $k$ 的二元樹之節點個數最多為 $2^k-1, k \geq 1$
\end{itemize}
證明：1．對 i 作歸納
歸納基礎：當階度 $\mathrm{i}=1$ 時，節點只有樹根。因此， $\mathrm{i}=1$ 階度的節點個數為
$$
2^0=2^{i-1}
$$
歸納假設：假設所有 $\mathrm{j}, 1 \leq \mathrm{j}<\mathrm{i}$ ，在 j 階度之最多節點個數為 $2^{\mathrm{j}-1}$