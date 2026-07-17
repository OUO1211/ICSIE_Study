230

離散數學（上）



鴿簐原理之一般化

將 $m$ 件物品置於 $n$ 個抽㨢中，

一定有某些抽屉中有大於等於 $\left\lceil\frac{m}{n}\right\rceil$ 件；也一定有某些抽屉中小於等於 $\left\lfloor\frac{m}{n}\right\rfloor$ 件。

例如：

三人共有 100 元，則必有某人 $\leq\left\lfloor\frac{100}{3}\right\rfloor=33$ 元，亦必有某人 $\geq\left\lceil\frac{100}{3}\right\rceil=34$ 元。



例題

（5\％）Show that at least four of any 22 days must fall on the same day of the week．

【98 台大工科、100 海洋資工、101 台大電機、105 成大電機類題、105 中正資工】

解 根據鴿籠原理， 22 天中必有 $\geq\left\lceil\frac{22}{7}\right\rceil=4$ 天落在一週的同一天。

否則，星期一到星期天都頂多出現 3 次，則總共才 21 天，不符題意。



例題

（3\％）A computer randomly prints three－digit codes，with no repeated digits in any code（for example， $387,072,760$ ）．What is the minimum number of codes that must be printed in order to guarantee that at least five of the codes are identical？



【104 交大資工】

解 長度 3 ，每個 digit 均可 $0 \sim 9$ 但不可重複的 code 有 $10 \times 9 \times 8=720$ 種，

故印出 $720 \times 4+1=2881$ 個 code 時，必有某 code 共印出 $\geq\left\lceil\frac{2881}{720}\right\rceil=5$ 次。



例題

6

$(10 \%)$ In a group of 20 people who join a lunch party，we know the sum of their ages is 380 and the youngest one has his／her age of 10 ．Show that there are at least two people who are at the same age．



【107 台科資工】

若遗 20 人都年紀不相同，

則其總和最少是： $10+11+\ldots+29=390$ ，與題目總和 380 不合，

故知，必有某兩人年紀相同。