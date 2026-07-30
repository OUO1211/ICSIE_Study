第11章 二元關係及其應用
387

\section*{偏序集的性質－卡氏積（Cartesian product of two posets）}

設 $\left(S, \leq_1\right),\left(T, \leq_2\right)$ 均為偏序集，
在 $S \times T$ 上定義一關係＂$\leq$＂為 $(s, t) \leq(u, v) \Leftrightarrow s \leq_1 u$ ，且 $t \leq_2 v$ ，則 $(S \times T, \leq)$ 亦為偏序集。
【證明】
反身性：$\forall(a, b) \in S \times T$ ，
$\because\left(S, \leq_1\right),\left(T, \leq_2\right)$ 具反身性，$\therefore a \leq_1 a$ 且 $b \leq_2 b$ ，故由定義知 $(a, b) \leq(a, b)$ 。
反對稱性：
設 $(a, b) \leq(c, d)$ 且 $(c, d) \leq(a, b)$ ，則由定義知 $a \leq_1 c$ 且 $c \leq_1 a, b \leq_2 d$ 且 $d \leq_2 b$ ，
但因為 $\left(S, \leq_1\right),\left(T, \leq_2\right)$ 都有反對稱性，$\therefore a=c, b=d, \therefore(a, b)=(c, d)$ 。
遞移性：
設 $(a, b) \leq(c, d)$ 且 $(c, d) \leq(e, f)$ ，則由定義知 $a \leq_1 c$ 且 $c \leq_1 e, b \leq_2 d$ 且 $d \leq_2 f$ ，
但因為 $\left(S, \leq_1\right),\left(T, \leq_2\right)$ 有遞移性，$\therefore a \leq_1 e, b \leq_2 f, \therefore(a, b) \leq(e, f)$ 。
故知 $(S \times T, \leq)$ 為一偏序集。

Note
偏序集之卡氏積的推廣應用：

偏序集的應用－字典編輯序（lexicographic ordering）
設 $(S, R)$ 為全序集，
則定義在 $S^m=\overbrace{S \times S \times \ldots \times S}^m$ 上的關係 $\prec$ 稱作字典編輯序，其定義如下：
$\forall a, b \in S^m$ ，設 $a=a_1 a_2 \ldots a_m, b=b_1 b_2 \ldots b_m$ ，其中 $a_i, b_j \in S, \forall i, j$ ，
$a \prec b \Leftrightarrow\left\{\begin{array}{l}a_1 \neq b_1 \\ a_1 R b_1\end{array}\right.$ or $\left\{\begin{array}{l}a_i=b_i, \forall i, 1 \leq i \leq k \\ a_{k+1} \neq b_{k+1} \\ a_{k+1} R b_{k+1}\end{array} \quad\right.$ for some $k, 1 \leq k \leq m 。$

例如，
$\{3,6,7,8\},\{1,3,4,7\},\{2,3,4,7\},\{1,3,5,6\},\{4,6,7,8\},\{2,3,5,6\}$ 之字典编輯序為：$\{1,3,4,7\} 、\{1,3,5,6\} 、\{2,3,4,7\} 、\{2,3,5,6\} 、\{3,6,7,8\} 、\{4,6,7,8\}$ 。【110中興資科】