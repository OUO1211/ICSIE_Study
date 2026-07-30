第三章 堆疊與佇列
107

Stack＆Queue
\begin{itemize}
\item[（二）] n 個 stacks $(\mathrm{n}>2)$ 之 Solution
為了表示 n 個（ $\mathrm{n}>2$ ）推疊在一維陣列中，我們可以將 $\mathrm{U}[1 \cdots \mathrm{~m}]$ 之空間分割成 n 段，而每一段給一個堆疊使用。將 U［1⋯m］平均分割。對於每個堆疊，我們利用 b［i］表示堆疊 i 的底端元素（ $1 \leq i \leq n$ ）。因此當 $b[i]=t[i]$ 就變成堆疊 i 為空的之充要條件。初始的 $\mathrm{b}[\mathrm{i}]$ 及 $\mathrm{t}[\mathrm{i}]$ 值如下：
$$
\mathrm{b}[\mathrm{i}]=\mathrm{t}[\mathrm{i}]=[\mathrm{m} / \mathrm{n}](\mathrm{i}-1), 1 \leq \mathrm{i} \leq \mathrm{n} \text {, 且 } \mathrm{b}[\mathrm{n}+1]=\mathrm{m}
$$
如此，堆疊 $\mathrm{i}(1 \leq \mathrm{i} \leq \mathrm{n})$ 就可以從 $\mathrm{b}[\mathrm{i}]+1$ 成長到 $\mathrm{b}[\mathrm{i}+1]$ ，直到碰到 $\mathrm{i}+1$ 堆疊為止。堆疊之插入與刪除運算的演算法如下。
\item[] 程式（a）：加入元素到第 i 個堆疊。
Procedure push（i ：integer ；x ：items）；
$$
\text { \{add x to the i th stack\} }
$$
BEGIN
$$
\text { if } \mathrm{t}[\mathrm{i}]=\mathrm{b}[\mathrm{i}+1] \text { then stackFull(i)] }
$$
else BEGIN
$$
\mathrm{t}[\mathrm{i}]:=\mathrm{t}[\mathrm{i}]+1 ;
$$
$\mathrm{u}[\mathrm{t}[\mathrm{i}]]:=\mathrm{x} ;\{$ add x to i th stack， u 為一維陣列 $(1 \ldots \mathrm{~m})\}$
END ；
END ；
\item[] 程式（b）：刪除堆疊 i 的最頂端元素。
Procedure pop（i ：integer ；var x ：items）；
$$
\text { \{delete topmost item of stack } \mathrm{i} \text { \} }
$$
BENGIN
$$
\text { if } t[i]=b[i] \text { then StackEmpty(i) }
$$
else BEGIN
x : = u[t[i]];
t［i］：＝t［i］－1；
END；
END．
\item[] 【討論】push演算法中的 stackfull 條件並不表示 U 陣列的所有 m 個空間均已用完，可能在其兩個堆疊 $j$ 與 $j+1(1 \leq j \neq n, j \neq i)$ 之間還有很多空間尚未使用，因此程序 stackfull（i）必須决定陣列中是否尚餘空間。若仍有空間，那 stackfull
\end{itemize}