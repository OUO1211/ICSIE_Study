第12章 代數結構
471

III．設 $G$ 為一非交換群，則 $|G| \geq 6$ 。（即證明：若 $|G| \leq 5$ ，則 $G$ is abelian．）
【證明】
$G \mid=1$ ，時 $G=\{e\}, \therefore G$ 為交換群。
$G \mid=2,3,5$ 為質數時，此時，$G$ 為循環群，$\therefore G$ 為交換群。
$|G|=4$ 時，
若存在 $a \in G$ ，且 $a^4=e$ ，則 $G=\langle a\rangle$ ，則 $G$ 為循環群，$\therefore G$ 為交換群。
否則即 $\forall x \in G, x \neq e, x^2=e$ 。（note：不會有 $x^3=e$ ），前面在第433頁有證明此為交換群。

IV．If $G$ is a group of order $n$ and $a \in G$ ，prove that $a^n=e$ ．
【語明】
若 $a=e$ ，則定理當然得證。
設 $a \in G, a \neq e$ ，考慮 $H=\langle a\rangle$ 為 $G$ 之子群，且 $a^{|H|}=e$ ，
由 Lagrange 定理知 $|H| \mid n$ ，即 $n=k \cdot|H|, k$ 為正整數，
則 $a^n=a^{k|H|}=\left(a^{|H|}\right)^k=e^k=e$ 。

V．設 $m \in Z, n \in N, \operatorname{gcd}(m, n)=1$ ，則 $m^{\phi(n)} \equiv 1 \bmod n$ ．【108中山資工】
其中， $\boldsymbol{\phi}(\boldsymbol{n})=\mid\{\boldsymbol{m} \mid 1 \leq m<n$ ，and $\operatorname{gcd}(m, n)=1\} \mid$ ：Euler＇s phi function．
【證明】
考慮與 $1 \sim n-1$ 中與 $n$ 互質之數所成集合在 ${ }_n$ 下為一群 $Z_n^*$ ，而 $\left|Z_n^*\right|=\phi(n)$ ，
若 $m \leq n$ ，則 $m \in Z^*$ ，由前述定理可得 $m^{\phi(n)}=1$ 。
若 $m>n$ ，令 $m=a n+r$ 即 $m \equiv r \bmod n$ ，其中 $0<r<n, \operatorname{gcd}(n, r)=1, a, r \in Z$ ，
則 $m^{(n)} \equiv r^{(n)} \equiv 1 \bmod n$ 。

VL（Fermat＇s Little theorem）
该 $m \in Z, p$ ：prime， $\operatorname{gcd}(m, p)=1$ ，则 $m^{p-1} \equiv 1 \bmod p$ 。【108中山資工】

此助为定理 V 在 $n$ 為質數 $p$ 時之特例，$\phi(p)=p-1$ 。