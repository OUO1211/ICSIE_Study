第8章 各內積算子及其應用
415

8－1 伴隨與正規

伴隨算子（adjoint operator）
考虑内積空間 $V$ 上的線性算子 $T$ ，
若存在線性映射 $T^*: V \rightarrow V$ 使滿足對任何向量 $\boldsymbol{u}, \boldsymbol{v},<T(\boldsymbol{u}), \boldsymbol{v}>=<\boldsymbol{u}, T^*(\boldsymbol{v})>$ ，
則稱 $T *$ 為 $T$ 的伴隨算子。

伴隨算子的性質
考慮 $V$ 上的算子 $T, U$ ，對任意向量 $\boldsymbol{u}, \boldsymbol{v}$ 任意純量 $\alpha$ ，
（1）$<\boldsymbol{u}, T(\boldsymbol{v})>=<T^*(\boldsymbol{u}), \boldsymbol{v}>, \forall \boldsymbol{u}, \boldsymbol{v} \in V$ ．
（2）$(T+U)^*=T^*+U^*$ ．
（3）$(\alpha T)^*=\bar{\alpha} T^*$ ．
（4）$\left(T^*\right)^*=T$ ．
（5）$(T U)^*=U^* T^*$ ．
（6）$I^*=I$ ．
（7）若 $T$ 可逆，則 $T^*$ 亦可逆，且 $\left(T^*\right)^{-1}=\left(T^{-1}\right)^*$ ．
（8）$\left[T^*\right]_\beta=\left([T]_\beta\right)^H$ ，其中，$\beta$ 為 $V$ 的一單範正交基底。【95中興應数、100東華應数】
（9）若 $\lambda$ 為 $T$ 的特徵根，則 $\bar{\lambda}$ 為 $T^*$ 的特徵根。
【105成大應数】

【證明】
$\forall \boldsymbol{u}, \boldsymbol{v} \in V$ ，
（1）$\langle\boldsymbol{u}, T(\boldsymbol{v})\rangle=\overline{\langle T(\boldsymbol{v}), \boldsymbol{u}\rangle}=\overline{\left\langle\boldsymbol{v}, T^*(\boldsymbol{u})\right\rangle}=\left\langle T^*(\boldsymbol{u}), \boldsymbol{v}\right\rangle$ ．
（2）$\left\langle\boldsymbol{u},(T+U)^*(\boldsymbol{v})\right\rangle=\langle(T+U)(\boldsymbol{u}), \boldsymbol{v}\rangle=\langle T(\boldsymbol{u})+U(\boldsymbol{u}), \boldsymbol{v}\rangle=\langle T(\boldsymbol{u}), \boldsymbol{v}\rangle+\langle U(\boldsymbol{u}), \boldsymbol{v}\rangle$
$$
=<\boldsymbol{u}, T^*(\boldsymbol{v})>+<\boldsymbol{u}, U^*(\boldsymbol{v})>=<\boldsymbol{u}, T^*(\boldsymbol{v})+U^*(\boldsymbol{v})>,
$$

故 $(T+U)^*(\boldsymbol{v})=T^*(\boldsymbol{v})+U^*(\boldsymbol{v}), \forall \boldsymbol{v} \in V$ ，即 $(T+U)^*=T^*+U^*$ ．
（3）$<\boldsymbol{u},(\alpha T)^*(\boldsymbol{v})>=<(\alpha T)(\boldsymbol{u}), \boldsymbol{v}>=<\alpha T(\boldsymbol{u}), \boldsymbol{v}>=\alpha<T(\boldsymbol{u}), \boldsymbol{v}>$
$$
=\alpha<\boldsymbol{u}, T^*(\boldsymbol{v})>=<\boldsymbol{u}, \bar{\alpha} T^*(\boldsymbol{v})>,
$$

故 $(\alpha T)^*(\boldsymbol{v})=\left(\bar{\alpha} T^*\right)(\boldsymbol{v}), \forall \boldsymbol{v} \in V$ ，即 $(\alpha T)^*=\bar{\alpha} T^*$ 。
（4）$<\boldsymbol{u}, T(\boldsymbol{v})>=<T^*(\boldsymbol{u}), \boldsymbol{v}>=<\boldsymbol{u},\left(T^*\right)^*(\boldsymbol{v})>$ ，故 $\left(T^*\right)^*(\boldsymbol{v})=T(\boldsymbol{v}), \forall \boldsymbol{v} \in V$ ，即 $\left(T^*\right)^*=T$ 。
（5）$\left\langle\boldsymbol{u},(T U)^*(\boldsymbol{v})\right\rangle=\langle(T U)(\boldsymbol{u}), \boldsymbol{v}\rangle=\langle T(U(\boldsymbol{u})), \boldsymbol{v}\rangle=\left\langle U(\boldsymbol{u}), T^*(\boldsymbol{v})\right\rangle$