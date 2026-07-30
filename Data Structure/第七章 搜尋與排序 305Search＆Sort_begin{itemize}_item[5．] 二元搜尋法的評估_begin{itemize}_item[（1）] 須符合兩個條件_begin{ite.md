第七章 搜尋與排序 305
Search＆Sort
\begin{itemize}
\item[5．] 二元搜尋法的評估
\begin{itemize}
\item[（1）] 須符合兩個條件
\begin{itemize}
\item[] ①檔案中的記錄必須事先經過排序。
\item[] ②檔案必須是可以 Direct Access File 或 Random File
\end{itemize}
\item[（2）] Time Complexity
$$
\begin{aligned}
& \because \mathrm{T}(\mathrm{n})=\mathrm{T}\left(\frac{\mathrm{n}}{2}\right)+1, \mathrm{~T}(1)=1 \\
& \therefore \mathrm{~T}(\mathrm{n})=\mathrm{O}\left(\log _2 \mathrm{n}\right)
\end{aligned}
$$
\item[（3）] 一般而言，n 值小時較適合 Sequential Search n 值大時較適合 Binary Search
\end{itemize}
\item[（三）] 費氏搜尋（Fibonacci Search）
\item[1．] 費氏數列
$$
\begin{aligned}
& \mathrm{F}_0=0 \quad, \quad \mathrm{~F}_1=1 \\
& \mathrm{~F}_{\mathrm{i}}=\mathrm{F}_{\mathrm{i}-1}+\mathrm{F}_{\mathrm{i}-2}, \mathrm{i} \geq 2 \\
& 0,1,1,2,3,5,8,13,21,34,55, \cdots
\end{aligned}
$$
\item[2．] 好處
費氏搜尋法只需用到加法與減法。而不需像二元搜尋法應用到除法。因此對於計算除法比加法費時很多的計算機而言，費氏搜尋法要比二元搜尋法來得好。
\item[3．] 流程
假記錄個數是某一個費氏數減 1 ，即 $\mathrm{n}=\mathrm{F}_{\mathrm{a}}-1$ 時，那在費氏搜尋法中，我們首先拿 k 與 f［ $\mathrm{F}_{\mathrm{a}-1}$ ］．key 相比：
\begin{itemize}
\item[（1）] 若 $\mathrm{k}<\mathrm{f}\left[\mathrm{F}_{\mathrm{a}-1}\right]$ ．key
那搜尋的範圍縮減成1到 $\mathrm{F}_{\mathrm{a}-1}-1$ ，而剩餘之記錄個數仍是某一個費氏數
\end{itemize}
\end{itemize}