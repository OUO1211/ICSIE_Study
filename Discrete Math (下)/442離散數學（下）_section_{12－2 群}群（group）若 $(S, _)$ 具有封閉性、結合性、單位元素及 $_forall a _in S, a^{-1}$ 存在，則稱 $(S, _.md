442
離散數學（下）

\section*{12－2 群}

群（group）
若 $(S, *)$ 具有封閉性、結合性、單位元素及 $\forall a \in S, a^{-1}$ 存在，則稱 $(S, *)$ 為一群。
Note
\begin{itemize}
\item[（1）] 若（ $S, *$ ）為一具有交換性的群，則稱（ $S, *$ ）為一交換群（commutative group），又稱做阿貝爾群（Abelian group）。
\item[（2）] 若 $|G|$ 為有限時，則稱 $G$ 為有限群（finite group），否則稱 $G$ 為無限群（infinite group），且稱 $|G|$ 為 $G$ 的基數（order）（也記作。 $(G)$ ）。
\item[（3）] 例如 ：$(Z,+),(R-\{0\}, \times),\left(R^{n \times n}:\right.$ 實數之 $n \times n$ 矩陣，＋）均為交換群，但（｛可逆矩陣\},×）為非交換群。
\item[（4）] 在（ $Z,+$ ）中單位元素為 0 ，每個元素皆有反元素（取負元素）。
\item[（5）] 在（ $Z, \times$ ）中單位元素為 1 ，只有 1 與 -1 有反元素（都是自己），所以不是群。
\item[（6）] 在 $(R, \times)$ 中單位元素為 1 ，除了 0 皆有反元素（都是自己的倒數），所以不是群。
\item[（7）] 令 $P(A)$ 為集合 $A$ 之冪集合，在 $(P(A), \cap)$ 中單位元素為 $A$ ，但並非每個元素都有反元素，所以不是群。
\end{itemize}

例題 1
Let＠be a binary operation defined on the set of integers $Z$ by $x @ y=x+y-5$ ．Prove that（ $Z$ ，＠）is an abelian group．

【 $91 、 93$ 北科資工】
【證明】
封閉性：$\forall x, y \in Z, x @ y=x+y-5 \in Z$ 。
結合性：$\forall x, y, z \in Z,(x @ y) @ z=(x+y-5) @ z=(x+y-5)+z-5=x+y+z-10$ ．
$$
\begin{aligned}
& x @(y @ z)=x @(y+z-5)=x+(y+z-5)-5=x+y+z-10 . \\
& \therefore(x @ y) @ z=x @(y @ z) .
\end{aligned}
$$
單位元素：$e=5 . \because 5 @ y=5+y-5=y, y @ 5=y+5-5=y$ 。
反元素：$\forall x \in Z, x^{-1}=(10-x) . \because x @(10-x)=x+(10-x)-5=5=e$.
$$
(10-x) @ x=(10-x)+x-5=5=e .
$$
交換性：$\forall x, y \in Z, x @ y=x+y-5, y @ x=y+x-5, \therefore x @ y=y @ x$.