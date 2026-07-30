36
離散數學（下）

完全子圖（clique）
對無向圖 $G=(V, E)$ ，考慮 $V$ 的子集 $S$ ，若 $S$ 中的點雨雨相鄰，則稱 $S$ 的誘導子圖 $G[S]$ 為$G$ 中的一完全子圖（clique）；並稱 $G$ 中最多點的完全子圖的點數為 $G$ 的 clique number，記為 $\omega(G)$ 。

【99台大資工】

Note
\begin{itemize}
\item[（1）] 若 $G[S]$ 為 $G$ 的一個 clique 且再加點給 $S$ ，則 $G[S]$ 不復為 clique，則稱 $G[S]$ 為 $G$ 的一個極大完全子圖（maximal clique）。
\item[（2）] 也有些書在定義 clique 時，就一併採用 maximal 的條件。
\end{itemize}

例如下圖中，
點集合 $\{a, b, g\}$ 可誘導出一個 clique，同時也是一個 maximal clique；
點集合 $\{b, c, e\}$ 可誘導出一個 clique，但不是 maximal clique ；
且 $\omega(G)=4$ 。