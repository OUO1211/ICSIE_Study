第3章 函數
249

取子集問題－第二型
$S=\{1,2, \ldots, n\}, A$ 為 $S$ 之任意子集合，計算 $A$ 中元素的和。
則取 $A$ 的方法多於和的可能狀況時，必可取出 2 種不同子集，其元素和相同。

例題 10
$(10 \%)$ Let $A \subseteq\{1,2, \ldots, 50\}$ where $|A|=10$ ．For any subset $B$ of $A$ let $s_B$ denote the sum of the elements in $B$ ．Prove that there are distinct subsets $C, D$ of $A$ such that $|C|=|D|=4$ and $s_C=s_D$ ．

【101暨南資エ】
解 由 $A$ 中取 4 個數，共有 $\binom{10}{4}=210$ 種取法，
而所取出的四數和，最小可能是 $1+2+3+4=10$ ，
最大可能是 $47+48+49+50=194$ ，
所以四數和的可能情形最多有 $194-10+1=185$ 種，故知必有兩種取法其和相同。

例題 11
Let $S$ be a set of five positive integers，the max of which is at most 9 ．Prove that the sums of the elements in all the nonempty subsets of $S$ cannot all be distinct．

【 100 、 104 暨南資エ】【 102 台南資工】【 108 中山資工】
解 由 $S$ 中取子集，共有 $2^5=32$ 種取法。而所取出的子集和，最小可能是 0 ，最大可能是 $5+6+7+8+9=35$ 。和的狀況比取法多，因此不能用上題的方法討論。
（＊）若排除空集合與本身 $S$ ，則子集取法有 30 種，而所取出的子集和，最小可能是 1 ，最大可能是 $6+7+8+9=30$ 。和的狀況與取法一樣多，因此還是無法用上題的方式。
（＊＊）若再排除四個元素的特殊情形，即只考慮1－子集、2－子集、3－子集，則取法共有 $\binom{5}{1}+\binom{5}{2}+\binom{5}{3}=25$ 種，而所取出的子集和，最小可能是 1 ，最大可能是 $7+8+9=24$ 。則子集和的可能情形最多有 $24-1+1=24$ 種，故知必至少有兩種取法其和相同。