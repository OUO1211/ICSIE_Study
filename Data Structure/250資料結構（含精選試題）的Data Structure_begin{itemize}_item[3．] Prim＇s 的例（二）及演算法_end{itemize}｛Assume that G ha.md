250
資料結構（含精選試題）
的

Data Structure
\begin{itemize}
\item[3．] Prim＇s 的例（二）及演算法
\end{itemize}
｛Assume that G has at least one vertex\}
$\mathrm{T}:=0$ ；
$\mathrm{U}:=\{1\} ; \quad\{$ Start with vertex 1 and on edges $\}$
Done ：＝false；
while $T$ contains fewer than（ $n-1$ ）edges and not done do begin
Let（ $\mathrm{u}, \mathrm{v}$ ）be a least cost edge such that $\mathrm{u} \in \mathrm{U}$ and $\mathrm{v} \in \mathrm{V}-\mathrm{U}$ ；
If there is no such edge then done ：＝true
else add v to U and（u，v）to T and delete v from $\mathrm{V}-\mathrm{U}$ ；
end；
if T contains fewer than n－1 edges
then writeln（＇no spanning tree＇）；