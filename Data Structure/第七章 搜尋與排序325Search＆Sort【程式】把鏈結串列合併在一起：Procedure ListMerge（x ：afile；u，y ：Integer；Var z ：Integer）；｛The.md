第七章 搜尋與排序
325
Search＆Sort

【程式】把鏈結串列合併在一起：
Procedure ListMerge（x ：afile；u，y ：Integer；Var z ：Integer）；
｛The linked lists u and y areerged to obtain z．In u，y and z the records are linked in order of nondecreasing key values．The file of records is named x of type afile．\}
Var i，j：Integer；
Begin
$\mathrm{i}:=\mathrm{u} ; \quad \mathrm{j}:=\mathrm{y} ; \quad \mathrm{z}:=0 ;$
While $((\mathrm{i}<>0)$ and $(\mathrm{j}<>0))$ Do
If $x[i]$ ．key＜＝x［j］．key
The Begin
$$
\begin{aligned}
\mathrm{x}[\mathrm{z}] . \text { key } & :=\mathrm{i} ; \\
\mathrm{z} & :=\mathrm{i} ; \\
\mathrm{i} & :=\mathrm{x}[\mathrm{i}] . \operatorname{link} ;
\end{aligned}
$$
End
else Begin
$\mathrm{x}[\mathrm{z}]$. link $:=\mathrm{j} ;$
z ：＝j；
$\mathrm{j}:=\mathrm{x}[\mathrm{j}]$. link $;$
End；｛of If\}
｛Move remainder\}
If $\mathrm{i}=0$ Then $\mathrm{x}[\mathrm{z}]$ ．link $:=\mathrm{j}$ ；
else $\mathrm{x}[\mathrm{z}]$. link $:=\mathrm{i}$ ；
$\mathrm{z}:=\mathrm{x}[0]$ ．link；
End；｛of ListMerge\}

\section*{三．堆積排序}
\begin{itemize}
\item[（一）] 雖然上述所討論的合併排序法，其平均行為與在最壞的情況下計算時間，兩者是$O(n \log n)$ ，但是其所需要之額外空間，亦與其所排列之記錄個數成正比。此處我們將討論一種只需固定的空間，而在最壞的情況與平均計算時間仍為 $0(\mathrm{n} \log \mathrm{n})$ 的排序方法。
\item[（二）] Heap Tree（堆積樹）的定義（Max－Heap）
\begin{itemize}
\item[1．] 是一個完整二元樹（Complete Binary Tree）。
\item[2．] 每個節點的值大於等於其子點的值。
\end{itemize}
\end{itemize}