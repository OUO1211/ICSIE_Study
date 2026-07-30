146
資料結構（含精選試題）
Data Structure

Procedure equivalence；
｛ input the equivalence pairs and output the equivalence
classes\}
type pointer＝inode；
node＝record
data ：1．．n；
link ：pointer；
end；
var seq ：array［1．．n］of pointer；
out ：array［1．．n］of voolean；
i，j ：integer；
x，y，top ：pointer；
done ：boolean；
Begin
｛initialize seq and out\}
for $\mathrm{i}:=1$ to n do Begin
seq［i］：－nil；
out［i］：－true；
End；
｛Phase 1 ：input equivalence pairs\}
while not eof（input）do Begin
readln（i，j）；
new（x）；｛add j to list seq［i］\}
$\mathrm{x} \uparrow$ ．data ：＝j；
$\mathrm{x} \uparrow$ ．link ：＝seq［i］；
seq［i］：－X ；
new（x）；｛add I to list seq［j］\}
$\mathrm{x} \uparrow$ ．data $:=\mathrm{i}$ ；
$\mathrm{x} \uparrow$. link $:=\operatorname{seq}[\mathrm{j}] ;$
seq［j］：＝x；
End；
｛Phase 2：output the equivalence classes\}
for $\mathrm{i}:=1$ to n do