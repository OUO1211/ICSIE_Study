96
離散數學（上）

集合的運算
宇集（universal set）$U:$ 代表收集所有元素的集合。
考虑 $U$ 中的雨子集 $A 、 B$ ，
（1）$A \cap B=\{x \in U \mid x \in A$ 且 $x \in B\}$ ，稱為集合 $A$ 和集合 $B$ 的交集（intersection）。
（2）$A \cup B=\{x \in U \mid x \in A$ 或 $x \in B\}$ ，稱為集合 $A$ 和集合 $B$ 的聯集（union）。
（3） $\bar{A}=\{x \in U \mid x \notin A\}$ ，稱為集合 $A$ 的補集（complement），也記成 $A^c, A^{\prime}$ 。
（4）$A-B=\{x \in U \mid x \in A$ 且 $x \notin B\}$ ，稱為 $A$ 與 $B$ 的差集（difference），也記成 $A \backslash B$ 。
（5）$A \oplus B=\{x \in U \mid x \in A \bigcup B$ 且 $x \notin A \bigcap B\}$ ，稱為 $A$ 和 $B$ 的對稱差（symmetric difference 、互斥或），也記成 $A \Delta B$ 或 $A$ Xor $B$ 。

$A \bigcap B$

$A \bigcup B$

$\bar{A}$

$A-B$

$A \oplus B$

Note
（1）文氏圖（Venn＇s diagram）：平面上對集合的圖形表示法。
（2）若 $A \cap B=\varnothing$ ，則稱 $A$ 與 $B$ 互斥（disjoint）。
（3）有些書上也把補集稱作餘集；若 $\bar{A}=B$ ，則稱 $A$ 與 $B$ 互補。
（4） $\bar{A}=U-A ; \quad A-B=A \bigcap \bar{B}$ 。
（5）$A \oplus B=(A \bigcup B)-(A \bigcap B)=(A-B) \bigcup(B-A)$ 。