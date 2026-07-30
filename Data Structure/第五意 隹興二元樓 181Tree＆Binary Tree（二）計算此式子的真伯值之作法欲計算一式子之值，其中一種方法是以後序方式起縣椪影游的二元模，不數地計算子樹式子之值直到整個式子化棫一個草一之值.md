第五意 隹興二元樓 181
Tree＆Binary Tree

（二）計算此式子的真伯值之作法
欲計算一式子之值，其中一種方法是以後序方式起縣椪影游的二元模，不數地計算子樹式子之值直到整個式子化棫一個草一之值，Data structure Mattur：假設二元樹中各篩點均包含四個欄位：

\begin{tabular}{|l|l|l|l|}
\hline LeftChild & data & value & Righ Chrild \\
\hline
\end{tabular}

其中，LeftChild ，data ，RightChild 之意義如航所進 • 而 value 是 Boolean 製製 •（三）演算法
```
    procedure PostOrderEval(tree : TreePointer)
    begin
        if tree <> nil then
            begin
                PostOrderEval(tree { LefiChild):
                PostOrderEval(tree ? RightChild):
                case tree ↑ data of
                    LogicalNOT:tree { value:=not tree } RightChild { value.
                    LogicalAND: tree { valuc:=tree } LeftChild } value and
                        tree | RightChild | values,
                    LogicalOR:tree { value:=tree } LeftChild } value or
                        tree | RightChild | value,
                    LogicalTRUE : tree { value : = true;
                LogicalFALSE : tree { .value : = false;
                end; {of case}
        end; {of if}
    end; {of PostOrderEval}
```


四．使用二元搜尋樹來排序資料
（一）將一組輸入資料，建立一個二元搜尋樹（Binary earch Tree），然後再使用中序追踥（LDR），便可得到由小到大之排序結果。
（二）建立二元搜尋樹的步驟
Step1：將第一個輸入資料當做二元樹的樹根。
Step 2：以後的輸入資料與樹根比較，若小於樹根則成為樹根的左子樹，若大於則成為右子樹，依此反覆執行下去。