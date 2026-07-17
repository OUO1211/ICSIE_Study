200
離散數學（上）

性質
考慮函數 $f: A \rightarrow B$ ，且 $A_1, A_2$ 为 $A$ 的兩子集，則
（1）若 $A_1 \subseteq A_2$ ，則 $f\left(A_1\right) \subseteq f\left(A_2\right)$ 。
（2）$f\left(\overline{A_1}\right)=\overline{f\left(A_1\right)} \cdot$（若 $f$ 为 $1-1$ 且 onto）
（3）$f\left(A_1 \bigcup A_2\right)=f\left(A_1\right) \bigcup f\left(A_2\right)$ ．
（4）$f\left(A_1 \cap A_2\right) \subseteq f\left(A_1\right) \cap f\left(A_2\right)$－（等號成立於 $f$ 为 1－1）
若 $f: A \rightarrow B$ 可逆，且 $B_1, B_2$ 為 $B$ 的兩子集，则
（5）若 $A_1 \subseteq A$ 且 $B_1=f\left(A_1\right)$ ，则 $A_1 \subseteq f^{-1}\left(B_1\right)$ 。
（6）若 $B_1 \subseteq B_2$ ，则 $f^{-1}\left(B_1\right) \subseteq f^{-1}\left(B_2\right)$ 。
（7）$f^{-1}\left(B_1 \cup B_2\right)=f^{-1}\left(B_1\right) \cup f^{-1}\left(B_2\right) ; f^{-1}\left(B_1 \cap B_2\right)=f^{-1}\left(B_1\right) \cap f^{-1}\left(B_2\right)$ ．
【譄明】
（1）對 $f\left(A_1\right)$ 中任意元素 $y$ ，令 $A_1$ 中的元素 $x$ ，使 $y=f(x)$ ，
則因為 $A_1 \subseteq A_2$ ，故 $x \in A_2$ 使 $y=f(x)$ ，得 $y \in f\left(A_2\right)$ ，
故得 $f\left(A_1\right) \subseteq f\left(A_2\right)$ 。
（2）任取 $y \in f\left(\bar{A}_1\right)$ 則存在 $x \in \bar{A}_1$ ，使 $y=f(x)$ ，
若 $y \in \overline{f\left(A_1\right)}$ ，則 $y \in f\left(A_1\right)$ ，即存在 $z \in A_1$ ，使 $y=f(z)$ ，與 $f$ 有 $1-1$ 矛盾 ＊故得 $y \in \overline{f\left(A_1\right)}, f\left(\overline{A_1}\right) \subseteq \overline{f\left(A_1\right)}$ 。
任取 $y \in \overline{f\left(A_1\right)}$ ，因为 $f$ 为 onto，故存在 $x \in A$ ，使得 $y=f(x)$ ，
若 $x \in A_1$ ，則 $y \in f\left(A_1\right)$ ，與 $y \in \overline{f\left(A_1\right)}$ 矛盾。
故得 $x \in \bar{A}_1, \therefore y \in f\left(\bar{A}_1\right), \therefore \overline{f\left(A_1\right)} \subseteq f\left(\overline{A_1}\right)$ ．
由上述討論可得 $\overline{f\left(A_1\right)}=f\left(\overline{A_1}\right)$ 。
（3）$y \in f\left(A_1 \cup A_2\right)$
⇔ 存在 $x \in A_1 \cup A_2$ 使得 $f(x)=y$
$\Leftrightarrow$ 存在 $x \in A_1$ 使得 $f(x)=y$ 或存在 $x \in A_2$ 使得 $f(x)=y$
$\Leftrightarrow y \in f\left(A_1\right)$ 或 $y \in f\left(A_2\right)$
$$
\Leftrightarrow y \in f\left(A_1\right) \bigcup f\left(A_2\right)
$$

故得 $f\left(A_1 \cup A_2\right)=f\left(A_1\right) \cup f\left(A_2\right)$ 。
（4）$y \in f\left(A_1 \cap A_2\right)$
⇒ 存在 $x \in A_1 \cap A_2$ 使得 $f(x)=y$
$\Leftrightarrow$ 存在 $x \in A_1$ 使得 $f(x)=y$ 且存在 $x \in A_2$ 使得 $f(x)=y$
$\Leftrightarrow y \in f\left(A_1\right)$ 且 $y \in f\left(A_2\right)$