第12章 代數結構
485

\section*{理想子環（Ideal）}

設 $(I,+, *)$ 為 $(R,+, *)$ 之一子環，且滿足 $\forall a \in I, r \in R, a * r \in I$ ，and $r^* a \in I$ ，則稱 $(I,+, *)$ 為 $(R,+, *)$ 的一個理想子環。

例如 ：已知 $(Z,+, \times)$ 為一群，
考慮 $I=<4>=\{4$ 的倍數 $\}$ ，則 $(I,+, \times)$ 為 $(Z,+, \times)$ 之子環，
且 $\forall a \in I, z \in Z, a \times z, z \times a$ 亦必為4的倍數，
$\therefore a \times z \in I, z \times a \in I$ ，即 $(I,+, \times)$ 為 $(Z,+, \times)$ 之理想子環。

\section*{基礎類題}

1．（5％）A nonempty subset $I$ of a ring $(R,+, \cdot)$ is called an ideal of $R$ if for all $a, b \in I$ and all $r \in R: a-b \in I, a \cdot r \in I, r \cdot a \in I$ ．If（ $R,+, \cdot$ ）is furthermore a field，then it has $\_\_\_\_$ ideals．

【94台大資工】
解 2 。
設 $I$ 為 $(R,+, \cdot)$ 中的一個 ideal，
因為 $I$ 中必有加法單位元素 0 ，但若還有其它元素，則 $I$ 一定含有乘法單位元素 1 ，（因為任取 $x \in I$ ，取其乘法反元素 $y \in R$ ，則 $x y=1 \in I$ ）
於是，任意 $z \in R, \quad 1 \in I$ ，造成了 $1 \cdot z=z \in I$ ，即 $R$ 有的 $I$ 也會有，也就是 $I=R$ ，即 $(R,+, \cdot)$ 就 $R$ 本身與 $\{0\}$ 這兩個 ideal。