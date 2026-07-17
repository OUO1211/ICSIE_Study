106
離散數學（上）

集合的運算性質
考虑全集合 $U$ 上的子集合 $A, B, C$ ：
1．冪等律（idempotent）
（1）$A \cup A=A$
（2）$A \cap A=A$
2．结合律（associative）
（1）$A \bigcup(B \bigcup C)=(A \bigcup B) \bigcup C$
（2）$A \bigcap(B \bigcap C)=(A \bigcap B) \bigcap C$
3．交换律（commutative）
（1）$A \bigcup B=B \bigcup A$
（2）$A \bigcap B=B \bigcap A$
4．分配律（distributive）
（1）$A \bigcup(B \bigcap C)=(A \bigcup B) \bigcap(A \bigcup C)$
（2）$A \bigcap(B \bigcup C)=(A \bigcap B) \bigcup(A \bigcap C)$
5．單位元性質（identity）
（1）$A \cup \varnothing=A$
（2）$A \cap U=A$
（3）$A \cup U=U$
（4）$A \cap \varnothing=\varnothing$
6．雙補集性質（double complement）
$$
\overline{\bar{A}}=A
$$

7．補元素性質（inverse）
（1）$A \bigcup \bar{A}=U$
（2）$A \bigcap \bar{A}=\varnothing$
（3） $\bar{U}=\varnothing$
（4） $\bar{\varnothing}=U$
8．吸收律（absorption）
（1）$A \bigcup(A \bigcap B)=A$
（2）$A \bigcap(A \bigcup B)=A$
9．笛摩根定律（De Morgan＇s law）
（1）$(\overline{A \bigcup B})=\bar{A} \bigcap \bar{B}$
（2）$(\overline{A \bigcap B})=\bar{A} \bigcup \bar{B}$
【證明】
此處證明9（1），其餘請讀者自行練習。
設 $x \in(\overline{A \cup B})$ ，
即 $x \notin(A \cup B), \therefore x \notin A$ and $x \notin B, \therefore x \in \bar{A}$ and $x \in \bar{B}, \therefore x \in \bar{A} \cap \bar{B}, \therefore(\overline{A \cup B}) \subseteq \bar{A} \cap \bar{B}$ ，同理可得 $\bar{A} \cap \bar{B} \subseteq(\overline{A \cup B})$ ，所以得證。

Note
（1）設 $s$ 為一個集合式的表達式，則賭 $s$ 中之 $\varnothing, \cup, \cap, U$ 依序改成 $U, \cap, \cup, \varnothing$ 所得的表達式 $s^d$ 稱為 $s$ 的對偶敘述（dual statement）。上述各定理中（1）與（2），（3）與（4）互為彼此的對偶敘述。
（2）對偶定律（principle of duality）：$s$ 為真 $\Leftrightarrow s^d$ 為真。