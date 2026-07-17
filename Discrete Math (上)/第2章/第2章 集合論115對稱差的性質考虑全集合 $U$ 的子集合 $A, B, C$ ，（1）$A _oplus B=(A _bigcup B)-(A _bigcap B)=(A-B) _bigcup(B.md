第2章 集合論

115



對稱差的性質

考虑全集合 $U$ 的子集合 $A, B, C$ ，

（1）$A \oplus B=(A \bigcup B)-(A \bigcap B)=(A-B) \bigcup(B-A)$ ．

【95成大工科】【99台大重機】

（2）$A \oplus B=B \oplus A$ ．

（交换性）

【99台大重機】

（3）$A \oplus \bar{A}=U, A \oplus U=\bar{A}$ ．

（4）$A \oplus \varnothing=A, A \oplus A=\varnothing$ ．

【 89 成大資工】【90台科資工】

（5）$(A \oplus B) \oplus C=A \oplus(B \oplus C)$ ．

（結合性）

【99台大電機】

（6）$A \cap(B \oplus C)=(A \cap B) \oplus(A \cap C),(B \oplus C) \cap A=(B \cap A) \oplus(C \cap A)$ 。（$\cap$ 對 $\oplus$ 具分配性）



【104台大電機】【110政大資科】

解（1），（2），（3）從定義明顯可得。

（4）$A \oplus \varnothing=(A \cup \varnothing)-(A \cap \varnothing)=A-\varnothing=A ; A \oplus A=(A \cup A)-(A \cap A)=A-A=\varnothing$ ．

（5），（6）以文氏圖檢查比較快。



基礎類題

1．True or False：

（1）$(A \Delta B) \bigcap C=(A \bigcap C) \Delta(B \cap C)$ ．



【97．98 台大電機】



（2）$(A \Delta B) \bigcup B \neq A \bigcup B$ ．

（3）$A \Delta B=C \Rightarrow A \Delta C=B$ and $B \Delta C=A$ ．

（4）$A \Delta(B \cap C)=(A \Delta B) \cap(A \Delta C)$ ．



【99成大資工】



（5）$(A \oplus B) \oplus B=A$ ．



【99台大電機】



（6）For a set，the ⊕ operation is neither left nor right distributive with respect to the operation．



【104 台栜電機】



解 True：（1），（3），（5），（6）．$\Delta$ 與 ⊕ 都是對稱差的運算。

因為 $A \oplus(B \cap C)=(A \oplus B) \cap(A \oplus C) ;(B \cap C) \oplus A=(B \oplus A) \cap(C \oplus A)$ 的確不恆成立。