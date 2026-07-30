324
資料結構（含精選試題）
■■■
Data Structure

從上述的例子中，我們可以得到如下之結論，如果 Merge 演算法是要將一個排好序的檔案合併到另一個，那它需要做部份檔案的拷貝工作。例如：要合併［5，26］與［77］，我們就必須將［77］拷貝到［5，26］的陣列中。此項拷貝工作之所以需要，主要是緣自其循序表示方式。為避免這種拷貝工作，我們將利用鏈結串列來表示各部份檔案。利用鏈結的表示方式可以使遞回形式的合併排序法更具效率。

【程式】採用遞回的合併排序 ：
Procedure rMergeSort（Var x ：afile；1，u ：Intger；Var p ：Integer）；
｛The list $\mathrm{x}=([1], \cdots, \mathrm{x}[\mathrm{u}])$ is to be sorted on the field key．link is a link field in each record and is initially set to 0．The sorted list is a chain beginning at p．x［0］is a record for intermediate results used only in ListMerge\}
Var mid，q，r：Integer；
Begin
```
If 1>= u Then p :=1
    else Begin
        mid : = (1+u) div 2;
        rMergeSort(x, 1, mid, q);
        rMergeSort(x, mid+1, u, r);
        ListMerge(x, q, r, p);
```

End; \{of if\}
End; \{of rMergeSort\}