156
資料結構（含精選試題）
```
    Data Structure
    qstack : array[1 ⋯stacksize] of listointer;
    pstack : array[1 ⋯stacksize] of listointer;
    labelstack : array[1 ⋯stacksize] of integer;
    returnlabel : integer;
    q : listpointer;
    z : listpointer;
begin
    stackpointer : = 0 {Initialize stacks}
1:
    q : = nil;
    if p<>nil then
begin
    new(q);
    q ↑ .tag : = p ↑ .tag;
    if not p ↑ .tag then q ↑ .data : = p ↑ .data
    else begin
            stackpointer : = stackpointer +1;
            if stackpointer> stacksize then stackfull;
        qstack[stackpointer] : = q;
        pstack[stackpointer] : = p;
        labelstack[stackpointer] : = 2;
        p : = p ↑ .dlik;
        goto 1;
            q ↑ .dlink := z;
        end; {of if not p ↑ .tag}
    stackpointer : = stackpointer+1;
    if stackpointer > stacksize then stackfull;
    qstack[stackpointer]: = q;
    pstack[stackpointer] : = p;
    labelstack[stackpointer] : = 3;
    p := p ↑ ,link;
```