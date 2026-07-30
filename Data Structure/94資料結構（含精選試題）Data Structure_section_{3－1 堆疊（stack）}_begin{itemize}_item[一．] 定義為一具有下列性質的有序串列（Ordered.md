94
資料結構（含精選試題）
Data Structure

\section*{3－1 堆疊（stack）}
\begin{itemize}
\item[一．] 定義
為一具有下列性質的有序串列（Ordered List）：
\begin{itemize}
\item[（一）] 插入（Insertion）與刪除（Deletion）均發生在同一端，此端稱為頂端（Top）。
\item[（二）] 具（Last－In－First－Out，LIFO）的性質或（FILO；First－In－Last－Out）。
\item[（三）] 插入元素的動作稱為 Push，刪除元素的動作稱為 Pop。
\end{itemize}
\item[二．] Stack ADT 之 Operations
\begin{itemize}
\item[（一）] Create（s）：建立一個空的 Stack S。
\item[（二）] $\operatorname{Add}(\mathrm{i}, \mathrm{s})$ ：將元素 i 插入 Stack 頂端，並得到一個新內容的 Stack 。
\item[（三）] Delete（s）：移出堆疊的頂端元素，得到一個新內容的 Stack。
\item[（四）] Top（s）：傳回 Stack 頂端元素。
\item[（五）] IsEmpty（s）：測試 S 是否為 Empty Stack，若是則傳回 True；否則傳回 False。
\item[（六）] IsFull（s）：測試 S 是否為滿，若為是傳回 True 值，否則傳回 False。
\end{itemize}
\end{itemize}

\section*{三．製作方式}

製作方式可分為利用 Array 及利用 Link List，在此先討論利用 Array 的作法。宣一維陣列 S［1⋯n］，則 STACK ADT 之 operations 製作如下：
\begin{itemize}
\begin{itemize}
\item[（一）] Create（Stack）
```
    var stack : array[1 . . n] of items;
        top : 0 - ^n;
        top := 0; // Top 初值。
```

\item[（二）] IsEmpty（s）
```
    if Top = 0 then return True;
        else return False;
```

\item[（三）] Top（stack）
```
    if top = 0 then return error // 因為 Empty
        else return stack[top];
```

\end{itemize}
\end{itemize}
（四）Push（item，stack）
```
    BEGIN
        if top = n then "stackfull error"
```