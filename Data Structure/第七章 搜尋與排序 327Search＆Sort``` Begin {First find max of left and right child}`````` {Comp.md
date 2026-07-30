第七章 搜尋與排序 327
Search＆Sort
```
    Begin {First find max of left and right child}
```

```
            {Compare max. Child with k. If k is max, then done.}
        If k >= tree[j].key
            Then done : = true;
            else Begin
                tree[j Div 2] : = tree[j];
                {Move j'th record up tree}
                j := 2* j;
        End; {of If}
    End; {of While}
    tree[j Div 2] : = r;
End; {of Adjust}
```


如果根部為 i 的樹之高度為 k，那麼 while 迴圈最多執行 k 次。因而演算法的計算時間為 $0(\mathrm{k})$ 。

【程式】堆積排序
Procedure HeapSort（Var r ：afile；n ：Integer）；
｛The file $\mathrm{r}=(\mathrm{r}[1], \cdots, \mathrm{r}[\mathrm{n}])$ is sorted into nondecreasing order on the field key．\}
Var i ：Integer；
```
t : records;
```


Begin
For $\mathrm{i}:=(\mathrm{n}$ Div 2）Downto 1 Do｛Convert r into a heap\}
```
Adjust(r, i, n);
For i : = (n - 1) Downto 1 Do {Sort r}
    Begin
        t : =r[i+1]; {Interchange r1 and rj+1}
        r[i+1] : = r[1];
        r[1]:=t;
            Adjust(r, 1, i); {Recreate Heap}
End; {of For loop}
End; {of HeapSort}
```