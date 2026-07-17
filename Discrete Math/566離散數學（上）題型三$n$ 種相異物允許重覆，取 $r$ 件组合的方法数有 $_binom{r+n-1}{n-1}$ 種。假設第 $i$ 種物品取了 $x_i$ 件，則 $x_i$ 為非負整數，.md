566
離散數學（上）

題型三
$n$ 種相異物允許重覆，取 $r$ 件组合的方法数有 $\binom{r+n-1}{n-1}$ 種。
假設第 $i$ 種物品取了 $x_i$ 件，則 $x_i$ 為非負整數，且原題即為求 $x_1+x_2+\ldots+x_n=r$ 的非負整數解個數，而為：$\binom{r+n-1}{n-1}$ 。

【106成大工科】

例題
（6\％）How many ways are there to choose the 10 items from 6 distinct items when
（1）$(3 \%)$ The items in the choices are ordered and repetition is allowed？
（2）$(3 \%)$ The items in the choices are unordered and repetition is allowed？
【97清大資工】
解（1）即求六個相異物品可重複的選出 10 個來排列的方法數，
而第一個物品有 6 種可能，第二個物品有 6 種可能，⋯，第十個物品有 6 種可能，故由乘法原理得知共 $6 \times 6 \times \cdots \times 6=6^{10}$ 種方法。
（2）即求六個相異物品可重複的選出 10 個來組合的方法數，
即 $x_1+x_2+\ldots+x_6=10, x_i \geq 0$ ，for $i=1 \sim 6$ ，的非負整數解個數，共 $\binom{10+5}{5}$ 種方法。

例題－
Choose a number uniformly at random between 0 and 999,999 ，inclusive．What is the probability that the digits sum to 19 ？（just need to give answer）

【 94 交大資訊】【 97 清大資應】【 88 、 98 中興資科】【 101 嘉義資工類題】
解 設滿足題意的正整數為 $x_1 x_2 x_3 x_4 x_5 x_6$ ，
則 $x_1+x_2+\ldots+x_6=19$ 且 $0 \leq x_i \leq 9$ ，for $1 \leq i \leq 6$ ，
而此方程式之整數解個數有 $\binom{19+5}{5}-\binom{6}{1}\binom{9+5}{5}$ 種，
又任取一數的方法有 $10 \cdot 10 \cdots \cdot 10=10^6$ 種，故機率為 $\frac{\binom{19+5}{5}-\binom{6}{1}\binom{9+5}{5}}{10^6}$