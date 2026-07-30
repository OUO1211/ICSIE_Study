第九章 高等樹結構
385

Advanced Tree Structure

【程式】DeleteMin
Procedure DeleteMin（var h：MinHeap；var y：element；var n：integer）；
｛Delete an element with minimum key in the Min－Max Heap h．\}
｛n is the number of elements in h ．The deleted element is returned in y ．\}
Var i，j，k，p ：integer；
x, t : element;
NotDone：boolean；
Begin
$$
\text { if } n=0 \text { then EmptyMinMaxHeap else }
$$
Begin
｛Save root and last elements and update heap size\}
$$
\begin{aligned}
& \mathrm{y}:=\mathrm{h}[1] ; \\
& \mathrm{x}:=\mathrm{h}[\mathrm{n}] ; \\
& \mathrm{n}:=\mathrm{n}-1 ;
\end{aligned}
$$
｛Initialize for reinseretion of x \}
NotDone ：＝true；
$$
\begin{aligned}
& \mathrm{i}:=1 ; \\
& \mathrm{j}:=\mathrm{n} \text { div } 2 ; \quad \text { \{Last node with a child }\}
\end{aligned}
$$
｛Find place to insert x \}
while $(\mathrm{i}<=\mathrm{j})$ and NotDone do
Begín｛I has a child，case（2）\}