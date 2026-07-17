第 5 章 組合計數
495

機率相關考題
例题
$(12 \%)$ What is the minimum number of times we must toss a fair coin so that the probability that we get at least two heads is at least 0.95 ？

【106 台科資工】
解 投擲 $n$ 次，而均不為 head 的機率是 $(0.5)^n$ ；
恰一次 head 的機率是 $\binom{n}{1}(0.5)^{n-1}(0.5)$ ，
故至少兩次 head 的機率是 $1-(0.5)^n-\binom{n}{1}(0.5)^{n-1}(0.5)=1-(n+1)(0.5)^n$ ，
代入 $n=7$ 時值為 0.9375 ，代入 $n=8$ 時值為 $0.9648 \ldots$
故回答 8 。

基礎類題
1．A biased coin with $P(H)=1 / 10$ is tossed 3 times．What is the probability of getting exactly one $H$ ？

解 $3\left(\frac{1}{10}\right)\left(\frac{9}{10}\right)^2$ 。
2．一個硬幣投搝 8 次，正面至少出現 2 次的機率為何？
解 $\left(2^8-1-8\right) / 2^8$ 。
3．What is the probability that a die never comes up an even number when it is rolled 5 times？
【98 台大電機】
1／32。
4．A famous basketball player is shooting free throws．He will make the shot with probability 0.90 ， and will miss with probability 0.10 ．Suppose he attempts 10 shots in a row．What is the probability that he misses at least one？

【103成大工科】
全部都命中的機率是 $(0.9)^{10}$ ，故至少錯失一球的機率是1－（0．9）${ }^{10}$ 。