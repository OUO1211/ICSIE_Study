第4章 數學歸納法與數論
345

最大公因數表現定理（Bézout 定理）
對任意正整数 $a, b$ ，其最大公因数必存在且唯一，且 $a, b$ 的最大公因数一定可以表達成 $a, b$ 的線性組合，即：
若 $d=\operatorname{gcd}(a, b)$ ，則存在 $m, n \in Z$ ，使得 $a m+b n=d$ 。【96雲科資工】【103中央資工】
【證明】
令 $S=\{a \cdot s+b \cdot t \mid s, t \in Z$ and $a \cdot s+b \cdot t>0\}$ ，則 $S \subseteq N$ 且 $S \neq \varnothing$ ，
故由良序法則知，$S$ 必有最小元素，令為 $d=a u+b v$ ，其中，$u, v$ 為整數。
以下證明 $\boldsymbol{d}=\operatorname{gcd}(\boldsymbol{a}, \boldsymbol{b})$ ：
（1）$d$ 為 $a$ 與 $b$ 的公因數 ：
否則，設 $d$ 不為 $a$ 的因數，則由除數法則知：存在唯一整數 $q, r$ ，使得 $a=d q+r$ ，且 $0<r<d$ ，
$$
\therefore r=a-d q=a-q(a u+b v)=a(1-q u)+b(-q v) \text {, 故 } r \in S \text {, }
$$

但 $r<d$ ，與 $d$ 為 $S$ 中的最小矛盾，$\therefore d$ 為 $a$ 的一個因數，
同理可得 $d$ 為 $b$ 的一個因數。
（2）若 $d^{\prime}$ 亦為 $a$ 與 $b$ 的公因數，則 $d^{\prime} \mid d:$
若 $d^{\prime} \mid a$ 且 $d^{\prime} \mid b$ ，即存在整數 $x, y$ ，使得 $a=d^{\prime} x, b=d^{\prime} y$ ，
$\because d$ 為 $S$ 中的元素，∴ 存在 $u, v \in Z$ ，使得 $d=a u+b v$ ，
$\therefore d=\left(d^{\prime} x\right) u+\left(d^{\prime} y\right) v=d^{\prime}(x u+y v)$ ，故得 $d^{\prime} \mid d$ 。