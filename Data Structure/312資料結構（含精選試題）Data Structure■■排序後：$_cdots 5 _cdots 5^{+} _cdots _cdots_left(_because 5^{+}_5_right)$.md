312
資料結構（含精選試題）

Data Structure

■■

排序後：$\cdots 5 \cdots 5^{+} \cdots \cdots\left(\because 5^{+}<5\right)$
\begin{itemize}
\item[4．] Space Complexity：O（1）。僅須固定空間，一為 Dummy Record，一為 r 變數。［變形］
\begin{itemize}
\item[（1）] Binary Insertion Sort
觀念：因 Insertion Sort 方法的工作步驟是
\begin{itemize}
\item[（1）] 找到要插入的正確位置；然後
\item[（2）] 插入。
\end{itemize}
\end{itemize}
\end{itemize}
若找到欲插入的位置是在 $\mathrm{R}_{\mathrm{i}}$ 與 $\mathrm{R}_{\mathrm{i}+1}$ 之間，那 $\mathrm{R}_{\mathrm{i}=1}, \cdots, \mathrm{R}_{\mathrm{i}=2}, \cdots, \mathrm{R}_0$ 的記錄就要往後移到 $R_i+2, \cdots, R_{n+1}$ 等位置。
而（1）的 Search 方式，可改為二分搜尋或者費氏搜尋，應用到此插入搜尋當中。演算法：三個副程式
（1）Procedure Binsrch（f ：afile；i ：Integer；n，k ：Integer）；
$\{$ 當 $\mathrm{f}[\mathrm{i}-1]$ ．key $\leq \mathrm{k}<\mathrm{f}[\mathrm{i}]$ ．key 時，傳回 i 值。\}
Var done ：Boolean；
l, u, m : Integer;
Begin
$$
\begin{aligned}
& \ell:=1 ; \mathrm{u}:=\mathrm{n} ; \text { done }:=\text { false; } \\
& \text { While }((\ell<=\mathrm{u}) \text { and (not done)) Do Begin } \\
& \qquad \mathrm{m}:=(\ell+\mathrm{u}) \operatorname{div} 2 ; \\
& \text { Case compare ( } \mathrm{k}, \mathrm{f}[\mathrm{~m}] . \text { key ) of }
\end{aligned}
$$
$$
\begin{aligned}
\prime>' & \text { Begin } \\
& \ell:=\mathrm{m}+1 ; \\
& i:=1 ;
\end{aligned}
$$
End；
'=' : Begin
$$
\begin{aligned}
& \mathrm{i}=\mathrm{m}+1 \\
& \text { done }:=\text { true }
\end{aligned}
$$
End；
'<': Begin
$$
\begin{aligned}
& \mathrm{u}:=\mathrm{m}-1 \\
& \mathrm{i}:=\mathrm{m}
\end{aligned}
$$