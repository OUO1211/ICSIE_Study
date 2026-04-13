## 向量空間的基本性質

> 考慮向量空間 $V$，則對任意向量 $u, v, w$，任意純量 $\alpha$，
>
> (1) 若 $u + w = v + w$，則 $u = v$。
>
> (2) $0v = 0$。
>
> (3) $\alpha 0 = 0$。
>
> (4) $(-\alpha)v = \alpha(-v) = -(\alpha v)$。

**【證明】**

(1) $\forall u, v, w \in V$，

$$
\because\ u + w + (-w) = v + w + (-w),
$$

$$
\text{故 } u + 0 = v + 0,
$$

$$
\text{故 } u = v,
$$

此即為向量加法的消去性，其實，因向量在加法下形成交換群故有消去性。

(2) $\forall v \in V$，

$$
\because\ 0 + 0v = 0v = (0 + 0)v = 0v + 0v,
$$

$$
\therefore\ 0 = 0v.
$$

(3) $\forall \alpha \in F$，

$$
\because\ 0 + \alpha 0 = \alpha 0 = \alpha(0 + 0) = \alpha 0 + \alpha 0,
$$

$$
\therefore\ 0 = \alpha 0.
$$

(4) $\forall v \in V,\ \forall \alpha \in F$，

$$
\alpha v + (-\alpha)v = (\alpha + (-\alpha))v = 0v = 0,\ \therefore\ -\alpha v = (-\alpha)v,
$$

$$
\alpha v + \alpha(-v) = \alpha(v + (-v)) = \alpha 0 = 0,\ \therefore\ -\alpha v = \alpha(-v).
$$