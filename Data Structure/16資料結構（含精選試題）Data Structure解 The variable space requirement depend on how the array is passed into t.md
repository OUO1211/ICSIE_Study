16
資料結構（含精選試題）
Data Structure

解 The variable space requirement depend on how the array is passed into the function．
\begin{itemize}
\item[（1）] Call－by－value ：Entire array 被放到 temporary storage before function is executed．
$$
\rightarrow \mathrm{S}_{\text {sum }}(\mathrm{I})=\mathrm{S}_{\text {sum }}(\mathrm{n})=(\mathrm{n})
$$
\item[（2）] Call－by－address ：Passing the address of the first element of the array．
$$
\rightarrow \mathrm{S}_{\mathrm{sum}}(\mathrm{n})=0
$$
\end{itemize}

例題 1－14
float rsum（float list［ ］，int n）
｛
if(n!=0) return rsum(list, n-1)+list[n-1];
return list［0］；
\}
假設 integer 和 pointer 佔 2 個 Bytes of storage，而 float 則佔 4 個 Bytes 且 list［］採取 call－by－address 傳遞，求出 space complexity？

解 Recursive，compiler 要考慮 save 下列到 system stack
\begin{itemize}
\item[（1）] Parameters．
\item[（2）] Local variables．
\item[（3）] Return address for each recursive call．
則下表表此函數 calling 所須之 space
\end{itemize}

\begin{tabular}{|l|l|l|}
\hline Type & Name & Number of bytes \\
\hline Parameter＝float & List［］ & 2 \\
\hline Parameter＝integer & N & 2 \\
\hline Return address & & 2 \\
\hline
\end{tabular}
∴ Total per recursive call $=6$ bytes and has n recursive calls
$$
\text { ∴ space complexity }=\mathrm{O}(6 \mathrm{n})
$$
（二）Time Complexity
\begin{itemize}
\item[1．] $\mathrm{T}(\mathrm{P})$ taken by a program， P ，is the sum of its compile time and run（execution）time．
\item[2．] 通常我們只注重 Execution time，最好的方式是用 System clock to time the program，但太耗費 Cost。
\item[3．] 替代方法
Count the number of operations that program performs．
違是一個 Machine－Independent Estimate．
\end{itemize}