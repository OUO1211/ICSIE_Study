第 2 章 集合論

149



排容原理的應用三：映成（onto）函數

考虑集合 $A 、 B$ ，其中 $|A|=m,|B|=n$ ，且 $m \geq n$ ，

則 $A$ 至 $B$ 的映成函数個数為 $\sum_{i=0}^n(-1)^i\binom{n}{i}(n-i)^m$ ，也記作 $\operatorname{Onto}(m, n)$ 。

（也是 $m$ 個相異物放入 $n$ 個相異箱子而不允許空箱的方法数）

（也是 $m$ 個工作分給 $n$ 個人而每人皆至少一項工作的方法数）

解 設 $U=\{f \mid f: A \rightarrow B\}, ~ B=\left\{y_1, y_2, \ldots, y_n\right\}$ ，

定義集合 $a_i=\left\{f \in U \mid \forall x \in A, f(x) \neq y_i\right\}$ ，

$\overline{a_i}=\left\{f \in U \mid \exists x \in A\right.$ ，使得 $\left.y_i=f(x)\right\}, 1 \leq i \leq n$ ，

則 $|U|=n^m$ ，且 $\left|a_i\right|=(n-1)^m, 1 \leq i \leq n$ ，

$$

\begin{aligned}

& \left|a_i \cap a_j\right|=(n-2)^m, 1 \leq i<j \leq n \\

& \left|a_i \cap a_j \cap a_k\right|=(n-3)^m, 1 \leq i<j<k \leq n

\end{aligned}

$$



故由排容原理知所求

Onto $(m, n)=\mid\left\{f \in U \mid \forall y_i \in B, \exists x \in A\right.$ ，such that $\left.f(x)=y_i\right\}\left|=\left|\overline{a_1} \cap \overline{a_2} \cap \ldots \cap \overline{a_n}\right|\right.$

$$

\begin{aligned}

& =U\left|-\sum_{1 \leq i \leq n}\right| a_i\left|+\sum_{1 \leq i<j \leq n}\right| a_i \cap a_j \mid-\ldots \\

& =n^m-\binom{n}{1} \cdot(n-1)^m+\binom{n}{2}(n-2)^m-\ldots+(-1)^n\binom{n}{n}(n-n)^m \\

& =\sum_{i=0}^n(-1)^i\binom{n}{i}(n-i)^m

\end{aligned}

$$



Note

（1）也可以從 Stirling 數（第五章會提到）切入討論 ：Onto $(m, n)=S(m, n) \times n!$ 。