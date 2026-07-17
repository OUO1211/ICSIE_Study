第 2 章 集合論 127

2－2 排容原理（The Principle of Inclusion and Exclusion）

令 $A_1, A_2, \ldots, A_n$ 為宇集合 $U$ 的子集合，則對任何 $t, 1 \leq t \leq n$ ，
$$
\begin{aligned}
& \left|\overline{A_1} \cap \overline{A_2} \cap \ldots \cap \overline{A_t}\right|=|U|-\left|A_1 \cup A_2 \cup \cdots \cup A_t\right| \\
& =|U|-\sum_{i=1}^t\left|A_i\right|+\sum_{1 \leq i<j \leq t}\left|A_i \cap A_j\right|-\sum_{1 \leq i<j<k \leq t}\left|A_i \cap A_j \cap A_k\right|+\ldots+(-1)^t\left|\bigcap_{i=1}^t A_i\right| .
\end{aligned}
$$

【90台大資工】【90中央資工】
＂解（以下以組合方法證明，亦可由數學歸納法證明）
$$
\forall x \in U,
$$
（1）$x$ 不滿足 $A_1 \sim A_7$ 中的任一件性質：
則 $x$ 在等號的左邊被計一次，
而在等號的右邊，$x$ 只在第一項 $|U|$ 被計算到，故等式成立。
（2）$x$ 滿足 $A_1 \sim A_t$ 中的某 $s$ 件性質（不失一般性，設為 $A_1, \ldots, A_s$ ）， $1 \leq s \leq t$ ：
則等號的左邊不會計算到 $x$ ，而在等號的右邊，
第一項 $|U|$ 中計算 $x$ 一次，（即 $\binom{s}{0}$ ）。
第二項中只 $\left|A_1\right|,\left|A_2\right|, \ldots,\left|A_s\right|$ 有計算 $x$ ，共 $\binom{s}{1}$ 次。
第三項中只 $\left|A_1 \cap A_2\right|,\left|A_1 \cap A_3\right|, \ldots,\left|A_i \cap A_j\right|, 1 \leq i<j \leq s$ ，有計算 $x$ ，共 $\binom{s}{2}$ 次。
第四項中只 $\left|A_i \cap A_j \cap A_k\right|, 1 \leq i<j<k \leq s$ ，有計算 $x$ ，共 $\binom{s}{3}$ 次。
∴ 等號右邊的值為 $\binom{s}{0}-\binom{s}{1}+\binom{s}{2}-\ldots+(-1)^s\binom{s}{s}=(1+(-1))^s=0$ ，故等式成立。