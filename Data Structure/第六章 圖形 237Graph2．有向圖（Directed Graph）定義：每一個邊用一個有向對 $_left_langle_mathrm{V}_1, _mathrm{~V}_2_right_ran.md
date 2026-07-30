第六章 圖形 237
Graph

2．有向圖（Directed Graph）
定義：每一個邊用一個有向對 $\left\langle\mathrm{V}_1, \mathrm{~V}_2\right\rangle$ 來表示，其中 $\mathrm{V}_1$ 是該邊的尾（Tail）而$\mathrm{V}_2$ 是頭（Head），$\left\langle\mathrm{V}_1, \mathrm{~V}_2\right\rangle$ 與 $\left\langle\mathrm{V}_2, \mathrm{~V}_1\right\rangle$ 代表兩個不同的邊。
（三）例子：

表示
G1：無向圖形，其中
$$
\begin{aligned}
& \mathrm{V}(\mathrm{G} 1)=\{1,2,3,4\} \\
& \mathrm{E}(\mathrm{G} 1)=\{(1,2),(1,3),(1,4),(2,3),(2,4),(3,4)\}
\end{aligned}
$$

G2 ：無向圖形，其中
$$
\begin{aligned}
& \mathrm{V}(\mathrm{G} 2)=\{1,2,3,4,5,6,7\} \\
& \mathrm{E}(\mathrm{G} 2)=\{(1,2),(1,3),(2,4),(2,5),(3,6),(3,7)\}
\end{aligned}
$$

G3：有向圖形，其中
$$
\begin{aligned}
& \mathrm{V}(\mathrm{G} 3)=\{1,2,3\} \\
& \mathrm{E}(\mathrm{G} 3)=\{\langle 1,2\rangle,\langle 2,1\rangle,\langle 2,3\rangle \quad\}
\end{aligned}
$$
（四）有關術語
1．Complete Graph
定義：在一具有 n 個頂點的無向圖形中，滿足 $V_i \neq V_j$ ，且無重複邊的條件時，若具有 $\mathrm{n}(\mathrm{n}-1) \div 2$ 個邊存在時，稱為 Complete Graph。
P．S．（1）Multigraph ：有重複邊存在（不是圖形），因為違反 $\mathrm{E}(\mathrm{G})$ 的集合定義。
（2）在一有向圖形中，最多的存在邊數為 n（n－1）。
2．Subgraph（子圖）
定義：假設 $\mathrm{G}^{\prime}$ 是 G 的子圖，則表示 $\mathrm{V}\left(\mathrm{G}^{\prime}\right) \subseteq \mathrm{V}(\mathrm{G})$ ，
$$
\text { 且 } E\left(G^{\prime}\right) \subseteq E(G)
$$

例：G1的一些子圖如下：（未完全列出）