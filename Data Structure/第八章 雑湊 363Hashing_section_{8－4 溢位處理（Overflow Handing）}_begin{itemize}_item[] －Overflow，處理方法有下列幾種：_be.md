第八章 雑湊 363
Hashing

\section*{8－4 溢位處理（Overflow Handing）}
\begin{itemize}
\item[] －Overflow，處理方法有下列幾種：
\begin{itemize}
\item[（一）] 線性探測（Linearing Probing）或線性開放定址（Linear Open Addressing），此法將散置空間位址視為環狀使用，當發生溢位時，則以線性方式從下一個位址繼續探測，若還有空餘的儲存區則將識別字存入，否則繼續往下，若搜尋完一個循環，尚未找到空餘的儲存區，則表示所有位置都已被填滿。
\end{itemize}
\end{itemize}

完整的演算法如下：
```
type identifier = packed array[1 ⋯ maxchar] of char;
        hashtable = array[1 = maxsize] of identifier;
```

procedure linsrch ( x : idenitfier; ht : bashtable; var j : integer;
            b : integer);
｛Search the hast table $\mathrm{ht}[0 \cdots \mathrm{~b}-1]$（each bucket has exactly $1 \mathrm{~s}!$ ot）using linear probing．If $\mathrm{h} \mathrm{t}[\mathrm{j}]=$ blankident then the j－th bucket is empty and x can be entered into the table．Otherwise $\mathrm{ht}[\mathrm{i}]=\mathrm{x}$ which is already in the table．F is the hash function．\}
```
var i : integer
begin
    i := f(x); j : = i;
    while {ht[j]<> x}and(ht[j]<> blankident) do
        begin
            j : = (j+1) mod b; {treat the table as circular}
            if j = i then {no empty slots}
                tablefull;
            end;
    end; {of linsrch}
```

\begin{itemize}
\item[] －缺點
當利用線性探測來解決溢位，識別字會有群聚現象（cluster），且相鄰群塊亦趨於連接在一起，因此增加不少搜尋時間。
\item[（二）] 二次方探測（Quadratic Probing）
線性探測很容易造成 Cluster，然後再繼續串連成更大的叢聚（Cluster）。因此利用二次方探測來加以改善。二次方探測中，當 $\mathrm{f}(\mathrm{x})$ 發生溢位時，則下一次探測的位址是 $\left(f(x)+i^2\right) \bmod b$ 與 $\left(f(x)-i^2\right) \bmod b$ ，其中 $1 \leq i \leq(b-1) / 2$ 。
\end{itemize}