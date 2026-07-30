394
資料結構（含精選試題）
■■

Data Structure

\section*{二．最小加權外部路徑長度的應用}
\begin{itemize}
\item[（一）] n＋1個行程（runs）的2路合併法的最好合併方式。
\item[（二）] 求出一組最佳碼（Optimal Set of Codes）來表示訊息 $\mathrm{M}_1, \mathrm{M}_2, \cdots, \mathrm{M}_{\mathrm{n}-1}$ ，此二元樹稱為解碼樹（Decode Tree）。
\end{itemize}

解碼樹是一二元樹其外部節點代表訊息。編碼位元組（Code Word）決定解碼樹中每個階層到達正確外部節點所需的分支。例如：0視為左分支，1為右分支，則下圖解碼樹的相對碼000，001，01和1分別代表訊息 $\mathrm{M}_1, \mathrm{M}_2 \mathrm{M}_3$ 和 $\mathrm{M}_4$ 。這些碼稱為Huffman 碼。解一個碼所需的成本隨碼的位元數目增加而增加。此數目等於從根部到相對外部節點的距離。如果 $\mathrm{q}_1$ 是 $\mathrm{M}_{\mathrm{i}}$ 被傳送的頻率，則預期的解碼時間為
$$
\sum_{1 \leq i \leq n+1} q_i d_i
$$
其中 $\mathrm{d}_{\mathrm{i}}$ 是從根部節點到訊息 $\mathrm{M}_{\mathrm{i}}$ 的外部節點的距離。預計解碼時間之最小值由最小外部路徑長度之解碼樹的編碼位元組來達成。
一個搜尋二元樹的最小加權外部路徑長度之方法。

\section*{－Huffman algo．D．Huffman 提出}

Procedure Huffman（var $\ell:$ ListPointer ；n ：integer）；
｛1 is a list to n single node binary trees as described above．\}
```
var t: TreePointer;
    i: integer;
begin
for i:= 1 to n - 1 do {loop n-1 times}
begin
```