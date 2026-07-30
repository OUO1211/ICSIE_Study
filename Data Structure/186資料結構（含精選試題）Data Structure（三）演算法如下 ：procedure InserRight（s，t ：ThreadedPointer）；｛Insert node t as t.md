186
資料結構（含精選試題）
Data Structure
（三）演算法如下 ：
procedure InserRight（s，t ：ThreadedPointer）；
｛Insert node t as the right child of s in a Theraded binary tree．\}
var temp ：ThreadedPointer；
begin
$$
\begin{array}{ll}
\mathrm{t} \uparrow . \text { RightChild } & :=\mathrm{s} \uparrow . \text { RightChild; } \\
\mathrm{t} \uparrow . \text { RightThreaded } & :=\mathrm{s} \uparrow . \text { RightThread; } \\
\mathrm{t} \uparrow . \text { LeftChild } & :=\mathrm{s} ; \\
\mathrm{t} \uparrow . \text { LeftThread } & :=\text { true; } \\
\mathrm{s} \uparrow . \text { RightChild } & :=\mathrm{t} ; \\
\mathrm{s} \uparrow . \text { RightThread } & :=\text { false; } \\
\text { if not } \mathrm{t} \uparrow . \text { RightThread then } & \{\mathrm{s} \text { had a right child }\} \\
\quad \text { begin } & \\
\quad \text { temp }:=\text { insuc }(\mathrm{t}) ; & \\
\quad \text { temp } \uparrow . \text { LeftChild }:=\mathrm{t} ; & \\
\quad \text { end; } & \\
\text { end; } &
\end{array}
$$

練習
播入 t 節點到 s 的左兒子之處