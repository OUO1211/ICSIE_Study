734
離散數學（上）

特定片段所造字串

例題
Let $\Sigma=\{0,1\}$ be an alphabet and $A=\{1,00,10\}$ be a subset of $\Sigma^*$ ．
（1）（ $10 \%$ ）For each integer $n \geq 1$ ，let $a_n$ be the number of strings in $A^*$ of length $n$ ．Find and solve a recurrence relation for $a_n$ ．

【104成大資工】
（2）$(10 \%)$ For each integer $n \geq 1$ ，let $b_n$ be the number of strings in $A^*$ which are of length $n$ and exactly divided by 2 when we regard each of the strings as a binary number．Find $b_n$ ．

【107中山資工】
解（1）明顯可得，$a_1=1, a_2=3$ ．
$n \geq 3$ 時，符合題目敘述的字串可分類計算如下：
未為 1 的字串有 $a_{n-1}$ 種（ $\because$ 剩前面長度 $n-1$ ），
末為 0 ，倒數第二是 1 的字串有 $a_{n-2}$ 種（即最末兩碼是 10 ，且剩前長度 $n-2$ ），
末為 0 ，倒數第二是 0 的字串有 $a_{n-2}$ 種（即最末兩碼是 00 ，且剩前長度 $n-2$ ），
故得遞迴關係式：$a_n=a_{n-1}+2 a_{n-2}$ ，
其特徵式為 $\alpha^2-\alpha-2=0$ ，解得特徵根為：$\alpha_1=2, \alpha_2=-1$ ，
設 $a_n=c_1 2^n+c_2(-1)^n$ ，代入 $\left\{\begin{array}{l}a_1=1 \\ a_2=3\end{array}\right.$ ，解得 $c_1=\frac{2}{3}, c_2=\frac{1}{3}$ ，
$\therefore a_n=\frac{1}{3}\left(2^{n+1}+(-1)^n\right), \quad n \geq 1 。$
（2）因為偶正整數的二進位字串表達，最末必為 0 ，
故 $b_n$ 即由 $A$ 組成長度 $n$ 且末為 0 的字串數，
明顯可得，$b_1=0, b_2=2, b_3=2$ ，且 $n \geq 4$ 時，$b_n$ 可如下討論：
最末為 10 的字串有 $a_{n-2}$ 種（ $\because$ 剩前面長度 $n-2$ 為任意字串），
最末為 00 的字串有 $a_{n-2}$ 種（ ∵ 剩前長度 $n-2$ 為任意字串），
故得 $b_n=2 a_{n-2}=\frac{2}{3}\left(2^{n-1}+(-1)^{n-2}\right), n \geq 3$ ，且 $b_2=2, b_1=0$ 。