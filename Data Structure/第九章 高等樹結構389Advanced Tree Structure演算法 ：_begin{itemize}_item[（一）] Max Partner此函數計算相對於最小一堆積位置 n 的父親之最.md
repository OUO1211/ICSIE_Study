第九章 高等樹結構
389
Advanced Tree Structure

演算法 ：
\begin{itemize}
\item[（一）] Max Partner
此函數計算相對於最小一堆積位置 n 的父親之最大一堆積中的節點。可由：$\left(\mathrm{n}+2^{\left\lfloor\log _2\right\rfloor-1}\right) \operatorname{div} 2$ 而得。
\item[（二）] 程序 Insert Min 和 Inset Max 分別把元素插入指定的最小和最大一堆積中。可藉著從此位置分別通向根部的路徑來完成。根部位置為2或3。
Procedure DeapInsert（var d：deap；var n：integer；x：element）：
｛Insert x into the deap d of size n－1 \}
var i ：integer
begin
if $\mathrm{n}=$ MaxElements then DeapFull
else begin
$\mathrm{n}:=\mathrm{n}+1 ;$
if $\mathrm{n}=2$ thend［2］：$=\mathrm{x}$｛insertion into an initially empty deap\}
else case MaxHeap（n）of
true ：begin｛n is a position in the max－heap\}
i ：＝MinPartner（n）；
if x．key＜d［i］．key
then begin
$\mathrm{d}[\mathrm{n}]:=\mathrm{d}[\mathrm{i}] ;$
MinInsert（d，i，x）；
end
else MaxInsert（d，n，x）；
false ：begin｛n is a position in the min－heap\}
i ：＝MaxPartner（n）；
if x．key＞d［i］，key
then begin
$\mathrm{d}[\mathrm{n}]:=\mathrm{d}[\mathrm{i}] ;$
MaxInsert（d，i，x）；
end
else MinInsert（d，n，x）；
end；｛of case and if $\mathrm{n}=2$ \}
end；｛of in $\mathrm{n}=$ MaxElements\}
end；
\end{itemize}