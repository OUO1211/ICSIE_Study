第四章 鏈結串列 133
Linked List

\section*{二．Linked Queue 的 Add 與 Delete 動作}
（一）Add 動作
Procedure AddQ（Y，front，rear）
Begin
New（I）；
I ↑ ． Data $=\mathrm{Y}$ ；
I ↑ ．Link＝nil；
if rear＝nil then front＝rear＝I；
else Begin
Rear ↑ ．Link＝I；
Rear＝I，
End；
End；
（二）Delete 動作
Procedure DeleteQ（Y，front，rear）
Begin
if front＝nil then QUEUE＿EMPTY
else Begin
$\mathrm{I}=$ Front；
Front $=\mathrm{I} \uparrow$ ．Link；
$\mathrm{Y}=\mathrm{I} \uparrow$ ．Data；
Ret（I）；
End；
if front＝nil then rear＝nil；
End；