第3章 函數
201
$$
\Rightarrow y \in f\left(A_1\right) \cap f\left(A_2\right),
$$

故得 $f\left(A_1 \cap A_2\right) \subseteq f\left(A_1\right) \cap f\left(A_2\right)$ 。
（5）任取 $x \in A_1$ ，則 $f(x) \in f\left(A_1\right)=B_1$ ，即 $x \in f^{-1}\left(B_1\right)$ ，故得 $A_1 \subseteq f^{-1}\left(B_1\right)$ 。
（6）任取 $x \in f^{-1}\left(B_1\right)$ ，則存在 $y \in B_1$ ，使得 $f(x)=y$ ，
則因為 $B_1 \subseteq B_2$ ，故 $y \in B_2$ ，使得 $f(x)=y$ ，即 $x \in f^{-1}\left(B_2\right)$ ，
故得 $f^{-1}\left(B_1\right) \subseteq f^{-1}\left(B_2\right)$ 。
（7）$x \in f^{-1}\left(B_1 \cup B_2\right)$
$\Leftrightarrow$ 存在 $y \in B_1 \cup B_2$ 使得 $f^{-1}(y)=x$
⇔ 存在 $y \in B_1$ 使得 $f^{-1}(y)=x$ 或存在 $y \in B_2$ 使得 $f^{-1}(y)=x$
$\Leftrightarrow x \in f^{-1}\left(B_1\right)$ 或 $x \in f^{-1}\left(B_2\right)$
$\Leftrightarrow x \in f^{-1}\left(B_1\right) \cup f^{-1}\left(B_2\right)$ ，故得 $f^{-1}\left(B_1 \cup B_2\right)=f^{-1}\left(B_1\right) \cup f^{-1}\left(B_2\right)$ 。
$$
\begin{aligned}
& x \in f^{-1}\left(B_1 \cap B_2\right) \\
& \Leftrightarrow f(x) \in B_1 \cap B_2 \\
& \Leftrightarrow f(x) \in B_1 \text { 且 } f(x) \in B_2 \\
& \Leftrightarrow x \in f^{-1}\left(B_1\right) \text { 且 } x \in f^{-1}\left(B_2\right) \\
& \Leftrightarrow x \in f^{-1}\left(B_1\right) \cap f^{-1}\left(B_2\right) \text {, 故得 } f^{-1}\left(B_1 \cap B_2\right)=f^{-1}\left(B_1\right) \cap f^{-1}\left(B_2\right) \text { 。 }
\end{aligned}
$$

Note
（1）$f\left(A_1\right) \cap f\left(A_2\right) \subseteq f\left(A_1 \cap A_2\right)$ 不恆成立 ：
例如考慮 $f: A \rightarrow B, A=\{1,2,3\}, B=\{a, b\}$ ，
$$
A_1=\{1,2\}, A_2=\{1,3\}, f(1)=a, f(2)=b, f(3)=b \text {, }
$$

則 $f\left(A_1\right)=\{a, b\}, f\left(A_2\right)=\{a, b\}, f\left(A_1 \cap A_2\right)=\{a\}$ ，
但當 $f$ 為 1－1 時，則定理（4）證明中的（ ⇒）皆可改成（ ⇔），
使 $f\left(A_1\right) \cap f\left(A_2\right)=f\left(A_1 \cap A_2\right)$ 成立。