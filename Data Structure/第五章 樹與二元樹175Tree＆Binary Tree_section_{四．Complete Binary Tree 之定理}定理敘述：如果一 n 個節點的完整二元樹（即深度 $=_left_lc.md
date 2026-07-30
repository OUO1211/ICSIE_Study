第五章 樹與二元樹
175

Tree＆Binary Tree

\section*{四．Complete Binary Tree 之定理}

定理敘述：如果一 n 個節點的完整二元樹（即深度 $=\left\lceil\log _2(\mathrm{n}+1)\right\rceil$ ，對於任一編號為 i的節點具有下列性質：
\begin{itemize}
\item[（1）] 如果 $i \neq 1$ ，則其父親 $p$ arent $(i)$ 的位置是 $[i / 2]$ ；如果 $\mathrm{i}=1$ 表示其為樹根，則沒有父親。
\item[（2）] 如果 $2 \mathrm{i} \leq \mathrm{n}$ ，則其左兒子 lchild（i）的位置是 2 i ；若 $2 \mathrm{i}>\mathrm{n}$ ，則 i 沒有左兒子。
\item[（3）] 如果 $2 \mathrm{i}+1 \leq \mathrm{n}$ ，則其右兒子 rchild（i）的位置 $2 \mathrm{i}+1$ ；若 $2 \mathrm{i}+1>\mathrm{n}$ ，則 i 沒有右兒子。
\end{itemize}

證明：只證明上述的第二項即可。因為同階度節點的編號是從左向右，因此②得證明後馬上可以得到③之結果，而①則可以由②3（3）之結果來得證。欲證明②，我們對 i 作歸納。當 $\mathrm{i}=1$ 時，除非 $2>\mathrm{n}$（即1沒有左兒子）否則其左兒子很顯然為2。現假設對所有 $\mathrm{j}(1 \leq \mathrm{j} \leq \mathrm{i})$ ，lchild（j）的位置均為 2 j 。那麼在 lchild（i＋1）的前面兩個節點應為 i 的右兒子及左兒子，而 i 的的左兒子已知為 2i（假設者），因此 i＋1之左兒子即為 $2 \mathrm{i}+2=2(\mathrm{i}+1)$ ，除非 $2(\mathrm{i}+1)>\mathrm{n}$（即 $\mathrm{i}+1$ 沒有左兒子）。

\section*{5－4 二元樹的資料表示方法【重要】}

主要有二種 ：
\begin{itemize}
\item[（一）] 利用陣列來儲存二元樹的節點。
\item[（二）] 用鏈結的表示方法來儲存。
\end{itemize}

茲分述如下：

\section*{一．Array 表示法}

作法：若高度為 k，則準備一一維陣列A［1⋯2k－1］，將節點依編號順序存放於陣列中。