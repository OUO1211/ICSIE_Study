526
離散數學（上）

使用組合證明

1．$\binom{2 n+2}{n+1}=\binom{2 n}{n+1}+2\binom{2 n}{n}+\binom{2 n}{n-1}=2\left(\binom{2 n}{n}+\binom{2 n}{n-1}\right)$ ．

【 103 海洋資工】

【組合證明】
利用加法原理 ：$\binom{2 n+2}{n+1}=\binom{2 n+1}{n+1}+\binom{2 n+1}{n}=\left[\binom{2 n}{n+1}+\binom{2 n}{n}\right]+\left[\binom{2 n}{n}+\binom{2 n}{n-1}\right]$
$$
=\binom{2 n}{n+1}+2 \cdot\binom{2 n}{n}+\binom{2 n}{n-1}=\binom{2 n}{n-1}+2 \cdot\binom{2 n}{n}+\binom{2 n}{n-1}=2 \cdot\left[\binom{2 n}{n}+\binom{2 n}{n-1}\right] .
$$

亦可以組合意義說明 ：
左式即為 $2 n+2$ 相異物中不重複選出 $n+1$ 件方法數；而亦可考慮如下：
（1）必取某物 $A$ 與 $B$ ，則只需再從剩下 $2 n$ 物中取出 $n-1$ 物，方法數有 $\binom{2 n}{n-1}$ 種，
（2）必取某物 $A$ 與但不取 $B$ ，則需再從剩下 $2 n$ 物中取出 $n$ 物，方法數有 $\binom{2 n}{n}$ 種，
（3）必取某物 $B$ 與但不取 $A$ ，則需再從剩下 $2 n$ 物中取出 $n$ 物，方法數有 $\binom{2 n}{n}$ 種，
（4）$A$ 與 $B$ 均不取，則需再從剩下 $2 n$ 物中取出 $n+1$ 物，方法數有 $\binom{2 n}{n+1}$ 種，
故等式成立。
2．$\binom{2 n}{2}=2\binom{n}{2}+n^2$ ．

【95清大資感】

【組合證明】
考慮相異物品 $A_1, \ldots, A_n, B_1, \ldots, B_n$ ，共 $2 n$ 件，則從中任取 2 件的方法數為 $\binom{2 n}{2}$ ，但亦可考慮如下：
Case 1：$A_i, B_j$ 中各取一件，for some $i, j$ ，方法數 $\binom{n}{1} \cdot\binom{n}{1}=n^2$ 。
Case 2： 2 件都從 $A$（或 $B$ ）中取，方法數 $\binom{n}{2} \cdot 2$ 。
得證：$\binom{2 n}{2}=n^2+2\binom{n}{2}$ 。
亦可另證如下：