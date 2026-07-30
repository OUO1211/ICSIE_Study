410
資料結構（含精選試題）
Data Structure

case compare（x，p）of
\begin{itemize}
\item[1：] $\mathrm{p}:=\mathrm{p} \uparrow$ ．LeftChild；$\quad\{\mathrm{x}<\mathrm{p} \uparrow$ ．dataL．key $\}$
\item[] 2：p：＝p ↑ ．MiddleChild；｛p↑．dataL．key＞x＞p↑．dataR．key\}
\item[3：] $\mathrm{p}:=\mathrm{p} \uparrow$ ．RightChild；$\quad\{\mathrm{x}>\mathrm{p} \uparrow$ ．dataR．key $\}$
\item[] 4：NotDonep：＝false；$\quad\{\mathrm{x}$ is one of the keys in p$\}$
\end{itemize}
end；｛of case and while\}
End；｛of Search23\}
（六）2－3 樹的插入
【例 1】：插入70，得到下圖

【例 2】：再插入30，則為

【例 3】：再插入60，