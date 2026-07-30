第七章 搜尋與排序
313
Search＆Sort
\begin{itemize}
\begin{itemize}
\begin{itemize}
\begin{itemize}
\item[] End；
End；｛of While and Case\}
End；｛of Binsrch\}
\end{itemize}
\end{itemize}
\item[（2）] Procedure Insert（ $\mathrm{r}:$ record，list ：afile， $\mathrm{i}:$ integer） ；
Var j，m ：Integer；
Begin
Binsrch（list，j，i，r）
For m ：＝i Downto j Do Begin
list［m＋1］：＝list［m］；
End；｛of For\}
list［j］：＝r；
End；
\item[（3）] Procedure InSort
\item[2．] List Insert Sort
將（2）中的 Array改成 Link List，利用 Pointer 改變，可避免大量搬移資料的負擔。
\end{itemize}
\end{itemize}

\section*{二．選擇排序（Selection Sort）}

觀念：令在 n 個記錄 $\mathrm{R}_1, \mathrm{R}_2, \cdots, \mathrm{R}_{\mathrm{n}}$ ，其鍵值分別為 $\mathrm{K}_1, \mathrm{~K}_2, \cdots, \mathrm{~K}_{\mathrm{n}}$ 欲將這個 n 個記錄由小到大排列時，則需執行以下兩個步驟：
（一）在所有的記錄中挑選一個具有最小鍵值的記錄然後將此記錄與第 i 個位置對調。
\begin{itemize}
\item[（二）] 在剩餘的 n－i 個記錄中，再次挑選一個具有最小鍵值的記錄，i 值加1，然後將此記錄與第 i 個記錄位置對調，重覆進行步驟（二）直到 i＝n 為止。
\end{itemize}

演算法 ：
```
Procedure SelectSort(R, n)
Begin
    For i :=1 To n - 1 Do Begin
        m := i;
        For j = i+1 To n Do
            If kj < km then m : = j;
    End; {of For loop}
    If i< > m then
```