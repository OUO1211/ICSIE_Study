386
資料結構（含精選試題）
```
Data Structure
        k : = MinChildGrandChild(i)
        if x.key<=h[k].key
            then NotDone : =false;
                {case2(1.), x is to be inserted into h[i]}
        else Begin {case2(2.) or (3.)}
            h[i] : = h[k];
            if k < = 2* i + 1
                then NotDone : = false;
                {k is a child of i, case2(1.)}
        else Begin {k is a grandchild of i, case2(3.)}
            p := k div 2; {parent of k}
            if x.key > h[p].key then
                Begin
                    t:= h[p]
                    h[p] :=x;
                    x:=t;
                End;
                End; {of if k<=2*i+1
                i := k;
            End; {of if x.key < = h[k].key}
            h[i]:=x; {insert x}
        End; {of if n = 0}
    End; {of DeleteMin}
```

\begin{itemize}
\item[] －Time Complexity：O（logn）插入，刪最小，刪最大元素皆同
\end{itemize}

\section*{9－2 雙堆積}

雙堆積是一雙堆積（Double－Ended－Heap），亦能提供雙邊優先序列的運算，—（1）插入，（2）刪除最小，及（3）刪最大元素。這些運算在雙堆中須花費 $O(\log n)$ 時間。然而雙堆積因使用一固定空間而更快，同時演算法也更簡單。

定義：雙堆積為一完整二元樹，它可能是空的或滿足下列特性