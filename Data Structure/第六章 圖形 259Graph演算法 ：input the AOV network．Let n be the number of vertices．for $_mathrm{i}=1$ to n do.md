第六章 圖形 259
Graph

演算法 ：
input the AOV network．Let n be the number of vertices．
for $\mathrm{i}=1$ to n do／／output the vertices／／
begin
if every vertex has a predecessor
then［the network has a cycle and is infeasible．stop］；
pick a vertex v which has no predecessors；
output v；
delete v and all edges leading out of v from the network；
end；
（二）例子
（a）初始圖形
（b）
（c）
（d）
（e）$\quad \mathrm{V}_4$
（f） $\mathrm{V}_2$
（g） $\mathrm{V}_5$

所產生之拓楼順序： $\mathrm{v}_1, \mathrm{v}_4, \mathrm{v}_3, \mathrm{v}_6, \mathrm{v}_2, \mathrm{v}_5$（不只一種）