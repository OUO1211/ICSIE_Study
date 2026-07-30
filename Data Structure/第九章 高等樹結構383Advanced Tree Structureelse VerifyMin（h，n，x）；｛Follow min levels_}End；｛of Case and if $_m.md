第九章 高等樹結構
383
Advanced Tree Structure

else VerifyMin（h，n，x）；｛Follow min levels\}
End；｛of Case and if $\mathrm{p}=0$ \}
End；｛of if $\mathrm{n}=$ MaxElements\}
End；｛of MinMaxInsert\}
【程式】VerifyMax
Procedure VerifyMax（var h：MinMaxheap；i：integer；x：element）；
｛Follow max nodes from the max node i to the root and insert x at proper place\}
Var gp ：integer；
Begin
$\mathrm{gp}:=\mathrm{i} \operatorname{div} 4 ;$ Grandparen of i \}
while $\mathrm{gp}<>0$ do
＠－if x．key＞h［gp］．key
then Begin｛Move h［gp］to h［p］\}
$$
\begin{aligned}
& \mathrm{h}[\mathrm{i}]:=\mathrm{h}[\mathrm{gp}] \\
& \mathrm{i}:=\mathrm{gp} \\
& \mathrm{gp}:=\mathrm{gp} \operatorname{div} 4 ; \\
& \text { End }
\end{aligned}
$$
else $\mathrm{gp}:=0 ; \quad\{\mathrm{x}$ is to be inserted into node i$\}$
$\mathrm{h}[\mathrm{i}]:=\mathrm{x}$ ；
End；｛of VerifyMax\}
若為 Verify Min，則將＠處改為 x．key＜h［gp］．key．

\section*{因 刪除最小鍵值元素}

最小鍵值元素，那麼此元素位於根部中。沿用上例將鍵7刪除，而在刪除之後，最小－最大堆積將剩下 11 個元素。它的形狀如下圖所示。鍵 12 的元素將重新被插入到堆積中，藉由從根部往樹葉檢視，尋找適當插入位置即可。