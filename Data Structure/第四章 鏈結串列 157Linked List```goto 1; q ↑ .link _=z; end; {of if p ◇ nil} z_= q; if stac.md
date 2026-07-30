第四章 鏈結串列 157
Linked List
```
goto 1;
        q ↑ .link :=z;
    end; {of if p ◇ nil}
    z:= q;
    if stackpointer <> 0 then
    begin {Simulate an end of function}
        q := qstack[stackpointer];
        p : = pstack[stackpointer];
        retrunlabel : = labelstack[stackpointer];
        stackpointer : = stackpointer -1;
        case returnlabel of
            2: goto 2;
            3: goto 3;
            end; {for case}
            end; {of if stackpointer <> 0}
        copy:=z;
    end; {of copy}
```