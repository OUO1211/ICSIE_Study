第2章 集合論

111



推廣

Let $A=\left\{A_1, \ldots, A_n\right\}$ be an arbitrary collection of sets，

The generalized intersection of $A: \bigcap_{i=1}^k A_i=A_1 \cap A_2 \cap \ldots \cap A_k=\left\{x: x \in A_i, \forall i=1,2, \ldots, k\right\}$ ．

The generalized union of $A: \bigcup_{i=1}^k A_i=A_1 \cup A_2 \cup \ldots \cup A_k=\left\{x: x \in A_i\right.$ ，for some $\left.i=1 \sim k\right\}$ ．

Note

（1）例如 ：Let $I=\{3,4,5,6,7\}, \forall i \in I, A_i=\{1,2, \ldots, i\} \subseteq Z^{+}$，then

$$

\bigcup_{i \in I} A_i=\bigcup_{i=3}^7 A_i=\{1,2,3,4,5,6,7\} ; \bigcap_{i \in I} A_i=\bigcap_{i=3}^7 A_i=\{1,2,3\} .

$$

（2）例如：考慮宇集合為實數集，指標集為正實數集，對任意正實數 $r$ ，定義 $A_r=[-r, r]$ ，則 $\bigcup_{i \in I} A_i=R ; \bigcap_{i \in I} A_i=\{0\}$ 。

（3）笛摩根定理的一般化 ：（1）$\overline{\bigcup_{i=1}^n A_i}=\bigcap_{i=1}^n \overline{A_i}$ ；（2）$\overline{\bigcap_{i=1}^n A_i}=\bigcup_{i=1}^n \overline{A_i}$ 。

【107台大工科】



解



（1）以歸納法證明如下：

$n=2$ 時，即笛摩根定理，

設 $n=k \geq 2$ 時原式成立，

則 $n=k+1$ 時，$\overline{\bigcup_{i=1}^{k+1} A_i}=\overline{\left(\bigcup_{i=1}^k A_i\right) \bigcup A_{k+1}}=\left(\overline{\bigcup_{i=1}^k A_i}\right) \cap \overline{A_{k+1}}=\left(\bigcap_{i=1}^k \overline{A_i}\right) \cap \overline{A_{k+1}}=\bigcap_{i=1}^{k+1} \overline{A_i} \cdot$

（2）由（1）與對偶性質，可得證。