第四章 鏈結串列
139
Linked List
```
                    p:=p ↑ .link;
                    q ; = q ↑ link; {advance to next term}
                end;
            '<': begin
                    attach(q ↑ .coef, q ↑ .exp, d);
                    q ; = q ↑ .link; {noxt term of b}
                end;
            '>': begin
                    attach(p ↑ .coef, p ↑ .exp, d);
                    p:=p ↑ .link; {next term of a}
                end;
    end; {of case and while}
    while p<>nil do {copy rest of a}
        begin
            attach(p ↑ .coef, p ↑ .exp, d);
            p : = p ↑ .link;
        end;
    while q<>nil do {copy rest of b}
        begin
            attach(q ↑ .coef, q ↑ .exp, d);
            q := q ↑ .link;
        end;
    d ↑ .link : = nil; {last node}
    {delete extra initial node}
    p : = c,
    c : = c ↑ .link
    dispose(p);
End; {of padd}
```

\begin{itemize}
\item[] －時間複雑度 $0(m+n) \rightarrow m: a$ 多項式的項數
\item[] －比較次數最多 $n+m-1$ 次 $n: b$ 多項式的項數
\end{itemize}