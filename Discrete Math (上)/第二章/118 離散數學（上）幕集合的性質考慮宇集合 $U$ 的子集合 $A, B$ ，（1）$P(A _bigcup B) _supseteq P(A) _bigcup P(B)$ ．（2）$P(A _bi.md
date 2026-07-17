118 離散數學（上）

幕集合的性質
考慮宇集合 $U$ 的子集合 $A, B$ ，
（1）$P(A \bigcup B) \supseteq P(A) \bigcup P(B)$ ．
（2）$P(A \bigcap B)=P(A) \bigcap P(B)$ ．
（3）$P(A)=P(B) \Leftrightarrow A=B$ ．
解（1）取集合 $s \in P(A) \cup P(B)$ ，
則 $s \in P(A)$ 或 $s \in P(B), \therefore s \subseteq A$ 或 $s \subseteq B \quad \therefore s \subseteq A \cup B$ ，
$$
\therefore s \in P(A \bigcup B), \quad \therefore P(A) \bigcup P(B) \subseteq P(A \bigcup B) .
$$
（2）任取 $s \in P(A) \bigcap P(B)$ ，
則 $s \in P(A)$ 且 $s \in P(B), \therefore s \subseteq A$ 且 $s \subseteq B \quad \therefore s \subseteq A \cap B$ ，
$$
\therefore s \in P(A \bigcap B), \quad \therefore P(A) \bigcap P(B) \subseteq P(A \bigcap B) .
$$

同理可得 $P(A) \bigcap P(B) \supseteq P(A \bigcap B)$ ，
$$
\therefore P(A) \cap P(B)=P(A \cap B) .
$$
（3）（ ⇒ ）任取 $x \in A$ ，則 $\{x\} \in P(A), ~ \therefore\{x\} \in P(B)$ ，
$$
\therefore x \in B, \therefore A \subseteq B,
$$

同理亦可得 $B \subseteq A, \therefore A=B$ ．
$(\Leftarrow)$ 任取 $s \in P(A)$ ，則 $s \subseteq A, \therefore s \subseteq B$ ，
$$
\therefore s \in P(B), \therefore P(A) \subseteq P(B),
$$

同理亦可得 $P(B) \subseteq P(A), \therefore P(A)=P(B)$ ．