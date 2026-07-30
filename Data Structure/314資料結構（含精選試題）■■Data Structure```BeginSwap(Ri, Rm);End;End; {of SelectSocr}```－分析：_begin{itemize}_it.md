314
資料結構（含精選試題）
■■

Data Structure
```
Begin
Swap(Ri, Rm);
End;
End; {of SelectSocr}
```

－分析：
\begin{itemize}
\item[1．] 其 Best、Average、Worst Case 的 Time Complexity 為 $O\left(n^2\right)$
因 Comparsion 次數要 ：
$$
\begin{aligned}
& (n-2+1)+(n-3+1)+\cdots 1 \\
& =(n-1)+(n-2)+\cdots 1=[(n-1) \cdot(n)] \div 2
\end{aligned}
$$
\item[2．] 為一不穩定的排序（Unstable Sort）
\item[3．] 需要一個額外空間 For Swap，Space complexity：O（1）
例 ：3，2，3＋，1， 4 排序後→1，2，3＋，3， 4
\end{itemize}

\section*{三．氣泡排序（Bubble Sort）}

演算法 ：
```
Procedure BubbleSort(R, n)
Begin
for i=1 to (n-1) do begin
    f=0;
for j=1 to (n -i) do
    if R[j+1].key<R[j].key then [ swap(Rj, Rj+1);
            f=1;
        ]
if f=0 then exit // No swap: exit / /
end;
End; {of BubbleSort}
```

－分析：
\begin{itemize}
\item[1．] Best Cass：資料為已排序好的，共需 $n-1$ 次的比較，故 $0(n)$ 。
Worst Cass：資料以相反次序排列，共需 $[\mathrm{n}(\mathrm{n}-1)] / 2$ 次比較，故 $0\left(\mathrm{n}^2\right)$ 。 Average Cass ： $0\left(\mathrm{n}^2\right)$
\end{itemize}