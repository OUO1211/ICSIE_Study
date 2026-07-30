第四章 鏈結串列
153
Linked List
```
            else q ↑ .dlink : = copy(p ↑ .dlink);
            q ↑ .link : = copy(p ↑ .link);
        End;
    copy:=q;
END; {of copy}
```


\section*{二．決定兩串列是否相同}
－亦即決定兩串列是否具有相同之結構而且相對應欄均有相同之資料，其演算法如下：
```
        function equal(s, t : listpointer) : boolean;
            {s and t are nonrecursive lists. This function has value true if the two lists are
            identical.}
        var x : Boolean;
    BEGIN
        equal : = false;
        if (s=nil) and (t=nil) then
            equal : = true;
        else if (s<>nil) and (t<>nil)
                then if s ↑ .tag = t ↑ .tag
                then Begin
                        if not s ↑ .tag then
                            if s ↑ .data = t ↑ .data then x : = true;
                                else x := false;
                        else x : = equal(s ↑ .dlink, t ↑ dlink)
                        if x then equal : = equal(s ↑ .link, t ↑ .link)
                    End;
        END; {of equal}
```


\section*{三．計算串列的深度（Depth）}
\begin{itemize}
\item[] －串列深度的定義如下：
$$
\operatorname{depth}(\mathrm{s})=\left[\begin{array}{l}
0, \quad \text { 如果 } \mathrm{s} \text { 為空串列 } \\
1+\max \left\{\operatorname{depth}\left(\mathrm{x}_1\right), \cdots, \operatorname{depth}\left(\mathrm{x}_{\mathrm{n}}\right)\right\}, \text { 如果 } \mathrm{s} \text { 為串列 }\left(\mathrm{x}_1, \cdots, \mathrm{x}_{\mathrm{n}}\right), \mathrm{n} \geq 1
\end{array}\right.
$$
程序 depth 如下 ：
\end{itemize}