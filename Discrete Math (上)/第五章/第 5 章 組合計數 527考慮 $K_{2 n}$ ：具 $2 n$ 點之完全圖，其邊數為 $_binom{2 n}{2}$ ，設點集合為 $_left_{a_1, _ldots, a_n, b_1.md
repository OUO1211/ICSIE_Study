第 5 章 組合計數 527

考慮 $K_{2 n}$ ：具 $2 n$ 點之完全圖，其邊數為 $\binom{2 n}{2}$ ，設點集合為 $\left\{a_1, \ldots, a_n, b_1, \ldots, b_n\right\}$ ，則因 $\left\{a_1, \ldots, a_n\right\},\left\{b_1, \ldots, b_n\right\}$ 均各自形成 $K_n$ ，故邊數 $2\binom{n}{2}$ ，
但每個 $a_i$ 均連到每個 $b_j$ ，故還有 $n^2$ 個邊，故得 $\binom{2 n}{2}=2\binom{n}{2}+n^2$ 。
3．$\binom{3 n}{3}=n^3+6 n\binom{n}{2}+3\binom{n}{3}$ ．
【93 交大應数】
【組合證明】
考慮相異物品 $A_1, \ldots, A_n, B_1, \ldots, B_n, C_1, \ldots, C_n$ 共 $3 n$ 件，則從中任取 3 件的方法數為 $\binom{3 n}{3}$ ，但亦可考慮如下：
Case 1：$A_i, B_j, C_k$ 中各取一件，方法數 $\binom{n}{1} \cdot\binom{n}{1} \cdot\binom{n}{1}=n^3$ 。
Case 2： 3 件都從 $A$（或 $B$ ，或 $C$ ）中取，方法數 $3\binom{n}{3}$ 。
Case 3：$A$ 取 2 件，$B$ 取 1 件，$C$ 取 0 件（記成數對 $(2,1,0)$ ），方法數 $\binom{n}{2} \cdot\binom{n}{1}=n\binom{n}{2}$ 。但因還有 $(2,0,1),(1,2,0),(1,0,2),(0,1,2),(0,2,1)$ 共六種配法，故方法數 $6 n\binom{n}{2}$ 。
得證 ：$\binom{3 n}{3}=n^3+3\binom{n}{3}+6 n\binom{n}{2}$ 。
4．$\binom{n}{r}\binom{r}{k}=\binom{n}{k}\binom{n-k}{r-k}$ ．
【組合證明】
左式 $\binom{n}{r}\binom{r}{k}$ 等同於從 $n$ 人中取 $r$ 人組成代表團參加比賽，而其中有 $k$ 人得獎的方法數，此問題可如此計算：先從 $n$ 人中決定出哪 $k$ 人是參加代表團並得獎的，方法數 $\binom{n}{k}$ ，再從剩下 $n-k$ 人中選出 $r-k$ 人，讓他們當陪考的方法有 $\binom{n-k}{r-k}$ ，故由乘法原理得 $\binom{n}{k}\binom{n-k}{r-k}$ 即右式。