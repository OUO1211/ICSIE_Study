第10章 樹 261

\section*{10－3 有根樹}
\begin{itemize}
\item[（1）] 考虑有向圖 $G$ ，若將 $G$ 視為無向圖時成為樹，則稱 $G$ 為有向樹（directed tree）。
\item[（2）] 若 $G$ 為有向樹且存在唯一一點 $r$ 使 indeg $(r)=0$ ，則稱 $G$ 為有根樹（rooted tree），$r$ 稱為其樹根（root）。
\end{itemize}
設 $G=(V, E)$ 為有根樹。
\begin{itemize}
\item[（3）] 若點 $v$ 的出度数為 0 ，則稱 $v$ 為樹葉（leaf）、終端點（terminal node）、或外部節點（externalnode）。
\item[（4）] 若點 $v$ 的出度数不為 0 ，則稱 $v$ 為內部節點（internal node），或樹枝節點（branch node）。
\item[（5）] 樹根到點 $v$ 的距離稱為 $v$ 的階層數（level）。 $T$ 的最大階層数稱為 $T$ 的高度（height）。
\item[（6）] 若 $T$ 中的樹葉階層均為 $h$ 或 $h-1$ ，則稱 $T$ 為平衡樹（balanced tree）。
\item[（7）] 若點 $u$ 與點 $v$ 有邊相連，且 $u$ 的階層小於 $v$ ，則稱 $u$ 為 $v$ 的父元素（parent），且 $v$ 為 $u$ 的子元素（child）。
\item[（8）] 若點 $u$ 與點 $v$ 有有向路徑相連，且 $u$ 的階層小於 $v$ ，則稱 $u$ 為 $v$ 的祖先（ancestor），且$v$ 為 $u$ 的後代（descendant）。
\end{itemize}

例如右圖中，
\begin{itemize}
\item[（1）] Which vertices are the leaves？
\item[（2）] Which vertex is the parent of $g$ ？
\item[（3）] Which vertices are the descendants of $c$ ？
\item[（4）] Which vertices are the siblings of $s$ ？
\item[（5）] What is the level number of vertex $f$ ？
\item[（6）] What is the height of the tree？
\item[（7）] Is the tree balanced？
\end{itemize}

【85中正資工】【96交大生資】

解
（1）$k, p, h, q, r, s, f$ ．
（2）$d$ ．
（3）$e, f, i, q, r, s$ ．
（4）$q, r$ ．
（5） 2.
（6） 4.
（7）No．