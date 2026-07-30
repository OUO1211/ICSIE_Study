第七章 搜尋與排序 317
Search＆Sort
```
        i := m; j :=n+1; k := list[m].key;
        Repeat
            Repeat
                i : = i+1;
            Until list[i].key \( 2 \)
            Repeat
                j : = j -1 ;
            Until list[j].key <=k ;
            If i<j Then interchange (list[i], list[j]);
        Until i>=j;
        interchange(list[m], list[j]);
        Qsort(list, m, j-1);
        Qsort(list, j+1, n);
        End; {of If}
    End; {of Qsort}
```

\begin{itemize}
\item[（三）] Quick sort 之分析
\begin{itemize}
\item[1．] Best Case 下，Time Complexity 為 $0\left(\mathrm{n} \log _2 \mathrm{n}\right)$
每次當 control key 記錄放到正確位置時所分割出來的兩個左右部份檔案大小相等，那每次就可以將原來要排序之檔案分割成兩個大小約為原來一半的部份檔案。在一大小為 n 的檔案中欲將一個記錄放在正確之位置所需之時間是 0 （n）。如果 $\mathrm{T}(\mathrm{n})$ 表示將 n 個記錄排好序所需之時間，那麼當每次排好一個記錄都把原來檔案分割成大約相等的兩半時，則時間函數如下：
$$
\begin{aligned}
T(n) & \leq \mathrm{cn}+2 \mathrm{~T}(n / 2) \quad, \quad \mathrm{c} \text { 為常數 } \\
& \leq \mathrm{cn}+2(\mathrm{cn} / 2+2 \mathrm{t}(n / 4)) \\
& \leq 2 \mathrm{cn}+4 \mathrm{~T}(n / 4)) \\
& \quad: \\
& \quad: \\
& \leq \mathrm{cn} \log _2 \mathrm{n}+\mathrm{nT}(1) \\
& =0\left(\mathrm{n} \log _2 \mathrm{n}\right)
\end{aligned}
$$
\end{itemize}
\item[2．] Worst Case下，Time Complexity 為 $0\left(\mathrm{n}^2\right)$
當資料是由小而大或由大而小排列時，為最壞的情況，所選擇的基準 key，不
\end{itemize}