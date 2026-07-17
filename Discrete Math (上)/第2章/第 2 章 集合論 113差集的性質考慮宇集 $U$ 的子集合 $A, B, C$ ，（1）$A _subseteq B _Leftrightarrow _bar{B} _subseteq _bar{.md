第 2 章 集合論 113



差集的性質

考慮宇集 $U$ 的子集合 $A, B, C$ ，

（1）$A \subseteq B \Leftrightarrow \bar{B} \subseteq \bar{A}$ ．

（2）$(A-B)-C=(A-C)-(B-C)$ ．

【108 中山電機】【110 政大資科】

（3）$(A-B)-C=(A-C)-B$ ．

【108 中山電機】【110 政大資科】

（4）$(A-B)-C=A-(B \cup C)$ ．

【98 台大電機】【108 中山電機】【110 政大資科】

（5）$(A \cup B)-C=(A-C) \cup(B-C)$ ．

【 89 成大資工】【 95 台大電機】

（6）$A-(B \cap C)=(A-B) \bigcup(A-C)$ ．

【102交大資工】【108政大資科】

（7）$A \bigcap(B-C)=(A \bigcap B)-(A \cap C)$ ．

解（1）由定義明顯可得。

（2）右式 $=(A \cap \bar{C}) \cap(\overline{B \cap \bar{C}})=(A \cap \bar{C}) \cap(\bar{B} \cup C)=(A \cap \bar{C} \cap \bar{B}) \cup(A \cap \bar{C} \cap C)$

$$

=(A \cap \bar{C} \cap \bar{B}) \cup \varnothing=(A \cap \bar{B}) \cap \bar{C}=\text { 左式。 }

$$

（3）右式 $=(A \cap \bar{C}) \cap \bar{B}=(A \cap \bar{B}) \cap \bar{C}=(A-B) \cap \bar{C}=$ 左式。

（4）右式 $=A \cap(\overline{B \cup C})=A \cap(\bar{B} \cap \bar{C})=(A \cap \bar{B}) \cap \bar{C}=(A-B) \cap \bar{C}=$ 左式•

（5）左式 $=(A \bigcup B) \bigcap \bar{C}=(A \bigcap \bar{C}) \bigcup(B \bigcap \bar{C})=$ 右式。

（6）左式 $=A \bigcap(\overline{B \bigcap C})=A \bigcap(\bar{B} \bigcup \bar{C})=(A \bigcap \bar{B}) \bigcup(A \bigcap \bar{C})=$ 右式•

（7）右式 $=(A \bigcap B) \bigcap \overline{(A \bigcap C)}=(A \bigcap B) \bigcap(\bar{A} \bigcup \bar{C})=(A \bigcap B \bigcap \bar{A}) \bigcup(A \bigcap B \bigcap \bar{C})$

$$

=\varnothing \bigcup(A \cap B \cap \bar{C})=A \cap B \cap \bar{C}=A \cap(B \cap \bar{C})=\text { 左式。 }

$$