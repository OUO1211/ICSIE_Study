116

離散數學（上）



卡式積的性質

考慮字集合 $U$ 的子集合 $A, B, C, D$ ，

（1）If $C \neq \varnothing$ and $A \times C=B \times C$ ，then $A=B$ ．

（2）$A \subseteq C$ and $B \subseteq D \Leftrightarrow A \times B \subseteq C \times D$ ．

（3）$(A \bigcup B) \times C=(A \times C) \bigcup(B \times C) ; A \times(B \bigcup C)=(A \times B) \bigcup(A \times C)$ ．

（4）$(A \cap B) \times C=(A \times C) \cap(B \times C) ; A \times(B \cap C)=(A \times B) \cap(A \times C)$ ．



【103台聘軍演】



（5）$(A \times C) \cup(B \times D) \subseteq(A \bigcup B) \times(C \bigcup D)$ ．

（6）$(A \times C) \cap(B \times D)=(A \cap B) \times(C \cap D)$ ．

（7）$A \times(B-C)=(A \times B)-(A \times C)$ ．



【95台大電䃀】



解（1），（2），（7）明顯可得。

（3）設 $(x, y) \in(A \bigcup B) \times C$ ，則 $x \in(A \bigcup B)$ and $y \in C$ ，

$\therefore[x \in A$ or $x \in B]$ and $y \in C$ ，

$\therefore(x, y) \in A \times C$ or $B \times C$ ，

$\therefore(A \cup B) \times C \subseteq(A \times C) \cup(B \times C)$ ，同理可得 $(A \times C) \cup(B \times C) \subseteq(A \cup B) \times C$ ．

得 $(A \bigcup B) \times C=(A \times C) \bigcup(B \times C)$ 。

再由交換性可得 $A \times(B \cup C)=(A \times B) \cup(A \times C)$ 。

（4）與（3）的證明技巧類似，讀者可自行嘗試證明。

（5）令 $(x, y) \in(A \times C) \cup(B \times D)$ ，則 $(x, y) \in A \times C$ 或 $(x, y) \in B \times D$ ，

即 $x \in A$ 且 $y \in C$ ，或 $x \in B$ 且 $y \in D$ ，故得 $x \in A \cup B$ 且 $y \in C \cup D$ ，

$$

\begin{aligned}

& \therefore(x, y) \in(A \bigcup B) \times(C \bigcup D) \\

& \therefore(A \times C) \bigcup(B \times D) \subseteq(A \bigcup B) \times(C \bigcup D)

\end{aligned}

$$

（6）$(x, y) \in(A \times C) \cap(B \times D) \Leftrightarrow(x, y) \in A \times C$ 且 $(x, y) \in B \times D$ ，

$$

\begin{aligned}

& \Leftrightarrow x \in A \text { 且 } y \in C, \text { 且 } x \in B \text { 且 } y \in D \Leftrightarrow x \in A \cap B \text { 且 } y \in C \cap D \\

& \Leftrightarrow(x, y) \in(A \cap B) \times(C \cap D) \\

& \therefore(A \times C) \cap(B \times D)=(A \cap B) \times(C \cap D) .

\end{aligned}

$$