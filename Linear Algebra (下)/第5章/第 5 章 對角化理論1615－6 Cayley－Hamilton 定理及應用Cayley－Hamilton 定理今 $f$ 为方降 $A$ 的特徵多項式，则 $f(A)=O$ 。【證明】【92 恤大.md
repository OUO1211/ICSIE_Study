第 5 章 對角化理論

161



5－6 Cayley－Hamilton 定理及應用



Cayley－Hamilton 定理

今 $f$ 为方降 $A$ 的特徵多項式，则 $f(A)=O$ 。

【證明】



【92 成大數學、100 中興資工



設 $f(x)=\operatorname{char}_A(x)=\operatorname{det}(A-x I)=(-x)^n+a_{n-1} x^{n-1}+\ldots+a_1 x+a_0$ ．

则因 $A-x I$ 的伴隨策陣 $\operatorname{adj}(A-x I)$ 為一 $n$ 階方陣，

且也可以表为以 $x$ 为變數的 $(n-1)$ 次的方陣多項式。

故可設 $\operatorname{adj}(A-x I)=A_{n-1} x^{n-1}+A_{n-2} x^{n-2}+\ldots+A_1 x+A_0$ ，其中 $A_{n-1}, A_2, \ldots, A_1, A_0 \in F^{* * *}$ 。

$$

\begin{align*}

& \because(A-x I) \operatorname{adj}(A-x I)=\operatorname{det}(A-x I) I_n, \cdots \cdots \cdots \cdots(*)  \tag{}\\

& \therefore(A-x I)\left(A_{n-1} x^{n-1}+A_{n-2} x^{n-2}+\ldots+A_1 x+A_0\right)=(-1) x^n I+a_{n-1} x^{*-1} I+\ldots+a_1 x I+a_0 I .

\end{align*}

$$



比較等式左右各項係數得：

$$

\left\{\begin{array}{l}

\left.-A_{n-1}=(-1)^n I \ldots \ldots . . \text { (第 } 1 \text { 式 }\right) \\

A A_{n-1}-A_{n-2}=a_{n-1} I \ldots . \text { (第 } 2 \text { 式) } \\

A A_{n-2}-A_{n-3}=a_{n-2} I \ldots . \text { (第 } 3 \text { 式) } \quad \text { 將第 }(i) \text { 式在右同乘 } A^{*-i+1} \\

\quad \vdots \\

\left.A A_1-A_0=a_1 I \ldots \ldots . . \text { (第 } n \text { 式 }\right) \\

\left.A A_0=a_0 I \ldots \ldots \ldots \ldots . . \text { (第 } n+1 \text { 式 }\right)

\end{array} .\right.

$$



可得 $\left\{\begin{array}{l}-A^n A_{n-1}=(-1)^n A^n \\ A^n A_{n-1}-A^{n-1} A_{n-2}=a_{n-1} A^{n-1} \\ A^{n-1} A_{n-2}-A^{n-2} A_{n-3}=a_{n-2} A^{n-2} \\ \quad \vdots \\ A^2 A_1-A A_0=a_1 A \\ A A_0=a_0 I\end{array}\right.$

再將所有式子加總得：$O=(-1)^n A^n+a_{n-1} A^{n-1}+\ldots+a_1 A+a_0 I=f(A)$ ．

例如，

$$

A=\left[\begin{array}{ll}

1 & 3 \\

2 & 4

\end{array}\right], \operatorname{char}_A(x)=\operatorname{det}(A-x I)=x^2-5 x-2,

$$



則 $\operatorname{char}_A(A)=A^2-5 A-2 I=\left[\begin{array}{ll}1 & 3 \\ 2 & 4\end{array}\right]^2-5\left[\begin{array}{ll}1 & 3 \\ 2 & 4\end{array}\right]-2\left[\begin{array}{ll}1 & 0 \\ 0 & 1\end{array}\right]=\left[\begin{array}{ll}0 & 0 \\ 0 & 0\end{array}\right]$ ．