310
資料結構（含精選試題）
Data Structure

\section*{一．插入排序（Insertion Sort）}

插入排序法的基本步驟是將一記錄插入到一串排序好的記錄 $\mathbf{R}_1, \mathbf{R}_2, \cdots, \mathbf{R}_i$ 中（ $\mathrm{K}_1 \leq \mathrm{K}_2 \leq \cdots \leq \mathrm{K}_{\mathrm{i}}$ ）使得 i＋1 個記錄又變成一串排序好之結果。以下為 Insert 演算法。

由兩個副程式所組成：
（一）插入到已排序檔案
Procedure Insert（r ：records；Var list ：afile；i ：Integer）；
｛Insert record r with key r．key into the ordered sequence list［0］，list［1］，⋯ ，list［i］ in such a way that the resulting sequence is also ordered on the field key．We assume that list contains a dummy record at index zero such that r．key $\geq$ list［0］．key for all i．\}
Var j：Integer；
Begin
$$
\begin{aligned}
& \mathrm{j}:=\mathrm{i} \text {; } \\
& \text { While r.key < list[j].key Do Begin } \\
& \qquad \operatorname{list}[\mathrm{j}+1]:=\text { list }[\mathrm{j}] ; \\
& \mathrm{j}:=\mathrm{j}-1 ;
\end{aligned}
$$
End；
$$
\operatorname{list}[j+1]:=r ;
$$
End；
（二）插入排序
Procedure Insort（Var list ：afile；n ：Integer）；
｛Sort list in nondecreasing value of the file key．Assume $\mathrm{n}>0$ ．\}
Var j ：Integer；
Begin
```
list[0].key : = ക ;
for j := 2 To n Do
    insert(list[j], list, j-1);
```


End；