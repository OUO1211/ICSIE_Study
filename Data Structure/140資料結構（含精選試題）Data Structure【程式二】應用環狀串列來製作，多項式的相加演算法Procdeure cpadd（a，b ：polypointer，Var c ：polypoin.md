140
資料結構（含精選試題）
Data Structure

【程式二】應用環狀串列來製作，多項式的相加演算法
Procdeure cpadd（a，b ：polypointer，Var c ：polypointer）；
｛ Polynomials a and b are represented as circular
lists with head nodes so that $\mathrm{a} \uparrow . \exp =\mathrm{b} \uparrow . \exp$
$=-1$ ．Their sum， c ，is returned as a circular list．\}
Var $\mathrm{p}, \mathrm{q}, \mathrm{d}:$ polypointer；
x ：integer；
done ：booleann；
Begin
$\mathrm{p}:=\mathrm{a} \uparrow$ ．link；
$\mathrm{q}:=\mathrm{b} \uparrow$ ．link；
getnode（c）；
c ↑ ．exp ：＝－1；｛head node for c\}
$\mathrm{d}:=\mathrm{c} ; \quad\{$ last node in c$\}$
done ：＝false；
repeat
case compare（p ↑ ．exp，q ↑ ．exp）of
＇＝＇：if p＝a then done ：＝true else
else begin
$\mathrm{x}:=\mathrm{p} \uparrow$ ．coef＋q ↑ ．coef；
if $\mathrm{x}<>0$ then attach（x，p ↑ ．exp，d）；
$\mathrm{p}:=\mathrm{p} \uparrow$ ．link；
$\mathrm{q}:=\mathrm{q} \uparrow$ ．link；
end；
＇＜＇：begin
attach（q ↑ ．coef，q ↑ ．exp，d）；
$\mathrm{q}:=\mathrm{q} \uparrow$ ．link；
end；
＇＞＇：begin
attach（p ↑ ．coef，p ↑ ．exp，d）；
$\mathbf{p}:=\mathbf{p} \uparrow$ ．link；
end；
end；｛of case\}
until done；
$\mathrm{d} \uparrow$ ．link ：$=\mathrm{c} ; \quad$｛link last node to first\}
End；｛of cpadd\}