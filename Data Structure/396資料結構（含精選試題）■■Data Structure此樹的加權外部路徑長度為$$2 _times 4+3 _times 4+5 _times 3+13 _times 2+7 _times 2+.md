396
資料結構（含精選試題）
■■

Data Structure
此樹的加權外部路徑長度為
$$
2 \times 4+3 \times 4+5 \times 3+13 \times 2+7 \times 2+9 \times 2=93
$$
比較之下最好的完整二元樹的加權路徑長度為 95 。

\section*{三．分析 Huffman 演算法}

主迴圈共執行了 $\mathrm{n}-1$ 次。如果 $\ell$ 以堆積來維持那麼每次呼叫 Least 和 Insert 僅需$0(\log n)$ 。因所以演算法的時間複雜度為 $0(n \log n)$ 。

\section*{9－5 最佳化二元搜尋樹（Optimal Binary Search Tree）}

二元搜尋樹含有識別字 $\mathrm{a}_1, \mathrm{a}_2, \cdots, \mathrm{a}_3$ 其中 $\mathrm{a}_1<\mathrm{a}_2 \cdots<\mathrm{a}_{\mathrm{n}}$ ，而且搜尋每個 $\mathrm{a}_{\mathrm{i}}$ 的機率為$\mathrm{p}_{\mathrm{i}}$ ，則任一二元尋樹的成功搜尋成本為 ：
$$
\sum_{0 \leq i \leq n} p_i \cdot \text { level }(a)
$$
而不成功的搜尋成本亦要考慮，令 E 表外部節點，對於階級 $\mathrm{E}_{\mathrm{i}}, 0 \leq \mathrm{i} \leq \mathrm{n}, \mathrm{i}$ 為失敗節點；失敗節點可以從 0 到 n 依序編號。如果 $\mathrm{q}_{\mathrm{i}}$ 是在 $\mathrm{E}_{\mathrm{i}}$ 中找到識別字的機率，那麼失敗的節點的成本為：
$$
\sum_{1 \leq i \leq 0} q_i \cdot(\text { level }(\text { failure node } i)-1)
$$
於是一個二元搜尋樹的總成本為 ：
$$
\sum_{1 \leq i \leq 0} q_i \cdot \operatorname{level}(a)+\sum_{1 \leq i \leq 0} q_i \cdot(\operatorname{level}(\text { failure node } i)-1)
$$
所以，對於識別字 $\mathrm{a}_1, \cdots, \mathrm{a}_{\mathrm{n}}$ 集合的最佳化二元搜尋樹（Optimal Binary Search Tree）即是所有可能的二元搜尋樹的成本中最小者。注意，因為所有搜尋不論成功與否都必須終止，所以我們可得：
$$
\sum_{0 \leq i \leq n} p_i+\sum_{1 \leq i \leq n} q_i=1
$$

\section*{【例題1】}

下圖列出由識別字（do，if，read）組成之可能的二元搜尋樹。
如果所有 i 和 j 有相同的機率 $\mathrm{p}_{\mathrm{i}}=\mathrm{a}_{\mathrm{j}}=1 / 7$ ，那麼 ：