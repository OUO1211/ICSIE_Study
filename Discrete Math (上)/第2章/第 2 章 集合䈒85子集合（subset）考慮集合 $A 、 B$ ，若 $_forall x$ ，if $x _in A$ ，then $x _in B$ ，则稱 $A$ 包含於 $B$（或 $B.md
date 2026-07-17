第 2 章 集合䈒

85



子集合（subset）

考慮集合 $A 、 B$ ，

若 $\forall x$ ，if $x \in A$ ，then $x \in B$ ，则稱 $A$ 包含於 $B$（或 $B$ 包含 $A$ ）．

记为 $A \subseteq B$ ，或訊 $A$ 为 $B$ 的一個子集合（也稱 $B$ 为 $A$ 的一個 superset）。



樓｜



例如：

$$

\{1,2\} \subseteq\{1,2,3\} \cdot\{\{1\}, a\} \subseteq\{a, b,\{1\}\} \cdot\{1,2\} \subseteq\{1,2\} \cdot\} \subseteq\{1,2\} \cdot

$$



Note

（1）$A=B \Leftrightarrow A \subseteq B$ and $B \subseteq A$ 。即 $A$ 、 $B$ 互为彼此的集合•



【106中央資工】



（2）若 $A \subseteq B$ 且 $A \neq B$ ，則又可表为 $A \subset B$ ，稱 $A$ 放 $B$ 之正（真）子集（proper subset）．

（3）本身亦為本身之子集，即任意集合 $A, A \subseteq A$ ；且稱 $A$ 方 $A$ 的非正篮子集（improper subset），而 $A$ 的其他子集稱為 $A$ 的正當子集（proper subset）•

（4）$x \in A \Leftrightarrow\{x\} \subseteq A$ ．

例如，考慮集合 $U=\{1,2,3,4,5,\{1,2\},\{1,2,3,4\}\}, A=\{1,2,3,4\}$ ，則下列均成立 ：$A \subseteq U ; A \subset U ; A \in U ;\{A\} \subseteq U ;\{A\} \notin U \cdot$

（5）空集合為任何集合之子集，即任意集合 $A, \varnothing \subseteq A$, 也稱 $\varnothing$ 为 $A$ 的䈹易子集（trivial subset）。

【證明】若 $\varnothing \not \subset A$ ，即存在 $x \in \varnothing$ 且 $x \notin A$ ，但此與 $\varnothing$ 內不存在元素矛盾。例如，下列均成立：$\varnothing \subseteq\{1,2\} ; \varnothing \subseteq\{1, \varnothing\} ; \varnothing \in\{1, \varnothing\}$－

（6）另外，$\varnothing \in\{\varnothing\}$ 成立，因為 $\{\varnothing\}$ 收集了 $\varnothing$ 當作元素。 $\varnothing \subseteq\{\varnothing\}$ 也成立，因為 $\varnothing$ 是任何集合的子集合。

（7）羅素的誖論（Russell＇s paradox）：不存在集合 $S$ ，使得 $S=\{A \mid A \notin A\}$ 。