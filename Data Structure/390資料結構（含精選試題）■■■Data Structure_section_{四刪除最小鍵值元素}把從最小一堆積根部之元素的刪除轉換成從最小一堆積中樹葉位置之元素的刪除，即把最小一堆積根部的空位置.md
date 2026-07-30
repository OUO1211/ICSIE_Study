390
資料結構（含精選試題）
■■■

Data Structure

\section*{四刪除最小鍵值元素}

把從最小一堆積根部之元素的刪除轉換成從最小一堆積中樹葉位置之元素的刪除，即把最小一堆積根部的空位置移到樹葉節點 p 。而此樹葉節點由雙堆積最後位置的元素 t 所填入。
例：把最後的元素鍵20的元素從雙堆積中移走。而刪除最小元素所產生的空位置2由兒子最小點來填補。每個移動的步驟是把目前節點的兒子中之較小元素上移。首先，8被上移。接著9移到它的父親上，然後比較20和它最大夥伴的鍵40。因為 $20<40$ ，所以不需交換，並且把20插入到以空位置為開始之 Min－Heap，結果如下圖。

Procedure DeapDeleteMin（var d：deap；var n：integer； var x：element）；
```
var i: integer;
    t : element;
begin
    if n<2 then DeapEmpty
    else begin
        x:=d[2];
        t:=d[n]; n:= n - 1
        i :=2;
        while i has a child do
        begin
            Let j be the child with smaller key;
        d[i] : = d[j];
```