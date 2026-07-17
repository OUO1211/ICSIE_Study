第 2 章 集合論
89

冪集合（power set）
給定集合 $A$ ，稱 $P(A)=\{X \mid X \subseteq A\}$ ，為 $A$ 的冪集合，有時記做 $2^A$ 。
例如，寫出下列各集合的冪集合 ：
（1）$\{1\}$ ．
（2）$\{1,2\}$ ．
（3）$\{7,8,9\}$ ．
（4）$\{\{a\}\}$ ．
（5）$\{\varnothing,\{\varnothing\}\}$ ．
【109 中興資科】
解（1）$\{\varnothing,\{1\}\}$ ．
（2）$\{\varnothing,\{1\},\{2\},\{1,2\}\}$ ．
（3）$\{\},\{7\},\{8\},\{9\},\{7,8\},\{7,9\},\{8,9\},\{7,8,9\}\}$.
（4）$\{\varnothing,\{\{a\}\}\}$ ．
（5）$\{\varnothing,\{\varnothing\},\{\{\varnothing\}\},\{\varnothing,\{\varnothing\}\}\}$.
Note
（1）即 $P(A)$ 為收集 $A$ 的所有子集合的一個集合。
（2）對任意集合 $A$ ， □ $\varnothing \in P(A), \varnothing \subseteq P(A),\{\varnothing\} \subseteq P(A)$都成立。
（3）對任意集合 $A,\{\varnothing\} \in P(A)$ 不一定成立。
（4）對任意集合 $A, \forall x \in A \Leftrightarrow\{x\} \subseteq A \Leftrightarrow\{x\} \in P(A)$ 。
說明：
$x \in A$
表示 $x$ 是 $A$ 的元素，
$\Leftrightarrow\{x\} \subseteq A$
以 $\}$ 包裝起來就成為 $A$ 的子集合，
$\Leftrightarrow\{x\} \in P(A)$
因為 $P(A)$ 這個集合專門收集 $A$ 的所有子集，當然會收集到 $\{x\}$ 。