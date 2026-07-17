第 5 章 組合計數
461

特殊條件的路徑問題
例題
14
A Lattice path from $\left(x_0, y_0\right)$ to $\left(x_n, y_n\right)$ in the $x-y$ plane is defined as a sequence of points $\left(x_0, y_0\right),\left(x_1, y_1\right), \ldots,\left(x_n, y_n\right)$ s．t．$x_{i+1}=x_i+1, y_{i+1}=y_i \pm 1, \forall i=1 \sim n-1$ ．
（1）How many lattices paths are there from $(0,1)$ to $(10,3)$ ？
（2）How many of them do not touch or cross the $x$－axis？

【90、101 中山資工】

解（1）每個 $U:(x, y) \rightarrow(x+1, y+1)$ 使 $x$ 方向增加 $1, y$ 方向增加 1 ；
每個 $D:(x, y) \rightarrow(x+1, y-1)$ 使 $x$ 方向增加 $1, y$ 方向減少 1 ；
設用了 $s$ 個 $U, t$ 個 $D$ ，則從 $(0,1)$ 到 $(10,3)$ ，則
$x$ 方向增加 $10, \therefore s+t=10$ ；
$y$ 方向增加 $2, \therefore s-t=2$ ；
解得 $s=6, t=4$ ，故方法數有 $\frac{10!}{6!4!}$ 種。
（2）先計算從 $(0,1)$ 到 $(10,3)$ 必 touch or cross $x$ 軸的走法（稱此為非法型）有多少種，則因為每一非法型的走法一對一對應於 $(0,-1)$ 到 $(10,3)$ 的走法…（原因說明如下＊）而 $(0,-1)$ 到 $(10,3)$ 的走法共 $\frac{10!}{7!3!}$ 種（同（1）的解法），故所求走法共 $\frac{10!}{6!4!}-\frac{10!}{7!3!}$ 種。
$\left(^*\right)$ ：每一種 $(0,1)$ 到 $(10,3)$ 非法型走法，把從 $(0,1)$ 到的第一個 touch 到 $x$ 軸的這一段對 $x$ 軸做鏡射，其餘保持不變，則所得即為一種 $(0,-1)$ 到 $(10,3)$ 走法。