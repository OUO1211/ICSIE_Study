260
資料結構（含精選試題）
■■■

Data Structure
\begin{itemize}
\item[五．] AOV 網路的資料結構表示
\begin{itemize}
\item[（一）] 設計想法
在求 Topological order 問題裡的運算有：
\begin{itemize}
\item[1．] 決定一個頂點是否有前導。
\item[2．] 去掉一個頂點及其相連之邊。
\end{itemize}
\end{itemize}
\end{itemize}
如果對每個頂點，都記錄一個其立即前導個數之計數，則1．可以很有效率的做到；如果網路是用相鄰串列來表示，則2．可以很容易的做到。因此，要把所有一個頂點 v 所出來的邊都去掉，則把其相鄰串列上所有頂點之前導計數都減1。當某個頂點的前導計數減至零時，該頂點就可輸出。
假設網路是用相鄰串列來表示的，這些串列的開頭節點有兩個欄：cout 及 link。count 欄存放該頂點的入支度，link 是一個指標，指到該相鄰串列上之第一個節點。每一個串列節點有兩個欄：vertex 及 link。
（二）程式：
Procedure Topological＿Order（var adlist：adjacencylists；n：integer）；
｛The n vertices of an AOV－Network are listed in topological order．The network is represented as a set of adjacency lists with adlist［i］．count＝the in－degree of vertex i．\}
```
var i, j, k, top : integer;
        ptr : nextnode
        done : Boolean;
Begin
    top :=0; {Initialize stack}
    for i : = 1 to n do {Create a linked stack of vertices with}
        if adlist[i]. count = 0 then {No predecessors}
```