第3章 函數
187

合成函數（composite function）
設 $f: A \rightarrow B \vee g: B \rightarrow C$ ，為兩函数，則
$f$ 和 $g$ 的合成函数，$g \circ f: A \rightarrow C$ ，
定義成 $g \circ f(x)=g(f(x)), \forall x \in A 。$

【107台大工科】

Note
（1）設 $a \in A, c \in C, g \circ f(a)=c \Leftrightarrow$ 存在 $b \in B$ ，使 $f(a)=b, g(b)=c$ 。
（2）這裡函數的合成是以右運算表達。
（3）函數的合成具結合性，即 $f \circ(g \circ h)=(f \circ g) \circ h \circ$
例如

例如：
$$
\begin{aligned}
& f(x)=3 x+5, \\
& g(x)=6 x^4, \\
& \text { 則 } f(g(x))=3 \cdot 6 x^4+5, \quad g(f(x))=6(3 x+5)^4
\end{aligned}
$$