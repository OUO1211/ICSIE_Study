438
離散數學（上）

可重覆排列
$n$ 件相異物允許重覆，取 $r$ 件排列的方法数有 $n^r$ 種。
Note
可重覆排列的組合應用：設 $A, B$ 為兩集合，$|A|=m,|B|=n$ ，則由 $A$ 至 $B$ 的函數個數有 $n^m$ 個。

【95台大資工】

例題
Six－digit numbers are to be formed using the integer in the set $A=\{1,2,3,4,5,6,7,8\}$ ．
（1）How many such numbers can be formed if repetitions are allowed？
（2）In part（1），how many of the numbers contain at least one 3 and at least one 5 ？
（3）How many six－digit numbers can be formed if each digit in $A$ can be used at most once？
解（1）每個 digit 有 8 種數字可選，故方法數為 $8 \times 8 \times \cdots \times 8=8^6$ 。
（2）沒有出現 3 的方法數為 $7^6$ ；
沒有出現 5 的方法數為 $7^6$ ；
同時沒有出現 3 與 5 的方法數為 $6^6$ ；故共有 $8^6-2 \cdot 7^6+6^6$ 。
（3）每個數字不重複出現，所以第一個 digit 有 8 種數字可選；
第二個 digit 有 7 種數字可選；．．．
故方法數為 $8 \times 7 \times 6 \times 5 \times 4 \times 3$ 。

例題
$(15 \%)$ Suppose that a＂word＂is any string of seven letters of the alphabet $\{A, B, C, \ldots, Z\}$ ，with repeated letters allowed．Answer the questions．
（1）How many words begin with $R$ and end with $T$ ？
（2）How many words begin with $A$ or end with $B$ ？
（3）How many words begin with $A$ or $R$ or end with $T$ or $B$ ？
【108台北資工】
解（1）只剩中間五格每個位置可為 $A \sim Z$ 的任意種，方法數為 $26 \times 26 \times 26 \times 26 \times 26=26^5$ 。
（2）首 $A$ 則後六格每格有 26 種變化，末 $B$ 則前六格有 26 種變化，首 $A$ 且末 $B$ ，則中間 5 格每格 26 種變化，故所求為 $26^6+26^6-26^5$ 。
（3） $26^6+26^6+26^6+26^6-4 \times 26^5$ 。