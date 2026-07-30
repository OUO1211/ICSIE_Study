第六章 圖形 261
Graph
```
        Begin
            adlist[i]. count : = top;
            top : = i;
        End;
    i : = 1;
    done : = false;
    while ((i <= n ) and not done) do
Begin {Print the vertices in topological order}
    if top = 0 then
        Begin
            writeln('Network has a cycle');
            done : = true;
        End
    else
        j : = top;
        top : = adlist[top]. count; {Unstack a vertex}
        writeln(j);
        ptr : = adlist[j]. link;
        while ptr <> nil do
            Begin {Decrease the count of successor vertices of j,
                k : = ptr ↑ .vertex, {k is a successor of j}
                adlist[k]. count := adlist[k].count-1; {Decrease count}
                if adlist[k].count = 0 then {Add vertex k to setck}
                    Begin
                        adlist[k]. count : = top;
                        top := k;
                End; {of if}
                ptr := ptr ↑ .link;
            End; {of while ptr <> nil}
            i : = i+1;
    End; {of while (i <= n ) and no done}
End; {of Topolical_Order}
```