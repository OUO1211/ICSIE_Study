第12章 代數結構
435

\section*{12－1 代數系統}

\section*{二元運算（binary operation）與代數系統（algebraic system）}

考虑非空集合 $A$ ，則稱函數＊：$A \times A \rightarrow A$ 為一種 $A$ 上的二元運算。
令 $*_1, *_2, \ldots, *_k$ 為 $A$ 上的二元運算，則稱 $\left(A, *_1, *_2, \ldots, *_k\right)$ 為一代數系统。
Note
例如 $(Z,+),(Q, \times),(R,+, \times)$ 都是常見代數系統。

代數系統的各種特性：
考虑 $A$ 上的二元運算＊與 $A$ 的一子集 $S$ ，（ $S, *$ ）為一代數系統，
若 $\forall a, b \in S, a * b \in S$ ，則稱（ $S, *$ ）具封閉性（closed）。
若 $\forall a, b, c \in S,(a * b)^* c=a^*\left(b^* c\right)$ ，則稱 $(S, *)$ 具結合性（associative）。
單位元素（identity）
若存在 $e_r$ 使得 $\forall a \in S, ~ a * e_r=a$ ，則稱 $e_r$ 為 $(S, *)$ 之右單位元素；
若存在 $e_l$ 使得 $\forall a \in S, e_l^* a=a$ ，則稱 $e_l$ 為 $(S, *)$ 之左單位元素；
若存在 $e$ 使得 $\forall a \in S, a * e=e * a=a$ ，則稱 $e$ 為 $(S, *)$ 之單位元素。
反元素（inverse element）
設 $(S, *)$ 為一具單位元素 $e$ 的代數系統，$a \in S$ ，
對元素 $a$ ，若存在 $b_r$ 使得 $a^* b_r=e$ ，則稱 $b_r$ 為 $a$ 之右反元素；
對元素 $a$ ，若存在 $b_l$ 使得 $b_l * a=e$ ，則稱 $b_l$ 為 $a$ 之左反元素；
對元素 $a$ ，若存在 $b$ 使得 $a * b=b * a=e$ ，則稱 $b$ 為 $a$ 之反元素，記作 $b=a^{-1}$ 。
交換性
若 $\forall a, b \in S, a * b=b * a$ ，則稱 $(S, *)$ 具交換性（commutative）。
消去性
若 $\forall a, b, c \in S$ ，若 $a * b=a * c \Rightarrow b=c$ ，則稱 $(S, *)$ 具有左消去性。
若 $\forall a, b, c \in S$ ，若 $b^* a=c^* a \Rightarrow b=c$ ，則稱 $(S, *)$ 具有右消去性。
若（ $S, *$ ）具有左消去性與右消去性，則稱（ $S, *$ ）有消去性。