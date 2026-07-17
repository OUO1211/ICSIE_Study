168
離散數學（上）

函數（function，mapping，transformation）
令 $f$ 為非空集合 $A$ 到 $B$ 上的一關係，且滿足：
對任意 $A$ 上的元素 $a$ ，均恰唯一存在 $B$ 中的某元素 $b$ ，使得 $f(a)=b$ ，
則稱 $f$ 為一種 $A$ 到 $B$ 的函数。
【107台大工科】
Note
（1）函數是一種加了限制的關係，但關係不一定是函數。

【91 清大資工】

（2）$A$ 稱為函數 $f$ 的定義域（domain），$B$ 稱為函數 $f$ 的對應域或陪域（co－domain）。
例如，Domain 為 $\{1,2\}$ ，Co－Domain 為 $\{a, b, c\}$ 的 function 有以下九種：
$$
\begin{aligned}
& \left\{\begin{array}{l}
f_1(1)=a \\
f_1(2)=a
\end{array} ;\left\{\begin{array}{l}
f_2(1)=a \\
f_2(2)=b
\end{array} ;\left\{\begin{array}{l}
f_3(1)=a \\
f_3(2)=c
\end{array} ;\right.\right.\right. \\
& \left\{\begin{array}{l}
f_4(1)=b \\
f_4(2)=a
\end{array} ;\left\{\begin{array}{l}
f_5(1)=b \\
f_5(2)=b
\end{array} ;\left\{\begin{array}{l}
f_6(1)=b \\
f_6(2)=c
\end{array} ;\right.\right.\right. \\
& \left\{\begin{array}{l}
f_7(1)=c \\
f_7(2)=a
\end{array} ;\left\{\begin{array}{l}
f_8(1)=c \\
f_8(2)=b
\end{array} ;\left\{\begin{array}{l}
f_9(1)=c \\
f_9(2)=c
\end{array} .\right.\right.\right.
\end{aligned}
$$
（3）$f(A)=\{y \in B \mid$ 存在 $x \in A$ 使 $f(x)=y\}$ 稱為 $A$ 在函數 $f$ 下的值域（range）或像（image）。
（4）對 $B$ 的子集 $S$ ，定義 $f^{-1}(S)=\{x \in A \mid f(x) \in S\}$ 為 $S$ 在函數 $f$ 下的前像（pre－image）。例如，考慮集合 $A=\{1,2,3\}, B=\{a, b, c\}$ ，定義 $f, g, h$ 如下，則
$g$ 不是函數，因為 3 沒有對應值；$h$ 不是函數，因為 2 有兩個對應值； $f$ 是函數且 $f(A)=\{a, b\}, f^{-1}(\{b\})=\{2,3\}$ 。
（5）$f$ 為遞增函數（increasing），若 $f$ 滿足：對任何 $x, y$ ，若 $x<y$ ，則 $f(x)<f(y)$ 。 （有些書上定義成嚴格遞增）
（6）$f$ 為遞減函數（decreasing），若 $f$ 滿足：對任何 $x, y$ ，若 $x<y$ ，則 $f(x)>f(y)$ 。 （有些書上定義成嚴格遞減）
（7）$f$ 為非遞減函數（non－decreasing），若 $f$ 滿足：對任何 $x, y$ ，若 $x<y$ ，則 $f(x) \leq f(y){ }^{\circ}$ （有些書上定義成遞增）
（8）$f$ 為非遞增函数（non－increasing），若 $f$ 滿足：對任何 $x, y$ ，若 $x<y$ ，則 $f(x) \geq f(y)$ 。 （有些書上定義成遞減）