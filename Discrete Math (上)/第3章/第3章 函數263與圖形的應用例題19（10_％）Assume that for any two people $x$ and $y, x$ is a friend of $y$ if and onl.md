第3章 函數
263

與圖形的應用
例題
19
（10\％）Assume that for any two people $x$ and $y, x$ is a friend of $y$ if and only if $y$ is a friend of $x$ ．Show that，in any group of two or more people，there are always two people with exactly the same number of friends inside the group．

【90 交大資科】【100 中山電機】【100 台大電機】【89、101 中山資工】
解 設一群共 $n$ 個人，則每人所認識的人數，可能值為 $0,1,2, \ldots, n-1$ ，
但 0 與 $n-1$ 不同時出現（因為同一個場合中，不會有人認識其他所有人，但又同時有人其他人都不認識），故頂多有 $n-1$ 種不同值，必有兩數字相同，即必有兩人之朋友數相同。

例題 20

任意 6 人中，必有 3 人彼此相識，或必有 3 人彼此不相識。
【重要】
解 設為 $a, b, c, d, e, f$ 六人，依是否認識 $a$ 將剩餘 5 人分成兩個集合 $A, B$ ，即 $A=\{$ 識 $a$者 $\}, B=\{$ 不識 $a$ 者 $\}$ 。則由鴿籠原理知，$|A| \geq 3$ 或 $|B| \geq 3$ 。
（1）$|A| \geq 3$ ，不失一般性，設 $b, c, d \in A$ ，考慮 $b, c, d$ 三人：
若 $b, c, d$ 彼此不識，則證明完畢。
否則，即 $b, c, d$ 至少有 2 人相識，再加上 $a$ ，找到 3 人彼此認識，得證。
（2）$|B| \geq 3$ ，不失一般性，設 $b, c, d \in B$ ，考慮 $b, c, d$ 三人：
若 $b, c, d$ 彼此相識，則證明完畢。
否則，即 $b, c, d$ 至少有 2 人彼此不識，再加上 $a$ ，找到 3 人彼此不認識，得證。