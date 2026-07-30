第五章 樹與二元樹
173

Tree＆Binary Tree
歸納步驟：由歸納假設得知 i－1 階度之節點的最多個數為 $2^{i-2}$ ，然而因為二元樹中每一個節點之最大次為2，因此 i 階度的節點個數最多是$2 \times \mathrm{i}-1$ 的最大節點數，亦即：
$$
2 \times 2^{\mathrm{i}-2}=2^{\mathrm{i}-1}
$$

2．深度為 $k$ 之二元樹，其節點個數最多是 $\sum_{i=1}^k$（i 階度的最多節點數）。
$$
=\sum_{i=1}^k 2^{i-1}=2^k-1
$$
定理5－2：對於任一非空二元樹 T，如果其終端節點個數 $\mathrm{n}_0$ ，而分支度為2之節點個數是 $n_2$ ，則 $n_0=n_2+1$ 。
證明：令 $\mathrm{n}_1$ 表分支度為1之節點數，n 表示節點總數。因為 T 中的所有節點之分支度均 $\leq 2$ ，因此：
$$
\begin{equation*}
\mathrm{n}=\mathrm{n}_0+\mathrm{n}_1+\mathrm{n}_2 \tag{1}
\end{equation*}
$$
假設 B 表示分支總數，則 $\mathrm{n}=\mathrm{B}+1$ ；而所有分支都源自 degree 為1或2之節點，故 $B=n_1+2 n_2$ 。所以，
$$
\begin{equation*}
\mathrm{n}=1+\mathrm{n}_1+2 \mathrm{n}_2 \tag{2}
\end{equation*}
$$
由（1）（2）知道：
$$
\mathrm{n}_0=\mathrm{n}_2+1
$$

\section*{5－3 二元樹的一些特例}
\begin{itemize}
\item[一、] 斜曲樹，歪斜樹（Skewed Binary Tree）
\item[二、] 完滿二元樹（Full Binary Tree）
\item[三、] 完整二元樹（Complete Binary Tree）
\end{itemize}

一．斜曲樹，歪斜樹（Skewed Binary Tree）
定義：當一個二元樹的所有節點都只有左子點（Left Child）或都只有右子點（RightChild）時，稱之。
可細分為 $\left\{\begin{array}{l}\text { Left }- \text { Skewed Binary Tree及 } \\ \text { Right }- \text { Skewed Binary Tree }\end{array}\right.$