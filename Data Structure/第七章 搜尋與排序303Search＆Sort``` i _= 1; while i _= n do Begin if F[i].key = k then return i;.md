第七章 搜尋與排序
303
Search＆Sort
```
    i := 1;
    while i <= n do Begin
        if F[i].key = k then return i;
            i := i+1
    End; {of while}
    return  0;
    End. {of Non_Sentinel}
```

\begin{itemize}
\item[（2）] Sentinel Sequential Seaching
Procedure Sentinel（f：afile；var i：integer；n，k：integer）
｛ Search a file f with key values f［1］．key，⋯，f［n］．key for a record such that $\mathrm{f}[\mathrm{i}]$ ．key $=\mathrm{k}$ ．If there is no such record， i is set to 0. \}
Begin
```
f[0].key := k;
i : = n;
while f[i].key < > k do
    i := i -1 ;
    return i
End. {of Sentinel}
```

作法：引入一個虛記錄 f［0］，其鍵 f［0］．key＝k 以簡化搜尋的程序。這樣在While 迴圈中就可以省略測試檔案是否結束。當 n 很大時，可以節省約50％的時間。
\item[5．] 搜尋成功的平均比較次數是：
$$
\begin{aligned}
& \Sigma_{1 \leq i \leq n}(n-i+1) / n=(n+1) / 2 \\
& \text { Time Complexity }=0(n)
\end{aligned}
$$
\item[（二）] 二元搜尋法（Binary Search）
\item[1．] 被搜尋的檔案須事先經過排序。
\item[2．] 首先比較中間的記錄而不像循序搜尋從檔案的一端開始找起。由於欲搜尋之檔案的記錄是按照鍵值從小到大排列，那麼在與中間的記錄（鍵值為 f［m］．key）比較之後，則依比較結果決定往後的動作：
\begin{itemize}
\item[（1）] 若 k＜f［m］．key，且欲搜尋之記錄存在的話，必然在檔案的前半段。
\item[（2）] 若 $\mathrm{k}=\mathrm{f}[\mathrm{m}]$ ．key，那該中間記錄即為所求。
\item[（3）] 若 $\mathrm{k}>\mathrm{f}[\mathrm{m}] . \mathrm{key}$ ，且欲搜尋之記錄存在的話，必然在檔案的後半段。
\end{itemize}
\end{itemize}