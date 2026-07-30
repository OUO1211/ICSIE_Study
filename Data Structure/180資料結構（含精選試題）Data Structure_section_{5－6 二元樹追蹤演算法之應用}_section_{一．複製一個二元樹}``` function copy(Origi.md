180
資料結構（含精選試題）
Data Structure

\section*{5－6 二元樹追蹤演算法之應用}

\section*{一．複製一個二元樹}
```
    function copy(Original : TreePointer) : TreePonter;
    var TempTree : TreePointer;
    begin
    if Original < > nil then
        begin
            new(Temp);
            Temp ↑ .LeftChild:=copy(Original ↑ .LeftChild);
            Temp ↑ .RightChild:=copy(Original ↑ .RightChild);
            Temp ↑ .data : = Original ↑ .Data;
            copy:= Temp; {相當 return Temp;}
            end;
    else copy:=nil; {相當於 return nil}
end; {of copy}
```


\section*{二．決定二元樹是否相等（equal）}
```
function equal(First, Second : TreePointer) : Boolean;
begin
    equal : = false; {Initialize answer}
    if ((First = nil) and (Second = nil)) then
        equal : = true;
    else
    if ((First <> nil) and (Second <>nil)) then
        if First ↑ .data = Second ↑ .data then
            if equal (First ↑ .LeftChild, Scond ↑ .LeftChild)
                then
            equal:=equal(First ↑ .RightChild,Second ↑ .RightChild)
    end; {of equal}
```


\section*{三．運算式之計算}
（一）考慮一式子，如下：
$$
\mathrm{x}_1 \Lambda \neg \mathrm{x}_2 \mathrm{~V} \neg \mathrm{x}_1 \Lambda \mathrm{x}_3 \mathrm{~V} \neg \mathrm{x}_3
$$