138
資料結構（含精選試題）
Data Structure

\section*{二．多項式相加}
（一）
\begin{itemize}
\item[a]
$p \uparrow . \exp =q \uparrow . \exp$
\item[b]
c
\item[（二）]
\item[a]
$p \uparrow . \exp <q \uparrow . \exp$
\item[b]
c
\item[（三）]
$p \uparrow . \exp >q \uparrow . \exp$ $p \uparrow . \exp >q \uparrow . \exp$
\item[b]
c
\end{itemize}

\section*{【程式一】計算兩個多項式的和}

Procedure padd（a，b ：polypointer，Var c ：polypointer）；
｛ polynomiais a and b represented as singly linked lists are summed to form the new polynomial named c
Var $\mathrm{p}, \mathrm{q}, \mathrm{d}:$ polypointer；
$$
\mathbf{x}: \text { integer; }
$$

Begin
$$
\begin{aligned}
& \mathrm{p}:=\mathrm{a} ; \quad \mathrm{q}:=\mathrm{b} ; \quad\{\mathrm{p}, \mathrm{q} \text { point to next term of } \mathrm{a} \text { and } \mathrm{b}\} \\
& \text { new }(\mathrm{c}) ; \\
& \mathrm{d}:=\mathrm{c} ; \quad\{\text { Initial node for } \mathrm{c}, \text { returned later }\} \\
& \text { while }(\mathrm{p}<\text { nil }) \text { and }(\mathrm{q}>\text { nil }) \text { do } \\
& \text { case compare }(\mathrm{p} \uparrow . \exp , \mathrm{q} \uparrow . \exp ) \text { of } \\
& \quad \text { ' }=\text { ' : begin } \\
& \quad \mathrm{x}:=\mathrm{p} \uparrow . \text { coef }+\mathrm{q} \uparrow . \text { coef; } \\
& \quad \text { if } \mathrm{x}>\mathrm{o} \text { then attach }(\mathrm{x}, \mathrm{p} \uparrow . \exp , \mathrm{d}) ;
\end{aligned}
$$