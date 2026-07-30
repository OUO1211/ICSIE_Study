132
資料結構（含精選試題）
Data Structure

（a）鏈結堆疊

\section*{一．Linked Stack 的 Push 與 Pop}
（一）Push 動作
Procedure PUSH（Y）
Begin
New（I）；
I ↑ ．Data Y；
I↑．Link＝Top；
$\mathrm{Top}=\mathrm{I} ;$
END；
（二）Pop 動作
Procedure POP（Y）
Begin
if top＝nil then STACK＿EMPTY；
I＝Top；
$\mathrm{Y}=\mathrm{I} \uparrow$ ．Data；
Top $=\mathrm{I} \uparrow$. Link；
Ret（I）；
END；