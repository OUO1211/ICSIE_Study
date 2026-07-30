第四章 鏈結串列 147
Linked List
```
        if out[i] then
            Begin {needs to be output}
                writeln('A new class:', i);
                out[i] : = false;
    x : = seq[i];
    top : = nil; {init stack}
    done : = false;
    repeat {find rest of class}
    while x >nil do {process the list}
    Begin
        j:=x ↑ .data;
        if out[j] then Begin
                    writeln(j);
                    out[j] : = false;
                    y:=x ↑ .link;
                    x ↑ .link : = top;
                    top :=x;
                    x : = y;
                End;
        else x : = x ↑ .link;
```

        End;
        if top = nil then done : = true
        else begin
                $\mathrm{x}:=\operatorname{seq}[\mathrm{top} \uparrow . \mathrm{data}] ;$
                top : = top ↑ .link; \{unstack\}
            end;
        until done;
    End; \{of if\}
End; \{of equivalence\}

\section*{四．Time Comlexity 分析}
\begin{itemize}
\item[（一）] seq 及 out 的初始設定需時 0（n）
\item[（二）] 第一階段的總時間為 0 （m）
\end{itemize}