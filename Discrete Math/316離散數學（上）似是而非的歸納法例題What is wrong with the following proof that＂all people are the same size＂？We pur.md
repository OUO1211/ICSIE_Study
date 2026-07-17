316
離散數學（上）

似是而非的歸納法

例題
What is wrong with the following proof that＂all people are the same size＂？We purpose to prove that all $n$ and for all $S$ ，if $S$ is a set with $n$ people，then all people in $S$ are the same size．
（1）（Basis）Let $S$ be an empty set of people．Then for all $x$ and $y$ ，if $x \in S$ and $y \in S$ ，then $x$ is the same size as $y$ ．
（2）（Induction）Assume the assertion is true for all sets containing $n$ people．We show it is true for sets containing $n+1$ people．Any set containing $n+1$ people contains two non－equal subsets of $n$ people which must overlap．Denote these sets by $S^{\prime}$ and $S^{\prime \prime}$ ．Then by induction hypothesis，all people in $S^{\prime}$ are the same size and all people in $S^{\prime \prime}$ are the same size．Since $S^{\prime}$ and $S^{\prime \prime}$ overlap，all people in $S=S^{\prime} \cup S^{\prime \prime}$ are the same size．

【94中央資工類題】【97清大資應】
解＂Any set containing $n+1$ people contains two non－equal subsets of $n$ people which must overlap．＂這句話在 $n=1$ 時出現錯誤。

基礎類題
1．下面是一個数學歸纳法的錯誤應用，請說明錯誤發生在哪裡？
命題：任何包含 $m$ 個元素的自然数集合，它裡面的元素必然都相等。 $m=1$ 時，此命題顯然成立。
假設 $m=n$ 時命題成立，
現令 $m=n+1$ ，而 $a_1, \ldots, a_n, a_{n+1}$ 為 $n+1$ 個自然数，由歸納法假設可知 $a_1=\ldots=a_n$ ，又因為 $a_2=\ldots=a_{n+1}$ ，故得 $a_1=\ldots=a_{n+1}$ ，因此命題恆成立。

解 歸納步驟中，＂$n=1$ 時 $a_1=a_1, a_2=a_2$ ，故得 $a_1=a_2$＂有誤。
2．某人説他有 $1 / 3$ 的中國人血統，別人問他這怎麼可能？他回答說：因為我的父親有 $1 / 3$ 的中图血统，我的母親也有 $1 / 3$ 的中國血統。這是不是利用歸納法的一個正確證明？

No．因歸納基底（basis）沒有被驗證。