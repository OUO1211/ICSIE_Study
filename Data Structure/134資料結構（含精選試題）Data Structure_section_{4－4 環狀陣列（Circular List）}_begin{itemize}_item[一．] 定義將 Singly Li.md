134
資料結構（含精選試題）
Data Structure

\section*{4－4 環狀陣列（Circular List）}
\begin{itemize}
\item[一．] 定義
將 Singly Linked List 的最後一個 Node 的指標指回第一個 Node。
\end{itemize}

二．特色
\begin{itemize}
\begin{itemize}
\item[（一）] 不論以那一節點開始找尋，必定能夠經過串列中所有節點。
\item[（二）] 回收整個串列所需的時間是固定的，只需改變兩個指標，與串列的長度無關，其Time Complexity 是 $0(1)$ 。
【註】Single Linked List 與串列的長度有關，是 0（n）。
\item[] 【圖示】清除環狀串列的情形，虛線為改變後之結果

（1）
\end{itemize}
\end{itemize}

三．清除 Circular List 的程式
Procedure CirErase（ var t ：polypointer）；
```
var x : polypointer;
Begin
    if t<> nil then
        Begin
            x : = t ↑ .link { Second node }
            t ↑ .link : = av; { first node linked to av }
            av : =x; { Second node of t becomes front of av list }
            t : = nil;
        End;
    End;
```