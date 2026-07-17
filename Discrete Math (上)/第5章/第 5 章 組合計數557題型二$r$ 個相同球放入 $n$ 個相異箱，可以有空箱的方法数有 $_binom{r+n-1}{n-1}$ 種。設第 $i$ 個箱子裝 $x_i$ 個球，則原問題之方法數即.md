第 5 章 組合計數
557

題型二
$r$ 個相同球放入 $n$ 個相異箱，可以有空箱的方法数有 $\binom{r+n-1}{n-1}$ 種。
設第 $i$ 個箱子裝 $x_i$ 個球，
則原問題之方法數即為 $x_1+x_2+\ldots+x_n=r, x_i \geq 0$ 之非負整數解個數 ：$\binom{r+n-1}{n-1}$ 。
Note
（1）$r$ 個相同球放入 $n$ 個相異箱，不可有空箱的方法數 $=\binom{r-n+n-1}{n-1}=\binom{r-1}{n-1}$ 。

例題
2
In how many ways can 36 identical robots be assigned to five assembly lines with
（1）（5\％）At least four robots assigned to each line？
（2）（ $5 \%$ ）At least four，but no more than ten，assigned to each line？
（no score if you give no details．）
【95台科資工】【106成大資工】
解 此處將組裝線視為相異。
設各線上各配置 $x_1, x_2, \cdots, x_5$ 個機器人，則 $x_1+x_2+\ldots+x_5=36$ ，
（1）即 $x_1 \geq 4, \ldots, x_5 \geq 4$ 時的整數解個數：$\binom{36-4 \times 5+4}{4}=\binom{20}{4}$ 。
（2）即 $10 \geq x_i \geq 4, \forall i$ 時的整數解個數，
即 $y_1+y_2+\ldots+y_5=16,0 \leq y_i \leq 6, \forall i$ 的整數解個數：
$$
\binom{16+4}{4}-\binom{5}{1}\binom{9+4}{4}+\binom{5}{2}\binom{2+4}{4} .
$$

例題

3

（10\％）In how many ways can we describe 8 red balls and 9 blue balls among 6 children so that each child receives at least one blue ball？

【 100 嘉義資工類題】【99 台大工科】
設四人所得紅球數與藍球數各為 $r_i$ 與 $b_i, i=1 \sim 6$ ，其中，$r_i \geq 0, b_i \geq 1$ ，
則 $r_1+r_2+\cdots+r_6=8$ 與 $b_1+b_2+\cdots+b_6=9$
整數解個數為 $\binom{8+5}{5} \times\binom{ 3+5}{5}$ 。