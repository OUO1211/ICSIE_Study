第六章 圖形 257
Graph
```
        A(i, j)←AdjacencyMatrix
    end
end
for k←1 to n do
    for i←1 to n do
        for j←1 to n do
            A(i,j)←A(i,j) or (A(i,k) and A(k,j));
        end
    end
end
end TRAN_CLOSURE
```


6－6 拓撲排序（Topologic al Sort）
作業網路（Activity on Vertex Network，AOV）
臨界路徑（Critical Paths）
\begin{itemize}
\item[一．] 拓撲排序的意義
大部份的計畫都包含許多細部計畫，這些細部計畫稱為工作（Activity），而這些 Activity之間往往存在有次序關係，如何安排處理這些細部的計畫之正確執行順序，正是拓撲排序的意義所在。
\item[二．] 作業網路的相關定義
定義：在一個有向圖形 G＝〈V，E〉中，其中頂點表示工作，邊表示工作之間的先後關係，則稱該圖形為一個作業頂點網路（Activity on Vertex Network）或稱為 AOV網路。
定義：在一個 AOV 網路上，若且唯若存在有一個從頂點 i 到頂點 j 的有向路徑，則稱頂點 i 為頂點 j 的前導（Predecessor）。而若且唯若 G 中有一個邊（i，j）則稱 i 是 j的立即前導（Immediate Predecessor）。如果 i 是 j 的立即前導，則稱 j 是 i 的立即後續（Immediate Successor）。
\end{itemize}