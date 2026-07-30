332
資料結構（含精選試題）
■■

Data Structure
```
    i, j, p, t : Integer;
    k : 0 | kr;
Begin
    For i := 1 To n Do {Link into a chain staring at p}
    r[i].link := i + 1;
    r[n].link :=0; p -1;
For i : = d Downto 1 Do {Sort on key[i]}
Begin
    For j:=0 To rminusl Do {Initialize bins to be empty queue}
        f[j] := 0;
    While p<>0 Do {Put records into queue}
    Begin
        k := r[p] ↑ .key[i];
        if f[k] = 0 Then f[k] : = p
            else re[e[k]] ↑ .link := p;
        e[k] := p;
        p:=r[p]↑ .link; {Get next record}
    End; {of While}
    j := 0;
    While f[j]=0 D
        j := j+1; {Find first nonempty queue}
        p := f[j];
        t:=e[j];
    For k :=j+1 To rminusl Do {Concatenate remaining queues}
        If f[k]<> 0 Then
            Begin
                r[t] ↑ .link : = f[k];
                t:= e[k];
            End; {of If and For}
                r[t] ↑ .link : =0;
    End; {of for}
End; {of RaixSort}
```