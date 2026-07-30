第四章 鏈結串列
143

Linked List

End；
return（i）；
End Length
二．Concatenate two link list into one list
將兩個鏈結串列連結成一個串列。

【程式】Procedure Concatenate（x，y，z）｛x，y，z 為 single link list\}
begin
case $1: \mathrm{x}=0: \mathrm{z}=\mathrm{y}$
case $2: y=0: z=x$
case 3 ：else ： $\mathrm{p}=\mathrm{x} ; \mathrm{z}=\mathrm{x}$ ；
while $\mathrm{P} \uparrow$ ．Link $\neq$ nil do
$\mathrm{P}=\mathrm{P} \uparrow$ ．Link；
$\mathrm{P} \uparrow$. Link $=\mathrm{y}$ ；
end．
三．Invert a link list
提示：利用 r，q，p 三個指標即可達成目的。

【程式】 Procedure Invert（ x ）｛ x 為 single link list\}
begin
$$
\mathrm{p}=\mathrm{x} ; \mathrm{q}=\mathrm{nil} ;
$$
while $p \neq$ nil do begin
$$
\begin{aligned}
& \mathrm{r}=\mathrm{q} \\
& \mathrm{q}=\mathrm{p} \\
& \mathrm{P}=\mathrm{P} \uparrow . \text { Link; }
\end{aligned}
$$