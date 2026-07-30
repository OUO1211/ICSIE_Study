第七章 搜尋與排序 321
Search＆Sort

【程式】合併兩個已排序的檔案
Procedure Merge（Var x，z ：afile，1，m，n ：Integer）；
$\{(\mathrm{x}[1], \cdots, \mathrm{x}[\mathrm{m}])$ and $(\mathrm{x}[\mathrm{m}+1], \cdots, \mathrm{x}[\mathrm{n}])$ are two sorted lists with keys such that $\mathrm{x}[1]$ ．key $\leq \cdots \leq \mathrm{x}[\mathrm{m}]$ ．key，and $\mathrm{x}[\mathrm{m}+1]$ ．key $\leq \cdots \leq \mathrm{x}[\mathrm{n}]$ ．key．These records are merged to obtain the sorted list $(\mathrm{z}[1], \cdots, \mathrm{z}[\mathrm{n}])$ such that $\mathrm{z}[1]$ ．key $\leq \cdots \leq \mathrm{z}[\mathrm{n}]$ ．key $\}$
Var i，j，k，t ：Integer；
Begin
```
i :=1;
k :=1;
j :=m+1; {i, j and k are positions in the three files}
```

While $((\mathrm{i}<=\mathrm{m})$ and $(\mathrm{j}<=\mathrm{n}))$ Do Begin
If $\mathrm{x}[\mathrm{i}]$.key $<=\mathrm{x}[\mathrm{j}]$.key Then
    begin
        $\mathrm{z}[\mathrm{k}]:=\mathrm{x}[\mathrm{ii}] ;$
        $\mathrm{i}:=\mathrm{i}+1$;
    end;
    else begin
        $\mathrm{z}[\mathrm{k}]:=\mathrm{x}[1] ;$
        $\mathrm{j}:=\mathrm{j}+1$;
        end;
        $\mathrm{k}:=\mathrm{k}+1$;
    End; \{of While\}
    If $\mathrm{i}>\mathrm{m} \quad$ Then $\quad\left\{\left(\mathrm{z}_{\mathrm{k}}, \cdots, \mathrm{z}_{\mathrm{n}}\right):=\left(\mathrm{x}_{\mathrm{j}}, \cdots, \mathrm{x}_{\mathrm{n}}\right)\right\}$
            For $\mathrm{t}:=\mathrm{j}$ To n Do
            $\mathrm{z}[\mathrm{k}+\mathrm{t}-\mathrm{j}]:=\mathrm{x}[\mathrm{t}] ;$
            $\left\{\left(\mathrm{z}_{\mathrm{k}}, \cdots, \mathrm{k}_{\mathrm{n}}\right):=\left(\mathrm{x}_{\mathrm{i}}, \cdots, \mathrm{x}_{\mathrm{n}}\right)\right\}$
        else
            For $\mathrm{t}:=\mathrm{i}$ To m Do
            $\mathrm{z}[\mathrm{k}+\mathrm{t}-\mathrm{j}]:=\mathrm{x}[\mathrm{t}] ;$
End; \{of Merge\}
\begin{itemize}
\item[] －有兩種版本的 Merge Sort 法
\begin{itemize}
\item[1．] Interative
\item[2．] Recursive
\end{itemize}
\end{itemize}