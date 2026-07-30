第七章 搜尋與排序 323
Search＆Sort
```
End; {of While}
    {Merge remaining file of length < 2*1 }
If (i+1-1)<n Then Merge(x, y, j, i+1-1, n);
else
For : = i To n Do
    y[t] : =x[t];
```


End；｛of Mpass\}
\begin{itemize}
\item[（三）] 分析
\begin{itemize}
\item[1．] Best，Worst，Average Case 的 Time Complexity 為： $0(\mathrm{n} \log \mathrm{n})$
因為
$$
T(n)=\left\{\begin{array}{cc}
1 & , \text { 若 } n=1 \\
2 T(n / 2)+c n & , \text { 若 } n>1
\end{array}\right.
$$
\item[2．] 是 Stable 的 Sorting Method。
\item[3．] 需要 0（n）之額外空間。
\end{itemize}
\item[] 一補充：Recursive 的 Merge Sort 寫法
\begin{itemize}
\item[1．] 合併排序的遞迴形式
合併排序亦可利用遞回之特性來完成。在遞迴形式中，我們每次將欲排序之檔案概略地分成兩等份，分別為左邊部份檔與右邊部份檔。左、右部份檔案再遞迴地利用排序之方法排好順序後，再合併到一排好序的檔案。
\item[] 例：有一輸入檔為
$$
26,5,77,1,61,11,59,15,48,19
$$
令欲利用遞回形式的雙向合併排序法將之排序，若正在被排序之檔案是從1到 u，那麼所分割出來的兩個部份檔則為1到 $[(1+\mathrm{u}) / 2]$ 與 $[(1+\mathrm{u}) / 2]+1$ 。下圖為分割部份檔案及排序的過程。注意到，這裡所合併的部份檔案與Msort 所合併者不一樣。
\end{itemize}
\end{itemize}