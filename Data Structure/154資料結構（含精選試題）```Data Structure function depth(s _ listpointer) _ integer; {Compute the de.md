154
資料結構（含精選試題）
```
Data Structure
    function depth(s : listpointer) : integer;
        {Compute the depth of the nonrecursive list s}
    var p : listpointer;
        m, n : integer;
    BEGIN
        if s <>nil then
            Begin
                p:=s;
                m : = 0;
            while p <> nil do
                Begin
                    if P ↑ .tag then Begin
                        n : = depth(p ↑ .dlink);
```

```
                    End;
                p : = p ↑ .link;
                End;
                depth : = m+1;
            End;
        else depth : = 0;
    END; {of depth}
```


\section*{4－12 遞迴式演算法改成非遞迴式之作法}
\begin{itemize}
\item[（一）] 在程序上或函數開頭處插入一行宣告個堆疊（叫做遞迴堆疊）的指令，同時將堆疊初置為空的。在一般的情況，堆疊是用來儲存每一次遞迴呼叫時的區域性變數值、參數值、函數值及返迴位址（Return Address）等。我們也可以為每一種值分別使用獨立的堆疊。
\item[（二）] 在第一個可執行的敘述前加一個標記1。
\item[（三）] 如果這是一個函數，那麼把出現在指定敘述（Assignment Statement）左邊的所有函數名稱以一個新的變數（與函數具有同樣的型態）取代之，比如說 z。
\end{itemize}