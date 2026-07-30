第七章 搜尋與排序 307
Search＆Sort
```
m : = n+1-(i+p);
if k>g[i].key {Set i so size of right subfile is P}
then i := i +m;
done := false;
while ((i <> 0) and (not done) do
case compare(k, g[i].key) of
' < ' : if q=0 then i :=0
else begin
i := i - q ;
t:=p;
p := q;
q := t -q ;
end
'>': if p=1 then i :=0
else begin
i : = i+q ;
p:=p-q;
q = q-p;
end
'=': done :=true; {found a match}
```


End；｛of case and while\}
End；｛of fibsrch\}
4．費氏搜尋的評估
\begin{itemize}
\item[（1）] 同二元搜尋法一般，須符合兩個條件：
\begin{itemize}
\item[] ①檔案中的記錄須事先排序過。
\item[（2）] 須是 Direct Access 或 Random access 機制支援。
\end{itemize}
\item[（2）] 優點：只有加減運算，不像二元搜尋法會用到除法運算。缺點是每次必須去求算下一個費氏數。
\item[（3）] Time Complexity 為 $0(\log \mathrm{n})$
在平均狀況下（Average Situation）費氏搜尋優於二元搜尋，而在最壞的狀況下，則遜於二元搜尋。
\end{itemize}