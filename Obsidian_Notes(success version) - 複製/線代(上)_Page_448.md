# 第 4 章　線性映射　455

> **例** 3
>
> Determine whether the following transformations are linear.
>
> (1) $T(ax^2+bx+c)=(a+b)x+(b+c)$.　【107 中央資工】
>
> (2) $T:P_2(R)\to P_2(R),\ T(f(x))=xf'(x)$.　【101 中正數學】
>
> (3) $T:P_2\to P_3$ by $T(p(t))=(t+3)p(t)$.　【110 成大電機】
>
> (4) $T:P_3\to P_3,\ L(p(t))=p''(t)+p(0)$.　【101 台北統計】
>
> (5) $T(f(x))=f(x)\cos x:V\to V$，where $V$ be the set of continuous real valued functions on $[0,2\pi]$.　【108 交大應數】

解

(1) 是線性映射。

$$
T(ax^2+bx+c+k(dx^2+ex+f))
$$

$$
=T((a+kd)x^2+(b+ke)x+(c+kf))
$$

$$
=(a+kd+b+ke)+((b+ke)+(c+kf))x
$$

$$
=[(a+b)+(b+c)x]+k[(d+e)+(e+f)x]
$$

$$
=T(ax^2+bx+c)+kT(dx^2+ex+f)
$$

(2) 是線性映射。

今 $f(x),g(x)\in P_2(R),a\in R,$

則 $T(af(x)+g(x))=x(af(x)+g(x))'=axf'(x)+xg'(x)=aT(f(x))+T(g(x))$

(3) 是線性映射。

對任意多項式 $p(t),q(t)$，任意純量 $a$，

則 $T(ap(t)+q(t))=(t+3)(ap(t)+q(t))=a(t+3)p(t)+(t+3)q(t)=aT(p(t))+T(q(t))$

故知 $T$ 為一線性映射。

(4) 是線性映射。

(5) 是線性映射。