382
資料結構（含精選試題）
＂

Data Structure
\begin{itemize}
\item[] －演算法
【程式】在最小－最大堆積中插入的程序
Procedure MinMaxInsert（var h：MinMaxHeap；var n ：integer；x ：element）； ｛Insert x into the min－max heap which presently has n elements\} Var p ：integer； Begin
```
if n= MaxElements then MinMaxFull
    else Begin
```

    $\mathrm{n}:=\mathrm{n}+1$;
    $\mathrm{p}:=\mathrm{n} \operatorname{div} 2 ; \quad\{\mathrm{p}$ is the parent of the new node $\}$
    if $\mathrm{p}=0$ then $\mathrm{h}[1]:=\mathrm{x}$ \{Insertion into an initially empty heap\}
        else Case level(p) of
        min : if x.key< h[p].key
            then Begin \{Follow min levels\}
                $\mathrm{h}[\mathrm{n}]:=\mathrm{h}[\mathrm{p}] ;$
                VerifyMin(h, p, x);
            End
            else VerifyMax(h,n,x); \{Follow max levels\}
        max : if x.key > h[p].key
            then Begin \{Follow max levels\}
                $\mathrm{h}[\mathrm{n}]:=\mathrm{h}[\mathrm{p}] ;$
                VerifyMax(h, p, x);
            End
\end{itemize}