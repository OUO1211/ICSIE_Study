180
離散數學（上）

計算函數個數
考虑集合 $A 、 B$ ，函数 $f: A \rightarrow B$ ，其中 $|A|=m,|B|=n$ ，則
（1）有 $n^m$ 種不同的 $f$ 。
（2）若 $f$ 為一對一，則
（1）$m \leq n$ 。
（2）有 $n(n-1)(n-2) \ldots(n-m+1)=P_m^n$ 種不同的 $f \circ$
（3）若 $f$ 為 onto，則
（1）$m \geq n$ 。
（2）有 $\sum_{i=0}^n(-1)^i\binom{n}{i}(n-i)^m=\operatorname{Onto}(m, n)$ 種不同的 $f$ 。
（4）若 $f$ 為一對一且 onto，則
（1）$m=n$ 。
（2）有 $n!$ 種不同的 $f$ 。
【很重要】

【證明】
（1）$A$ 中的元素每個均有 $n$ 個 $B$ 中的元素可對，
故由乘法原理知，共 $\underbrace{n \times n \times \ldots \times n}_{m \text { 個 }}=n^m$ 種 $A$ 到 $B$ 函數。
（2）設 $A=\left\{a_1, a_2, \ldots, a_m\right\}$ ，若為 1－1 函數，則 $a_i$ 與 $a_j$ 的對應值必不相同，$\forall i \neq j \circ$
則 $a_1$ 有 $n$ 個 $B$ 中的元素可對應；
$a_2$ 剩 $n-1$ 個 $B$ 中的元素可對；
$a_3$ 剩 $n-2$ 個 $B$ 中的元素可對；
⋯
$a_m$ 剩 $n-m+1$ 個 $B$ 中的元素可對，
故由乘法原理知，共 $n \times(n-1) \times \ldots \times(n-m+1)$ 種 1－1 函數。
（3）排容原理中已討論過。
（4）由（2）（3）可得•
Note
（1）若 $m=n$ ，則 $f$ 為一對一 ⇔ $f$ 為映成。
【證明】
$\because f: A \rightarrow B, \therefore f(A) \subseteq B$,
若 $f: 1-1$ ，則 $|f(A)|=|A|=|B|, ~ \therefore f(A)=B, ~ \therefore f$ ：onto。