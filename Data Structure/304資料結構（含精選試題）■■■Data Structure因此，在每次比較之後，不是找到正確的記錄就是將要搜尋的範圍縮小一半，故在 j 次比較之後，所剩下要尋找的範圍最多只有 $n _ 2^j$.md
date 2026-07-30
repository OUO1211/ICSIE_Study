304
資料結構（含精選試題）
■■■

Data Structure
因此，在每次比較之後，不是找到正確的記錄就是將要搜尋的範圍縮小一半，故在 j 次比較之後，所剩下要尋找的範圍最多只有 $n / 2^j$ 個記錄（n 為記錄個數）。因此，在最壞的情況下，此種搜尋法所需之比較次數是 $\left\lceil\log _2(\mathrm{n}+1)\right\rceil$ ，∴ time為 $\mathrm{O}(\log \mathrm{n})$ 。
\begin{itemize}
\item[3．] 程式如下所示：
Procedure BinSeach（f ：afile；var i ：integer；n，k ：integer）
Var done ：boolean；
$\ell, \mathrm{u}, \mathrm{m}:$ integer；
Begin
$\ell:=1 ; \mathrm{u}:=\mathrm{n} ; \mathrm{i}:=0 ;$ done $:=$ false；
while（（ $\ell<=\mathrm{u}$ ）and（not done））do Begin
$\mathrm{m}:=(\ell+\mathrm{u}) \operatorname{div} 2$ ；
case compare（k，f［m］．key）of
＇＞＇$: \ell:=\mathrm{m}+1 \quad$｛Look in upper half\}
＇＝＇：Begin
$\mathrm{i}:=\mathrm{m} ;$ done $:=$ true $;$
End；
＇＜＇：u ：＝m－1；｛Look in lower half\}
end；｛of case\}
End；｛of while\}
End；｛of BinSearch\}
\item[4．] Decision tree of Binary Search
假設共有31個記錄，則 Binary Search 的步驟可利用如下圖之決策樹表示。在二元樹中從樹根到節點的路徑代表 BinSearch 尋找 k 的比較順序，而從二元樹的深度，可以知道比較的次數絕不會超過 O（ $\log _2 n$ ）。
\end{itemize}