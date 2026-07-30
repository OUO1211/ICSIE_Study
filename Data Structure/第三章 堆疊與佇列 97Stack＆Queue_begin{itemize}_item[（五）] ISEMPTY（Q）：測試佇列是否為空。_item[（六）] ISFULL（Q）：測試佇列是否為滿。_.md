第三章 堆疊與佇列 97
Stack＆Queue
\begin{itemize}
\item[（五）] ISEMPTY（Q）：測試佇列是否為空。
\item[（六）] ISFULL（Q）：測試佇列是否為滿。
\end{itemize}

\section*{三．製作方式}

可利用 Array 或 Link List 製作，在此先討論 Array 之製作方式。其用 Array 製作有下列三種方式。

【方法1】用一維陣列 $\mathrm{q}[1 \cdots \mathrm{n}]$ ，及兩個變數 front 及 rear，則
\begin{itemize}
\item[（一）] Create Q（q）
var q ：array［1．．n］of items；
front $:=0$ ，rear $:=0 \quad / /$ 初值設定
\item[（二）] ISEMPTYQ（q）
if front＝rear then return true；
else return false；
\item[（三）] FRONT（q）
if ISEMPTY（q）then error；
else return q［front＋1］；
\item[（四）] ADDQ（item，q）／／加入 item 到 q 中
BEGIN
if rear＝n then queuefull；
else
BEGIN
rear ：＝rear＋1；
q［rear］：＝item；
END；
END；
\item[（五）] DELETE（q）
BEGIN
if front＝rear then queue empty
else
BEGIN
front ：＝front＋1；
item ：＝q［front］；
\end{itemize}