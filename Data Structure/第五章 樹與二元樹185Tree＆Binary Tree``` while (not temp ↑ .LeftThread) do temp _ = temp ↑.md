第五章 樹與二元樹
185
Tree＆Binary Tree
```
        while (not temp ↑ .LeftThread) do
            temp : = temp ↑ .LeftChild;
        return temp;
    end; {of insuc}
```


\section*{六．引線二元樹的中序追蹤法}
\begin{itemize}
\item[（一）] 重複呼叫 Insuc 即可。
\begin{itemize}
\item[（二）] 其演算法如下 ：
```
procedure tinorder(tree TheadedPointer);
var temp : ThreadedPointer;
begin
    temp : = tree;
    repeat
        temp : = insuc(temp);
        if temp < tree then
            write(temp ↑ .data);
        until temp = tree;
end.
```

\end{itemize}
\item[七．] 引線二元樹的插入（Insert）
\item[（一）] 插入一節點 t 到某節點 s 的右兒子處。
\item[（二）] 考慮下列二種情況：
\begin{itemize}
\item[1．] 如果 s 的右兒子是空的，則 s 的 RightChild 指到 t，而 t 的左引線指到 s，右引線指到 s 先前右引線所指之 Node，如下圖所示：
\end{itemize}
\item[2．] 若 s 的右兒子存在，那麼該右子樹在 t 插人後就變成 t 的右子樹。當完成插入後，t 就變成某一個節點（Left Thread＝ture）之中序先行者，因此就要修正一引線以指到 t，而包含此引線之節點即為原來是 s 的中序後繼者。如下圖：
\end{itemize}