第七章 搜尋與排序
315

Search＆Sort
\begin{itemize}
\item[2．] 為一 Stable Sort（穩定排序）
\item[3．] Space complexity： $\mathrm{O}(1)$
\item[] 例：給予1，2，3，4，5由小到大排序
$$
\rightarrow \quad \mathrm{i}=1
$$
j 從 1 to n－ 1 do 比較（if $\mathrm{kj}+1<\mathrm{kj}$ ）
結果無一次成立，故 f 仍為 0 ，所以 exit
→只作 n－1次比較，但無任何 swap 故為 Best Cass →0（n）
\item[] 例：給予5，4，3，2，1电小到大排序
\item[] →要作比較（且有 swap 動作，所以 $\mathrm{kj}+1<\mathrm{kj}$ 均成立）
$$
\begin{aligned}
& (n-1)+(n-2)+\cdots 1=[(n-1)(n)] / 2 \text { 次 } \\
\rightarrow & \text { Worst Case } \rightarrow 0\left(n^2\right)
\end{aligned}
$$
\end{itemize}

\section*{7－3 高等排序技巧}

常見的有：（一）Quick Sort
\begin{itemize}
\item[（二）] Merge Sort
\item[（三）] Heap Sort
\end{itemize}

\section*{一．快速排序法（Quick Sort Method）}
\begin{itemize}
\item[（一）] Quick Sort 又稱為 Partition Exchange Sort，具有最佳的平均執行時間的排序方法。Quick Sort 是指在 n 個記錄中 $\mathrm{R}_1, \mathrm{R}_2, \cdots, \mathrm{R}_{\mathrm{n}}$ 的檔案，把鍵值 $\mathrm{K}_{\mathrm{i}}$ 的記錄放在 S（i）的位置上，則 $K_j \leq K_{s(i)}$ 當 $j<S(i)$ ，而當 $j>S(i)$ ，則 $k_j \geq K_{s(i)}$ ，經此放置後該檔案被分成兩個部份，即：
$$
\left(\mathrm{R}_1, \mathrm{R}_2, \cdots, \mathrm{R}_{\mathrm{s}(\mathrm{i})-1}\right) \mathrm{R}_{\mathrm{s}(\mathrm{i})} \quad\left(\mathrm{R}_{\mathrm{s}(\mathrm{i})}+1, \cdots, \mathrm{R}_{\mathrm{n}}\right)
$$
$R^{s(i)}$ 的位置固定，而其左右兩個檔案可分別再被快排序，此種排序方式最適宜以遞迴形式來描述。
\item[] 一補充：
與 Insert Sort 的不同，在於插入排序中，每次控制插入的鍵值 $\mathrm{K}_{\mathrm{i}}$ 是插入到已排序好的部份檔案 $\left(\mathrm{R}_1, \cdots, \mathrm{R}_{\mathrm{i}-1}\right)$ 中的正確位置，而快速排序法與插入排序法的差別乃是將 $\mathrm{K}_{\mathrm{i}}$ 腱放在整個檔案的正確位置。
\end{itemize}