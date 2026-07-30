第12章 代數結構
453

單位元素為 $1: \because 1 \cdot{ }_n a=a=a \cdot{ }_n 1$ 。
反元素性質：$\because n$ 為質數，且 $a<n, \therefore(n, a)=1, \therefore$ 存在整數 $b, k$ ，使 $a b+n k=1$ ，故 $a b \equiv_n 1$ ，即 $b=a^{-1}$ 。
交換性：$\because a \cdot{ }_n b=a b=b a=b \cdot{ }_n a \bmod n$ 。
（⇒）設 $n$ 不為質數，令 $n=a b$ ，其中 $a 、 b \in Z_n-\{0\}$ ，故存在 $b$ 的反元素 $b^{-1}$ ，使得$b \cdot{ }_n b^{-1}=1 \in Z_n-\{0\}$ ，則 $a=a \cdot{ }_n b \cdot{ }_n b^{-1}=(a b) b^{-1}=n b^{-1}=0 \bmod n \ldots$ 矛盾。
（4）$Z_n$ 中，$a$ 有乘法反元素 $\Leftrightarrow a$ 與 $n$ 互質。
【99 中山資工】
【證明】
$a$ 有乘法反元素
⇔ 存在 $b \neq 0, a b \equiv_n 1 \bmod n$ ，
$\Leftrightarrow 1-a b=n k$ ，for some $k \in Z$ ，
$\Leftrightarrow a b+n k=1$ ，for some $b, k \in Z$ ，
$\Leftrightarrow \operatorname{gcd}(a, n)=1$ 。
（6）$Z_n$ 中有 $\phi(n)$ 個元素有乘法反元素。
【94 台大資工】【99 中山資工】
（7）另有一乘法模同餘群 $\left(Z_n^*, *\right)$ ，其中 $Z_n^*=\{x \mid 1 \leq x \leq n-1, x$ 與 $n$ 互質 $\}$ 。
（8）應用以證明 Wilson 定理：若 $p$ 為質數，則 $(p-1)!\equiv-1(\bmod p)$ 。
【證明】
$p=2$ 或3時，此定理顯然成立。
當 $p \geq 5$ ，考慮 $\left(Z_p,{ }_p\right)$ 中，$x^2-1=(x+1)(x-1)=0$ 恰兩解： $1,-1$（即 $p-1$ ），
即 $1^2 \equiv 1(\bmod p) 、(p-1)^2 \equiv 1(\bmod p)$,
即1與 $p-1$ 本身為本身之反元素，
即 $2 \sim p-2$ 中兩兩互為反元素，$\therefore 2 \cdot 3 \cdot \ldots \cdot p-2 \equiv 1(\bmod p)$ ，
所以 $(p-1)!\equiv(p-1) \equiv-1(\bmod p)$ 。